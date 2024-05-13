# Comparing `tmp/pami-2024.5.1.2.tar.gz` & `tmp/pami-2024.5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2024.5.1.2.tar", last modified: Mon May 13 08:33:12 2024, max compression
+gzip compressed data, was "pami-2024.5.7.1.tar", last modified: Tue May  7 07:53:15 2024, max compression
```

## Comparing `pami-2024.5.1.2.tar` & `pami-2024.5.7.1.tar`

### file list

```diff
@@ -1,512 +1,512 @@
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.101029 pami-2024.5.1.2/
--rw-r--r--   0 vanithak   (502) staff       (20)    35149 2024-03-12 04:33:29.000000 pami-2024.5.1.2/LICENSE
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.155040 pami-2024.5.1.2/PAMI/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.156549 pami-2024.5.1.2/PAMI/AssociationRules/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.172607 pami-2024.5.1.2/PAMI/AssociationRules/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    14350 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/AssociationRules/basic/_ARWithLeverage.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14263 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/AssociationRules/basic/_ARWithLift.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19416 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/AssociationRules/basic/_RuleMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6613 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12724 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/AssociationRules/basic/confidence.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12638 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/AssociationRules/basic/leverage.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12430 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/AssociationRules/basic/lift.py
--rw-r--r--   0 vanithak   (502) staff       (20)      139 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.174336 pami-2024.5.1.2/PAMI/correlatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.183991 pami-2024.5.1.2/PAMI/correlatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    26443 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/correlatedPattern/basic/CoMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)    27988 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/correlatedPattern/basic/CoMinePlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6208 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.185279 pami-2024.5.1.2/PAMI/coveragePattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.192357 pami-2024.5.1.2/PAMI/coveragePattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    14643 2024-05-01 06:38:00.000000 pami-2024.5.1.2/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17200 2024-05-01 06:38:00.000000 pami-2024.5.1.2/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7155 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.205806 pami-2024.5.1.2/PAMI/extras/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.220106 pami-2024.5.1.2/PAMI/extras/DF2DB/
--rw-r--r--   0 vanithak   (502) staff       (20)     4360 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4287 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    10331 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/DF2DB/DenseFormatDF.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5413 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/DF2DB/SparseFormatDF.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3103 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6948 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    11940 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5336 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.225717 pami-2024.5.1.2/PAMI/extras/calculateMISValues/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6468 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6499 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/extras/calculateMISValues/usingSD.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7345 2024-04-17 06:00:20.000000 pami-2024.5.1.2/PAMI/extras/convertMultiTSIntoFuzzy.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.238175 pami-2024.5.1.2/PAMI/extras/dbStats/
--rw-r--r--   0 vanithak   (502) staff       (20)    14951 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/extras/dbStats/FuzzyDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13796 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16034 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/dbStats/SequentialDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16883 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/extras/dbStats/TemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12839 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/extras/dbStats/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15120 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/extras/dbStats/UncertainTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    11953 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/extras/dbStats/UncertainTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12679 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/dbStats/UtilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/dbStats/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.247624 pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5238 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8594 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8792 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8313 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.252563 pami-2024.5.1.2/PAMI/extras/generateDatabase/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5685 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     9558 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5971 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5157 2024-04-10 08:52:08.000000 pami-2024.5.1.2/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.264406 pami-2024.5.1.2/PAMI/extras/graph/
--rw-r--r--   0 vanithak   (502) staff       (20)     3223 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/graph/DF2Fig.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3577 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/graph/DF2Tex.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/graph/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2750 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3599 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4465 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/graph/visualizeFuzzyPatterns.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4240 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.265608 pami-2024.5.1.2/PAMI/extras/image2Database/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.267496 pami-2024.5.1.2/PAMI/extras/imageProcessing/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6488 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.270827 pami-2024.5.1.2/PAMI/extras/messaging/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/messaging/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)      533 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/messaging/discord.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1575 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/messaging/gmail.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.276646 pami-2024.5.1.2/PAMI/extras/neighbours/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4784 2024-04-17 06:00:20.000000 pami-2024.5.1.2/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4410 2024-04-17 06:00:20.000000 pami-2024.5.1.2/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4305 2024-04-17 06:00:20.000000 pami-2024.5.1.2/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5013 2024-04-10 08:52:08.000000 pami-2024.5.1.2/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5183 2024-04-10 08:52:08.000000 pami-2024.5.1.2/PAMI/extras/plotPointOnMap_dump.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.279569 pami-2024.5.1.2/PAMI/extras/sampleDatasets/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/sampleDatasets/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4024 2024-04-10 08:52:08.000000 pami-2024.5.1.2/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.295929 pami-2024.5.1.2/PAMI/extras/stats/
--rw-r--r--   0 vanithak   (502) staff       (20)    12724 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/stats/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/stats/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4144 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/stats/graphDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15998 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/stats/sequentialDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16926 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/stats/temporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12692 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/extras/stats/utilityDatabase.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.328729 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/
--rw-r--r--   0 vanithak   (502) staff       (20)     7276 2024-05-01 06:38:00.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7096 2024-05-13 08:32:49.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2325 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2254 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2539 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1880 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1843 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2117 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2066 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2262 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/fuzzyDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1121 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1111 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1625 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1610 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3613 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3603 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/georeferencedTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/georeferencedTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4324 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3283 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4842 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/utilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3240 2024-04-10 08:52:08.000000 pami-2024.5.1.2/PAMI/extras/topKPatterns.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2322 2024-04-10 08:52:08.000000 pami-2024.5.1.2/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.330840 pami-2024.5.1.2/PAMI/extras/visualize/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/extras/visualize/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1897 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/extras/visualize/graphs.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.332585 pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.338383 pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    14510 2024-05-01 06:38:00.000000 pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23166 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6856 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.339587 pami-2024.5.1.2/PAMI/frequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.402457 pami-2024.5.1.2/PAMI/frequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    13838 2024-05-13 08:32:49.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13542 2024-05-13 08:32:49.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/Aprioribitset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13631 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14033 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13440 2024-05-03 04:25:04.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19496 2024-05-13 08:32:49.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15219 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/_Apriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22703 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/_FPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6818 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.411188 pami-2024.5.1.2/PAMI/frequentPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    20178 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6580 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.453645 pami-2024.5.1.2/PAMI/frequentPattern/cuda/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5980 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13664 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14418 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13015 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14583 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14499 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17118 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14178 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.464611 pami-2024.5.1.2/PAMI/frequentPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    26092 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6561 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.473774 pami-2024.5.1.2/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5573 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15452 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12947 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17438 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.481828 pami-2024.5.1.2/PAMI/frequentPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)    15426 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4575 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.484125 pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.489400 pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28229 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6652 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.491708 pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.503037 pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    22973 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28621 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6442 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.505374 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.515518 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    26162 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28607 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6730 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.516960 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.528306 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28521 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    33585 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6623 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.530060 pami-2024.5.1.2/PAMI/fuzzyPartialPeriodicPatterns/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.535423 pami-2024.5.1.2/PAMI/fuzzyPartialPeriodicPatterns/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    22562 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyPartialPeriodicPatterns/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6469 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.537403 pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.548982 pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25786 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    27472 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6683 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.550420 pami-2024.5.1.2/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.556056 pami-2024.5.1.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    22107 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6791 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.557118 pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.568342 pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    22965 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21152 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6697 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.570656 pami-2024.5.1.2/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6696 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.572247 pami-2024.5.1.2/PAMI/georeferencedPartialPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/georeferencedPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.579015 pami-2024.5.1.2/PAMI/georeferencedPartialPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    21718 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6178 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.580853 pami-2024.5.1.2/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.585885 pami-2024.5.1.2/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    38524 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6179 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.588093 pami-2024.5.1.2/PAMI/highUtilityGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.596053 pami-2024.5.1.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    42772 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6307 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.597543 pami-2024.5.1.2/PAMI/highUtilityPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.613417 pami-2024.5.1.2/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35224 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26511 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28921 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19909 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.620344 pami-2024.5.1.2/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17831 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.629427 pami-2024.5.1.2/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 vanithak   (502) staff       (20)    30022 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32848 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5193 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.632995 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6716 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.639505 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29850 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)    37379 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5934 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.646571 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)    37519 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.649959 pami-2024.5.1.2/PAMI/localPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.662303 pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35370 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24681 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23709 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8385 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.663626 pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.670009 pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    24308 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22008 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5921 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.671055 pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.679846 pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28270 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21954 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5398 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.681307 pami-2024.5.1.2/PAMI/partialPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.692240 pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    26420 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4329 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    25525 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19577 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5520 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.697599 pami-2024.5.1.2/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    22070 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5605 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.702364 pami-2024.5.1.2/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    29144 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4278 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.706401 pami-2024.5.1.2/PAMI/partialPeriodicPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5765 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28554 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.712636 pami-2024.5.1.2/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6441 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19588 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.720085 pami-2024.5.1.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/
--rw-r--r--   0 vanithak   (502) staff       (20)    28160 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6350 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.724662 pami-2024.5.1.2/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.734893 pami-2024.5.1.2/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    27559 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6691 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.737782 pami-2024.5.1.2/PAMI/periodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.784036 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    17272 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21302 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26383 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18106 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 vanithak   (502) staff       (20)    36300 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17904 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/_PFECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28583 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/_PFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      726 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6549 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26643 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.791629 pami-2024.5.1.2/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    24417 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6539 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.801367 pami-2024.5.1.2/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6568 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23867 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18982 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.806491 pami-2024.5.1.2/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    31832 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7869 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.812849 pami-2024.5.1.2/PAMI/periodicFrequentPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5219 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26749 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.815259 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.820449 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 vanithak   (502) staff       (20)    19951 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6862 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.828245 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4589 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17514 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.830190 pami-2024.5.1.2/PAMI/recurringPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.834774 pami-2024.5.1.2/PAMI/recurringPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29135 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6637 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.837910 pami-2024.5.1.2/PAMI/relativeFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.855369 pami-2024.5.1.2/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30349 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4261 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.861003 pami-2024.5.1.2/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.869517 pami-2024.5.1.2/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35406 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6052 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.872792 pami-2024.5.1.2/PAMI/sequence/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/sequence/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.879321 pami-2024.5.1.2/PAMI/sequentialPatternMining/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.896187 pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    42265 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19986 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/SPAM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6569 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24786 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.905430 pami-2024.5.1.2/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6285 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.906045 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.942594 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    18431 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26770 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19807 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7271 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.952608 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 vanithak   (502) staff       (20)    27859 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7173 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.953639 pami-2024.5.1.2/PAMI/subgraphMining/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.971696 pami-2024.5.1.2/PAMI/subgraphMining/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1241 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2396 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/dfsCode.py
--rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/edge.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2616 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/extendedEdge.py
--rw-r--r--   0 vanithak   (502) staff       (20)      670 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/frequentSubgraph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4943 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/graph.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28244 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/gspan.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1748 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/sparseTriangularMatrix.py
--rw-r--r--   0 vanithak   (502) staff       (20)      826 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/basic/vertex.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:11.995738 pami-2024.5.1.2/PAMI/subgraphMining/topK/
--rw-r--r--   0 vanithak   (502) staff       (20)     1949 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/DFSCode.py
--rw-r--r--   0 vanithak   (502) staff       (20)      593 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/DFSThread.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1316 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/edge.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2613 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/extendedEdge.py
--rw-r--r--   0 vanithak   (502) staff       (20)      674 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/frequentSubgraph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4295 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/graph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1486 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/sparseTriangularMatrix.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20979 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/tkg.py
--rw-r--r--   0 vanithak   (502) staff       (20)      818 2024-03-29 21:11:29.000000 pami-2024.5.1.2/PAMI/subgraphMining/topK/vertex.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.005603 pami-2024.5.1.2/PAMI/uncertainFaultTolerantFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)    17694 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6756 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.006785 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.034437 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28251 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 vanithak   (502) staff       (20)    27430 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20311 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20112 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28047 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 vanithak   (502) staff       (20)    25675 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19871 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4945 2024-04-09 02:02:26.000000 pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.036009 pami-2024.5.1.2/PAMI/uncertainGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.045823 pami-2024.5.1.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30577 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4986 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.047242 pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.053665 pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    33173 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    33178 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6536 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.054732 pami-2024.5.1.2/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.061411 pami-2024.5.1.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29414 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6603 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.062723 pami-2024.5.1.2/PAMI/weightedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.067723 pami-2024.5.1.2/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25844 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6659 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.069568 pami-2024.5.1.2/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.077964 pami-2024.5.1.2/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29035 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7495 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.079226 pami-2024.5.1.2/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.083578 pami-2024.5.1.2/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    31245 2024-05-01 06:38:01.000000 pami-2024.5.1.2/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4771 2024-03-12 04:33:29.000000 pami-2024.5.1.2/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    72970 2024-05-13 08:33:12.097916 pami-2024.5.1.2/PKG-INFO
--rw-r--r--   0 vanithak   (502) staff       (20)    71479 2024-05-13 08:32:49.000000 pami-2024.5.1.2/README.md
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-05-13 08:33:12.088010 pami-2024.5.1.2/pami.egg-info/
--rw-r--r--   0 vanithak   (502) staff       (20)    72970 2024-05-13 08:33:10.000000 pami-2024.5.1.2/pami.egg-info/PKG-INFO
--rw-r--r--   0 vanithak   (502) staff       (20)    18350 2024-05-13 08:33:10.000000 pami-2024.5.1.2/pami.egg-info/SOURCES.txt
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-05-13 08:33:10.000000 pami-2024.5.1.2/pami.egg-info/dependency_links.txt
--rw-r--r--   0 vanithak   (502) staff       (20)      255 2024-05-13 08:33:10.000000 pami-2024.5.1.2/pami.egg-info/requires.txt
--rw-r--r--   0 vanithak   (502) staff       (20)        5 2024-05-13 08:33:10.000000 pami-2024.5.1.2/pami.egg-info/top_level.txt
--rw-r--r--   0 vanithak   (502) staff       (20)       38 2024-05-13 08:33:12.101307 pami-2024.5.1.2/setup.cfg
--rw-r--r--   0 vanithak   (502) staff       (20)     1535 2024-05-13 08:32:59.000000 pami-2024.5.1.2/setup.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:15.934216 pami-2024.5.7.1/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2024-02-19 12:10:44.000000 pami-2024.5.7.1/LICENSE
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:04.077991 pami-2024.5.7.1/PAMI/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:06.209582 pami-2024.5.7.1/PAMI/AssociationRules/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:06.217030 pami-2024.5.7.1/PAMI/AssociationRules/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14350 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/AssociationRules/basic/_ARWithLeverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14263 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/AssociationRules/basic/_ARWithLift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19416 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/AssociationRules/basic/_RuleMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6613 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12724 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/AssociationRules/basic/confidence.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12638 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/AssociationRules/basic/leverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12430 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/AssociationRules/basic/lift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:06.217762 pami-2024.5.7.1/PAMI/correlatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:07.302034 pami-2024.5.7.1/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26443 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/correlatedPattern/basic/CoMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27988 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/correlatedPattern/basic/CoMinePlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6208 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:07.761518 pami-2024.5.7.1/PAMI/coveragePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/coveragePattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:09.787669 pami-2024.5.7.1/PAMI/coveragePattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14643 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/coveragePattern/basic/CMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17200 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/coveragePattern/basic/CPPG.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/coveragePattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7155 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/coveragePattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:14.515242 pami-2024.5.7.1/PAMI/extras/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:19.571452 pami-2024.5.7.1/PAMI/extras/DF2DB/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4360 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4287 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10331 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/DF2DB/DenseFormatDF.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5413 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/DF2DB/SparseFormatDF.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3103 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6948 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11940 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5336 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:20.571618 pami-2024.5.7.1/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6468 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6499 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/calculateMISValues/usingSD.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7345 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/convertMultiTSIntoFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:25.517301 pami-2024.5.7.1/PAMI/extras/dbStats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14951 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/dbStats/FuzzyDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13796 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16034 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/dbStats/SequentialDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16883 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/dbStats/TemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12839 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/dbStats/TransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15120 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11953 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12679 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/dbStats/UtilityDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/dbStats/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:26.881603 pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5238 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8594 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8792 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8313 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:28.353069 pami-2024.5.7.1/PAMI/extras/generateDatabase/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5685 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9558 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5971 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5157 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:31.609764 pami-2024.5.7.1/PAMI/extras/graph/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3223 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/graph/DF2Fig.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3577 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/graph/DF2Tex.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2750 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3599 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4465 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/graph/visualizeFuzzyPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4240 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:32.114052 pami-2024.5.7.1/PAMI/extras/image2Database/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:32.512117 pami-2024.5.7.1/PAMI/extras/imageProcessing/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6488 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:33.664654 pami-2024.5.7.1/PAMI/extras/messaging/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/messaging/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      533 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/messaging/discord.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1575 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/messaging/gmail.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:35.152172 pami-2024.5.7.1/PAMI/extras/neighbours/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4784 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4410 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4305 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5013 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5183 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/plotPointOnMap_dump.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:35.733803 pami-2024.5.7.1/PAMI/extras/sampleDatasets/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/sampleDatasets/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4024 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:38.888297 pami-2024.5.7.1/PAMI/extras/stats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12724 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/stats/TransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/stats/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4144 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/stats/graphDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15998 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/stats/sequentialDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16926 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/stats/temporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12692 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/stats/utilityDatabase.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:47.358784 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7276 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6930 2024-05-07 07:49:33.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2325 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2254 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2539 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1880 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1843 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2117 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2066 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2262 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/fuzzyDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1121 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1111 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1625 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1610 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3613 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3603 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/georeferencedTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/georeferencedTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4324 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3283 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4842 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3240 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2322 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:47.809100 pami-2024.5.7.1/PAMI/extras/visualize/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/visualize/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1897 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/extras/visualize/graphs.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:48.251818 pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:50.689479 pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14510 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23166 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6856 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:51.036520 pami-2024.5.7.1/PAMI/frequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:52.796321 pami-2024.5.7.1/PAMI/frequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13840 2024-05-01 07:34:25.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13544 2024-04-30 09:23:37.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/Aprioribitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13631 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14033 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13440 2024-05-05 10:33:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19498 2024-05-01 07:34:25.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15219 2024-04-18 05:41:27.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/_Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22703 2024-04-18 05:41:27.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/_FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6818 2024-04-30 08:51:40.000000 pami-2024.5.7.1/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:52.798085 pami-2024.5.7.1/PAMI/frequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20178 2024-05-01 07:34:25.000000 pami-2024.5.7.1/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:56.613931 pami-2024.5.7.1/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5980 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13664 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14418 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13015 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14583 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14499 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17118 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14178 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:51:58.077779 pami-2024.5.7.1/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26092 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6561 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:00.749285 pami-2024.5.7.1/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5573 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15452 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12947 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17438 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:02.338817 pami-2024.5.7.1/PAMI/frequentPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15426 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:02.878077 pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:03.813240 pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28229 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:03.813617 pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:04.752458 pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22973 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28621 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6442 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:04.753915 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:05.144229 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26162 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28607 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6730 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:05.145081 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:05.541550 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28521 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33585 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6623 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:05.542454 pami-2024.5.7.1/PAMI/fuzzyPartialPeriodicPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:06.954523 pami-2024.5.7.1/PAMI/fuzzyPartialPeriodicPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22562 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyPartialPeriodicPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6469 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:06.956333 pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:08.240652 pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25786 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27472 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6683 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:08.242241 pami-2024.5.7.1/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:08.699162 pami-2024.5.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22107 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6791 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:08.700057 pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:10.108287 pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22965 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21152 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6697 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:10.109569 pami-2024.5.7.1/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6696 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:10.110437 pami-2024.5.7.1/PAMI/georeferencedPartialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:10.547357 pami-2024.5.7.1/PAMI/georeferencedPartialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21718 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6178 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:10.948842 pami-2024.5.7.1/PAMI/highUtilityFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:10.951914 pami-2024.5.7.1/PAMI/highUtilityFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    38524 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6179 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:11.451342 pami-2024.5.7.1/PAMI/highUtilityGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:12.341965 pami-2024.5.7.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    42772 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6307 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:12.762762 pami-2024.5.7.1/PAMI/highUtilityPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:14.583966 pami-2024.5.7.1/PAMI/highUtilityPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35224 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/basic/EFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26511 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/basic/HMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28921 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/basic/UPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5166 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19909 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/basic/efimParallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:16.199955 pami-2024.5.7.1/PAMI/highUtilityPattern/parallel/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/parallel/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5166 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/parallel/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17831 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilityPattern/parallel/efimparallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:17.924365 pami-2024.5.7.1/PAMI/highUtilityPatternsInStreams/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    30022 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32848 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityPatternsInStreams/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5193 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilityPatternsInStreams/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:18.778353 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6716 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:20.160402 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29850 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    37379 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5934 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:21.405131 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    37519 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:21.911432 pami-2024.5.7.1/PAMI/localPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:23.124520 pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35370 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24681 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23709 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8385 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:23.527273 pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:24.843594 pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24308 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22008 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5921 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:25.299834 pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:25.303207 pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28270 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21954 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5398 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:25.752184 pami-2024.5.7.1/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:27.923986 pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26420 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4329 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25525 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19577 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5520 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:29.234435 pami-2024.5.7.1/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22070 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5605 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:30.449126 pami-2024.5.7.1/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29144 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4278 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:31.916874 pami-2024.5.7.1/PAMI/partialPeriodicPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5765 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28554 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:33.441602 pami-2024.5.7.1/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6441 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19588 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:34.222296 pami-2024.5.7.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28160 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6350 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:34.223413 pami-2024.5.7.1/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:34.656140 pami-2024.5.7.1/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27559 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6691 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:34.657070 pami-2024.5.7.1/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:39.231540 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17272 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21302 2024-04-19 05:15:04.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26383 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18106 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    36300 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17904 2024-04-18 05:41:27.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/_PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28583 2024-04-18 05:41:27.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/_PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6549 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26643 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:40.438175 pami-2024.5.7.1/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24417 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6539 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:41.859397 pami-2024.5.7.1/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6568 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23867 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18982 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:43.027722 pami-2024.5.7.1/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31832 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7869 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:43.925963 pami-2024.5.7.1/PAMI/periodicFrequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5219 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26749 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:44.612639 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:45.939605 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19951 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6862 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:47.404188 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4589 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17514 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:48.051389 pami-2024.5.7.1/PAMI/recurringPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:48.930217 pami-2024.5.7.1/PAMI/recurringPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29135 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6637 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:49.717874 pami-2024.5.7.1/PAMI/relativeFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/relativeFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:51.079349 pami-2024.5.7.1/PAMI/relativeFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    30349 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/relativeFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/relativeFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:51.573335 pami-2024.5.7.1/PAMI/relativeHighUtilityPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/relativeHighUtilityPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:52.003649 pami-2024.5.7.1/PAMI/relativeHighUtilityPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35406 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6052 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:52.451514 pami-2024.5.7.1/PAMI/sequence/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/sequence/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:52.452042 pami-2024.5.7.1/PAMI/sequentialPatternMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:54.437135 pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    42265 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19986 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/SPAM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6569 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24786 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:55.397868 pami-2024.5.7.1/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6285 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:55.398301 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:57.271849 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18431 2024-04-19 08:53:38.000000 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26770 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19807 2024-04-19 08:53:38.000000 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7271 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:58.473503 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27859 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7173 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:52:58.970602 pami-2024.5.7.1/PAMI/subgraphMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:03.198155 pami-2024.5.7.1/PAMI/subgraphMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1241 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2396 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/dfsCode.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      772 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/edge.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2616 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/extendedEdge.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      670 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/frequentSubgraph.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4943 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/graph.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28244 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/gspan.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1748 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      826 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/basic/vertex.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:08.142214 pami-2024.5.7.1/PAMI/subgraphMining/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1949 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/DFSCode.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      593 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/DFSThread.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1316 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      772 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/edge.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2613 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/extendedEdge.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      674 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/frequentSubgraph.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4295 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/graph.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1486 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20979 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/tkg.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      818 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/subgraphMining/topK/vertex.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:08.561951 pami-2024.5.7.1/PAMI/uncertainFaultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17694 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6756 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:08.936691 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:09.885566 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28251 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27430 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20311 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20112 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28047 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25675 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19871 2024-04-25 00:26:02.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4945 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:10.430157 pami-2024.5.7.1/PAMI/uncertainGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:11.213712 pami-2024.5.7.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    30577 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4986 2024-04-17 07:22:09.000000 pami-2024.5.7.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:11.600435 pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:12.049758 pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33173 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33178 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6536 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:12.550226 pami-2024.5.7.1/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:12.996215 pami-2024.5.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29414 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6603 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:13.469807 pami-2024.5.7.1/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:14.009251 pami-2024.5.7.1/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25844 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6659 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:14.479639 pami-2024.5.7.1/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:14.481543 pami-2024.5.7.1/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29035 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7495 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:14.912905 pami-2024.5.7.1/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:15.367209 pami-2024.5.7.1/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31245 2024-04-24 02:44:32.000000 pami-2024.5.7.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4771 2024-02-19 12:10:44.000000 pami-2024.5.7.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    72970 2024-05-07 07:53:15.932895 pami-2024.5.7.1/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    71479 2024-05-05 10:56:29.000000 pami-2024.5.7.1/README.md
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2024-05-07 07:53:15.916416 pami-2024.5.7.1/pami.egg-info/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    72970 2024-05-07 07:51:02.000000 pami-2024.5.7.1/pami.egg-info/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18350 2024-05-07 07:51:02.000000 pami-2024.5.7.1/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2024-05-07 07:51:02.000000 pami-2024.5.7.1/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      255 2024-05-07 07:51:02.000000 pami-2024.5.7.1/pami.egg-info/requires.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2024-05-07 07:51:02.000000 pami-2024.5.7.1/pami.egg-info/top_level.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2024-05-07 07:53:15.934379 pami-2024.5.7.1/setup.cfg
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1535 2024-05-07 07:50:57.000000 pami-2024.5.7.1/setup.py
```

### Comparing `pami-2024.5.1.2/LICENSE` & `pami-2024.5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/AssociationRules/basic/_ARWithLeverage.py` & `pami-2024.5.7.1/PAMI/AssociationRules/basic/_ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/AssociationRules/basic/_ARWithLift.py` & `pami-2024.5.7.1/PAMI/AssociationRules/basic/_ARWithLift.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/AssociationRules/basic/_RuleMiner.py` & `pami-2024.5.7.1/PAMI/AssociationRules/basic/_RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/AssociationRules/basic/abstract.py` & `pami-2024.5.7.1/PAMI/AssociationRules/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/AssociationRules/basic/confidence.py` & `pami-2024.5.7.1/PAMI/AssociationRules/basic/confidence.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/AssociationRules/basic/leverage.py` & `pami-2024.5.7.1/PAMI/AssociationRules/basic/leverage.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/AssociationRules/basic/lift.py` & `pami-2024.5.7.1/PAMI/AssociationRules/basic/lift.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/correlatedPattern/__init__.py` & `pami-2024.5.7.1/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/correlatedPattern/basic/CoMine.py` & `pami-2024.5.7.1/PAMI/correlatedPattern/basic/CoMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/correlatedPattern/basic/CoMinePlus.py` & `pami-2024.5.7.1/PAMI/correlatedPattern/basic/CoMinePlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/correlatedPattern/basic/__init__.py` & `pami-2024.5.7.1/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/correlatedPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/coveragePattern/basic/CMine.py` & `pami-2024.5.7.1/PAMI/coveragePattern/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/coveragePattern/basic/CPPG.py` & `pami-2024.5.7.1/PAMI/coveragePattern/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/coveragePattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/coveragePattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/DF2DB/DF2DB.py` & `pami-2024.5.7.1/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2024.5.7.1/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/DF2DB/DenseFormatDF.py` & `pami-2024.5.7.1/PAMI/extras/DF2DB/DenseFormatDF.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/DF2DB/SparseFormatDF.py` & `pami-2024.5.7.1/PAMI/extras/DF2DB/SparseFormatDF.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/DF2DB/createTDB.py` & `pami-2024.5.7.1/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2024.5.7.1/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2024.5.7.1/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2024.5.7.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2024.5.7.1/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2024.5.7.1/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/convertMultiTSIntoFuzzy.py` & `pami-2024.5.7.1/PAMI/extras/convertMultiTSIntoFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/dbStats/FuzzyDatabase.py` & `pami-2024.5.7.1/PAMI/extras/dbStats/FuzzyDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py` & `pami-2024.5.7.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/dbStats/SequentialDatabase.py` & `pami-2024.5.7.1/PAMI/extras/dbStats/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/dbStats/TemporalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/dbStats/TemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/dbStats/TransactionalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/dbStats/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/dbStats/UncertainTemporalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/dbStats/UncertainTransactionalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/dbStats/UtilityDatabase.py` & `pami-2024.5.7.1/PAMI/extras/dbStats/UtilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py` & `pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2024.5.7.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/generateLatexGraphFile.py` & `pami-2024.5.7.1/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/graph/DF2Fig.py` & `pami-2024.5.7.1/PAMI/extras/graph/DF2Fig.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/graph/DF2Tex.py` & `pami-2024.5.7.1/PAMI/extras/graph/DF2Tex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2024.5.7.1/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2024.5.7.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/graph/visualizeFuzzyPatterns.py` & `pami-2024.5.7.1/PAMI/extras/graph/visualizeFuzzyPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/graph/visualizePatterns.py` & `pami-2024.5.7.1/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2024.5.7.1/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/messaging/discord.py` & `pami-2024.5.7.1/PAMI/extras/messaging/discord.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/messaging/gmail.py` & `pami-2024.5.7.1/PAMI/extras/messaging/gmail.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py` & `pami-2024.5.7.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2024.5.7.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py` & `pami-2024.5.7.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/plotPointOnMap.py` & `pami-2024.5.7.1/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/plotPointOnMap_dump.py` & `pami-2024.5.7.1/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2024.5.7.1/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/stats/TransactionalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/stats/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/stats/graphDatabase.py` & `pami-2024.5.7.1/PAMI/extras/stats/graphDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/stats/sequentialDatabase.py` & `pami-2024.5.7.1/PAMI/extras/stats/sequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/stats/temporalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/stats/temporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/stats/utilityDatabase.py` & `pami-2024.5.7.1/PAMI/extras/stats/utilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,20 +204,16 @@
     def getTransactions(self) -> pd.DataFrame:
         """
         Get the transactional database in dataFrame format
 
         Returns:
         db: pd.dataFrame - transactional database
         """
-        column = "Transactions"
-        db = pd.DataFrame(columns=[column])
-        self.db = [tuple(x) for x in self.db]
-        for i in range(len(self.db)):
-            db.at[i,column] = self.db[i]
-        return db
+        df = pd.DataFrame(self.db)
+        return df
         
 
 if __name__ == "__main__":
     if len(sys.argv) == 5:
         obj = TransactionalDatabase(int(sys.argv[1]), int(sys.argv[2]), int(sys.argv[3]))
         obj.create()
         obj.save(sys.argv[4])
```

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateTemporal.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateTransactional.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/syntheticDataGenerator/utilityDatabase.py` & `pami-2024.5.7.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/topKPatterns.py` & `pami-2024.5.7.1/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/uncertaindb_convert.py` & `pami-2024.5.7.1/PAMI/extras/uncertaindb_convert.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/extras/visualize/graphs.py` & `pami-2024.5.7.1/PAMI/extras/visualize/graphs.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/__init__.py` & `pami-2024.5.7.1/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/basic/Apriori.py` & `pami-2024.5.7.1/PAMI/frequentPattern/basic/Apriori.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 
         :return: None
 
         """
         with open(outFile, 'w') as f:
             for x, y in self._finalPatterns.items():
                 x = self._sep.join(x)
-                f.write(f"{x}:{y}\n")
+                f.write(f"{x} : {y}\n")
 
     def getPatterns(self) -> Dict[str, int]:
         """
 
         Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
```

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/basic/Aprioribitset.py` & `pami-2024.5.7.1/PAMI/frequentPattern/basic/Aprioribitset.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 from PAMI.frequentPattern.basic import abstract as _ab
 from deprecated import deprecated
 
 
-class Aprioribitset(_ab._frequentPatterns):
+class AprioriBitset(_ab._frequentPatterns):
     """
     :Description:  AprioriBitset is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 
     :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
             372-390 (2000), https://ieeexplore.ieee.org/document/846291
 
     :param  iFile: str :
@@ -364,15 +364,15 @@
 
         :return: None
 
         """
         with open(outFile, 'w') as f:
             for x, y in self._finalPatterns.items():
                 x = self._sep.join(x)
-                f.write(f"{x}:{y}\n")
+                f.write(f"{x} : {y}\n")
 
     def getPatterns(self):
         """
         Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
@@ -388,17 +388,17 @@
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = Aprioribitset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = AprioriBitset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = Aprioribitset(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = AprioriBitset(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
```

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2024.5.7.1/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2024.5.7.1/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2024.5.7.1/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2024.5.7.1/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
         :param outFile: name of the output file
         :type outFile: csvfile
         :return: None
         """
         with open(outFile, 'w') as f:
             for x, y in self._finalPatterns.items():
                 x = self._sep.join(x)
-                f.write(f"{x}:{y}\n")
+                f.write(f"{x} : {y}\n")
 
     def getPatterns(self) -> Dict[str, int]:
         """
 
         Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
```

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/basic/_Apriori.py` & `pami-2024.5.7.1/PAMI/frequentPattern/basic/_Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/basic/_FPGrowth.py` & `pami-2024.5.7.1/PAMI/frequentPattern/basic/_FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/closed/CHARM.py` & `pami-2024.5.7.1/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/closed/abstract.py` & `pami-2024.5.7.1/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/cuda/abstract.py` & `pami-2024.5.7.1/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2024.5.7.1/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2024.5.7.1/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2024.5.7.1/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2024.5.7.1/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2024.5.7.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2024.5.7.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2024.5.7.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2024.5.7.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/maximal/__init__.py` & `pami-2024.5.7.1/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/maximal/abstract.py` & `pami-2024.5.7.1/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2024.5.7.1/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2024.5.7.1/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2024.5.7.1/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2024.5.7.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/topk/FAE.py` & `pami-2024.5.7.1/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/frequentPattern/topk/abstract.py` & `pami-2024.5.7.1/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/fuzzyFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py` & `pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py` & `pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py` & `pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py` & `pami-2024.5.7.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py` & `pami-2024.5.7.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2024.5.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/__init__.py` & `pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py` & `pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py` & `pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/georeferencedFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/georeferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2024.5.7.1/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py` & `pami-2024.5.7.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2024.5.7.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/highUtilityFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py` & `pami-2024.5.7.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py` & `pami-2024.5.7.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2024.5.7.1/PAMI/highUtilityPattern/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2024.5.7.1/PAMI/highUtilityPattern/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2024.5.7.1/PAMI/highUtilityPattern/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/highUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2024.5.7.1/PAMI/highUtilityPattern/basic/efimParallel.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2024.5.7.1/PAMI/highUtilityPattern/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2024.5.7.1/PAMI/highUtilityPattern/parallel/efimparallel.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2024.5.7.1/PAMI/highUtilityPatternsInStreams/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2024.5.7.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2024.5.7.1/PAMI/highUtilityPatternsInStreams/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2024.5.7.1/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/__init__.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/pyspark/__init__.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/pyspark/abstract.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py` & `pami-2024.5.7.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2024.5.7.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/__init__.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/_PFECLAT.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/_PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/_PFPGrowth.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/_PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/pyspark/abstract.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2024.5.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2024.5.7.1/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/recurringPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2024.5.7.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/relativeFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2024.5.7.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/relativeHighUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/SPAM.py` & `pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/SPAM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2024.5.7.1/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2024.5.7.1/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2024.5.7.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/basic/abstract.py` & `pami-2024.5.7.1/PAMI/subgraphMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/basic/dfsCode.py` & `pami-2024.5.7.1/PAMI/subgraphMining/basic/dfsCode.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/basic/edge.py` & `pami-2024.5.7.1/PAMI/subgraphMining/basic/edge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/basic/extendedEdge.py` & `pami-2024.5.7.1/PAMI/subgraphMining/basic/extendedEdge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/basic/frequentSubgraph.py` & `pami-2024.5.7.1/PAMI/subgraphMining/basic/frequentSubgraph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/basic/graph.py` & `pami-2024.5.7.1/PAMI/subgraphMining/basic/graph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/basic/gspan.py` & `pami-2024.5.7.1/PAMI/subgraphMining/basic/gspan.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/basic/sparseTriangularMatrix.py` & `pami-2024.5.7.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/basic/vertex.py` & `pami-2024.5.7.1/PAMI/subgraphMining/basic/vertex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/DFSCode.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/DFSCode.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/DFSThread.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/DFSThread.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/abstract.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/edge.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/edge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/extendedEdge.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/extendedEdge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/frequentSubgraph.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/frequentSubgraph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/graph.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/graph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/sparseTriangularMatrix.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/tkg.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/tkg.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/subgraphMining/topK/vertex.py` & `pami-2024.5.7.1/PAMI/subgraphMining/topK/vertex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py` & `pami-2024.5.7.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py` & `pami-2024.5.7.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2024.5.7.1/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py` & `pami-2024.5.7.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2024.5.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2024.5.7.1/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2024.5.7.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2024.5.7.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2024.5.7.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/PKG-INFO` & `pami-2024.5.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2024.5.1.2
+Version: 2024.5.7.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pami-2024.5.1.2/README.md` & `pami-2024.5.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/pami.egg-info/PKG-INFO` & `pami-2024.5.7.1/pami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2024.5.1.2
+Version: 2024.5.7.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pami-2024.5.1.2/pami.egg-info/SOURCES.txt` & `pami-2024.5.7.1/pami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pami-2024.5.1.2/setup.py` & `pami-2024.5.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pami',
-    version='2024.5.1.2',
+    version='2024.5.7.1',
     author='Rage Uday Kiran',
     author_email='uday.rage@gmail.com',
     description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     url='https://github.com/udayLab/PAMI',
```

