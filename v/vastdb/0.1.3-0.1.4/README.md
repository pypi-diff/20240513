# Comparing `tmp/vastdb-0.1.3.tar.gz` & `tmp/vastdb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastdb-0.1.3.tar", last modified: Sun May  5 11:44:30 2024, max compression
+gzip compressed data, was "vastdb-0.1.4.tar", last modified: Mon May 13 08:36:48 2024, max compression
```

## Comparing `vastdb-0.1.3.tar` & `vastdb-0.1.4.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.497443 vastdb-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     4052 2024-05-05 10:46:44.000000 vastdb-0.1.3/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11333 2024-05-05 10:46:44.000000 vastdb-0.1.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-05 10:46:44.000000 vastdb-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1318 2024-05-05 11:44:30.497443 vastdb-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6027 2024-05-05 10:46:44.000000 vastdb-0.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-05 10:46:44.000000 vastdb-0.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 11:44:30.497443 vastdb-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1702 2024-05-05 10:46:44.000000 vastdb-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/org/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/org/apache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.477443 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     5630 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
--rw-rw-rw-   0 root         (0) root         (0)     3260 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2602 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
--rw-rw-rw-   0 root         (0) root         (0)     4455 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
--rw-rw-rw-   0 root         (0) root         (0)     1723 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     3847 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
--rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
--rw-rw-rw-   0 root         (0) root         (0)     3678 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
--rw-rw-rw-   0 root         (0) root         (0)     3952 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
--rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
--rw-rw-rw-   0 root         (0) root         (0)     5650 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
--rw-rw-rw-   0 root         (0) root         (0)     7527 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.488443 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2855 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
--rw-rw-rw-   0 root         (0) root         (0)     3148 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     4091 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
--rw-rw-rw-   0 root         (0) root         (0)     1925 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/List.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
--rw-rw-rw-   0 root         (0) root         (0)     5589 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     6042 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
--rw-rw-rw-   0 root         (0) root         (0)     5785 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
--rw-rw-rw-   0 root         (0) root         (0)     6091 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     6389 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
--rw-rw-rw-   0 root         (0) root         (0)     9409 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
--rw-rw-rw-   0 root         (0) root         (0)     5767 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
--rw-rw-rw-   0 root         (0) root         (0)     2639 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     7925 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.491443 vastdb-0.1.3/vast_flatbuf/tabular/
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/AlterColumnRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/AlterProjectionTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/AlterSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/AlterTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/Column.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ColumnType.py
--rw-rw-rw-   0 root         (0) root         (0)     2516 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/CreateProjectionRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/CreateSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/GetTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ImportDataRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ListProjectionsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ListSchemasResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ListTablesResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ObjectDetails.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/S3File.py
--rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/VipRange.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.493443 vastdb-0.1.3/vastdb/
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.494443 vastdb-0.1.3/vastdb/bench/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/bench/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/bench/test_perf.py
--rw-rw-rw-   0 root         (0) root         (0)     3566 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/bucket.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3793 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    99575 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/internal_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     3346 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2323 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/session.py
--rw-rw-rw-   0 root         (0) root         (0)    25661 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.496443 vastdb-0.1.3/vastdb/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_duckdb.py
--rw-rw-rw-   0 root         (0) root         (0)     5705 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_imports.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_nested.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_projections.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_sanity.py
--rw-rw-rw-   0 root         (0) root         (0)     1739 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_schemas.py
--rw-rw-rw-   0 root         (0) root         (0)    26672 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_tables.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/util.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     4276 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.496443 vastdb-0.1.3/vastdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1318 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9048 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.725018 vastdb-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     4344 2024-05-13 07:47:14.000000 vastdb-0.1.4/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11333 2024-05-13 07:47:14.000000 vastdb-0.1.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-13 07:47:14.000000 vastdb-0.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-13 08:36:48.725018 vastdb-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6027 2024-05-13 07:47:14.000000 vastdb-0.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-13 07:47:14.000000 vastdb-0.1.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 08:36:48.725018 vastdb-0.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2024-05-13 07:47:14.000000 vastdb-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.669021 vastdb-0.1.4/vast_flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.669021 vastdb-0.1.4/vast_flatbuf/org/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.670021 vastdb-0.1.4/vast_flatbuf/org/apache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.670021 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.670021 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.692020 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2602 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
+-rw-rw-rw-   0 root         (0) root         (0)     4455 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     3847 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
+-rw-rw-rw-   0 root         (0) root         (0)     7527 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.710019 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3148 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4091 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/List.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
+-rw-rw-rw-   0 root         (0) root         (0)     5589 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6042 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5785 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
+-rw-rw-rw-   0 root         (0) root         (0)     6091 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     6389 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
+-rw-rw-rw-   0 root         (0) root         (0)     9409 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
+-rw-rw-rw-   0 root         (0) root         (0)     5767 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7925 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.716018 vastdb-0.1.4/vast_flatbuf/tabular/
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/AlterColumnRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/AlterProjectionTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/AlterSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/AlterTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/Column.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ColumnType.py
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/CreateProjectionRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/CreateSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/GetTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ImportDataRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ListProjectionsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ListSchemasResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ListTablesResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/ObjectDetails.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/S3File.py
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-13 07:47:14.000000 vastdb-0.1.4/vast_flatbuf/tabular/VipRange.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vast_flatbuf/tabular/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.719018 vastdb-0.1.4/vastdb/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.721018 vastdb-0.1.4/vastdb/bench/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vastdb/bench/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/bench/test_perf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3566 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/bucket.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)   100414 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/internal_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     3346 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/session.py
+-rw-rw-rw-   0 root         (0) root         (0)    28891 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.724018 vastdb-0.1.4/vastdb/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:52:02.000000 vastdb-0.1.4/vastdb/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_duckdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5705 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_projections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_sanity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)    27499 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_tables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/test_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/tests/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2024-05-13 07:47:14.000000 vastdb-0.1.4/vastdb/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:36:48.724018 vastdb-0.1.4/vastdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9048 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-13 08:36:48.000000 vastdb-0.1.4/vastdb.egg-info/top_level.txt
```

### Comparing `vastdb-0.1.3/CHANGELOG.md` & `vastdb-0.1.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## [0.1.4] (2024-05-13)
+[0.1.4]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.3...v0.1.4
+
+### Added
+ - Resume `Table.select()` on HTTP 503 code
+ - Allow pushing down True/False boolean literals
+ - Support `between` predicate pushdown
+ - Support inserting wide rows (larger than 5MB)
+
 ## [0.1.3] (2024-05-05)
 [0.1.3]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.2...v0.1.3
 
 ### Added
  - Document predicate pushdown support
  - Access imports' table (for VAST 5.2+)
  - Support `is_in` predicate pushdown
```

### Comparing `vastdb-0.1.3/LICENSE` & `vastdb-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/PKG-INFO` & `vastdb-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.3
+Version: 0.1.4
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,14 +21,15 @@
 Requires-Dist: aws-requests-auth
 Requires-Dist: boto3
 Requires-Dist: flatbuffers
 Requires-Dist: ibis-framework==8.0.0
 Requires-Dist: pyarrow
 Requires-Dist: requests
 Requires-Dist: xmltodict
+Requires-Dist: backoff==2.2.1
 
 
 `vastdb` is a Python-based SDK designed for interacting
 with [VAST Database](https://vastdata.com/database)
 and [VAST Catalog](https://vastdata.com/blog/vast-catalog-treat-your-file-system-like-a-database),
 enabling schema and table management, efficient ingest, query and modification of columnar data.
```

### Comparing `vastdb-0.1.3/README.md` & `vastdb-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/setup.py` & `vastdb-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 if os.environ.get('VASTDB_APPEND_VERSION_SUFFIX'):
     suffix = _get_version_suffix()
 
 setup(
     name='vastdb',
     python_requires='>=3.9.0',
     description='VAST Data SDK',
-    version='0.1.3' + suffix,
+    version='0.1.4' + suffix,
     url='https://github.com/vast-data/vastdb_sdk',
     author='VAST DATA',
     author_email='hello@vastdata.com',
     license='Copyright (C) VAST Data Ltd.',
     packages=find_packages(),
     install_requires=open('requirements.txt').read().strip().split('\n'),
     long_description=long_description,
```

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Block.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Block.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Date.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Date.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Field.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Field.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Int.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Int.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/List.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/List.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Map.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Map.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Message.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Message.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Null.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Null.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Time.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Time.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Type.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Type.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Union.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Union.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py` & `vastdb-0.1.4/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/AlterColumnRequest.py` & `vastdb-0.1.4/vast_flatbuf/tabular/AlterColumnRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/AlterProjectionTableRequest.py` & `vastdb-0.1.4/vast_flatbuf/tabular/AlterProjectionTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/AlterSchemaRequest.py` & `vastdb-0.1.4/vast_flatbuf/tabular/AlterSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/AlterTableRequest.py` & `vastdb-0.1.4/vast_flatbuf/tabular/AlterTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/Column.py` & `vastdb-0.1.4/vast_flatbuf/tabular/Column.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/CreateProjectionRequest.py` & `vastdb-0.1.4/vast_flatbuf/tabular/CreateProjectionRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/CreateSchemaRequest.py` & `vastdb-0.1.4/vast_flatbuf/tabular/CreateSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py` & `vastdb-0.1.4/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/GetTableStatsResponse.py` & `vastdb-0.1.4/vast_flatbuf/tabular/GetTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/ImportDataRequest.py` & `vastdb-0.1.4/vast_flatbuf/tabular/ImportDataRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/ListProjectionsResponse.py` & `vastdb-0.1.4/vast_flatbuf/tabular/ListProjectionsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/ListSchemasResponse.py` & `vastdb-0.1.4/vast_flatbuf/tabular/ListSchemasResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/ListTablesResponse.py` & `vastdb-0.1.4/vast_flatbuf/tabular/ListTablesResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/ObjectDetails.py` & `vastdb-0.1.4/vast_flatbuf/tabular/ObjectDetails.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/S3File.py` & `vastdb-0.1.4/vast_flatbuf/tabular/S3File.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vast_flatbuf/tabular/VipRange.py` & `vastdb-0.1.4/vast_flatbuf/tabular/VipRange.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/bench/test_perf.py` & `vastdb-0.1.4/vastdb/bench/test_perf.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/bucket.py` & `vastdb-0.1.4/vastdb/bucket.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/conftest.py` & `vastdb-0.1.4/vastdb/conftest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/errors.py` & `vastdb-0.1.4/vastdb/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,18 @@
     pass
 
 
 class ServiceUnavailable(HttpError):
     pass
 
 
+class Slowdown(ServiceUnavailable):
+    pass
+
+
 class UnexpectedError(HttpError):
     pass
 
 
 @dataclass
 class ImportFilesError(Exception):
     message: str
@@ -93,14 +97,18 @@
     pass
 
 
 class MissingTransaction(Missing):
     pass
 
 
+class MissingRowIdColumn(Missing):
+    pass
+
+
 class NotSupported(Exception):
     pass
 
 
 @dataclass
 class MissingBucket(Missing):
     bucket: str
@@ -159,24 +167,30 @@
 
 @dataclass
 class NotSupportedVersion(NotSupported):
     err_msg: str
     version: str
 
 
+def handle_unavailable(**kwargs):
+    if kwargs['code'] == 'SlowDown':
+        raise Slowdown(**kwargs)
+    raise ServiceUnavailable(**kwargs)
+
+
 ERROR_TYPES_MAP = {
     HttpStatus.BAD_REQUEST: BadRequest,
     HttpStatus.FOBIDDEN: Forbidden,
     HttpStatus.NOT_FOUND: NotFound,
     HttpStatus.METHOD_NOT_ALLOWED: MethodNotAllowed,
     HttpStatus.REQUEST_TIMEOUT: RequestTimeout,
     HttpStatus.CONFLICT: Conflict,
     HttpStatus.INTERNAL_SERVER_ERROR: InternalServerError,
     HttpStatus.NOT_IMPLEMENTED: NotImplemented,
-    HttpStatus.SERVICE_UNAVAILABLE: ServiceUnavailable,
+    HttpStatus.SERVICE_UNAVAILABLE: handle_unavailable,
 }
 
 
 def from_response(res: requests.Response):
     if res.status_code == HttpStatus.SUCCESS.value:
         return None
 
@@ -201,8 +215,8 @@
         url=res.request.url,
         status=res.status_code,
         headers=res.headers,
     )
     log.warning("RPC failed: %s", kwargs)
     status = HttpStatus(res.status_code)
     error_type = ERROR_TYPES_MAP.get(status, UnexpectedError)
-    return error_type(**kwargs)
+    return error_type(**kwargs)  # type: ignore
```

### Comparing `vastdb-0.1.3/vastdb/internal_commands.py` & `vastdb-0.1.4/vastdb/internal_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         from ibis.expr.operations.generic import (
             IsNull,
             Literal,
             TableColumn,
         )
         from ibis.expr.operations.logical import (
             And,
+            Between,
             Equals,
             Greater,
             GreaterEqual,
             InValues,
             Less,
             LessEqual,
             Not,
@@ -196,14 +197,15 @@
             Less: self.build_less,
             LessEqual: self.build_less_equal,
             Equals: self.build_equal,
             NotEquals: self.build_not_equal,
             IsNull: self.build_is_null,
             Not: self.build_is_not_null,
             StringContains: self.build_match_substring,
+            Between: self.build_between,
         }
 
         positions_map = dict((f.name, index) for index, f in enumerate(self.schema))  # TODO: BFS
 
         self.builder = builder
 
         offsets = []
@@ -233,14 +235,17 @@
                     elif builder_func == self.build_is_not_null:
                         not_arg, = inner_op.args
                         # currently we only support not is_null, checking we really got is_null under the not:
                         if not builder_map.get(type(not_arg)) == self.build_is_null:
                             raise NotImplementedError(self.expr)
                         column, = not_arg.args
                         literals = (None,)
+                    elif builder_func == self.build_between:
+                        column, lower, upper = inner_op.args
+                        literals = (None,)
                     else:
                         column, arg = inner_op.args
                         if isinstance(arg, tuple):
                             literals = arg
                         else:
                             literals = (arg,)
                         for literal in literals:
@@ -258,14 +263,17 @@
 
                     column_offset = self.build_column(position=positions_map[field_name])
                     field = self.schema.field(field_name)
                     for literal in literals:
                         args_offsets = [column_offset]
                         if literal is not None:
                             args_offsets.append(self.build_literal(field=field, value=literal.value))
+                        if builder_func == self.build_between:
+                            args_offsets.append(self.build_literal(field=field, value=lower.value))
+                            args_offsets.append(self.build_literal(field=field, value=upper.value))
 
                         inner_offsets.append(builder_func(*args_offsets))
 
                 if not inner_offsets:
                     raise NotImplementedError(self.expr)  # an empty OR is equivalent to a 'FALSE' literal
 
                 domain_offset = self.build_or(inner_offsets)
@@ -552,14 +560,21 @@
 
     def build_is_not_null(self, column: int):
         return self.build_function('is_valid', column)
 
     def build_match_substring(self, column: int, literal: int):
         return self.build_function('match_substring', column, literal)
 
+    def build_between(self, column: int, lower: int, upper: int):
+        offsets = [
+            self.build_greater_equal(column, lower),
+            self.build_less_equal(column, upper),
+        ]
+        return self.build_and(offsets)
+
 
 class FieldNodesState:
     def __init__(self) -> None:
         # will be set during by the parser (see below)
         self.buffers: Dict[int, Any] = defaultdict(lambda: None)  # a list of Arrow buffers (https://arrow.apache.org/docs/format/Columnar.html#buffer-listing-for-each-layout)
         self.length: Dict[int, Any] = defaultdict(lambda: None)  # each array must have it's length specified (https://arrow.apache.org/docs/python/generated/pyarrow.Array.html#pyarrow.Array.from_buffers)
 
@@ -1574,16 +1589,15 @@
         Request Body
             RecordBatch
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
         headers['Content-Length'] = str(len(record_batch))
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="rows"),
                                 data=record_batch, headers=headers, stream=True)
-        self._check_res(res, "insert_rows", expected_retvals)
-        res.raw.read()  # flush the response
+        return self._check_res(res, "insert_rows", expected_retvals)
 
     def update_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[]):
         """
         PUT /mybucket/myschema/mytable?rows HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
@@ -2103,14 +2117,21 @@
 class QueryDataRequest:
     def __init__(self, serialized, response_schema, response_parser):
         self.serialized = serialized
         self.response_schema = response_schema
         self.response_parser = response_parser
 
 
+def get_response_schema(schema: 'pa.Schema' = pa.schema([]), field_names: Optional[List[str]] = None):
+    if field_names is None:
+        field_names = [field.name for field in schema]
+
+    return pa.schema([schema.field(name) for name in field_names])
+
+
 def build_query_data_request(schema: 'pa.Schema' = pa.schema([]), predicate: ibis.expr.types.BooleanColumn = None, field_names: Optional[List[str]] = None):
     builder = flatbuffers.Builder(1024)
 
     source_name = builder.CreateString('')  # required
 
     fields = [build_field(builder, f, f.name) for f in schema]
 
@@ -2123,21 +2144,19 @@
     fb_schema.AddFields(builder, fields)
     schema_obj = fb_schema.End(builder)
 
     predicate = Predicate(schema=schema, expr=predicate)
     filter_obj = predicate.serialize(builder)
 
     parser = QueryDataParser(schema)
-    fields_map = {node.field.name: node.field for node in parser.nodes}
     leaves_map = {node.field.name: [leaf.index for leaf in node._iter_leaves()] for node in parser.nodes}
 
-    if field_names is None:
-        field_names = [field.name for field in schema]
+    response_schema = get_response_schema(schema, field_names)
+    field_names = [field.name for field in response_schema]
 
-    response_schema = pa.schema([fields_map[name] for name in field_names])
     projection_fields = []
     for field_name in field_names:
         # TODO: only root-level projection pushdown is supported (i.e. no support for SELECT s.x FROM t)
         positions = leaves_map[field_name]
         for leaf_position in positions:
             fb_field_index.Start(builder)
             fb_field_index.AddPosition(builder, leaf_position)
```

### Comparing `vastdb-0.1.3/vastdb/schema.py` & `vastdb-0.1.4/vastdb/schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/session.py` & `vastdb-0.1.4/vastdb/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,19 @@
         self.vast_version = vast_version
 
     def check_imports_table(self):
         """Check if the feature that support imports table is supported."""
         if self.vast_version < (5, 2):
             raise errors.NotSupportedVersion("import_table requires 5.2+", self.vast_version)
 
+    def check_return_row_ids(self):
+        """Check if insert/update/delete can return the row_ids."""
+        if self.vast_version < (5, 1):
+            raise errors.NotSupportedVersion("return_row_ids requires 5.1+", self.vast_version)
+
 
 class Session:
     """VAST database session."""
 
     def __init__(self, access=None, secret=None, endpoint=None):
         """Connect to a VAST Database endpoint, using specified credentials."""
         if access is None:
```

### Comparing `vastdb-0.1.3/vastdb/table.py` & `vastdb-0.1.4/vastdb/table.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,34 @@
 import concurrent.futures
 import logging
 import os
 import queue
 from dataclasses import dataclass, field
 from math import ceil
 from threading import Event
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
+import backoff
 import ibis
 import pyarrow as pa
 
 from . import errors, internal_commands, schema, util
 
 log = logging.getLogger(__name__)
 
 
 INTERNAL_ROW_ID = "$row_id"
+INTERNAL_ROW_ID_FIELD = pa.field(INTERNAL_ROW_ID, pa.uint64())
+
 MAX_ROWS_PER_BATCH = 512 * 1024
 # for insert we need a smaller limit due to response amplification
 # for example insert of 512k uint8 result in 512k*8bytes response since row_ids are uint64
 MAX_INSERT_ROWS_PER_PATCH = 512 * 1024
+# in case insert has TooWideRow - need to insert in smaller batches - each cell could contain up to 128K, and our wire is limited to 5MB
+MAX_COLUMN_IN_BATCH = int(5 * 1024 / 128)
 
 
 @dataclass
 class TableStats:
     """Table-related information."""
 
     num_rows: int
@@ -42,14 +47,16 @@
     num_splits: int = 1
     data_endpoints: Optional[List[str]] = None
     limit_rows_per_sub_split: int = 128 * 1024
     num_row_groups_per_sub_split: int = 8
     use_semi_sorted_projections: bool = True
     rows_per_split: int = 4000000
     query_id: str = ""
+    max_slowdown_retry: int = 10
+    backoff_func: Any = field(default=backoff.on_exception(backoff.expo, errors.Slowdown, max_tries=max_slowdown_retry))
 
 
 @dataclass
 class ImportConfig:
     """Import execution configiration."""
 
     import_concurrency: int = 2
@@ -68,15 +75,16 @@
 
     def batches(self, api: internal_commands.VastdbApi):
         """Execute QueryData request, and yield parsed RecordBatch objects.
 
         Can be called repeatedly, to allow pagination.
         """
         while not self.done:
-            response = api.query_data(
+            query_with_backoff = self.config.backoff_func(api.query_data)
+            response = query_with_backoff(
                             bucket=self.table.bucket.name,
                             schema=self.table.schema.name,
                             table=self.table.name,
                             params=self.query_data_request.serialized,
                             split=(self.split_id, self.config.num_splits, self.config.num_row_groups_per_sub_split),
                             num_sub_splits=self.config.num_sub_splits,
                             response_row_id=False,
@@ -287,19 +295,25 @@
         log.debug(f"num_rows={stats.num_rows} rows_per_splits={config.rows_per_split} num_splits={config.num_splits} ")
 
         if columns is None:
             columns = [f.name for f in self.arrow_schema]
 
         query_schema = self.arrow_schema
         if internal_row_id:
-            queried_fields = [pa.field(INTERNAL_ROW_ID, pa.uint64())]
+            queried_fields = [INTERNAL_ROW_ID_FIELD]
             queried_fields.extend(column for column in self.arrow_schema)
             query_schema = pa.schema(queried_fields)
             columns.append(INTERNAL_ROW_ID)
 
+        if predicate is True:
+            predicate = None
+        if predicate is False:
+            response_schema = internal_commands.get_response_schema(schema=query_schema, field_names=columns)
+            return pa.RecordBatchReader.from_batches(response_schema, [])
+
         query_data_request = internal_commands.build_query_data_request(
             schema=query_schema,
             predicate=predicate,
             field_names=columns)
 
         splits_queue: queue.Queue[int] = queue.Queue()
 
@@ -381,35 +395,76 @@
                     stop_event.set()
                     while tasks_running > 0:
                         if record_batches_queue.get() is None:
                             tasks_running -= 1
 
         return pa.RecordBatchReader.from_batches(query_data_request.response_schema, batches_iterator())
 
-    def insert(self, rows: pa.RecordBatch) -> pa.RecordBatch:
+    def insert_in_column_batches(self, rows: pa.RecordBatch):
+        """Split the RecordBatch into max_columns that can be inserted in single RPC.
+
+        Insert first MAX_COLUMN_IN_BATCH columns and get the row_ids. Then loop on the rest of the columns and
+        update in groups of MAX_COLUMN_IN_BATCH.
+        """
+        column_record_batch = pa.RecordBatch.from_arrays([_combine_chunks(rows.column(i)) for i in range(0, MAX_COLUMN_IN_BATCH)],
+                                                         schema=pa.schema([rows.schema.field(i) for i in range(0, MAX_COLUMN_IN_BATCH)]))
+        row_ids = self.insert(rows=column_record_batch)  # type: ignore
+
+        columns_names = [field.name for field in rows.schema]
+        columns = list(rows.schema)
+        arrays = [_combine_chunks(rows.column(i)) for i in range(len(rows.schema))]
+        for start in range(MAX_COLUMN_IN_BATCH, len(rows.schema), MAX_COLUMN_IN_BATCH):
+            end = start + MAX_COLUMN_IN_BATCH if start + MAX_COLUMN_IN_BATCH < len(rows.schema) else len(rows.schema)
+            columns_name_chunk = columns_names[start:end]
+            columns_chunks = columns[start:end]
+            arrays_chunks = arrays[start:end]
+            columns_chunks.append(INTERNAL_ROW_ID_FIELD)
+            arrays_chunks.append(row_ids.to_pylist())
+            column_record_batch = pa.RecordBatch.from_arrays(arrays_chunks, schema=pa.schema(columns_chunks))
+            self.update(rows=column_record_batch, columns=columns_name_chunk)
+        return row_ids
+
+    def insert(self, rows: pa.RecordBatch):
         """Insert a RecordBatch into this table."""
         if self._imports_table:
             raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
-        serialized_slices = util.iter_serialized_slices(rows, MAX_INSERT_ROWS_PER_PATCH)
-        for slice in serialized_slices:
-            self.tx._rpc.api.insert_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
-                                               txid=self.tx.txid)
+        try:
+            row_ids = []
+            serialized_slices = util.iter_serialized_slices(rows, MAX_INSERT_ROWS_PER_PATCH)
+            for slice in serialized_slices:
+                res = self.tx._rpc.api.insert_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
+                                                   txid=self.tx.txid)
+                (batch,) = pa.RecordBatchStreamReader(res.raw)
+                row_ids.append(batch[INTERNAL_ROW_ID])
+            try:
+                self.tx._rpc.features.check_return_row_ids()
+            except errors.NotSupportedVersion:
+                return  # type: ignore
+            return pa.chunked_array(row_ids)
+        except errors.TooWideRow:
+            self.tx._rpc.features.check_return_row_ids()
+            return self.insert_in_column_batches(rows)
 
     def update(self, rows: Union[pa.RecordBatch, pa.Table], columns: Optional[List[str]] = None) -> None:
         """Update a subset of cells in this table.
 
-        Row IDs are specified using a special field (named "$row_id" of uint64 type).
+        Row IDs are specified using a special field (named "$row_id" of uint64 type) - this function assume that this
+        special field is part of arguments.
 
         A subset of columns to be updated can be specified via the `columns` argument.
         """
         if self._imports_table:
             raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
+        try:
+            rows_chunk = rows[INTERNAL_ROW_ID]
+        except KeyError:
+            raise errors.MissingRowIdColumn
         if columns is not None:
             update_fields = [(INTERNAL_ROW_ID, pa.uint64())]
-            update_values = [_combine_chunks(rows[INTERNAL_ROW_ID])]
+            update_values = [_combine_chunks(rows_chunk)]
             for col in columns:
                 update_fields.append(rows.field(col))
                 update_values.append(_combine_chunks(rows[col]))
 
             update_rows_rb = pa.record_batch(schema=pa.schema(update_fields), data=update_values)
         else:
             update_rows_rb = rows
@@ -420,16 +475,22 @@
                                          txid=self.tx.txid)
 
     def delete(self, rows: Union[pa.RecordBatch, pa.Table]) -> None:
         """Delete a subset of rows in this table.
 
         Row IDs are specified using a special field (named "$row_id" of uint64 type).
         """
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
+        try:
+            rows_chunk = rows[INTERNAL_ROW_ID]
+        except KeyError:
+            raise errors.MissingRowIdColumn
         delete_rows_rb = pa.record_batch(schema=pa.schema([(INTERNAL_ROW_ID, pa.uint64())]),
-                                         data=[_combine_chunks(rows[INTERNAL_ROW_ID])])
+                                         data=[_combine_chunks(rows_chunk)])
 
         serialized_slices = util.iter_serialized_slices(delete_rows_rb, MAX_ROWS_PER_BATCH)
         for slice in serialized_slices:
             self.tx._rpc.api.delete_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
                                          txid=self.tx.txid, delete_from_imports_table=self._imports_table)
 
     def drop(self) -> None:
```

### Comparing `vastdb-0.1.3/vastdb/tests/test_duckdb.py` & `vastdb-0.1.4/vastdb/tests/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/tests/test_imports.py` & `vastdb-0.1.4/vastdb/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/tests/test_nested.py` & `vastdb-0.1.4/vastdb/tests/test_nested.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/tests/test_projections.py` & `vastdb-0.1.4/vastdb/tests/test_projections.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/tests/test_sanity.py` & `vastdb-0.1.4/vastdb/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/tests/test_schemas.py` & `vastdb-0.1.4/vastdb/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/tests/test_tables.py` & `vastdb-0.1.4/vastdb/tests/test_tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,24 @@
         assert actual.to_pydict() == {
             'a': [333],
             'b': [2.5],
             's': ['ccc']
         }
 
 
+def test_insert_wide_row(session, clean_bucket_name):
+    columns = pa.schema([pa.field(f's{i}', pa.utf8()) for i in range(500)])
+    data = [['a' * 10**4] for i in range(500)]
+    expected = pa.table(schema=columns, data=data)
+
+    with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
+        actual = pa.Table.from_batches(t.select())
+        assert actual == expected
+
+
 def test_exists(session, clean_bucket_name):
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s1')
         assert s.tables() == []
 
         t = s.create_table('t', pa.schema([('x', pa.int64())]))
 
@@ -261,14 +271,19 @@
     ])
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
         def select(predicate):
             return pa.Table.from_batches(t.select(predicate=predicate), t.arrow_schema)
 
         assert select(None) == expected
+        assert select(True) == expected
+        assert select(False) == pa.Table.from_batches([], schema=columns)
+
+        assert select(t['a'].between(222, 444)) == expected.filter((pc.field('a') >= 222) & (pc.field('a') <= 444))
+        assert select((t['a'].between(222, 444)) & (t['b'] > 2.5)) == expected.filter((pc.field('a') >= 222) & (pc.field('a') <= 444) & (pc.field('b') > 2.5))
 
         assert select(t['a'] > 222) == expected.filter(pc.field('a') > 222)
         assert select(t['a'] < 222) == expected.filter(pc.field('a') < 222)
         assert select(t['a'] == 222) == expected.filter(pc.field('a') == 222)
         assert select(t['a'] != 222) == expected.filter(pc.field('a') != 222)
         assert select(t['a'] <= 222) == expected.filter(pc.field('a') <= 222)
         assert select(t['a'] >= 222) == expected.filter(pc.field('a') >= 222)
@@ -327,15 +342,16 @@
 
         rb = pa.record_batch(schema=columns, data=[
             [111, 222],
             [0.5, 1.5],
             ['a', 'b'],
         ])
         expected = pa.Table.from_batches([rb])
-        t.insert(rb)
+        rb = t.insert(rb)
+        assert rb.to_pylist() == [0, 1]
         actual = pa.Table.from_batches(t.select())
         assert actual == expected
 
         table_batches = t.select()
 
         with NamedTemporaryFile() as parquet_file:
             log.info("Writing table into parquet file: '%s'", parquet_file.name)
```

### Comparing `vastdb-0.1.3/vastdb/tests/test_util.py` & `vastdb-0.1.4/vastdb/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/transaction.py` & `vastdb-0.1.4/vastdb/transaction.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb/util.py` & `vastdb-0.1.4/vastdb/util.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.3/vastdb.egg-info/PKG-INFO` & `vastdb-0.1.4/vastdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.3
+Version: 0.1.4
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,14 +21,15 @@
 Requires-Dist: aws-requests-auth
 Requires-Dist: boto3
 Requires-Dist: flatbuffers
 Requires-Dist: ibis-framework==8.0.0
 Requires-Dist: pyarrow
 Requires-Dist: requests
 Requires-Dist: xmltodict
+Requires-Dist: backoff==2.2.1
 
 
 `vastdb` is a Python-based SDK designed for interacting
 with [VAST Database](https://vastdata.com/database)
 and [VAST Catalog](https://vastdata.com/blog/vast-catalog-treat-your-file-system-like-a-database),
 enabling schema and table management, efficient ingest, query and modification of columnar data.
```

### Comparing `vastdb-0.1.3/vastdb.egg-info/SOURCES.txt` & `vastdb-0.1.4/vastdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

