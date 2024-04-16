# Comparing `tmp/vastdb-0.1.0.tar.gz` & `tmp/vastdb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastdb-0.1.0.tar", last modified: Wed Apr 10 18:33:22 2024, max compression
+gzip compressed data, was "vastdb-0.1.1.tar", last modified: Tue Apr 16 14:52:46 2024, max compression
```

## Comparing `vastdb-0.1.0.tar` & `vastdb-0.1.1.tar`

### file list

```diff
@@ -1,188 +1,196 @@
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.986759 vastdb-0.1.0/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)    11333 2023-12-17 10:00:47.000000 vastdb-0.1.0/LICENSE
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1148 2024-04-10 18:33:22.986595 vastdb-0.1.0/PKG-INFO
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5891 2024-04-10 18:32:20.000000 vastdb-0.1.0/README.md
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       38 2024-04-10 18:33:22.986822 vastdb-0.1.0/setup.cfg
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1699 2024-04-10 18:32:20.000000 vastdb-0.1.0/setup.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.945854 vastdb-0.1.0/vast_flatbuf/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.945979 vastdb-0.1.0/vast_flatbuf/org/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.946099 vastdb-0.1.0/vast_flatbuf/org/apache/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.946228 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.946358 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.961830 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5630 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2212 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1567 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2494 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      182 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4434 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2429 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2520 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      236 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3490 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1059 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2576 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      484 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2258 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      498 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1584 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2850 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3260 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2602 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1515 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      186 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2403 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1487 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2197 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      211 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1578 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4455 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      230 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2309 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3368 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2400 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2797 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2526 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      682 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3284 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1723 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2392 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3847 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      349 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2378 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3941 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1526 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2113 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      315 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      217 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3678 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3952 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2221 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5650 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1533 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1593 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2539 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1529 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1051 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     7527 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.974321 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1026 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1326 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2310 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      836 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1430 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      155 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1760 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      149 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2855 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3148 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4091 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      410 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      267 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1289 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     7048 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1669 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1589 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1569 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1541 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6448 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1925 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      180 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1131 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/List.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2541 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4486 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      671 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      786 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1054 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      161 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5589 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6042 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      162 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5785 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6091 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      226 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     6389 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     9409 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1193 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5767 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2149 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2639 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      191 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     7925 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      698 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3142 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      147 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1023 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.979609 vastdb-0.1.0/vast_flatbuf/tabular/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2114 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/AlterColumnRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2222 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/AlterProjectionTableRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1618 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/AlterSchemaRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1610 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/AlterTableRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1901 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/Column.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      151 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ColumnType.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2516 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/CreateProjectionRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1626 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/CreateSchemaRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3474 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4655 2024-04-09 14:04:20.000000 vastdb-0.1.0/vast_flatbuf/tabular/GetTableStatsResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2450 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ImportDataRequest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4240 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ListProjectionsResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3036 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ListSchemasResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3550 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ListTablesResponse.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3589 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/ObjectDetails.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     4450 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/S3File.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2069 2024-04-09 14:04:20.000000 vastdb-0.1.0/vast_flatbuf/tabular/VipRange.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.0/vast_flatbuf/tabular/__init__.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.983124 vastdb-0.1.0/vastdb/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)      206 2024-04-10 13:32:04.000000 vastdb-0.1.0/vastdb/__init__.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2526 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/bucket.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     3119 2024-04-10 18:32:20.000000 vastdb-0.1.0/vastdb/errors.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)   104441 2024-04-10 18:29:55.000000 vastdb-0.1.0/vastdb/internal_commands.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2836 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/schema.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1731 2024-04-10 13:33:23.000000 vastdb-0.1.0/vastdb/session.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)    20442 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/table.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.986088 vastdb-0.1.0/vastdb/tests/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-04-07 08:41:05.000000 vastdb-0.1.0/vastdb/tests/__init__.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1694 2024-04-10 13:50:46.000000 vastdb-0.1.0/vastdb/tests/conftest.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     5035 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/tests/test_imports.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1253 2024-04-09 14:04:20.000000 vastdb-0.1.0/vastdb/tests/test_projections.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2959 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/tests/test_sanity.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1253 2024-04-09 14:04:20.000000 vastdb-0.1.0/vastdb/tests/test_schemas.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)    23634 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/tests/test_tables.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1797 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/transaction.py
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     2908 2024-04-10 15:50:25.000000 vastdb-0.1.0/vastdb/util.py
-drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-10 18:33:22.984138 vastdb-0.1.0/vastdb.egg-info/
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     1148 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/PKG-INFO
--rw-r--r--   0 roman.zeyde   (501) staff       (20)     8858 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/SOURCES.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)        1 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/dependency_links.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       78 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/requires.txt
--rw-r--r--   0 roman.zeyde   (501) staff       (20)       20 2024-04-10 18:33:22.000000 vastdb-0.1.0/vastdb.egg-info/top_level.txt
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.980522 vastdb-0.1.1/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3026 2024-04-16 08:04:31.000000 vastdb-0.1.1/CHANGELOG.md
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)    11333 2023-12-17 10:00:47.000000 vastdb-0.1.1/LICENSE
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)       38 2024-04-14 12:15:26.000000 vastdb-0.1.1/MANIFEST.in
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1148 2024-04-16 14:52:46.980368 vastdb-0.1.1/PKG-INFO
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5891 2024-04-13 15:33:57.000000 vastdb-0.1.1/README.md
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)       78 2024-04-12 16:51:13.000000 vastdb-0.1.1/requirements.txt
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)       38 2024-04-16 14:52:46.980587 vastdb-0.1.1/setup.cfg
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1700 2024-04-16 08:04:31.000000 vastdb-0.1.1/setup.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939438 vastdb-0.1.1/vast_flatbuf/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939565 vastdb-0.1.1/vast_flatbuf/org/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939701 vastdb-0.1.1/vast_flatbuf/org/apache/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939831 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.939959 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.956086 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5630 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2212 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1567 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2494 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      182 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4434 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2429 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2520 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      236 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3490 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1059 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2576 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      484 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2258 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      498 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1584 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2850 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3260 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2602 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1515 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1521 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      186 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2403 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1487 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2197 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      211 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1578 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4455 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      230 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2309 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3368 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2400 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2797 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2526 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      682 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3284 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1723 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2392 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3847 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      349 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2378 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2130 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3941 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1526 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2113 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      315 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      217 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3678 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3952 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2221 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5650 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1533 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1593 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2539 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1489 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1529 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1507 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1497 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1051 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     7527 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:54.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.968767 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1026 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1326 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2310 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      836 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1430 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      155 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1760 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      149 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2855 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3148 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4091 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      410 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      267 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1289 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     7048 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1669 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1589 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1569 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1541 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     6448 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1925 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1456 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      180 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2139 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1131 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1117 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      993 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/List.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2541 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4486 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      671 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      786 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1054 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      161 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5589 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     6042 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      162 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5785 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     6091 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      226 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     6389 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     9409 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1193 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5767 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2149 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2639 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      191 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     7925 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      698 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3142 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      147 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1023 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.973477 vastdb-0.1.1/vast_flatbuf/tabular/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2114 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/AlterColumnRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2222 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/AlterProjectionTableRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1618 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/AlterSchemaRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1610 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/AlterTableRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1901 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/Column.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      151 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ColumnType.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2516 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/CreateProjectionRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1626 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/CreateSchemaRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3474 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4655 2024-04-11 20:45:30.000000 vastdb-0.1.1/vast_flatbuf/tabular/GetTableStatsResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2450 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ImportDataRequest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4240 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ListProjectionsResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3036 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ListSchemasResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3550 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ListTablesResponse.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3589 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/ObjectDetails.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     4450 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/S3File.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2069 2024-04-11 20:45:30.000000 vastdb-0.1.1/vast_flatbuf/tabular/VipRange.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-02-13 11:15:55.000000 vastdb-0.1.1/vast_flatbuf/tabular/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.976905 vastdb-0.1.1/vastdb/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      206 2024-04-13 15:16:53.000000 vastdb-0.1.1/vastdb/__init__.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.978057 vastdb-0.1.1/vastdb/bench/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-04-13 15:33:57.000000 vastdb-0.1.1/vastdb/bench/__init__.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1111 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/bench/test_perf.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2854 2024-04-16 07:09:04.000000 vastdb-0.1.1/vastdb/bucket.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2132 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/conftest.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3315 2024-04-16 07:09:04.000000 vastdb-0.1.1/vastdb/errors.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)   101564 2024-04-16 08:04:31.000000 vastdb-0.1.1/vastdb/internal_commands.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     3192 2024-04-16 07:09:04.000000 vastdb-0.1.1/vastdb/schema.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1718 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/session.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)    20443 2024-04-16 08:04:31.000000 vastdb-0.1.1/vastdb/table.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.980129 vastdb-0.1.1/vastdb/tests/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        0 2024-04-14 19:07:27.000000 vastdb-0.1.1/vastdb/tests/__init__.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     5033 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/test_imports.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      951 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/test_nested.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1254 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/test_projections.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2958 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/test_sanity.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1721 2024-04-16 08:04:31.000000 vastdb-0.1.1/vastdb/tests/test_schemas.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)    26226 2024-04-16 08:04:31.000000 vastdb-0.1.1/vastdb/tests/test_tables.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)      597 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/tests/util.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1796 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/transaction.py
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     2974 2024-04-16 07:05:01.000000 vastdb-0.1.1/vastdb/util.py
+drwxr-xr-x   0 roman.zeyde   (501) staff       (20)        0 2024-04-16 14:52:46.977787 vastdb-0.1.1/vastdb.egg-info/
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     1148 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/PKG-INFO
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)     8994 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/SOURCES.txt
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)        1 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/dependency_links.txt
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)       78 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/requires.txt
+-rw-r--r--   0 roman.zeyde   (501) staff       (20)       20 2024-04-16 14:52:46.000000 vastdb-0.1.1/vastdb.egg-info/top_level.txt
```

### Comparing `vastdb-0.1.0/LICENSE` & `vastdb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/PKG-INFO` & `vastdb-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vastdb-0.1.0/README.md` & `vastdb-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/setup.py` & `vastdb-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 long_description = """
 `vastdb` is a Python-based SDK designed for interacting
 with [VAST Database](https://vastdata.com/database)
 and [VAST Catalog](https://vastdata.com/blog/vast-catalog-treat-your-file-system-like-a-database),
 enabling schema and table management, efficient ingest, query and modification of columnar data.
 
@@ -21,15 +22,15 @@
 if os.environ.get('VASTDB_APPEND_VERSION_SUFFIX'):
     suffix = _get_version_suffix()
 
 setup(
     name='vastdb',
     python_requires='>=3.9.0',
     description='VAST Data SDK',
-    version='0.1.0' + suffix,
+    version='0.1.1' + suffix,
     url='https://github.com/vast-data/vastdb_sdk',
     author='VAST DATA',
     author_email='hello@vastdata.com',
     license='Copyright (C) VAST Data Ltd.',
     packages=find_packages(),
     install_requires=open('requirements.txt').read().strip().split('\n'),
     long_description=long_description,
```

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Block.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Block.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Date.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Date.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Field.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Field.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Int.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Int.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/List.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/List.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Map.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Map.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Message.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Message.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Null.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Null.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Time.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Time.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Type.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Type.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Union.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Union.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py` & `vastdb-0.1.1/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/AlterColumnRequest.py` & `vastdb-0.1.1/vast_flatbuf/tabular/AlterColumnRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/AlterProjectionTableRequest.py` & `vastdb-0.1.1/vast_flatbuf/tabular/AlterProjectionTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/AlterSchemaRequest.py` & `vastdb-0.1.1/vast_flatbuf/tabular/AlterSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/AlterTableRequest.py` & `vastdb-0.1.1/vast_flatbuf/tabular/AlterTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/Column.py` & `vastdb-0.1.1/vast_flatbuf/tabular/Column.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/CreateProjectionRequest.py` & `vastdb-0.1.1/vast_flatbuf/tabular/CreateProjectionRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/CreateSchemaRequest.py` & `vastdb-0.1.1/vast_flatbuf/tabular/CreateSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py` & `vastdb-0.1.1/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/GetTableStatsResponse.py` & `vastdb-0.1.1/vast_flatbuf/tabular/GetTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/ImportDataRequest.py` & `vastdb-0.1.1/vast_flatbuf/tabular/ImportDataRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/ListProjectionsResponse.py` & `vastdb-0.1.1/vast_flatbuf/tabular/ListProjectionsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/ListSchemasResponse.py` & `vastdb-0.1.1/vast_flatbuf/tabular/ListSchemasResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/ListTablesResponse.py` & `vastdb-0.1.1/vast_flatbuf/tabular/ListTablesResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/ObjectDetails.py` & `vastdb-0.1.1/vast_flatbuf/tabular/ObjectDetails.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/S3File.py` & `vastdb-0.1.1/vast_flatbuf/tabular/S3File.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vast_flatbuf/tabular/VipRange.py` & `vastdb-0.1.1/vast_flatbuf/tabular/VipRange.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.0/vastdb/bucket.py` & `vastdb-0.1.1/vastdb/bucket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """VAST Database bucket.
 
 VAST S3 buckets can be used to create Database schemas and tables.
 It is possible to list and access VAST snapshots generated over a bucket.
 """
 
-from . import errors, schema, transaction
-
-from dataclasses import dataclass
 import logging
+from dataclasses import dataclass
+
+from . import errors, schema, transaction
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class Snapshot:
     """VAST bucket-level snapshot."""
@@ -23,26 +23,34 @@
 @dataclass
 class Bucket:
     """VAST bucket."""
 
     name: str
     tx: "transaction.Transaction"
 
-    def create_schema(self, path: str) -> "schema.Schema":
+    def create_schema(self, path: str, fail_if_exists=True) -> "schema.Schema":
         """Create a new schema (a container of tables) under this bucket."""
+        if current := self.schema(path, fail_if_missing=False):
+            if fail_if_exists:
+                raise errors.SchemaExists(self.name, path)
+            else:
+                return current
         self.tx._rpc.api.create_schema(self.name, path, txid=self.tx.txid)
         log.info("Created schema: %s", path)
         return self.schema(path)
 
-    def schema(self, path: str) -> "schema.Schema":
+    def schema(self, path: str, fail_if_missing=True) -> "schema.Schema":
         """Get a specific schema (a container of tables) under this bucket."""
         s = self.schemas(path)
         log.debug("schema: %s", s)
         if not s:
-            raise errors.MissingSchema(self.name, path)
+            if fail_if_missing:
+                raise errors.MissingSchema(self.name, path)
+            else:
+                return None
         assert len(s) == 1, f"Expected to receive only a single schema, but got: {len(s)}. ({s})"
         log.debug("Found schema: %s", s[0].name)
         return s[0]
 
     def schemas(self, name: str = None) -> ["schema.Schema"]:
         """List bucket's schemas."""
         schemas = []
```

### Comparing `vastdb-0.1.0/vastdb/errors.py` & `vastdb-0.1.1/vastdb/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
-import requests
 import xml.etree.ElementTree
-
-from enum import Enum
 from dataclasses import dataclass
+from enum import Enum
+
+import requests
 
 
 class HttpStatus(Enum):
     SUCCESS = 200
     BAD_REQUEST = 400
     FOBIDDEN = 403
     NOT_FOUND = 404
@@ -110,14 +110,31 @@
 class MissingProjection(Missing):
     bucket: str
     schema: str
     table: str
     projection: str
 
 
+class Exists(Exception):
+    pass
+
+
+@dataclass
+class SchemaExists(Exists):
+    bucket: str
+    schema: str
+
+
+@dataclass
+class TableExists(Exists):
+    bucket: str
+    schema: str
+    table: str
+
+
 ERROR_TYPES_MAP = {
     HttpStatus.BAD_REQUEST: BadRequest,
     HttpStatus.FOBIDDEN: Forbidden,
     HttpStatus.NOT_FOUND: NotFound,
     HttpStatus.METHOD_NOT_ALLOWED: MethodNotAllowed,
     HttpStatus.REQUEST_TIMEOUT: RequestTimeout,
     HttpStatus.CONFLICT: Conflict,
```

### Comparing `vastdb-0.1.0/vastdb/internal_commands.py` & `vastdb-0.1.1/vastdb/internal_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,89 +1,95 @@
+import itertools
+import json
 import logging
+import math
+import re
 import struct
 import urllib.parse
 from collections import defaultdict, namedtuple
-from datetime import datetime
 from enum import Enum
-from typing import Union, Optional, Iterator
-import ibis
-import xmltodict
-import math
-from functools import cmp_to_key
-import pyarrow.parquet as pq
+from ipaddress import IPv4Address, IPv6Address
+from typing import Iterator, Optional, Union
+
 import flatbuffers
+import ibis
 import pyarrow as pa
+import pyarrow.parquet as pq
 import requests
-import json
-import itertools
-from aws_requests_auth.aws_auth import AWSRequestsAuth
 import urllib3
-import re
-
-from . import errors
-from ipaddress import IPv4Address, IPv6Address
+import xmltodict
+from aws_requests_auth.aws_auth import AWSRequestsAuth
 
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.BinaryLiteral as fb_binary_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.BooleanLiteral as fb_bool_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Call as fb_call
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.DateLiteral as fb_date32_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.DecimalLiteral as fb_decimal_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Expression as fb_expression
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.FieldIndex as fb_field_index
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.FieldRef as fb_field_ref
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Float32Literal as fb_float32_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Float64Literal as fb_float64_lit
+import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Int8Literal as fb_int8_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Int16Literal as fb_int16_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Int32Literal as fb_int32_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Int64Literal as fb_int64_lit
-import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Int8Literal as fb_int8_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Literal as fb_literal
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Relation as fb_relation
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.RelationImpl as rel_impl
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.Source as fb_source
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.StringLiteral as fb_string_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.TimeLiteral as fb_time_lit
 import vast_flatbuf.org.apache.arrow.computeir.flatbuf.TimestampLiteral as fb_timestamp_lit
 import vast_flatbuf.org.apache.arrow.flatbuf.Binary as fb_binary
 import vast_flatbuf.org.apache.arrow.flatbuf.Bool as fb_bool
 import vast_flatbuf.org.apache.arrow.flatbuf.Date as fb_date
 import vast_flatbuf.org.apache.arrow.flatbuf.Decimal as fb_decimal
 import vast_flatbuf.org.apache.arrow.flatbuf.Field as fb_field
+import vast_flatbuf.org.apache.arrow.flatbuf.FixedSizeBinary as fb_fixed_size_binary
 import vast_flatbuf.org.apache.arrow.flatbuf.FloatingPoint as fb_floating_point
 import vast_flatbuf.org.apache.arrow.flatbuf.Int as fb_int
-import vast_flatbuf.org.apache.arrow.flatbuf.Schema as fb_schema
-import vast_flatbuf.org.apache.arrow.flatbuf.Time as fb_time
-import vast_flatbuf.org.apache.arrow.flatbuf.Struct_ as fb_struct
 import vast_flatbuf.org.apache.arrow.flatbuf.List as fb_list
 import vast_flatbuf.org.apache.arrow.flatbuf.Map as fb_map
-import vast_flatbuf.org.apache.arrow.flatbuf.FixedSizeBinary as fb_fixed_size_binary
+import vast_flatbuf.org.apache.arrow.flatbuf.Schema as fb_schema
+import vast_flatbuf.org.apache.arrow.flatbuf.Struct_ as fb_struct
+import vast_flatbuf.org.apache.arrow.flatbuf.Time as fb_time
 import vast_flatbuf.org.apache.arrow.flatbuf.Timestamp as fb_timestamp
 import vast_flatbuf.org.apache.arrow.flatbuf.Utf8 as fb_utf8
 import vast_flatbuf.tabular.AlterColumnRequest as tabular_alter_column
+import vast_flatbuf.tabular.AlterProjectionTableRequest as tabular_alter_projection
 import vast_flatbuf.tabular.AlterSchemaRequest as tabular_alter_schema
 import vast_flatbuf.tabular.AlterTableRequest as tabular_alter_table
-import vast_flatbuf.tabular.AlterProjectionTableRequest as tabular_alter_projection
+import vast_flatbuf.tabular.Column as tabular_projecion_column
+import vast_flatbuf.tabular.ColumnType as tabular_proj_column_type
+import vast_flatbuf.tabular.CreateProjectionRequest as tabular_create_projection
 import vast_flatbuf.tabular.CreateSchemaRequest as tabular_create_schema
 import vast_flatbuf.tabular.ImportDataRequest as tabular_import_data
 import vast_flatbuf.tabular.S3File as tabular_s3_file
-import vast_flatbuf.tabular.CreateProjectionRequest as tabular_create_projection
-import vast_flatbuf.tabular.Column as tabular_projecion_column
-import vast_flatbuf.tabular.ColumnType as tabular_proj_column_type
-
 from vast_flatbuf.org.apache.arrow.computeir.flatbuf.Deref import Deref
-from vast_flatbuf.org.apache.arrow.computeir.flatbuf.ExpressionImpl import ExpressionImpl
+from vast_flatbuf.org.apache.arrow.computeir.flatbuf.ExpressionImpl import (
+    ExpressionImpl,
+)
 from vast_flatbuf.org.apache.arrow.computeir.flatbuf.LiteralImpl import LiteralImpl
 from vast_flatbuf.org.apache.arrow.flatbuf.DateUnit import DateUnit
 from vast_flatbuf.org.apache.arrow.flatbuf.TimeUnit import TimeUnit
 from vast_flatbuf.org.apache.arrow.flatbuf.Type import Type
+from vast_flatbuf.tabular.GetProjectionTableStatsResponse import (
+    GetProjectionTableStatsResponse as get_projection_table_stats,
+)
+from vast_flatbuf.tabular.GetTableStatsResponse import (
+    GetTableStatsResponse as get_table_stats,
+)
+from vast_flatbuf.tabular.ListProjectionsResponse import (
+    ListProjectionsResponse as list_projections,
+)
 from vast_flatbuf.tabular.ListSchemasResponse import ListSchemasResponse as list_schemas
 from vast_flatbuf.tabular.ListTablesResponse import ListTablesResponse as list_tables
-from vast_flatbuf.tabular.GetTableStatsResponse import GetTableStatsResponse as get_table_stats
-from vast_flatbuf.tabular.GetProjectionTableStatsResponse import GetProjectionTableStatsResponse as get_projection_table_stats
-from vast_flatbuf.tabular.ListProjectionsResponse import ListProjectionsResponse as list_projections
+
+from . import errors
 
 UINT64_MAX = 18446744073709551615
 
 TABULAR_KEEP_ALIVE_STREAM_ID = 0xFFFFFFFF
 TABULAR_QUERY_DATA_COMPLETED_STREAM_ID = 0xFFFFFFFF - 1
 TABULAR_QUERY_DATA_FAILED_STREAM_ID = 0xFFFFFFFF - 2
 TABULAR_INVALID_ROW_ID = 0xFFFFFFFFFFFF # (1<<48)-1
@@ -118,21 +124,14 @@
         'us': TimeUnit.MICROSECOND,
         'ms': TimeUnit.MILLISECOND,
         's': TimeUnit.SECOND
     }
     return unit_to_flatbuff_time_unit[type]
 
 class Predicate:
-    unit_to_epoch = {
-        'ns': 1_000_000,
-        'us': 1_000,
-        'ms': 1,
-        's': 0.001
-    }
-
     def __init__(self, schema: 'pa.Schema', expr: ibis.expr.types.BooleanColumn):
         self.schema = schema
         self.expr = expr
         self.builder = None
 
     def get_field_indexes(self, field: 'pa.Field', field_name_per_index: list) -> None:
         field_name_per_index.append(field.name)
@@ -169,16 +168,26 @@
             projection_fields.append(offset)
         fb_source.StartProjectionVector(builder, len(projection_fields))
         for offset in reversed(projection_fields):
             builder.PrependUOffsetTRelative(offset)
         return builder.EndVector()
 
     def serialize(self, builder: 'flatbuffers.builder.Builder'):
-        from ibis.expr.operations.generic import TableColumn, Literal, IsNull
-        from ibis.expr.operations.logical import Greater, GreaterEqual, Less, LessEqual, Equals, NotEquals, And, Or, Not
+        from ibis.expr.operations.generic import IsNull, Literal, TableColumn
+        from ibis.expr.operations.logical import (
+            And,
+            Equals,
+            Greater,
+            GreaterEqual,
+            Less,
+            LessEqual,
+            Not,
+            NotEquals,
+            Or,
+        )
         from ibis.expr.operations.strings import StringContains
 
         builder_map = {
             Greater: self.build_greater,
             GreaterEqual: self.build_greater_equal,
             Less: self.build_less,
             LessEqual: self.build_less_equal,
@@ -399,53 +408,65 @@
             literal_impl = LiteralImpl.StringLiteral
 
             field_type_type = Type.Utf8
             fb_utf8.Start(self.builder)
             field_type = fb_utf8.End(self.builder)
 
             value = self.builder.CreateString(value)
-        elif field.type.equals(pa.date32()):  # pa.date64()
+        elif field.type.equals(pa.date32()):  # pa.date64() is not supported
             literal_type = fb_date32_lit
             literal_impl = LiteralImpl.DateLiteral
 
             field_type_type = Type.Date
             fb_date.Start(self.builder)
             fb_date.AddUnit(self.builder, DateUnit.DAY)
             field_type = fb_date.End(self.builder)
-
-            start_date = datetime.fromtimestamp(0).date()
-            date_delta = value - start_date
-            value = date_delta.days
+            value, = pa.array([value], field.type).cast(pa.int32()).to_pylist()
         elif isinstance(field.type, pa.TimestampType):
             literal_type = fb_timestamp_lit
             literal_impl = LiteralImpl.TimestampLiteral
 
+            if field.type.equals(pa.timestamp('s')):
+                unit = TimeUnit.SECOND
+            if field.type.equals(pa.timestamp('ms')):
+                unit = TimeUnit.MILLISECOND
+            if field.type.equals(pa.timestamp('us')):
+                unit = TimeUnit.MICROSECOND
+            if field.type.equals(pa.timestamp('ns')):
+                unit = TimeUnit.NANOSECOND
+
             field_type_type = Type.Timestamp
             fb_timestamp.Start(self.builder)
-            fb_timestamp.AddUnit(self.builder, get_unit_to_flatbuff_time_unit(field.type.unit))
+            fb_timestamp.AddUnit(self.builder, unit)
             field_type = fb_timestamp.End(self.builder)
-
-            value = int(int(value) * self.unit_to_epoch[field.type.unit])
-        elif field.type.equals(pa.time32('s')) or field.type.equals(pa.time32('ms')) or field.type.equals(pa.time64('us')) or field.type.equals(pa.time64('ns')):
-
+            value, = pa.array([value], field.type).cast(pa.int64()).to_pylist()
+        elif isinstance(field.type, (pa.Time32Type, pa.Time64Type)):
             literal_type = fb_time_lit
             literal_impl = LiteralImpl.TimeLiteral
 
-            field_type_str = str(field.type)
-            start = field_type_str.index('[')
-            end = field_type_str.index(']')
-            unit = field_type_str[start + 1:end]
+            if field.type.equals(pa.time32('s')):
+                target_type = pa.int32()
+                unit = TimeUnit.SECOND
+            if field.type.equals(pa.time32('ms')):
+                target_type = pa.int32()
+                unit = TimeUnit.MILLISECOND
+            if field.type.equals(pa.time64('us')):
+                target_type = pa.int64()
+                unit = TimeUnit.MICROSECOND
+            if field.type.equals(pa.time64('ns')):
+                target_type = pa.int64()
+                unit = TimeUnit.NANOSECOND
 
             field_type_type = Type.Time
             fb_time.Start(self.builder)
             fb_time.AddBitWidth(self.builder, field.type.bit_width)
-            fb_time.AddUnit(self.builder, get_unit_to_flatbuff_time_unit(unit))
+            fb_time.AddUnit(self.builder, unit)
             field_type = fb_time.End(self.builder)
 
-            value = int(value) * self.unit_to_epoch[unit]
+            value, = pa.array([value], field.type).cast(target_type).to_pylist()
         elif field.type.equals(pa.bool_()):
             literal_type = fb_bool_lit
             literal_impl = LiteralImpl.BooleanLiteral
 
             field_type_type = Type.Bool
             fb_bool.Start(self.builder)
             field_type = fb_bool.End(self.builder)
@@ -554,16 +575,14 @@
             self.children = [FieldNode(field, index_iter, parent=self)]
         else:
             self.children = [] # for non-nested types
 
         # will be set during by the parser (see below)
         self.buffers = None # a list of Arrow buffers (https://arrow.apache.org/docs/format/Columnar.html#buffer-listing-for-each-layout)
         self.length = None # each array must have it's length specified (https://arrow.apache.org/docs/python/generated/pyarrow.Array.html#pyarrow.Array.from_buffers)
-        self.is_projected = False
-        self.projected_field = self.field
 
     def _iter_to_root(self) -> Iterator['FieldNode']:
         yield self
         if self.parent is not None:
             yield from self.parent._iter_to_root()
 
     def _iter_nodes(self) -> Iterator['FieldNode']:
@@ -576,23 +595,21 @@
         """Generate only leaf nodes (i.e. columns having scalar types)."""
         if not self.children:
             yield self
         else:
             for child in self.children:
                 yield from child._iter_leaves()
 
-    def _iter_projected_leaves(self) -> Iterator['FieldNode']:
+    def _iter_leaves(self) -> Iterator['FieldNode']:
         """Generate only leaf nodes (i.e. columns having scalar types)."""
         if not self.children:
-            if self.is_projected:
-                yield self
+            yield self
         else:
             for child in self.children:
-                if child.is_projected:
-                    yield from child._iter_projected_leaves()
+                yield from child._iter_leaves()
 
     def debug_log(self, level=0):
         """Recursively dump this node state to log."""
         bufs = self.buffers and [b and b.hex() for b in self.buffers]
         _logger.debug('%s%d: %s, bufs=%s, len=%s', '    '*level, self.index, self.field, bufs, self.length)
         for child in self.children:
             child.debug_log(level=level+1)
@@ -621,60 +638,41 @@
                 if not self.buffers == buffers:
                     raise ValueError(f'self.buffers: {self.buffers} are not equal with buffers: {buffers}')
             if not self.length == len(arr):
                 raise ValueError(f'self.length: {self.length} are not equal with len(arr): {len(arr)}')
 
     def build(self) -> pa.Array:
         """Construct an Arrow array from the collected buffers (recursively)."""
-        children = self.children and [node.build() for node in self.children if node.is_projected]
-        _logger.debug('build: self.field.name=%s, self.projected_field.type=%s, self.length=%s, self.buffers=%s children=%s',
-                      self.field.name, self.projected_field.type, self.length, self.buffers, children)
-        result = pa.Array.from_buffers(self.projected_field.type, self.length, buffers=self.buffers, children=children)
+        children = self.children and [node.build() for node in self.children]
+        result = pa.Array.from_buffers(self.type, self.length, buffers=self.buffers, children=children)
         if self.debug:
             _logger.debug('%s result=%s', self.field, result)
         return result
 
-    def build_projected_field(self):
-        if isinstance(self.type, pa.StructType):
-            [child.build_projected_field() for child in self.children if child.is_projected]
-            self.projected_field = pa.field(self.field.name,
-                                            pa.struct([child.projected_field for child in self.children if child.is_projected]),
-                                            self.field.nullable,
-                                            self.field.metadata)
 
 class QueryDataParser:
     """Used to parse VAST QueryData RPC response."""
-    def __init__(self, arrow_schema: pa.Schema, *, debug=False, projection_positions=None):
+    def __init__(self, arrow_schema: pa.Schema, *, debug=False):
         self.arrow_schema = arrow_schema
-        self.projection_positions = projection_positions
         index = itertools.count() # used to generate leaf column positions for VAST QueryData RPC
         self.nodes = [FieldNode(field, index, debug=debug) for field in arrow_schema]
         self.debug = debug
         if self.debug:
             for node in self.nodes:
                 node.debug_log()
         self.leaves = [leaf for node in self.nodes for leaf in node._iter_leaves()]
-        self.mark_projected_nodes()
-        [node.build_projected_field() for node in self.nodes]
-        self.projected_leaves = [leaf for node in self.nodes for leaf in node._iter_projected_leaves()]
 
         self.leaf_offset = 0
 
-    def mark_projected_nodes(self):
-        for leaf in self.leaves:
-            if self.projection_positions is None or leaf.index in self.projection_positions:
-                for node in leaf._iter_to_root():
-                    node.is_projected = True
-
     def parse(self, column: pa.Array):
         """Parse a single column response from VAST (see FieldNode.set for details)"""
-        if not self.leaf_offset < len(self.projected_leaves):
+        if not self.leaf_offset < len(self.leaves):
             raise ValueError(f'self.leaf_offset: {self.leaf_offset} are not < '
                              f'than len(self.leaves): {len(self.leaves)}')
-        leaf = self.projected_leaves[self.leaf_offset]
+        leaf = self.leaves[self.leaf_offset]
 
         # A column response may be sent in multiple chunks, therefore we need to combine
         # it into a single chunk to allow reconstruction using `Array.from_buffers()`.
         column = column.combine_chunks()
 
         if self.debug:
             _logger.debug("parse: index=%d buffers=%s", leaf.index, [b and b.hex() for b in column.buffers()])
@@ -687,40 +685,27 @@
             raise ValueError(f'len(array_list): {len(array_list)} are not eq '
                              f'with len(node_list): {len(node_list)}')
         for node, arr in zip(node_list, array_list):
             node.set(arr)
 
         self.leaf_offset += 1
 
-    def build(self, output_field_names=None) -> Optional[pa.Table]:
+    def build(self) -> Optional[pa.Table]:
         """Try to build the resulting Table object (if all columns were parsed)"""
-        if self.projection_positions is not None:
-            if self.leaf_offset < len(self.projection_positions):
-                return None
-        else:
-            if self.leaf_offset < len(self.leaves):
-                return None
+        if self.leaf_offset < len(self.leaves):
+            return None
 
         if self.debug:
             for node in self.nodes:
                 node.debug_log()
 
-        # sort resulting table according to the output field names
-        projected_nodes = [node for node in self.nodes if node.is_projected]
-        if output_field_names is not None:
-            def key_func(projected_node):
-                return output_field_names.index(projected_node.field.name)
-            sorted_projected_nodes = sorted(projected_nodes, key=key_func)
-        else:
-            sorted_projected_nodes = projected_nodes
-
         result = pa.Table.from_arrays(
-            arrays=[node.build() for node in sorted_projected_nodes],
-            schema = pa.schema([node.projected_field for node in sorted_projected_nodes]))
-        result.validate(full=True) # does expensive validation checks only if debug is enabled
+            arrays=[node.build() for node in self.nodes],
+            schema=self.arrow_schema)
+        result.validate(full=self.debug) # does expensive validation checks only if debug is enabled
         return result
 
 def _iter_nested_arrays(column: pa.Array) -> Iterator[pa.Array]:
     """Iterate over a single column response, and recursively generate all of its children."""
     yield column
     if isinstance(column.type, pa.StructType):
         if not column.type.num_fields == 1:  # Note: VAST serializes only a single struct field at a time
@@ -1657,28 +1642,31 @@
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(record_batch))
         res = self.session.put(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows"),
                                 data=record_batch, headers=headers)
         return self._check_res(res, "update_rows", expected_retvals)
 
-    def delete_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[]):
+    def delete_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[],
+                    delete_from_imports_table=False):
         """
         DELETE /mybucket/myschema/mytable?rows HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
 
         Request Body
             RecordBatch with single column '$row_id'
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(record_batch))
-        res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows"),
-                               data=record_batch, headers=headers)
+        url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if delete_from_imports_table else {}
+
+        res = self.session.delete(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows", url_params=url_params),
+                                  data=record_batch, headers=headers)
         return self._check_res(res, "delete_rows", expected_retvals)
 
     def create_projection(self, bucket, schema, table, name, columns, txid=0, client_tags=[], expected_retvals=[]):
         """
         Create a table, use the following request
         POST /bucket/schema/table?projection&name=my_projection HTTP/1.1
 
@@ -1939,26 +1927,24 @@
     """
     Generates pyarrow.Table objects from QueryData API response stream.
 
     A pyarrow.Table is a helper class that combines a Schema with multiple RecordBatches and allows easy data access.
     """
     if start_row_ids is None:
         start_row_ids = {}
-    projection_positions = schema.projection_positions
-    arrow_schema = schema.arrow_schema
-    output_field_names = schema.output_field_names
-    _logger.debug(f'projection_positions={projection_positions} len(arrow_schema)={len(arrow_schema)} arrow_schema={arrow_schema}')
-    is_empty_projection = (len(projection_positions) == 0)
-    parsers = defaultdict(lambda: QueryDataParser(arrow_schema, debug=debug, projection_positions=projection_positions))  # {stream_id: QueryDataParser}
+
+    is_empty_projection = (len(schema) == 0)
+    parsers = defaultdict(lambda: QueryDataParser(schema, debug=debug))  # {stream_id: QueryDataParser}
+
     for stream_id, next_row_id, table in _iter_query_data_response_columns(conn, stream_ids):
         parser = parsers[stream_id]
         for column in table.columns:
             parser.parse(column)
 
-        parsed_table = parser.build(output_field_names)
+        parsed_table = parser.build()
         if parsed_table is not None:  # when we got all columns (and before starting a new "select_rows" cycle)
             parsers.pop(stream_id)
             if is_empty_projection:  # VAST returns an empty RecordBatch, with the correct rows' count
                 parsed_table = table
 
             _logger.debug("stream_id=%d rows=%d next_row_id=%d table=%s",
                           stream_id, len(parsed_table), next_row_id, parsed_table)
@@ -2038,15 +2024,15 @@
         field_type = fb_floating_point.End(builder)
 
     elif field.type.equals(pa.string()):
         field_type_type = Type.Utf8
         fb_utf8.Start(builder)
         field_type = fb_utf8.End(builder)
 
-    elif field.type.equals(pa.date32()):  # pa.date64()
+    elif field.type.equals(pa.date32()):  # pa.date64() is not supported
         field_type_type = Type.Date
         fb_date.Start(builder)
         fb_date.AddUnit(builder, DateUnit.DAY)
         field_type = fb_date.End(builder)
 
     elif isinstance(field.type, pa.TimestampType):
         field_type_type = Type.Timestamp
@@ -2151,20 +2137,14 @@
     fb_field.AddTypeType(builder, field_type_type)
     fb_field.AddType(builder, field_type)
     if children is not None:
         fb_field.AddChildren(builder, children)
     return fb_field.End(builder)
 
 
-class VastDBResponseSchema:
-    def __init__(self, arrow_schema, projection_positions, output_field_names):
-        self.arrow_schema = arrow_schema
-        self.projection_positions = projection_positions
-        self.output_field_names = output_field_names
-
 class QueryDataRequest:
     def __init__(self, serialized, response_schema):
         self.serialized = serialized
         self.response_schema = response_schema
 
 
 def build_query_data_request(schema: 'pa.Schema' = pa.schema([]), predicate: ibis.expr.types.BooleanColumn = None, field_names: list = None):
@@ -2183,51 +2163,35 @@
     fb_schema.AddFields(builder, fields)
     schema_obj = fb_schema.End(builder)
 
     predicate = Predicate(schema=schema, expr=predicate)
     filter_obj = predicate.serialize(builder)
 
     parser = QueryDataParser(schema)
-    leaves_map = {}
-    for node in parser.nodes:
-        for descendent in node._iter_nodes():
-            if descendent.parent and isinstance(descendent.parent.type, (pa.ListType, pa.MapType)):
-                continue
-            iter_from_root = reversed(list(descendent._iter_to_root()))
-            descendent_full_name = '.'.join([n.field.name for n in iter_from_root])
-            descendent_leaves = [leaf.index for leaf in descendent._iter_leaves()]
-            leaves_map[descendent_full_name] = descendent_leaves
+    fields_map = {node.field.name: node.field for node in parser.nodes}
+    leaves_map = {node.field.name: [leaf.index for leaf in node._iter_leaves()] for node in parser.nodes}
 
-    output_field_names = None
     if field_names is None:
         field_names = [field.name for field in schema]
-    else:
-        output_field_names  = [f.split('.')[0] for f in field_names]
-        # sort projected field_names according to positions to maintain ordering according to the schema
-        def compare_field_names_by_pos(field_name1, field_name2):
-            return leaves_map[field_name1][0]-leaves_map[field_name2][0]
-        field_names = sorted(field_names, key=cmp_to_key(compare_field_names_by_pos))
 
+    response_schema = pa.schema([fields_map[name] for name in field_names])
     projection_fields = []
-    projection_positions = []
     for field_name in field_names:
+        # TODO: only root-level projection pushdown is supported (i.e. no support for SELECT s.x FROM t)
         positions = leaves_map[field_name]
-        projection_positions.extend(positions)
         for leaf_position in positions:
             fb_field_index.Start(builder)
             fb_field_index.AddPosition(builder, leaf_position)
             offset = fb_field_index.End(builder)
             projection_fields.append(offset)
     fb_source.StartProjectionVector(builder, len(projection_fields))
     for offset in reversed(projection_fields):
         builder.PrependUOffsetTRelative(offset)
     projection = builder.EndVector()
 
-    response_schema = VastDBResponseSchema(schema, projection_positions, output_field_names=output_field_names)
-
     fb_source.Start(builder)
     fb_source.AddName(builder, source_name)
     fb_source.AddSchema(builder, schema_obj)
     fb_source.AddFilter(builder, filter_obj)
     fb_source.AddProjection(builder, projection)
     source = fb_source.End(builder)
```

### Comparing `vastdb-0.1.0/vastdb/schema.py` & `vastdb-0.1.1/vastdb/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """VAST Database schema (a container of tables).
 
 VAST S3 buckets can be used to create Database schemas and tables.
 It is possible to list and access VAST snapshots generated over a bucket.
 """
 
-from . import bucket, errors, schema, table
+import logging
+from dataclasses import dataclass
 
 import pyarrow as pa
 
-from dataclasses import dataclass
-import logging
+from . import bucket, errors, schema, table
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class Schema:
     """VAST Schema."""
@@ -22,25 +22,33 @@
     bucket: "bucket.Bucket"
 
     @property
     def tx(self):
         """VAST transaction used for this schema."""
         return self.bucket.tx
 
-    def create_table(self, table_name: str, columns: pa.Schema) -> "table.Table":
+    def create_table(self, table_name: str, columns: pa.Schema, fail_if_exists=True) -> "table.Table":
         """Create a new table under this schema."""
+        if current := self.table(table_name, fail_if_missing=False):
+            if fail_if_exists:
+                raise errors.TableExists(self.bucket.name, self.name, table_name)
+            else:
+                return current
         self.tx._rpc.api.create_table(self.bucket.name, self.name, table_name, columns, txid=self.tx.txid)
         log.info("Created table: %s", table_name)
         return self.table(table_name)
 
-    def table(self, name: str) -> "table.Table":
+    def table(self, name: str, fail_if_missing=True) -> "table.Table":
         """Get a specific table under this schema."""
         t = self.tables(table_name=name)
         if not t:
-            raise errors.MissingTable(self.bucket.name, self.name, name)
+            if fail_if_missing:
+                raise errors.MissingTable(self.bucket.name, self.name, name)
+            else:
+                return None
         assert len(t) == 1, f"Expected to receive only a single table, but got: {len(t)}. tables: {t}"
         log.debug("Found table: %s", t[0])
         return t[0]
 
     def tables(self, table_name=None) -> ["table.Table"]:
         """List all tables under this schema."""
         tables = []
```

### Comparing `vastdb-0.1.0/vastdb/session.py` & `vastdb-0.1.1/vastdb/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 It should be used to interact with a specific VAST cluster.
 For more details see:
 - [Virtual IP pool configured with DNS service](https://support.vastdata.com/s/topic/0TOV40000000FThOAM/configuring-network-access-v50)
 - [S3 access & secret keys on VAST cluster](https://support.vastdata.com/s/article/UUID-4d2e7e23-b2fb-7900-d98f-96c31a499626)
 - [Tabular identity policy with the proper permissions](https://support.vastdata.com/s/article/UUID-14322b60-d6a2-89ac-3df0-3dfbb6974182)
 """
 
-from . import internal_commands
-from . import transaction
+import os
 
 import boto3
 
-import os
+from . import internal_commands, transaction
 
 
 class Session:
     """VAST database session."""
 
     def __init__(self, access=None, secret=None, endpoint=None):
         """Connect to a VAST Database endpoint, using specified credentials."""
```

### Comparing `vastdb-0.1.0/vastdb/table.py` & `vastdb-0.1.1/vastdb/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from . import errors, schema
-from .internal_commands import build_query_data_request, parse_query_data_response, \
-    TABULAR_INVALID_ROW_ID, VastdbApi
-
-import pyarrow as pa
-import ibis
-
 import concurrent.futures
+import logging
+import os
 import queue
-from threading import Event
-from math import ceil
-
 from dataclasses import dataclass, field
+from math import ceil
+from threading import Event
 from typing import List, Union
-import logging
-import os
+
+import ibis
+import pyarrow as pa
+
+from . import errors, schema
+from .internal_commands import (
+    TABULAR_INVALID_ROW_ID,
+    VastdbApi,
+    build_query_data_request,
+    parse_query_data_response,
+)
 
 log = logging.getLogger(__name__)
 
 
 INTERNAL_ROW_ID = "$row_id"
 MAX_ROWS_PER_BATCH = 512 * 1024
 # for insert we need a smaller limit due to response amplification
@@ -323,15 +326,15 @@
                     propagate_first_exception(futures, block=True)
                 finally:
                     stop_event.set()
                     while tasks_running > 0:
                         if record_batches_queue.get() is None:
                             tasks_running -= 1
 
-        return pa.RecordBatchReader.from_batches(query_data_request.response_schema.arrow_schema, batches_iterator())
+        return pa.RecordBatchReader.from_batches(query_data_request.response_schema, batches_iterator())
 
     def _combine_chunks(self, col):
         if hasattr(col, "combine_chunks"):
             return col.combine_chunks()
         else:
             return col
```

### Comparing `vastdb-0.1.0/vastdb/tests/conftest.py` & `vastdb-0.1.1/vastdb/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-import vastdb
+import os
+from pathlib import Path
 
-import pytest
 import boto3
-import os
+import pytest
+
+import vastdb
 
 
 def pytest_addoption(parser):
-    parser.addoption("--tabular-bucket-name", help="Name of the S3 bucket with Tabular enabled", default = "vastdb")
-    parser.addoption("--tabular-access-key", help="Access key with Tabular permissions (AWS_ACCESS_KEY_ID)", default = os.environ.get("AWS_ACCESS_KEY_ID", None))
-    parser.addoption("--tabular-secret-key", help="Secret key with Tabular permissions (AWS_SECRET_ACCESS_KEY)" , default = os.environ.get("AWS_SECRET_ACCESS_KEY", None))
-    parser.addoption("--tabular-endpoint-url", help="Tabular server endpoint", default = "http://localhost:9090")
+    parser.addoption("--tabular-bucket-name", help="Name of the S3 bucket with Tabular enabled", default="vastdb")
+    parser.addoption("--tabular-access-key", help="Access key with Tabular permissions (AWS_ACCESS_KEY_ID)", default=os.environ.get("AWS_ACCESS_KEY_ID", None))
+    parser.addoption("--tabular-secret-key", help="Secret key with Tabular permissions (AWS_SECRET_ACCESS_KEY)", default=os.environ.get("AWS_SECRET_ACCESS_KEY", None))
+    parser.addoption("--tabular-endpoint-url", help="Tabular server endpoint", default="http://localhost:9090")
+    parser.addoption("--data-path", help="Data files location", default=None)
+    parser.addoption("--crater-path", help="Save benchmark results in a dedicated location", default=None)
 
 
 @pytest.fixture(scope="session")
 def session(request):
     return vastdb.connect(
         access=request.config.getoption("--tabular-access-key"),
         secret=request.config.getoption("--tabular-secret-key"),
@@ -40,7 +44,17 @@
 @pytest.fixture(scope="session")
 def s3(request):
     return boto3.client(
         's3',
         aws_access_key_id=request.config.getoption("--tabular-access-key"),
         aws_secret_access_key=request.config.getoption("--tabular-secret-key"),
         endpoint_url=request.config.getoption("--tabular-endpoint-url"))
+
+
+@pytest.fixture(scope="function")
+def parquets_path(request):
+    return Path(request.config.getoption("--data-path"))
+
+
+@pytest.fixture(scope="function")
+def crater_path(request):
+    return request.config.getoption("--crater-path")
```

### Comparing `vastdb-0.1.0/vastdb/tests/test_imports.py` & `vastdb-0.1.1/vastdb/tests/test_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import pytest
-
-from tempfile import NamedTemporaryFile
 import logging
+from tempfile import NamedTemporaryFile
 
 import pyarrow as pa
 import pyarrow.parquet as pq
+import pytest
 
-from vastdb.errors import InvalidArgument, ImportFilesError
 from vastdb import util
-
+from vastdb.errors import ImportFilesError, InvalidArgument
 
 log = logging.getLogger(__name__)
 
 
 def test_parallel_imports(session, clean_bucket_name, s3):
     num_rows = 1000
     num_files = 53
```

### Comparing `vastdb-0.1.0/vastdb/tests/test_projections.py` & `vastdb-0.1.1/vastdb/tests/test_projections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import pyarrow as pa
 import logging
 
+import pyarrow as pa
+
 log = logging.getLogger(__name__)
 
 def test_basic_projections(session, clean_bucket_name):
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s1')
         columns = pa.schema([
             ('a', pa.int8()),
```

### Comparing `vastdb-0.1.0/vastdb/tests/test_sanity.py` & `vastdb-0.1.1/vastdb/tests/test_sanity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from http.server import HTTPServer, BaseHTTPRequestHandler
-from itertools import cycle
+import contextlib
 import logging
 import threading
-import contextlib
+from http.server import BaseHTTPRequestHandler, HTTPServer
+from itertools import cycle
 
 import pytest
 import requests
 
 import vastdb
 
-
 log = logging.getLogger(__name__)
 
 
 def test_hello_world(session):
     with session.transaction() as tx:
         assert tx.txid is not None
```

### Comparing `vastdb-0.1.0/vastdb/tests/test_schemas.py` & `vastdb-0.1.1/vastdb/tests/test_schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import pytest
 
+from .. import errors
+
 
 def test_schemas(session, clean_bucket_name):
     with session.transaction() as tx:
         b = tx.bucket(clean_bucket_name)
         assert b.schemas() == []
 
         s = b.create_schema('s1')
@@ -15,14 +17,30 @@
         assert s.name == 's2'
         assert b.schemas()[0].name == 's2'
 
         s.drop()
         assert b.schemas() == []
 
 
+def test_exists(session, clean_bucket_name):
+    with session.transaction() as tx:
+        b = tx.bucket(clean_bucket_name)
+        assert b.schemas() == []
+
+        s = b.create_schema('s1')
+
+        assert b.schemas() == [s]
+        with pytest.raises(errors.SchemaExists):
+            b.create_schema('s1')
+
+        assert b.schemas() == [s]
+        assert b.create_schema('s1', fail_if_exists=False) == s
+        assert b.schemas() == [s]
+
+
 def test_commits_and_rollbacks(session, clean_bucket_name):
     with session.transaction() as tx:
         b = tx.bucket(clean_bucket_name)
         assert b.schemas() == []
         b.create_schema("s3")
         assert b.schemas() != []
         # implicit commit
```

### Comparing `vastdb-0.1.0/vastdb/tests/test_tables.py` & `vastdb-0.1.1/vastdb/tests/test_tables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,29 @@
-import duckdb
-import pytest
-import threading
+import datetime as dt
+import decimal
+import logging
 import random
+import threading
+from contextlib import closing
+from tempfile import NamedTemporaryFile
+
+import duckdb
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.parquet as pq
-import decimal
-import datetime as dt
-
-from tempfile import NamedTemporaryFile
-from contextlib import contextmanager, closing
-
+import pytest
 from requests.exceptions import HTTPError
-import logging
 
-from ..table import INTERNAL_ROW_ID, QueryConfig
 from .. import errors
-
+from ..table import INTERNAL_ROW_ID, QueryConfig
+from .util import prepare_data
 
 log = logging.getLogger(__name__)
 
 
-@contextmanager
-def prepare_data(session, clean_bucket_name, schema_name, table_name, arrow_table):
-    with session.transaction() as tx:
-        s = tx.bucket(clean_bucket_name).create_schema(schema_name)
-        t = s.create_table(table_name, arrow_table.schema)
-        row_ids_array = t.insert(arrow_table)
-        row_ids = row_ids_array.to_pylist()
-        log.debug("row_ids=%s" % row_ids)
-        assert row_ids == list(range(arrow_table.num_rows))
-        yield t
-        t.drop()
-        s.drop()
-
-log = logging.getLogger(__name__)
-
 def test_tables(session, clean_bucket_name):
     columns = pa.schema([
         ('a', pa.int64()),
         ('b', pa.float32()),
         ('s', pa.utf8()),
     ])
     expected = pa.table(schema=columns, data=[
@@ -82,14 +66,36 @@
         actual = pa.Table.from_batches(t.select(columns=['a', 'b', 's']))
         assert actual.to_pydict() == {
             'a': [333],
             'b': [2.5],
             's': ['ccc']
         }
 
+
+def test_exists(session, clean_bucket_name):
+    with session.transaction() as tx:
+        s = tx.bucket(clean_bucket_name).create_schema('s1')
+        assert s.tables() == []
+
+        t = s.create_table('t', pa.schema([('x', pa.int64())]))
+
+        assert s.tables() == [t]
+        with pytest.raises(errors.TableExists):
+            s.create_table('t', pa.schema([('x', pa.int64())]))
+
+        assert s.tables() == [t]
+        assert s.create_table('t', pa.schema([('x', pa.int64())]), fail_if_exists=False) == t
+        assert s.tables() == [t]
+        assert s.create_table('t', pa.schema([('y', pa.int64())]), fail_if_exists=False) == t
+        assert s.tables() == [t]
+        assert s.create_table('t', pa.schema([('x', pa.int64())]), fail_if_exists=False) == t
+        assert s.tables() == [t]
+
+
+
 def test_update_table(session, clean_bucket_name):
     columns = pa.schema([
         ('a', pa.int64()),
         ('b', pa.float32()),
         ('s', pa.utf8()),
     ])
     expected = pa.table(schema=columns, data=[
@@ -165,43 +171,84 @@
         ('a2', pa.int16()),
         ('a4', pa.int64()),
         ('b', pa.float32()),
         ('s', pa.string()),
         ('d', pa.decimal128(7, 3)),
         ('bin', pa.binary()),
         ('date', pa.date32()),
-        ('ts' ,pa.timestamp('s')),
+        ('t0', pa.time32('s')),
+        ('t3', pa.time32('ms')),
+        ('t6', pa.time64('us')),
+        ('t9', pa.time64('ns')),
+        ('ts0' ,pa.timestamp('s')),
+        ('ts3' ,pa.timestamp('ms')),
+        ('ts6' ,pa.timestamp('us')),
+        ('ts9' ,pa.timestamp('ns')),
     ])
 
     expected = pa.table(schema=columns, data=[
         [True, True, False],
         [1 , 2, 4],
         [1999, 2000, 2001],
         [11122221, 222111122, 333333],
         [0.5, 1.5, 2.5],
         ["a", "v", "s"],
         [decimal.Decimal('110.52'), decimal.Decimal('231.15'), decimal.Decimal('3332.44')],
         [b"\x01\x02", b"\x01\x05", b"\x01\x07"],
-        [dt.datetime.now().date(), dt.datetime.now().date(), dt.datetime.now().date()],
-        [dt.datetime.fromtimestamp(10000), dt.datetime.fromtimestamp(100), dt.datetime.fromtimestamp(0)]
+        [dt.date(2024, 4, 10), dt.date(2024, 4, 11), dt.date(2024, 4, 12)],
+        [dt.time(12, 34, 56), dt.time(12, 34, 57), dt.time(12, 34, 58)],
+        [dt.time(12, 34, 56, 789000), dt.time(12, 34, 57, 789000), dt.time(12, 34, 58, 789000)],
+        [dt.time(12, 34, 56, 789789), dt.time(12, 34, 57, 789789), dt.time(12, 34, 58, 789789)],
+        [dt.time(12, 34, 56, 789789), dt.time(12, 34, 57, 789789), dt.time(12, 34, 58, 789789)],
+        [dt.datetime(2024, 4, 10, 12, 34, 56), dt.datetime(2025, 4, 10, 12, 34, 56), dt.datetime(2026, 4, 10, 12, 34, 56)],
+        [dt.datetime(2024, 4, 10, 12, 34, 56, 789000), dt.datetime(2025, 4, 10, 12, 34, 56, 789000), dt.datetime(2026, 4, 10, 12, 34, 56, 789000)],
+        [dt.datetime(2024, 4, 10, 12, 34, 56, 789789), dt.datetime(2025, 4, 10, 12, 34, 56, 789789), dt.datetime(2026, 4, 10, 12, 34, 56, 789789)],
+        [dt.datetime(2024, 4, 10, 12, 34, 56, 789789), dt.datetime(2025, 4, 10, 12, 34, 56, 789789), dt.datetime(2026, 4, 10, 12, 34, 56, 789789)],
     ])
+
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
         def select(predicate):
             return pa.Table.from_batches(t.select(predicate=predicate))
 
         assert select(None) == expected
         assert select(t['tb'] == False) == expected.filter(pc.field('tb') == False)  # noqa: E712
         assert select(t['a1'] == 2) == expected.filter(pc.field('a1') == 2)
         assert select(t['a2'] == 2000) == expected.filter(pc.field('a2') == 2000)
         assert select(t['a4'] == 222111122) == expected.filter(pc.field('a4') == 222111122)
         assert select(t['b'] == 1.5) == expected.filter(pc.field('b') == 1.5)
         assert select(t['s'] == "v") == expected.filter(pc.field('s') == "v")
         assert select(t['d'] == 231.15) == expected.filter(pc.field('d') == 231.15)
         assert select(t['bin'] == b"\x01\x02") == expected.filter(pc.field('bin') == b"\x01\x02")
-        assert select(t['date'] == dt.datetime.now().date()) == expected.filter(pc.field('date') == dt.datetime.now().date())
+
+        date_literal = dt.date(2024, 4, 10)
+        assert select(t['date'] == date_literal) == expected.filter(pc.field('date') == date_literal)
+
+        time_literal = dt.time(12, 34, 56)
+        assert select(t['t0'] == time_literal) == expected.filter(pc.field('t0') == time_literal)
+
+        time_literal = dt.time(12, 34, 56, 789000)
+        assert select(t['t3'] == time_literal) == expected.filter(pc.field('t3') == time_literal)
+
+        time_literal = dt.time(12, 34, 56, 789789)
+        assert select(t['t6'] == time_literal) == expected.filter(pc.field('t6') == time_literal)
+
+        time_literal = dt.time(12, 34, 56, 789789)
+        assert select(t['t9'] == time_literal) == expected.filter(pc.field('t9') == time_literal)
+
+        ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56)
+        assert select(t['ts0'] == ts_literal) == expected.filter(pc.field('ts0') == ts_literal)
+
+        ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56, 789000)
+        assert select(t['ts3'] == ts_literal) == expected.filter(pc.field('ts3') == ts_literal)
+
+        ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56, 789789)
+        assert select(t['ts6'] == ts_literal) == expected.filter(pc.field('ts6') == ts_literal)
+
+        ts_literal = dt.datetime(2024, 4, 10, 12, 34, 56, 789789)
+        assert select(t['ts9'] == ts_literal) == expected.filter(pc.field('ts9') == ts_literal)
 
 
 def test_filters(session, clean_bucket_name):
     columns = pa.schema([
         ('a', pa.int32()),
         ('b', pa.float64()),
         ('s', pa.utf8()),
```

### Comparing `vastdb-0.1.0/vastdb/transaction.py` & `vastdb-0.1.1/vastdb/transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 A transcation is used as a context manager, since every Database-related operation in VAST requires a transaction.
 
     with session.transaction() as tx:
         tx.bucket("bucket").create_schema("schema")
 """
 
-from . import bucket, errors, session
+import logging
+from dataclasses import dataclass
 
 import botocore
 
-from dataclasses import dataclass
-import logging
-
+from . import bucket, errors, session
 
 log = logging.getLogger(__name__)
 
 @dataclass
 class Transaction:
     """A holder of a single VAST transaction."""
```

### Comparing `vastdb-0.1.0/vastdb/util.py` & `vastdb-0.1.1/vastdb/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from typing import Callable
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 from .errors import InvalidArgument
 from .schema import Schema
-from .table import Table
+from .table import ImportConfig, Table
 
 log = logging.getLogger(__name__)
 
 
 def create_table_from_files(
-        schema: Schema, table_name: str, parquet_files: [str], schema_merge_func: Callable = None) -> Table:
+        schema: Schema, table_name: str, parquet_files: [str], schema_merge_func: Callable = None,
+        config: ImportConfig = None) -> Table:
     if not schema_merge_func:
         schema_merge_func = default_schema_merge
     else:
         assert schema_merge_func in [default_schema_merge, strict_schema_merge, union_schema_merge]
     tx = schema.tx
     current_schema = pa.schema([])
     s3fs = pa.fs.S3FileSystem(
@@ -28,15 +29,15 @@
         current_schema = schema_merge_func(current_schema, parquet_ds.schema)
 
     log.info("Creating table %s from %d Parquet files, with columns: %s",
              table_name, len(parquet_files), list(current_schema))
     table = schema.create_table(table_name, current_schema)
 
     log.info("Starting import of %d files to table: %s", len(parquet_files), table)
-    table.import_files(parquet_files)
+    table.import_files(parquet_files, config=config)
     log.info("Finished import of %d files to table: %s", len(parquet_files), table)
     return table
 
 
 def default_schema_merge(current_schema: pa.Schema, new_schema: pa.Schema) -> pa.Schema:
     """
     This function validates a schema is contained in another schema
```

### Comparing `vastdb-0.1.0/vastdb.egg-info/PKG-INFO` & `vastdb-0.1.1/vastdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vastdb-0.1.0/vastdb.egg-info/SOURCES.txt` & `vastdb-0.1.1/vastdb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+CHANGELOG.md
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 vast_flatbuf/__init__.py
 vast_flatbuf/org/__init__.py
 vast_flatbuf/org/apache/__init__.py
 vast_flatbuf/org/apache/arrow/__init__.py
 vast_flatbuf/org/apache/arrow/computeir/__init__.py
 vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
@@ -149,26 +152,30 @@
 vast_flatbuf/tabular/ListTablesResponse.py
 vast_flatbuf/tabular/ObjectDetails.py
 vast_flatbuf/tabular/S3File.py
 vast_flatbuf/tabular/VipRange.py
 vast_flatbuf/tabular/__init__.py
 vastdb/__init__.py
 vastdb/bucket.py
+vastdb/conftest.py
 vastdb/errors.py
 vastdb/internal_commands.py
 vastdb/schema.py
 vastdb/session.py
 vastdb/table.py
 vastdb/transaction.py
 vastdb/util.py
 vastdb.egg-info/PKG-INFO
 vastdb.egg-info/SOURCES.txt
 vastdb.egg-info/dependency_links.txt
 vastdb.egg-info/requires.txt
 vastdb.egg-info/top_level.txt
+vastdb/bench/__init__.py
+vastdb/bench/test_perf.py
 vastdb/tests/__init__.py
-vastdb/tests/conftest.py
 vastdb/tests/test_imports.py
+vastdb/tests/test_nested.py
 vastdb/tests/test_projections.py
 vastdb/tests/test_sanity.py
 vastdb/tests/test_schemas.py
-vastdb/tests/test_tables.py
+vastdb/tests/test_tables.py
+vastdb/tests/util.py
```

