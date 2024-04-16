# Comparing `tmp/sdv-1.9.0.tar.gz` & `tmp/sdv-1.9.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdv-1.9.0.tar", last modified: Thu Jan 11 19:46:46 2024, max compression
+gzip compressed data, was "sdv-1.9.0.dev0.tar", last modified: Thu Jan 11 17:29:54 2024, max compression
```

## Comparing `sdv-1.9.0.tar` & `sdv-1.9.0.dev0.tar`

### file list

```diff
@@ -1,659 +1,659 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.999766 sdv-1.9.0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-24 21:06:49.000000 sdv-1.9.0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8104 2023-10-13 17:28:40.000000 sdv-1.9.0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    86557 2024-01-11 19:46:44.000000 sdv-1.9.0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4818 2023-01-24 21:06:49.000000 sdv-1.9.0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-21 19:18:25.000000 sdv-1.9.0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    97375 2024-01-11 19:46:45.999941 sdv-1.9.0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9787 2023-10-13 17:28:40.000000 sdv-1.9.0/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.879970 sdv-1.9.0/docs/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/Makefile
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.881344 sdv-1.9.0/docs/api_reference/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.881987 sdv-1.9.0/docs/api_reference/constraints/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.899574 sdv-1.9.0/docs/api_reference/constraints/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      666 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      627 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Range.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      117 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Range.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Range.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Range.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Range.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Range.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Range.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      131 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Range.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Range.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      588 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      523 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      359 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/constraints/base.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/constraints/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2609 2022-07-22 02:55:50.000000 sdv-1.9.0/docs/api_reference/constraints/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      353 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/evaluation.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2022-07-22 02:55:50.000000 sdv-1.9.0/docs/api_reference/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.900029 sdv-1.9.0/docs/api_reference/lite/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.901595 sdv-1.9.0/docs/api_reference/lite/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      205 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.list_available_presets.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      502 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.9.0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       94 2022-07-22 02:55:50.000000 sdv-1.9.0/docs/api_reference/lite/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      348 2022-07-22 02:55:50.000000 sdv-1.9.0/docs/api_reference/lite/tabular.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.902198 sdv-1.9.0/docs/api_reference/metadata/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.910147 sdv-1.9.0/docs/api_reference/metadata/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_field.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_relationship.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_children.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_dtypes.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_field_meta.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_fields.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_foreign_keys.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_parents.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_table_meta.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_tables.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_tables.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      877 2022-09-29 22:36:12.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.set_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.validate.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.visualize.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_dtypes.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_fields.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_model_kwargs.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      668 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_model_kwargs.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      854 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/metadata/dataset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      116 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/metadata/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      583 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/metadata/table.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.911007 sdv-1.9.0/docs/api_reference/metrics/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.939056 sdv-1.9.0/docs/api_reference/metrics/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.demos.load_multi_table_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.demos.load_single_table_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.demos.load_timeseries_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:23.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      614 2022-08-30 22:45:23.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      506 2022-08-30 22:45:24.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-08-30 23:02:40.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-08-30 23:02:40.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 23:02:40.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-08-30 23:02:15.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-08-30 23:02:15.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      534 2022-08-30 23:02:15.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      638 2022-08-30 22:45:24.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      242 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2022-08-30 22:45:24.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      236 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      582 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:24.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      204 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      661 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      210 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      897 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      811 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      762 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      565 2022-08-30 22:45:24.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      734 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      818 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      842 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      720 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      192 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      788 2022-10-05 00:20:25.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      760 2022-10-05 00:20:25.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-08-30 23:02:40.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-08-30 23:02:40.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      649 2022-08-30 23:02:40.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-08-30 23:02:15.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-08-30 23:02:15.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-08-30 23:02:15.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      717 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      657 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      688 2022-10-05 00:20:25.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      701 2022-08-30 22:45:24.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      957 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      195 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      822 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      819 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      239 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      895 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      257 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      857 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      551 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      683 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      230 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      672 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      213 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/metrics/demos.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/metrics/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1402 2022-09-22 23:47:45.000000 sdv-1.9.0/docs/api_reference/metrics/relational.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4109 2022-09-22 23:47:45.000000 sdv-1.9.0/docs/api_reference/metrics/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      735 2022-12-21 22:30:23.000000 sdv-1.9.0/docs/api_reference/metrics/timeseries.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.939494 sdv-1.9.0/docs/api_reference/relational/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.941046 sdv-1.9.0/docs/api_reference/relational/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      416 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/relational/hma1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/relational/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.941585 sdv-1.9.0/docs/api_reference/sampling/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.942221 sdv-1.9.0/docs/api_reference/sampling/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_column_values.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      151 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_num_rows.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      417 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/sampling/api/sdv.sampling.Condition.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/sampling/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/sampling/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/sdv.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.943219 sdv-1.9.0/docs/api_reference/tabular/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.951069 sdv-1.9.0/docs/api_reference/tabular/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_distributions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      655 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_distributions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_likelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_parameters.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      663 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.set_parameters.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      450 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      129 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      187 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      339 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/tabular/copulagan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      489 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/tabular/copulas.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      260 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/tabular/ctgan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      136 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/tabular/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      249 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/tabular/tvae.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.951599 sdv-1.9.0/docs/api_reference/timeseries/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.952648 sdv-1.9.0/docs/api_reference/timeseries/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      338 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.9.0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      108 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/timeseries/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/api_reference/timeseries/par.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6932 2023-10-13 17:28:40.000000 sdv-1.9.0/docs/conf.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.953287 sdv-1.9.0/docs/developer_guides/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8607 2023-10-13 17:28:40.000000 sdv-1.9.0/docs/developer_guides/contributing.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      364 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/developer_guides/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2905 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/developer_guides/overview.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.954597 sdv-1.9.0/docs/developer_guides/sdv/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5889 2022-07-22 02:55:50.000000 sdv-1.9.0/docs/developer_guides/sdv/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      292 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/developer_guides/sdv/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7480 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/developer_guides/sdv/metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9508 2023-02-02 20:58:41.000000 sdv-1.9.0/docs/developer_guides/sdv/tabular.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.955232 sdv-1.9.0/docs/getting_started/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      113 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/getting_started/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2555 2023-10-13 17:28:40.000000 sdv-1.9.0/docs/getting_started/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3664 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/getting_started/quickstart.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/history.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.963257 sdv-1.9.0/docs/images/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    47569 2024-01-11 19:46:44.000000 sdv-1.9.0/docs/images/CTGAN-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45265 2024-01-11 19:46:44.000000 sdv-1.9.0/docs/images/Copulas-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60600 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/images/DataCebo-Blue.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    35119 2024-01-11 19:46:44.000000 sdv-1.9.0/docs/images/DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42776 2024-01-11 19:46:44.000000 sdv-1.9.0/docs/images/DeepEcho-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17657 2024-01-11 19:46:44.000000 sdv-1.9.0/docs/images/RDT-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   243101 2023-03-28 20:22:54.000000 sdv-1.9.0/docs/images/Real-vs-Synthetic-Evaluation.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18827 2024-01-11 19:46:44.000000 sdv-1.9.0/docs/images/SDGym-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27257 2024-01-11 19:46:44.000000 sdv-1.9.0/docs/images/SDMetrics-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17776 2024-01-11 19:30:49.000000 sdv-1.9.0/docs/images/SDV-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67366 2024-01-11 19:30:49.000000 sdv-1.9.0/docs/images/SDV-logo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8765 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/images/SDV.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   412158 2023-03-28 20:22:54.000000 sdv-1.9.0/docs/images/Single-Table-Metadata-Example.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    99815 2022-07-22 02:55:50.000000 sdv-1.9.0/docs/images/custom_constraint.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50140 2023-03-28 20:22:54.000000 sdv-1.9.0/docs/images/datacebo-logo-dark-mode.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    34161 2024-01-11 19:46:44.000000 sdv-1.9.0/docs/images/datacebo-logo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      547 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/images/google_colab.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.9.0/docs/images/hma1_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8748 2022-12-08 23:36:42.000000 sdv-1.9.0/docs/images/metadata_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67425 2022-12-08 23:36:42.000000 sdv-1.9.0/docs/images/metadata_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2497 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/images/mybinder.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.9.0/docs/images/quickstart_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   176980 2023-01-24 21:06:49.000000 sdv-1.9.0/docs/images/rdt_main_tranformation.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2283 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/images/slack.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6069 2023-10-13 17:28:40.000000 sdv-1.9.0/docs/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      765 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/make.bat
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.965048 sdv-1.9.0/docs/savefig/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:00:09.000000 sdv-1.9.0/docs/savefig/copulagan_experience_years_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12668 2022-12-08 23:00:10.000000 sdv-1.9.0/docs/savefig/copulagan_experience_years_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10277 2022-12-08 23:00:37.000000 sdv-1.9.0/docs/savefig/copulagan_experience_years_3.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:05:15.000000 sdv-1.9.0/docs/savefig/experience_years_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10270 2022-12-08 23:05:16.000000 sdv-1.9.0/docs/savefig/experience_years_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12415 2022-12-08 23:05:16.000000 sdv-1.9.0/docs/savefig/experience_years_3.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.873634 sdv-1.9.0/docs/sdv_theme/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.965316 sdv-1.9.0/docs/sdv_theme/static/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1046 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/sdv_theme/static/slack-32.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.965523 sdv-1.9.0/docs/user_guides/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.966932 sdv-1.9.0/docs/user_guides/benchmarking/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/benchmarking/datasets.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1883 2023-10-13 17:28:40.000000 sdv-1.9.0/docs/user_guides/benchmarking/docker.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      563 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/benchmarking/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2558 2023-10-13 17:28:40.000000 sdv-1.9.0/docs/user_guides/benchmarking/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7764 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/benchmarking/run.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1731 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/benchmarking/synthesizers.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.967675 sdv-1.9.0/docs/user_guides/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3240 2022-12-21 22:30:23.000000 sdv-1.9.0/docs/user_guides/evaluation/evaluation_framework.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      504 2022-12-21 22:30:23.000000 sdv-1.9.0/docs/user_guides/evaluation/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-12-21 22:30:23.000000 sdv-1.9.0/docs/user_guides/evaluation/synthetic_data_metrics.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      277 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.968836 sdv-1.9.0/docs/user_guides/relational/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2131 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/relational/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      141 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/relational/data_description.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8143 2022-12-21 22:30:23.000000 sdv-1.9.0/docs/user_guides/relational/hma1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/relational/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       79 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/relational/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6906 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/relational/relational_metadata.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.971669 sdv-1.9.0/docs/user_guides/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/single_table/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    24765 2023-02-02 20:58:41.000000 sdv-1.9.0/docs/user_guides/single_table/copulagan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18899 2023-02-02 20:58:41.000000 sdv-1.9.0/docs/user_guides/single_table/ctgan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6108 2022-09-22 23:47:45.000000 sdv-1.9.0/docs/user_guides/single_table/custom_constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      121 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/single_table/data_description.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20259 2023-02-02 20:58:41.000000 sdv-1.9.0/docs/user_guides/single_table/gaussian_copula.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14530 2022-09-22 23:47:45.000000 sdv-1.9.0/docs/user_guides/single_table/handling_constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      980 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/single_table/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/single_table/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/single_table/table_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8354 2022-07-22 02:55:50.000000 sdv-1.9.0/docs/user_guides/single_table/tabular_preset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18149 2023-02-02 20:58:41.000000 sdv-1.9.0/docs/user_guides/single_table/tvae.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.972293 sdv-1.9.0/docs/user_guides/timeseries/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       92 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/timeseries/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       78 2022-06-21 19:18:25.000000 sdv-1.9.0/docs/user_guides/timeseries/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14863 2022-12-21 22:30:23.000000 sdv-1.9.0/docs/user_guides/timeseries/par.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.972877 sdv-1.9.0/sdv/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2983 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.974834 sdv-1.9.0/sdv/constraints/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      542 2023-06-07 20:46:09.000000 sdv-1.9.0/sdv/constraints/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18207 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/constraints/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      976 2023-11-07 17:19:09.000000 sdv-1.9.0/sdv/constraints/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    56262 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/constraints/tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6326 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/constraints/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.976252 sdv-1.9.0/sdv/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/data_processing/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    41419 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/data_processing/data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1526 2023-04-20 18:31:25.000000 sdv-1.9.0/sdv/data_processing/datetime_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      522 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/data_processing/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4010 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/data_processing/numerical_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      726 2023-10-23 20:46:20.000000 sdv-1.9.0/sdv/data_processing/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.976859 sdv-1.9.0/sdv/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       43 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7046 2023-12-05 18:40:58.000000 sdv-1.9.0/sdv/datasets/demo.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1333 2023-11-07 17:19:09.000000 sdv-1.9.0/sdv/datasets/local.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1558 2023-11-07 17:19:09.000000 sdv-1.9.0/sdv/errors.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.977453 sdv-1.9.0/sdv/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       49 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/evaluation/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5998 2023-11-16 18:47:09.000000 sdv-1.9.0/sdv/evaluation/multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6918 2023-11-16 18:47:09.000000 sdv-1.9.0/sdv/evaluation/single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.977937 sdv-1.9.0/sdv/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      145 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6955 2023-12-05 18:40:58.000000 sdv-1.9.0/sdv/lite/single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.979620 sdv-1.9.0/sdv/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      400 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      238 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/metadata/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10362 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/metadata/metadata_upgrader.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    40831 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/metadata/multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    39743 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/metadata/single_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      793 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/metadata/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1310 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/metadata/validation.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4084 2023-11-16 18:47:09.000000 sdv-1.9.0/sdv/metadata/visualization.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.980391 sdv-1.9.0/sdv/metrics/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      252 2022-06-21 19:18:25.000000 sdv-1.9.0/sdv/metrics/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-21 19:18:25.000000 sdv-1.9.0/sdv/metrics/demos.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.9.0/sdv/metrics/relational.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-21 19:18:25.000000 sdv-1.9.0/sdv/metrics/tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.9.0/sdv/metrics/timeseries.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.981187 sdv-1.9.0/sdv/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2023-06-07 20:46:09.000000 sdv-1.9.0/sdv/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21521 2023-12-05 18:40:58.000000 sdv-1.9.0/sdv/multi_table/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    24413 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/multi_table/hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.982005 sdv-1.9.0/sdv/sampling/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      302 2023-07-13 19:59:39.000000 sdv-1.9.0/sdv/sampling/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10432 2023-12-05 18:40:58.000000 sdv-1.9.0/sdv/sampling/hierarchical_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6428 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/sampling/independent_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      913 2022-06-21 19:18:25.000000 sdv-1.9.0/sdv/sampling/tabular.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.982938 sdv-1.9.0/sdv/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2023-03-28 20:22:54.000000 sdv-1.9.0/sdv/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14918 2023-12-05 18:40:58.000000 sdv-1.9.0/sdv/sequential/par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.984081 sdv-1.9.0/sdv/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      358 2023-06-07 20:46:09.000000 sdv-1.9.0/sdv/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    41455 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/single_table/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11161 2023-06-07 20:46:09.000000 sdv-1.9.0/sdv/single_table/copulagan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14893 2023-10-13 17:28:40.000000 sdv-1.9.0/sdv/single_table/copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13649 2024-01-11 19:46:44.000000 sdv-1.9.0/sdv/single_table/ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11469 2023-11-07 17:19:09.000000 sdv-1.9.0/sdv/single_table/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6107 2023-11-07 17:19:09.000000 sdv-1.9.0/sdv/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.973846 sdv-1.9.0/sdv.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    97375 2024-01-11 19:46:45.000000 sdv-1.9.0/sdv.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    35812 2024-01-11 19:46:45.000000 sdv-1.9.0/sdv.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-01-11 19:46:45.000000 sdv-1.9.0/sdv.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-01-11 19:46:45.000000 sdv-1.9.0/sdv.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1561 2024-01-11 19:46:45.000000 sdv-1.9.0/sdv.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2024-01-11 19:46:45.000000 sdv-1.9.0/sdv.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1228 2024-01-11 19:46:46.000317 sdv-1.9.0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3895 2024-01-11 19:46:44.000000 sdv-1.9.0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.984447 sdv-1.9.0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.984822 sdv-1.9.0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0/tests/integration/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.985016 sdv-1.9.0/tests/integration/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13887 2023-10-13 17:28:40.000000 sdv-1.9.0/tests/integration/data_processing/test_data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/integration/dataset.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.985394 sdv-1.9.0/tests/integration/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/integration/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3642 2023-11-07 17:19:09.000000 sdv-1.9.0/tests/integration/datasets/test_demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.985910 sdv-1.9.0/tests/integration/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/integration/evaluation/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1709 2023-12-05 18:40:58.000000 sdv-1.9.0/tests/integration/evaluation/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1816 2023-12-05 18:40:58.000000 sdv-1.9.0/tests/integration/evaluation/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.986179 sdv-1.9.0/tests/integration/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.9.0/tests/integration/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1447 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/integration/lite/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.986811 sdv-1.9.0/tests/integration/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/integration/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11178 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/integration/metadata/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11402 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/integration/metadata/test_single_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1470 2023-11-16 18:47:09.000000 sdv-1.9.0/tests/integration/metadata/test_visualization.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.987073 sdv-1.9.0/tests/integration/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/integration/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    44172 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/integration/multi_table/test_hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.987324 sdv-1.9.0/tests/integration/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/integration/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6401 2023-12-05 18:40:58.000000 sdv-1.9.0/tests/integration/sequential/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.988484 sdv-1.9.0/tests/integration/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/integration/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1769 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/integration/single_table/custom_constraints.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14852 2023-10-13 17:28:40.000000 sdv-1.9.0/tests/integration/single_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29183 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/integration/single_table/test_constraints.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15220 2023-11-16 18:47:09.000000 sdv-1.9.0/tests/integration/single_table/test_copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8266 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/integration/single_table/test_ctgan.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.988615 sdv-1.9.0/tests/readme_test/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13973 2022-08-16 22:57:14.000000 sdv-1.9.0/tests/readme_test/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.989951 sdv-1.9.0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.991724 sdv-1.9.0/tests/unit/constraints/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0/tests/unit/constraints/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    32386 2023-08-23 19:41:59.000000 sdv-1.9.0/tests/unit/constraints/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      644 2023-11-07 17:19:09.000000 sdv-1.9.0/tests/unit/constraints/test_errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   165119 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/constraints/test_tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7889 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/constraints/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.992735 sdv-1.9.0/tests/unit/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/unit/data_processing/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    97367 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/data_processing/test_data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2765 2023-04-20 18:31:25.000000 sdv-1.9.0/tests/unit/data_processing/test_datetime_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14718 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/unit/data_processing/test_numerical_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      926 2023-10-23 19:13:19.000000 sdv-1.9.0/tests/unit/data_processing/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.993226 sdv-1.9.0/tests/unit/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/unit/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10856 2023-12-05 18:40:58.000000 sdv-1.9.0/tests/unit/datasets/test_demo.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2516 2023-11-07 17:19:09.000000 sdv-1.9.0/tests/unit/datasets/test_local.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.993687 sdv-1.9.0/tests/unit/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6471 2023-11-16 18:47:09.000000 sdv-1.9.0/tests/unit/evaluation/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    16415 2023-11-16 18:47:09.000000 sdv-1.9.0/tests/unit/evaluation/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.994179 sdv-1.9.0/tests/unit/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0/tests/unit/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9991 2023-12-05 18:40:58.000000 sdv-1.9.0/tests/unit/lite/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.995685 sdv-1.9.0/tests/unit/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0/tests/unit/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22557 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/unit/metadata/test_metadata_upgrader.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   104351 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/metadata/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   100846 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/metadata/test_single_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2726 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/metadata/test_validation.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.996139 sdv-1.9.0/tests/unit/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/unit/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    48373 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/multi_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    38854 2023-11-07 17:19:09.000000 sdv-1.9.0/tests/unit/multi_table/test_hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.997267 sdv-1.9.0/tests/unit/sampling/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.9.0/tests/unit/sampling/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22218 2023-12-05 18:40:58.000000 sdv-1.9.0/tests/unit/sampling/test_hierarchical_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15667 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/sampling/test_independent_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2140 2022-06-21 19:18:25.000000 sdv-1.9.0/tests/unit/sampling/test_tabular.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.998033 sdv-1.9.0/tests/unit/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/unit/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30363 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/sequential/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 19:46:45.999611 sdv-1.9.0/tests/unit/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0/tests/unit/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    66221 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/single_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13803 2023-06-07 20:46:09.000000 sdv-1.9.0/tests/unit/single_table/test_copulagan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18091 2023-05-10 21:10:34.000000 sdv-1.9.0/tests/unit/single_table/test_copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15823 2024-01-11 19:46:44.000000 sdv-1.9.0/tests/unit/single_table/test_ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10041 2023-11-07 17:19:09.000000 sdv-1.9.0/tests/unit/single_table/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4604 2023-06-07 20:46:09.000000 sdv-1.9.0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2023-11-07 17:19:09.000000 sdv-1.9.0/tests/unit/test_errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6113 2023-10-13 17:28:40.000000 sdv-1.9.0/tests/unit/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3051 2023-05-10 21:10:34.000000 sdv-1.9.0/tests/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.991531 sdv-1.9.0.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-24 21:06:49.000000 sdv-1.9.0.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8104 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    84401 2024-01-11 17:29:02.000000 sdv-1.9.0.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4818 2023-01-24 21:06:49.000000 sdv-1.9.0.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    95224 2024-01-11 17:29:54.991752 sdv-1.9.0.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9787 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.867658 sdv-1.9.0.dev0/docs/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/Makefile
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.869126 sdv-1.9.0.dev0/docs/api_reference/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.869882 sdv-1.9.0.dev0/docs/api_reference/constraints/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.888561 sdv-1.9.0.dev0/docs/api_reference/constraints/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      666 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      627 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      117 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      131 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      588 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      523 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      359 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/base.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2609 2022-07-22 02:55:50.000000 sdv-1.9.0.dev0/docs/api_reference/constraints/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      353 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/evaluation.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2022-07-22 02:55:50.000000 sdv-1.9.0.dev0/docs/api_reference/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.888978 sdv-1.9.0.dev0/docs/api_reference/lite/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.890464 sdv-1.9.0.dev0/docs/api_reference/lite/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      205 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.list_available_presets.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      502 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.9.0.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       94 2022-07-22 02:55:50.000000 sdv-1.9.0.dev0/docs/api_reference/lite/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      348 2022-07-22 02:55:50.000000 sdv-1.9.0.dev0/docs/api_reference/lite/tabular.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.891230 sdv-1.9.0.dev0/docs/api_reference/metadata/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.899061 sdv-1.9.0.dev0/docs/api_reference/metadata/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_field.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_relationship.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_children.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_dtypes.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_field_meta.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_fields.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_foreign_keys.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_parents.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_table_meta.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_tables.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_tables.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      877 2022-09-29 22:36:12.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.set_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.validate.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.visualize.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_dtypes.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_fields.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_model_kwargs.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      668 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_model_kwargs.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      854 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/dataset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      116 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      583 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/metadata/table.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.900129 sdv-1.9.0.dev0/docs/api_reference/metrics/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.928319 sdv-1.9.0.dev0/docs/api_reference/metrics/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_multi_table_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_single_table_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_timeseries_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:23.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      614 2022-08-30 22:45:23.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      506 2022-08-30 22:45:24.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-08-30 23:02:40.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-08-30 23:02:40.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 23:02:40.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-08-30 23:02:15.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-08-30 23:02:15.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      534 2022-08-30 23:02:15.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      638 2022-08-30 22:45:24.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      242 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2022-08-30 22:45:24.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      236 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      582 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:24.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      204 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      661 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      210 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      897 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      811 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      762 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      565 2022-08-30 22:45:24.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      734 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      818 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      842 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      720 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      192 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      788 2022-10-05 00:20:25.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      760 2022-10-05 00:20:25.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-08-30 23:02:40.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-08-30 23:02:40.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      649 2022-08-30 23:02:40.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-08-30 23:02:15.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-08-30 23:02:15.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-08-30 23:02:15.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      717 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      657 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      688 2022-10-05 00:20:25.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      701 2022-08-30 22:45:24.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      957 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      195 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      822 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      819 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      239 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      895 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      257 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      857 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      551 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      683 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      230 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      672 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      213 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/demos.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1402 2022-09-22 23:47:45.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/relational.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4109 2022-09-22 23:47:45.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      735 2022-12-21 22:30:23.000000 sdv-1.9.0.dev0/docs/api_reference/metrics/timeseries.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.928741 sdv-1.9.0.dev0/docs/api_reference/relational/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.930178 sdv-1.9.0.dev0/docs/api_reference/relational/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      416 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/relational/hma1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/relational/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.930695 sdv-1.9.0.dev0/docs/api_reference/sampling/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.931204 sdv-1.9.0.dev0/docs/api_reference/sampling/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_column_values.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      151 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_num_rows.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      417 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/sampling/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/sampling/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/sdv.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.932034 sdv-1.9.0.dev0/docs/api_reference/tabular/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.939515 sdv-1.9.0.dev0/docs/api_reference/tabular/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_distributions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      655 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_distributions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_likelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_parameters.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      663 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.set_parameters.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      450 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      129 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      187 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      339 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/copulagan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      489 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/copulas.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      260 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/ctgan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      136 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      249 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/tabular/tvae.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.940044 sdv-1.9.0.dev0/docs/api_reference/timeseries/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.941232 sdv-1.9.0.dev0/docs/api_reference/timeseries/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      338 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.9.0.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      108 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/timeseries/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/api_reference/timeseries/par.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6932 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/docs/conf.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.941923 sdv-1.9.0.dev0/docs/developer_guides/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8607 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/docs/developer_guides/contributing.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      364 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/developer_guides/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2905 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/developer_guides/overview.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.943296 sdv-1.9.0.dev0/docs/developer_guides/sdv/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5889 2022-07-22 02:55:50.000000 sdv-1.9.0.dev0/docs/developer_guides/sdv/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      292 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/developer_guides/sdv/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7480 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/developer_guides/sdv/metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9508 2023-02-02 20:58:41.000000 sdv-1.9.0.dev0/docs/developer_guides/sdv/tabular.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.944037 sdv-1.9.0.dev0/docs/getting_started/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      113 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/getting_started/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2555 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/docs/getting_started/install.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3664 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/getting_started/quickstart.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/history.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.955534 sdv-1.9.0.dev0/docs/images/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    52078 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/CTGAN-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50900 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/Copulas-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60600 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/DataCebo-Blue.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    54065 2023-04-20 22:38:57.000000 sdv-1.9.0.dev0/docs/images/DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    46250 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/DeepEcho-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25573 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/RDT-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   243101 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/docs/images/Real-vs-Synthetic-Evaluation.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27285 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/SDGym-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    35670 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/SDMetrics-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17776 2023-12-06 18:41:03.000000 sdv-1.9.0.dev0/docs/images/SDV-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67366 2023-12-06 18:41:03.000000 sdv-1.9.0.dev0/docs/images/SDV-logo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8765 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/SDV.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   412158 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/docs/images/Single-Table-Metadata-Example.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    99815 2022-07-22 02:55:50.000000 sdv-1.9.0.dev0/docs/images/custom_constraint.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50140 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/docs/images/datacebo-logo-dark-mode.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50481 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/docs/images/datacebo-logo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      547 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/google_colab.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.9.0.dev0/docs/images/hma1_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8748 2022-12-08 23:36:42.000000 sdv-1.9.0.dev0/docs/images/metadata_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67425 2022-12-08 23:36:42.000000 sdv-1.9.0.dev0/docs/images/metadata_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2497 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/mybinder.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.9.0.dev0/docs/images/quickstart_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   176980 2023-01-24 21:06:49.000000 sdv-1.9.0.dev0/docs/images/rdt_main_tranformation.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2283 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/images/slack.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6069 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/docs/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      765 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/make.bat
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.957920 sdv-1.9.0.dev0/docs/savefig/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:00:09.000000 sdv-1.9.0.dev0/docs/savefig/copulagan_experience_years_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12668 2022-12-08 23:00:10.000000 sdv-1.9.0.dev0/docs/savefig/copulagan_experience_years_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10277 2022-12-08 23:00:37.000000 sdv-1.9.0.dev0/docs/savefig/copulagan_experience_years_3.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:05:15.000000 sdv-1.9.0.dev0/docs/savefig/experience_years_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10270 2022-12-08 23:05:16.000000 sdv-1.9.0.dev0/docs/savefig/experience_years_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12415 2022-12-08 23:05:16.000000 sdv-1.9.0.dev0/docs/savefig/experience_years_3.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.861299 sdv-1.9.0.dev0/docs/sdv_theme/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.958210 sdv-1.9.0.dev0/docs/sdv_theme/static/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1046 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/sdv_theme/static/slack-32.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.958452 sdv-1.9.0.dev0/docs/user_guides/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.959932 sdv-1.9.0.dev0/docs/user_guides/benchmarking/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/benchmarking/datasets.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1883 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/docs/user_guides/benchmarking/docker.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      563 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/benchmarking/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2558 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/docs/user_guides/benchmarking/install.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7764 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/benchmarking/run.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1731 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/benchmarking/synthesizers.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.960678 sdv-1.9.0.dev0/docs/user_guides/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3240 2022-12-21 22:30:23.000000 sdv-1.9.0.dev0/docs/user_guides/evaluation/evaluation_framework.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      504 2022-12-21 22:30:23.000000 sdv-1.9.0.dev0/docs/user_guides/evaluation/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-12-21 22:30:23.000000 sdv-1.9.0.dev0/docs/user_guides/evaluation/synthetic_data_metrics.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      277 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.961800 sdv-1.9.0.dev0/docs/user_guides/relational/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2131 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/relational/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      141 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/relational/data_description.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8143 2022-12-21 22:30:23.000000 sdv-1.9.0.dev0/docs/user_guides/relational/hma1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/relational/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       79 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/relational/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6906 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/relational/relational_metadata.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.964548 sdv-1.9.0.dev0/docs/user_guides/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    24765 2023-02-02 20:58:41.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/copulagan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18899 2023-02-02 20:58:41.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/ctgan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6108 2022-09-22 23:47:45.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/custom_constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      121 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/data_description.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20259 2023-02-02 20:58:41.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/gaussian_copula.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14530 2022-09-22 23:47:45.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/handling_constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      980 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/table_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8354 2022-07-22 02:55:50.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/tabular_preset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18149 2023-02-02 20:58:41.000000 sdv-1.9.0.dev0/docs/user_guides/single_table/tvae.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.965157 sdv-1.9.0.dev0/docs/user_guides/timeseries/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       92 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/timeseries/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       78 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/docs/user_guides/timeseries/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14863 2022-12-21 22:30:23.000000 sdv-1.9.0.dev0/docs/user_guides/timeseries/par.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.965729 sdv-1.9.0.dev0/sdv/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2988 2024-01-11 17:29:40.000000 sdv-1.9.0.dev0/sdv/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.967827 sdv-1.9.0.dev0/sdv/constraints/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      542 2023-06-07 20:46:09.000000 sdv-1.9.0.dev0/sdv/constraints/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18207 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/sdv/constraints/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      976 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/sdv/constraints/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    56262 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/sdv/constraints/tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6326 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/sdv/constraints/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.969209 sdv-1.9.0.dev0/sdv/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/data_processing/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    41419 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/sdv/data_processing/data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1526 2023-04-20 18:31:25.000000 sdv-1.9.0.dev0/sdv/data_processing/datetime_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      522 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/data_processing/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4010 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/data_processing/numerical_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      726 2023-10-23 20:46:20.000000 sdv-1.9.0.dev0/sdv/data_processing/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.969808 sdv-1.9.0.dev0/sdv/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       43 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7046 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/sdv/datasets/demo.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1333 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/sdv/datasets/local.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1558 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/sdv/errors.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.970401 sdv-1.9.0.dev0/sdv/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       49 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/evaluation/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5998 2023-11-16 18:47:09.000000 sdv-1.9.0.dev0/sdv/evaluation/multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6918 2023-11-16 18:47:09.000000 sdv-1.9.0.dev0/sdv/evaluation/single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.970948 sdv-1.9.0.dev0/sdv/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      145 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6955 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/sdv/lite/single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.973089 sdv-1.9.0.dev0/sdv/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      400 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      238 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/metadata/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10362 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/metadata/metadata_upgrader.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    40831 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/sdv/metadata/multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    39743 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/sdv/metadata/single_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      793 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/metadata/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1310 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/sdv/metadata/validation.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4084 2023-11-16 18:47:09.000000 sdv-1.9.0.dev0/sdv/metadata/visualization.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.973908 sdv-1.9.0.dev0/sdv/metrics/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      252 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/sdv/metrics/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/sdv/metrics/demos.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/sdv/metrics/relational.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/sdv/metrics/tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/sdv/metrics/timeseries.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.974578 sdv-1.9.0.dev0/sdv/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2023-06-07 20:46:09.000000 sdv-1.9.0.dev0/sdv/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21521 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/sdv/multi_table/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    24413 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/sdv/multi_table/hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.975429 sdv-1.9.0.dev0/sdv/sampling/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      302 2023-07-13 19:59:39.000000 sdv-1.9.0.dev0/sdv/sampling/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10432 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/sdv/sampling/hierarchical_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6428 2023-12-18 21:51:01.000000 sdv-1.9.0.dev0/sdv/sampling/independent_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      913 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/sdv/sampling/tabular.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.975854 sdv-1.9.0.dev0/sdv/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/sdv/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14918 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/sdv/sequential/par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.977189 sdv-1.9.0.dev0/sdv/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      358 2023-06-07 20:46:09.000000 sdv-1.9.0.dev0/sdv/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    41455 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/sdv/single_table/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11161 2023-06-07 20:46:09.000000 sdv-1.9.0.dev0/sdv/single_table/copulagan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14893 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/sdv/single_table/copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13649 2023-12-18 21:51:01.000000 sdv-1.9.0.dev0/sdv/single_table/ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11469 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/sdv/single_table/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6107 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/sdv/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.966932 sdv-1.9.0.dev0/sdv.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    95224 2024-01-11 17:29:54.000000 sdv-1.9.0.dev0/sdv.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    35812 2024-01-11 17:29:54.000000 sdv-1.9.0.dev0/sdv.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-01-11 17:29:54.000000 sdv-1.9.0.dev0/sdv.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-01-11 17:29:54.000000 sdv-1.9.0.dev0/sdv.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1561 2024-01-11 17:29:54.000000 sdv-1.9.0.dev0/sdv.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2024-01-11 17:29:54.000000 sdv-1.9.0.dev0/sdv.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1233 2024-01-11 17:29:54.992141 sdv-1.9.0.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3900 2024-01-11 17:29:40.000000 sdv-1.9.0.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.977547 sdv-1.9.0.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/tests/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.977902 sdv-1.9.0.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/tests/integration/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.978145 sdv-1.9.0.dev0/tests/integration/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13887 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/tests/integration/data_processing/test_data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/integration/dataset.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.978511 sdv-1.9.0.dev0/tests/integration/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/integration/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3642 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/tests/integration/datasets/test_demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.979014 sdv-1.9.0.dev0/tests/integration/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/integration/evaluation/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1709 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/tests/integration/evaluation/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1816 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/tests/integration/evaluation/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.979265 sdv-1.9.0.dev0/tests/integration/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.9.0.dev0/tests/integration/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1447 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/integration/lite/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.979939 sdv-1.9.0.dev0/tests/integration/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/integration/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11178 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/tests/integration/metadata/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11402 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/tests/integration/metadata/test_single_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1470 2023-11-16 18:47:09.000000 sdv-1.9.0.dev0/tests/integration/metadata/test_visualization.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.980211 sdv-1.9.0.dev0/tests/integration/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/integration/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    44172 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/tests/integration/multi_table/test_hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.980543 sdv-1.9.0.dev0/tests/integration/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/integration/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6401 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/tests/integration/sequential/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.981679 sdv-1.9.0.dev0/tests/integration/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/integration/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1769 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/integration/single_table/custom_constraints.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14852 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/tests/integration/single_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29183 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/tests/integration/single_table/test_constraints.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    15220 2023-11-16 18:47:09.000000 sdv-1.9.0.dev0/tests/integration/single_table/test_copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8266 2023-12-18 21:51:01.000000 sdv-1.9.0.dev0/tests/integration/single_table/test_ctgan.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.981945 sdv-1.9.0.dev0/tests/readme_test/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13973 2022-08-16 22:57:14.000000 sdv-1.9.0.dev0/tests/readme_test/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.982757 sdv-1.9.0.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.984034 sdv-1.9.0.dev0/tests/unit/constraints/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/tests/unit/constraints/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    32386 2023-08-23 19:41:59.000000 sdv-1.9.0.dev0/tests/unit/constraints/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      644 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/tests/unit/constraints/test_errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   165119 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/tests/unit/constraints/test_tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7889 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/tests/unit/constraints/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.984923 sdv-1.9.0.dev0/tests/unit/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/unit/data_processing/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    97367 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/tests/unit/data_processing/test_data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2765 2023-04-20 18:31:25.000000 sdv-1.9.0.dev0/tests/unit/data_processing/test_datetime_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14718 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/unit/data_processing/test_numerical_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      926 2023-10-23 19:13:19.000000 sdv-1.9.0.dev0/tests/unit/data_processing/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.985405 sdv-1.9.0.dev0/tests/unit/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/unit/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10856 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/tests/unit/datasets/test_demo.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2516 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/tests/unit/datasets/test_local.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.985886 sdv-1.9.0.dev0/tests/unit/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6471 2023-11-16 18:47:09.000000 sdv-1.9.0.dev0/tests/unit/evaluation/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    16415 2023-11-16 18:47:09.000000 sdv-1.9.0.dev0/tests/unit/evaluation/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.986341 sdv-1.9.0.dev0/tests/unit/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/tests/unit/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9991 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/tests/unit/lite/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.987879 sdv-1.9.0.dev0/tests/unit/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/tests/unit/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22557 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/unit/metadata/test_metadata_upgrader.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   104351 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/tests/unit/metadata/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   100846 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/tests/unit/metadata/test_single_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2726 2024-01-10 21:31:54.000000 sdv-1.9.0.dev0/tests/unit/metadata/test_validation.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.988278 sdv-1.9.0.dev0/tests/unit/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/unit/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    48373 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/tests/unit/multi_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    38854 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/tests/unit/multi_table/test_hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.989452 sdv-1.9.0.dev0/tests/unit/sampling/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.9.0.dev0/tests/unit/sampling/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22218 2023-12-05 18:40:58.000000 sdv-1.9.0.dev0/tests/unit/sampling/test_hierarchical_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    15667 2023-12-18 21:51:01.000000 sdv-1.9.0.dev0/tests/unit/sampling/test_independent_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2140 2022-06-21 19:18:25.000000 sdv-1.9.0.dev0/tests/unit/sampling/test_tabular.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.989946 sdv-1.9.0.dev0/tests/unit/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/unit/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30363 2023-12-18 21:51:01.000000 sdv-1.9.0.dev0/tests/unit/sequential/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-01-11 17:29:54.991382 sdv-1.9.0.dev0/tests/unit/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.9.0.dev0/tests/unit/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    66221 2024-01-11 17:29:06.000000 sdv-1.9.0.dev0/tests/unit/single_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13803 2023-06-07 20:46:09.000000 sdv-1.9.0.dev0/tests/unit/single_table/test_copulagan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18091 2023-05-10 21:10:34.000000 sdv-1.9.0.dev0/tests/unit/single_table/test_copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    15823 2023-12-18 21:51:01.000000 sdv-1.9.0.dev0/tests/unit/single_table/test_ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10041 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/tests/unit/single_table/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4604 2023-06-07 20:46:09.000000 sdv-1.9.0.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2023-11-07 17:19:09.000000 sdv-1.9.0.dev0/tests/unit/test_errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6113 2023-10-13 17:28:40.000000 sdv-1.9.0.dev0/tests/unit/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3051 2023-05-10 21:10:34.000000 sdv-1.9.0.dev0/tests/utils.py
```

### Comparing `sdv-1.9.0/CONTRIBUTING.rst` & `sdv-1.9.0.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/HISTORY.md` & `sdv-1.9.0.dev0/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 # Release Notes
 
-## 1.9.0 - 2024-01-11
-
-This release makes a number of improvements. It introduces a new concept to the metadata known as column relationships! Column relationships can be used to define when certain groups of columns in a table should be treated as a special concept (eg. address). You can add a column relationship by using the new `add_column_relationship` method. The metadata detection was also improved by allowing semantic sdtypes (eg. 'email', 'phone_number') to be detected as primary keys.
-
-This release also patches some bugs. An issue messing up the likelihood matching in the `HMASynthesizer` was resolved. The `CTGANSynthesizer` no longer fails when using the `FixedCombinations` constraint. The `Inequality` constraint was also patched to handle datetimes better.
-
-### Deprecations
-
-* The `set_address_columns` method is deprecated in favor of `add_column_relationship`.
-
-### New Features
-
-* Improve error messages for composite keys - Issue [#1684](https://github.com/sdv-dev/SDV/issues/1684) by @frances-h
-* Add column relationship validation to single table metadata - Issue [#1698](https://github.com/sdv-dev/SDV/issues/1698) by @frances-h
-* Add add_column_relationship method to single table metadata - Issue [#1699](https://github.com/sdv-dev/SDV/issues/1699) by @frances-h
-* Make synthesizers work with column_relationships - Issue [#1700](https://github.com/sdv-dev/SDV/issues/1700) by @R-Palazzo
-* Metadata auto-detection should find primary keys of semantic sdtypes - Issue [#1724](https://github.com/sdv-dev/SDV/issues/1724) by @fealho
-
-### Bugs Fixed
-
-* InvalidDataError for Inequality constraint (even though data is valid) - Issue [#1692](https://github.com/sdv-dev/SDV/issues/1692) by @fealho
-* `BaseIndependentSampler` crashes because it tries to cast id columns - Issue [#1712](https://github.com/sdv-dev/SDV/issues/1712) by @pvk-developer
-* KeyError in `CTGANSynthesizer` when applying `FixedCombinations` constraint - Issue [#1717](https://github.com/sdv-dev/SDV/issues/1717) by @pvk-developer
-* Fix _get_likelihoods not generating likelihood values - Issue [#1720](https://github.com/sdv-dev/SDV/pull/1720) by @frances-h
-
 ## 1.8.0 - 2023-12-05
 
 This release adds support for the new Diagnostic Report from SDMetrics. This report calculates scores for three basic but important properties of your data: data validity, data structure and in the multi table case, relationship validity. Data validity checks that the columns of your data are valid (eg. correct range or values). Data structure makes sure the synthetic data has the correct columns. Relationship validity checks to make sure key references are correct and the cardinality is within ranges seen in the real data.
 
 Additionally, a few bugs were fixed and functionality was improved around synthesizers. It is now possible to access the loss values for the `TVAESynthesizer` and `CTGANSynthesizer` by using the `get_loss_values` method. The `get_parameters` method is now more detailed and returns all the parameters used to make a synthesizer. The metadata is now capable of detecting some common pii sdtypes. Finally, a bug that made every parent row generated by the `HMASynthesizer` have at least one child row was patched. This should improve cardinality.
 
 ### Maintenance
```

### Comparing `sdv-1.9.0/LICENSE` & `sdv-1.9.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/PKG-INFO` & `sdv-1.9.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdv
-Version: 1.9.0
+Version: 1.9.0.dev0
 Summary: Generate synthetic data for single table, multi table and sequential data
 Home-page: https://github.com/sdv-dev/SDV
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: sdv synthetic-data synhtetic-data-generation timeseries single-table multi-table
 Classifier: Development Status :: 5 - Production/Stable
@@ -242,39 +242,14 @@
 [Get started using the SDV package](https://bit.ly/sdv-docs) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # Release Notes
 
-## 1.9.0 - 2024-01-11
-
-This release makes a number of improvements. It introduces a new concept to the metadata known as column relationships! Column relationships can be used to define when certain groups of columns in a table should be treated as a special concept (eg. address). You can add a column relationship by using the new `add_column_relationship` method. The metadata detection was also improved by allowing semantic sdtypes (eg. 'email', 'phone_number') to be detected as primary keys.
-
-This release also patches some bugs. An issue messing up the likelihood matching in the `HMASynthesizer` was resolved. The `CTGANSynthesizer` no longer fails when using the `FixedCombinations` constraint. The `Inequality` constraint was also patched to handle datetimes better.
-
-### Deprecations
-
-* The `set_address_columns` method is deprecated in favor of `add_column_relationship`.
-
-### New Features
-
-* Improve error messages for composite keys - Issue [#1684](https://github.com/sdv-dev/SDV/issues/1684) by @frances-h
-* Add column relationship validation to single table metadata - Issue [#1698](https://github.com/sdv-dev/SDV/issues/1698) by @frances-h
-* Add add_column_relationship method to single table metadata - Issue [#1699](https://github.com/sdv-dev/SDV/issues/1699) by @frances-h
-* Make synthesizers work with column_relationships - Issue [#1700](https://github.com/sdv-dev/SDV/issues/1700) by @R-Palazzo
-* Metadata auto-detection should find primary keys of semantic sdtypes - Issue [#1724](https://github.com/sdv-dev/SDV/issues/1724) by @fealho
-
-### Bugs Fixed
-
-* InvalidDataError for Inequality constraint (even though data is valid) - Issue [#1692](https://github.com/sdv-dev/SDV/issues/1692) by @fealho
-* `BaseIndependentSampler` crashes because it tries to cast id columns - Issue [#1712](https://github.com/sdv-dev/SDV/issues/1712) by @pvk-developer
-* KeyError in `CTGANSynthesizer` when applying `FixedCombinations` constraint - Issue [#1717](https://github.com/sdv-dev/SDV/issues/1717) by @pvk-developer
-* Fix _get_likelihoods not generating likelihood values - Issue [#1720](https://github.com/sdv-dev/SDV/pull/1720) by @frances-h
-
 ## 1.8.0 - 2023-12-05
 
 This release adds support for the new Diagnostic Report from SDMetrics. This report calculates scores for three basic but important properties of your data: data validity, data structure and in the multi table case, relationship validity. Data validity checks that the columns of your data are valid (eg. correct range or values). Data structure makes sure the synthetic data has the correct columns. Relationship validity checks to make sure key references are correct and the cardinality is within ranges seen in the real data.
 
 Additionally, a few bugs were fixed and functionality was improved around synthesizers. It is now possible to access the loss values for the `TVAESynthesizer` and `CTGANSynthesizer` by using the `get_loss_values` method. The `get_parameters` method is now more detailed and returns all the parameters used to make a synthesizer. The metadata is now capable of detecting some common pii sdtypes. Finally, a bug that made every parent row generated by the `HMASynthesizer` have at least one child row was patched. This should improve cardinality.
 
 ### Maintenance
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: sdv Version: 1.9.0 Summary: Generate synthetic data
-for single table, multi table and sequential data Home-page: https://
+Metadata-Version: 2.1 Name: sdv Version: 1.9.0.dev0 Summary: Generate synthetic
+data for single table, multi table and sequential data Home-page: https://
 github.com/sdv-dev/SDV Author: DataCebo, Inc. Author-email: info@sdv.dev
 License: BSL-1.1 Keywords: sdv synthetic-data synhtetic-data-generation
 timeseries single-table multi-table Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Free for non-commercial use Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -131,51 +131,22 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://bit.ly/sdv-docs) -- a fully integrated solution and your one-stop shop
 for synthetic data. Or, use the standalone libraries for specific needs. #
-Release Notes ## 1.9.0 - 2024-01-11 This release makes a number of
-improvements. It introduces a new concept to the metadata known as column
-relationships! Column relationships can be used to define when certain groups
-of columns in a table should be treated as a special concept (eg. address). You
-can add a column relationship by using the new `add_column_relationship`
-method. The metadata detection was also improved by allowing semantic sdtypes
-(eg. 'email', 'phone_number') to be detected as primary keys. This release also
-patches some bugs. An issue messing up the likelihood matching in the
-`HMASynthesizer` was resolved. The `CTGANSynthesizer` no longer fails when
-using the `FixedCombinations` constraint. The `Inequality` constraint was also
-patched to handle datetimes better. ### Deprecations * The
-`set_address_columns` method is deprecated in favor of
-`add_column_relationship`. ### New Features * Improve error messages for
-composite keys - Issue [#1684](https://github.com/sdv-dev/SDV/issues/1684) by
-@frances-h * Add column relationship validation to single table metadata -
-Issue [#1698](https://github.com/sdv-dev/SDV/issues/1698) by @frances-h * Add
-add_column_relationship method to single table metadata - Issue [#1699](https:/
-/github.com/sdv-dev/SDV/issues/1699) by @frances-h * Make synthesizers work
-with column_relationships - Issue [#1700](https://github.com/sdv-dev/SDV/
-issues/1700) by @R-Palazzo * Metadata auto-detection should find primary keys
-of semantic sdtypes - Issue [#1724](https://github.com/sdv-dev/SDV/issues/1724)
-by @fealho ### Bugs Fixed * InvalidDataError for Inequality constraint (even
-though data is valid) - Issue [#1692](https://github.com/sdv-dev/SDV/issues/
-1692) by @fealho * `BaseIndependentSampler` crashes because it tries to cast id
-columns - Issue [#1712](https://github.com/sdv-dev/SDV/issues/1712) by @pvk-
-developer * KeyError in `CTGANSynthesizer` when applying `FixedCombinations`
-constraint - Issue [#1717](https://github.com/sdv-dev/SDV/issues/1717) by @pvk-
-developer * Fix _get_likelihoods not generating likelihood values - Issue
-[#1720](https://github.com/sdv-dev/SDV/pull/1720) by @frances-h ## 1.8.0 -
-2023-12-05 This release adds support for the new Diagnostic Report from
-SDMetrics. This report calculates scores for three basic but important
-properties of your data: data validity, data structure and in the multi table
-case, relationship validity. Data validity checks that the columns of your data
-are valid (eg. correct range or values). Data structure makes sure the
-synthetic data has the correct columns. Relationship validity checks to make
-sure key references are correct and the cardinality is within ranges seen in
-the real data. Additionally, a few bugs were fixed and functionality was
+Release Notes ## 1.8.0 - 2023-12-05 This release adds support for the new
+Diagnostic Report from SDMetrics. This report calculates scores for three basic
+but important properties of your data: data validity, data structure and in the
+multi table case, relationship validity. Data validity checks that the columns
+of your data are valid (eg. correct range or values). Data structure makes sure
+the synthetic data has the correct columns. Relationship validity checks to
+make sure key references are correct and the cardinality is within ranges seen
+in the real data. Additionally, a few bugs were fixed and functionality was
 improved around synthesizers. It is now possible to access the loss values for
 the `TVAESynthesizer` and `CTGANSynthesizer` by using the `get_loss_values`
 method. The `get_parameters` method is now more detailed and returns all the
 parameters used to make a synthesizer. The metadata is now capable of detecting
 some common pii sdtypes. Finally, a bug that made every parent row generated by
 the `HMASynthesizer` have at least one child row was patched. This should
 improve cardinality. ### Maintenance * Address `SettingWithCopyWarning`
```

### Comparing `sdv-1.9.0/README.md` & `sdv-1.9.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/Makefile` & `sdv-1.9.0.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/constraints/tabular.rst` & `sdv-1.9.0.dev0/docs/api_reference/constraints/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst` & `sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst` & `sdv-1.9.0.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metadata/dataset.rst` & `sdv-1.9.0.dev0/docs/api_reference/metadata/dataset.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metadata/table.rst` & `sdv-1.9.0.dev0/docs/api_reference/metadata/table.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/relational.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/relational.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/tabular.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/metrics/timeseries.rst` & `sdv-1.9.0.dev0/docs/api_reference/metrics/timeseries.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst` & `sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst` & `sdv-1.9.0.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/conf.py` & `sdv-1.9.0.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/developer_guides/contributing.rst` & `sdv-1.9.0.dev0/docs/developer_guides/contributing.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/developer_guides/overview.rst` & `sdv-1.9.0.dev0/docs/developer_guides/overview.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/developer_guides/sdv/constraints.rst` & `sdv-1.9.0.dev0/docs/developer_guides/sdv/constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/developer_guides/sdv/metadata.rst` & `sdv-1.9.0.dev0/docs/developer_guides/sdv/metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/developer_guides/sdv/tabular.rst` & `sdv-1.9.0.dev0/docs/developer_guides/sdv/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/getting_started/install.rst` & `sdv-1.9.0.dev0/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/getting_started/quickstart.rst` & `sdv-1.9.0.dev0/docs/getting_started/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/DataCebo-Blue.png` & `sdv-1.9.0.dev0/docs/images/DataCebo-Blue.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/Real-vs-Synthetic-Evaluation.png` & `sdv-1.9.0.dev0/docs/images/Real-vs-Synthetic-Evaluation.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/SDV-DataCebo.png` & `sdv-1.9.0.dev0/docs/images/SDV-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/SDV-logo.png` & `sdv-1.9.0.dev0/docs/images/SDV-logo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/SDV.png` & `sdv-1.9.0.dev0/docs/images/SDV.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/Single-Table-Metadata-Example.png` & `sdv-1.9.0.dev0/docs/images/Single-Table-Metadata-Example.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/custom_constraint.png` & `sdv-1.9.0.dev0/docs/images/custom_constraint.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/datacebo-logo-dark-mode.png` & `sdv-1.9.0.dev0/docs/images/datacebo-logo-dark-mode.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/google_colab.png` & `sdv-1.9.0.dev0/docs/images/google_colab.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/hma1_1.png` & `sdv-1.9.0.dev0/docs/images/hma1_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/metadata_1.png` & `sdv-1.9.0.dev0/docs/images/metadata_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/metadata_2.png` & `sdv-1.9.0.dev0/docs/images/metadata_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/mybinder.png` & `sdv-1.9.0.dev0/docs/images/mybinder.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/quickstart_1.png` & `sdv-1.9.0.dev0/docs/images/quickstart_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/rdt_main_tranformation.png` & `sdv-1.9.0.dev0/docs/images/rdt_main_tranformation.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/images/slack.png` & `sdv-1.9.0.dev0/docs/images/slack.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/index.rst` & `sdv-1.9.0.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/make.bat` & `sdv-1.9.0.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/savefig/copulagan_experience_years_1.png` & `sdv-1.9.0.dev0/docs/savefig/copulagan_experience_years_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/savefig/copulagan_experience_years_2.png` & `sdv-1.9.0.dev0/docs/savefig/copulagan_experience_years_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/savefig/copulagan_experience_years_3.png` & `sdv-1.9.0.dev0/docs/savefig/copulagan_experience_years_3.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/savefig/experience_years_1.png` & `sdv-1.9.0.dev0/docs/savefig/experience_years_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/savefig/experience_years_2.png` & `sdv-1.9.0.dev0/docs/savefig/experience_years_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/savefig/experience_years_3.png` & `sdv-1.9.0.dev0/docs/savefig/experience_years_3.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/sdv_theme/static/slack-32.png` & `sdv-1.9.0.dev0/docs/sdv_theme/static/slack-32.png`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/benchmarking/datasets.rst` & `sdv-1.9.0.dev0/docs/user_guides/benchmarking/datasets.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/benchmarking/docker.rst` & `sdv-1.9.0.dev0/docs/user_guides/benchmarking/docker.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/benchmarking/index.rst` & `sdv-1.9.0.dev0/docs/user_guides/benchmarking/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/benchmarking/install.rst` & `sdv-1.9.0.dev0/docs/user_guides/benchmarking/install.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/benchmarking/run.rst` & `sdv-1.9.0.dev0/docs/user_guides/benchmarking/run.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/benchmarking/synthesizers.rst` & `sdv-1.9.0.dev0/docs/user_guides/benchmarking/synthesizers.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/evaluation/evaluation_framework.rst` & `sdv-1.9.0.dev0/docs/user_guides/evaluation/evaluation_framework.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/relational/constraints.rst` & `sdv-1.9.0.dev0/docs/user_guides/relational/constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/relational/hma1.rst` & `sdv-1.9.0.dev0/docs/user_guides/relational/hma1.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/relational/relational_metadata.rst` & `sdv-1.9.0.dev0/docs/user_guides/relational/relational_metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/single_table/copulagan.rst` & `sdv-1.9.0.dev0/docs/user_guides/single_table/copulagan.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/single_table/ctgan.rst` & `sdv-1.9.0.dev0/docs/user_guides/single_table/ctgan.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/single_table/custom_constraints.rst` & `sdv-1.9.0.dev0/docs/user_guides/single_table/custom_constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/single_table/gaussian_copula.rst` & `sdv-1.9.0.dev0/docs/user_guides/single_table/gaussian_copula.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/single_table/handling_constraints.rst` & `sdv-1.9.0.dev0/docs/user_guides/single_table/handling_constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/single_table/index.rst` & `sdv-1.9.0.dev0/docs/user_guides/single_table/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/single_table/tabular_preset.rst` & `sdv-1.9.0.dev0/docs/user_guides/single_table/tabular_preset.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/single_table/tvae.rst` & `sdv-1.9.0.dev0/docs/user_guides/single_table/tvae.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/docs/user_guides/timeseries/par.rst` & `sdv-1.9.0.dev0/docs/user_guides/timeseries/par.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/__init__.py` & `sdv-1.9.0.dev0/sdv/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # configure logging for the library with a null handler (nothing is printed by default). See
 # http://docs.python-guide.org/en/latest/writing/logging/
 
 """Top-level package for SDV."""
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.9.0'
+__version__ = '1.9.0.dev0'
 
 
 import sys
 import warnings
 from operator import attrgetter
 
 from pkg_resources import iter_entry_points
```

### Comparing `sdv-1.9.0/sdv/constraints/__init__.py` & `sdv-1.9.0.dev0/sdv/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/constraints/base.py` & `sdv-1.9.0.dev0/sdv/constraints/base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/constraints/errors.py` & `sdv-1.9.0.dev0/sdv/constraints/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/constraints/tabular.py` & `sdv-1.9.0.dev0/sdv/constraints/tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/constraints/utils.py` & `sdv-1.9.0.dev0/sdv/constraints/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/data_processing/data_processor.py` & `sdv-1.9.0.dev0/sdv/data_processing/data_processor.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/data_processing/datetime_formatter.py` & `sdv-1.9.0.dev0/sdv/data_processing/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/data_processing/errors.py` & `sdv-1.9.0.dev0/sdv/data_processing/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/data_processing/numerical_formatter.py` & `sdv-1.9.0.dev0/sdv/data_processing/numerical_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/data_processing/utils.py` & `sdv-1.9.0.dev0/sdv/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/datasets/demo.py` & `sdv-1.9.0.dev0/sdv/datasets/demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/datasets/local.py` & `sdv-1.9.0.dev0/sdv/datasets/local.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/errors.py` & `sdv-1.9.0.dev0/sdv/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/evaluation/multi_table.py` & `sdv-1.9.0.dev0/sdv/evaluation/multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/evaluation/single_table.py` & `sdv-1.9.0.dev0/sdv/evaluation/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/lite/single_table.py` & `sdv-1.9.0.dev0/sdv/lite/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/metadata/metadata_upgrader.py` & `sdv-1.9.0.dev0/sdv/metadata/metadata_upgrader.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/metadata/multi_table.py` & `sdv-1.9.0.dev0/sdv/metadata/multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/metadata/single_table.py` & `sdv-1.9.0.dev0/sdv/metadata/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/metadata/utils.py` & `sdv-1.9.0.dev0/sdv/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/metadata/validation.py` & `sdv-1.9.0.dev0/sdv/metadata/validation.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/metadata/visualization.py` & `sdv-1.9.0.dev0/sdv/metadata/visualization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/multi_table/base.py` & `sdv-1.9.0.dev0/sdv/multi_table/base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/multi_table/hma.py` & `sdv-1.9.0.dev0/sdv/multi_table/hma.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/sampling/hierarchical_sampler.py` & `sdv-1.9.0.dev0/sdv/sampling/hierarchical_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/sampling/independent_sampler.py` & `sdv-1.9.0.dev0/sdv/sampling/independent_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/sampling/tabular.py` & `sdv-1.9.0.dev0/sdv/sampling/tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/sequential/par.py` & `sdv-1.9.0.dev0/sdv/sequential/par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/single_table/base.py` & `sdv-1.9.0.dev0/sdv/single_table/base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/single_table/copulagan.py` & `sdv-1.9.0.dev0/sdv/single_table/copulagan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/single_table/copulas.py` & `sdv-1.9.0.dev0/sdv/single_table/copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/single_table/ctgan.py` & `sdv-1.9.0.dev0/sdv/single_table/ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/single_table/utils.py` & `sdv-1.9.0.dev0/sdv/single_table/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv/utils.py` & `sdv-1.9.0.dev0/sdv/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv.egg-info/PKG-INFO` & `sdv-1.9.0.dev0/sdv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdv
-Version: 1.9.0
+Version: 1.9.0.dev0
 Summary: Generate synthetic data for single table, multi table and sequential data
 Home-page: https://github.com/sdv-dev/SDV
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: sdv synthetic-data synhtetic-data-generation timeseries single-table multi-table
 Classifier: Development Status :: 5 - Production/Stable
@@ -242,39 +242,14 @@
 [Get started using the SDV package](https://bit.ly/sdv-docs) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # Release Notes
 
-## 1.9.0 - 2024-01-11
-
-This release makes a number of improvements. It introduces a new concept to the metadata known as column relationships! Column relationships can be used to define when certain groups of columns in a table should be treated as a special concept (eg. address). You can add a column relationship by using the new `add_column_relationship` method. The metadata detection was also improved by allowing semantic sdtypes (eg. 'email', 'phone_number') to be detected as primary keys.
-
-This release also patches some bugs. An issue messing up the likelihood matching in the `HMASynthesizer` was resolved. The `CTGANSynthesizer` no longer fails when using the `FixedCombinations` constraint. The `Inequality` constraint was also patched to handle datetimes better.
-
-### Deprecations
-
-* The `set_address_columns` method is deprecated in favor of `add_column_relationship`.
-
-### New Features
-
-* Improve error messages for composite keys - Issue [#1684](https://github.com/sdv-dev/SDV/issues/1684) by @frances-h
-* Add column relationship validation to single table metadata - Issue [#1698](https://github.com/sdv-dev/SDV/issues/1698) by @frances-h
-* Add add_column_relationship method to single table metadata - Issue [#1699](https://github.com/sdv-dev/SDV/issues/1699) by @frances-h
-* Make synthesizers work with column_relationships - Issue [#1700](https://github.com/sdv-dev/SDV/issues/1700) by @R-Palazzo
-* Metadata auto-detection should find primary keys of semantic sdtypes - Issue [#1724](https://github.com/sdv-dev/SDV/issues/1724) by @fealho
-
-### Bugs Fixed
-
-* InvalidDataError for Inequality constraint (even though data is valid) - Issue [#1692](https://github.com/sdv-dev/SDV/issues/1692) by @fealho
-* `BaseIndependentSampler` crashes because it tries to cast id columns - Issue [#1712](https://github.com/sdv-dev/SDV/issues/1712) by @pvk-developer
-* KeyError in `CTGANSynthesizer` when applying `FixedCombinations` constraint - Issue [#1717](https://github.com/sdv-dev/SDV/issues/1717) by @pvk-developer
-* Fix _get_likelihoods not generating likelihood values - Issue [#1720](https://github.com/sdv-dev/SDV/pull/1720) by @frances-h
-
 ## 1.8.0 - 2023-12-05
 
 This release adds support for the new Diagnostic Report from SDMetrics. This report calculates scores for three basic but important properties of your data: data validity, data structure and in the multi table case, relationship validity. Data validity checks that the columns of your data are valid (eg. correct range or values). Data structure makes sure the synthetic data has the correct columns. Relationship validity checks to make sure key references are correct and the cardinality is within ranges seen in the real data.
 
 Additionally, a few bugs were fixed and functionality was improved around synthesizers. It is now possible to access the loss values for the `TVAESynthesizer` and `CTGANSynthesizer` by using the `get_loss_values` method. The `get_parameters` method is now more detailed and returns all the parameters used to make a synthesizer. The metadata is now capable of detecting some common pii sdtypes. Finally, a bug that made every parent row generated by the `HMASynthesizer` have at least one child row was patched. This should improve cardinality.
 
 ### Maintenance
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: sdv Version: 1.9.0 Summary: Generate synthetic data
-for single table, multi table and sequential data Home-page: https://
+Metadata-Version: 2.1 Name: sdv Version: 1.9.0.dev0 Summary: Generate synthetic
+data for single table, multi table and sequential data Home-page: https://
 github.com/sdv-dev/SDV Author: DataCebo, Inc. Author-email: info@sdv.dev
 License: BSL-1.1 Keywords: sdv synthetic-data synhtetic-data-generation
 timeseries single-table multi-table Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Free for non-commercial use Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -131,51 +131,22 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://bit.ly/sdv-docs) -- a fully integrated solution and your one-stop shop
 for synthetic data. Or, use the standalone libraries for specific needs. #
-Release Notes ## 1.9.0 - 2024-01-11 This release makes a number of
-improvements. It introduces a new concept to the metadata known as column
-relationships! Column relationships can be used to define when certain groups
-of columns in a table should be treated as a special concept (eg. address). You
-can add a column relationship by using the new `add_column_relationship`
-method. The metadata detection was also improved by allowing semantic sdtypes
-(eg. 'email', 'phone_number') to be detected as primary keys. This release also
-patches some bugs. An issue messing up the likelihood matching in the
-`HMASynthesizer` was resolved. The `CTGANSynthesizer` no longer fails when
-using the `FixedCombinations` constraint. The `Inequality` constraint was also
-patched to handle datetimes better. ### Deprecations * The
-`set_address_columns` method is deprecated in favor of
-`add_column_relationship`. ### New Features * Improve error messages for
-composite keys - Issue [#1684](https://github.com/sdv-dev/SDV/issues/1684) by
-@frances-h * Add column relationship validation to single table metadata -
-Issue [#1698](https://github.com/sdv-dev/SDV/issues/1698) by @frances-h * Add
-add_column_relationship method to single table metadata - Issue [#1699](https:/
-/github.com/sdv-dev/SDV/issues/1699) by @frances-h * Make synthesizers work
-with column_relationships - Issue [#1700](https://github.com/sdv-dev/SDV/
-issues/1700) by @R-Palazzo * Metadata auto-detection should find primary keys
-of semantic sdtypes - Issue [#1724](https://github.com/sdv-dev/SDV/issues/1724)
-by @fealho ### Bugs Fixed * InvalidDataError for Inequality constraint (even
-though data is valid) - Issue [#1692](https://github.com/sdv-dev/SDV/issues/
-1692) by @fealho * `BaseIndependentSampler` crashes because it tries to cast id
-columns - Issue [#1712](https://github.com/sdv-dev/SDV/issues/1712) by @pvk-
-developer * KeyError in `CTGANSynthesizer` when applying `FixedCombinations`
-constraint - Issue [#1717](https://github.com/sdv-dev/SDV/issues/1717) by @pvk-
-developer * Fix _get_likelihoods not generating likelihood values - Issue
-[#1720](https://github.com/sdv-dev/SDV/pull/1720) by @frances-h ## 1.8.0 -
-2023-12-05 This release adds support for the new Diagnostic Report from
-SDMetrics. This report calculates scores for three basic but important
-properties of your data: data validity, data structure and in the multi table
-case, relationship validity. Data validity checks that the columns of your data
-are valid (eg. correct range or values). Data structure makes sure the
-synthetic data has the correct columns. Relationship validity checks to make
-sure key references are correct and the cardinality is within ranges seen in
-the real data. Additionally, a few bugs were fixed and functionality was
+Release Notes ## 1.8.0 - 2023-12-05 This release adds support for the new
+Diagnostic Report from SDMetrics. This report calculates scores for three basic
+but important properties of your data: data validity, data structure and in the
+multi table case, relationship validity. Data validity checks that the columns
+of your data are valid (eg. correct range or values). Data structure makes sure
+the synthetic data has the correct columns. Relationship validity checks to
+make sure key references are correct and the cardinality is within ranges seen
+in the real data. Additionally, a few bugs were fixed and functionality was
 improved around synthesizers. It is now possible to access the loss values for
 the `TVAESynthesizer` and `CTGANSynthesizer` by using the `get_loss_values`
 method. The `get_parameters` method is now more detailed and returns all the
 parameters used to make a synthesizer. The metadata is now capable of detecting
 some common pii sdtypes. Finally, a bug that made every parent row generated by
 the `HMASynthesizer` have at least one child row was patched. This should
 improve cardinality. ### Maintenance * Address `SettingWithCopyWarning`
```

### Comparing `sdv-1.9.0/sdv.egg-info/SOURCES.txt` & `sdv-1.9.0.dev0/sdv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/sdv.egg-info/requires.txt` & `sdv-1.9.0.dev0/sdv.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/setup.cfg` & `sdv-1.9.0.dev0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.9.0
+current_version = 1.9.0.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `sdv-1.9.0/setup.py` & `sdv-1.9.0.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,10 +132,10 @@
     name='sdv',
     packages=find_packages(include=['sdv', 'sdv.*']),
     python_requires='>=3.8,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/SDV',
-    version='1.9.0',
+    version='1.9.0.dev0',
     zip_safe=False,
 )
```

### Comparing `sdv-1.9.0/tests/integration/data_processing/test_data_processor.py` & `sdv-1.9.0.dev0/tests/integration/data_processing/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/dataset.py` & `sdv-1.9.0.dev0/tests/integration/dataset.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/datasets/test_demo.py` & `sdv-1.9.0.dev0/tests/integration/datasets/test_demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/evaluation/test_multi_table.py` & `sdv-1.9.0.dev0/tests/integration/evaluation/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/evaluation/test_single_table.py` & `sdv-1.9.0.dev0/tests/integration/evaluation/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/lite/test_single_table.py` & `sdv-1.9.0.dev0/tests/integration/lite/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/metadata/test_multi_table.py` & `sdv-1.9.0.dev0/tests/integration/metadata/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/metadata/test_single_table.py` & `sdv-1.9.0.dev0/tests/integration/metadata/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/metadata/test_visualization.py` & `sdv-1.9.0.dev0/tests/integration/metadata/test_visualization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/multi_table/test_hma.py` & `sdv-1.9.0.dev0/tests/integration/multi_table/test_hma.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/sequential/test_par.py` & `sdv-1.9.0.dev0/tests/integration/sequential/test_par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/single_table/custom_constraints.py` & `sdv-1.9.0.dev0/tests/integration/single_table/custom_constraints.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/single_table/test_base.py` & `sdv-1.9.0.dev0/tests/integration/single_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/single_table/test_constraints.py` & `sdv-1.9.0.dev0/tests/integration/single_table/test_constraints.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/single_table/test_copulas.py` & `sdv-1.9.0.dev0/tests/integration/single_table/test_copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/integration/single_table/test_ctgan.py` & `sdv-1.9.0.dev0/tests/integration/single_table/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/readme_test/README.md` & `sdv-1.9.0.dev0/tests/readme_test/README.md`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/constraints/test_base.py` & `sdv-1.9.0.dev0/tests/unit/constraints/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/constraints/test_errors.py` & `sdv-1.9.0.dev0/tests/unit/constraints/test_errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/constraints/test_tabular.py` & `sdv-1.9.0.dev0/tests/unit/constraints/test_tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/constraints/test_utils.py` & `sdv-1.9.0.dev0/tests/unit/constraints/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/data_processing/test_data_processor.py` & `sdv-1.9.0.dev0/tests/unit/data_processing/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/data_processing/test_datetime_formatter.py` & `sdv-1.9.0.dev0/tests/unit/data_processing/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/data_processing/test_numerical_formatter.py` & `sdv-1.9.0.dev0/tests/unit/data_processing/test_numerical_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/data_processing/test_utils.py` & `sdv-1.9.0.dev0/tests/unit/data_processing/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/datasets/test_demo.py` & `sdv-1.9.0.dev0/tests/unit/datasets/test_demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/datasets/test_local.py` & `sdv-1.9.0.dev0/tests/unit/datasets/test_local.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/evaluation/test_multi_table.py` & `sdv-1.9.0.dev0/tests/unit/evaluation/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/evaluation/test_single_table.py` & `sdv-1.9.0.dev0/tests/unit/evaluation/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/lite/test_single_table.py` & `sdv-1.9.0.dev0/tests/unit/lite/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/metadata/test_metadata_upgrader.py` & `sdv-1.9.0.dev0/tests/unit/metadata/test_metadata_upgrader.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/metadata/test_multi_table.py` & `sdv-1.9.0.dev0/tests/unit/metadata/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/metadata/test_single_table.py` & `sdv-1.9.0.dev0/tests/unit/metadata/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/metadata/test_validation.py` & `sdv-1.9.0.dev0/tests/unit/metadata/test_validation.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/multi_table/test_base.py` & `sdv-1.9.0.dev0/tests/unit/multi_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/multi_table/test_hma.py` & `sdv-1.9.0.dev0/tests/unit/multi_table/test_hma.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/sampling/test_hierarchical_sampler.py` & `sdv-1.9.0.dev0/tests/unit/sampling/test_hierarchical_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/sampling/test_independent_sampler.py` & `sdv-1.9.0.dev0/tests/unit/sampling/test_independent_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/sampling/test_tabular.py` & `sdv-1.9.0.dev0/tests/unit/sampling/test_tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/sequential/test_par.py` & `sdv-1.9.0.dev0/tests/unit/sequential/test_par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/single_table/test_base.py` & `sdv-1.9.0.dev0/tests/unit/single_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/single_table/test_copulagan.py` & `sdv-1.9.0.dev0/tests/unit/single_table/test_copulagan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/single_table/test_copulas.py` & `sdv-1.9.0.dev0/tests/unit/single_table/test_copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/single_table/test_ctgan.py` & `sdv-1.9.0.dev0/tests/unit/single_table/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/single_table/test_utils.py` & `sdv-1.9.0.dev0/tests/unit/single_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/test___init__.py` & `sdv-1.9.0.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/test_errors.py` & `sdv-1.9.0.dev0/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/unit/test_utils.py` & `sdv-1.9.0.dev0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.9.0/tests/utils.py` & `sdv-1.9.0.dev0/tests/utils.py`

 * *Files identical despite different names*

