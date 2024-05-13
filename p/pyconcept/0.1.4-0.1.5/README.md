# Comparing `tmp/pyconcept-0.1.4.tar.gz` & `tmp/pyconcept-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconcept-0.1.4.tar", last modified: Thu May  9 23:28:41 2024, max compression
+gzip compressed data, was "pyconcept-0.1.5.tar", last modified: Mon May 13 09:03:59 2024, max compression
```

## Comparing `pyconcept-0.1.4.tar` & `pyconcept-0.1.5.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.555448 pyconcept-0.1.4/
--rw-rw-rw-   0        0        0      944 2024-05-09 22:41:52.000000 pyconcept-0.1.4/CHANGELOG.md
--rw-rw-rw-   0        0        0      955 2024-04-19 23:54:16.000000 pyconcept-0.1.4/CMakeLists.txt
--rw-rw-rw-   0        0        0     1101 2024-04-15 19:05:00.000000 pyconcept-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      162 2024-04-18 08:33:28.000000 pyconcept-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      953 2024-05-09 23:28:41.554449 pyconcept-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      115 2024-04-17 11:33:45.000000 pyconcept-0.1.4/README.md
--rw-rw-rw-   0        0        0        5 2024-05-09 22:40:47.000000 pyconcept-0.1.4/VERSION
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.433610 pyconcept-0.1.4/ccl/
--rw-rw-rw-   0        0        0     2133 2024-04-17 08:48:56.000000 pyconcept-0.1.4/ccl/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.274368 pyconcept-0.1.4/ccl/cclCommons/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.274368 pyconcept-0.1.4/ccl/cclCommons/include/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.460652 pyconcept-0.1.4/ccl/cclCommons/include/ccl/
--rw-rw-rw-   0        0        0    10473 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/Strings.hpp
--rw-rw-rw-   0        0        0      895 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/Substitutes.hpp
--rw-rw-rw-   0        0        0     1506 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclChange.hpp
--rw-rw-rw-   0        0        0    11710 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclMeta.hpp
--rw-rw-rw-   0        0        0     6078 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclTypes.hpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.275366 pyconcept-0.1.4/ccl/cclGraph/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.275366 pyconcept-0.1.4/ccl/cclGraph/include/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.461652 pyconcept-0.1.4/ccl/cclGraph/include/ccl/
--rw-rw-rw-   0        0        0     2749 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclGraph/include/ccl/Entity.hpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.462654 pyconcept-0.1.4/ccl/cclGraph/include/ccl/graph/
--rw-rw-rw-   0        0        0     2907 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclGraph/include/ccl/graph/CGraph.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.464653 pyconcept-0.1.4/ccl/cclGraph/src/
--rw-rw-rw-   0        0        0     9187 2024-05-06 12:39:34.000000 pyconcept-0.1.4/ccl/cclGraph/src/CGraph.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.277368 pyconcept-0.1.4/ccl/cclLang/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.276365 pyconcept-0.1.4/ccl/cclLang/include/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.276365 pyconcept-0.1.4/ccl/cclLang/include/ccl/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.488349 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/
--rw-rw-rw-   0        0        0     1191 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp
--rw-rw-rw-   0        0        0     1941 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/LexicalTerm.h
--rw-rw-rw-   0        0        0      345 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Literals.h
--rw-rw-rw-   0        0        0     1327 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/ManagedText.h
--rw-rw-rw-   0        0        0     8108 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Morphology.h
--rw-rw-rw-   0        0        0     2748 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Reference.h
--rw-rw-rw-   0        0        0     2766 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/RefsManager.h
--rw-rw-rw-   0        0        0      514 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/TextEnvironment.h
--rw-rw-rw-   0        0        0     1278 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/TextProcessor.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.541760 pyconcept-0.1.4/ccl/cclLang/src/
--rw-rw-rw-   0        0        0     2111 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/LexicalTerm.cpp
--rw-rw-rw-   0        0        0      307 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/Literals.cpp
--rw-rw-rw-   0        0        0     2016 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/ManagedText.cpp
--rw-rw-rw-   0        0        0     2239 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/Morphology.cpp
--rw-rw-rw-   0        0        0     7475 2024-05-06 12:47:43.000000 pyconcept-0.1.4/ccl/cclLang/src/Reference.cpp
--rw-rw-rw-   0        0        0     6529 2024-05-06 12:48:14.000000 pyconcept-0.1.4/ccl/cclLang/src/RefsManager.cpp
--rw-rw-rw-   0        0        0      452 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/TextEnvironment.cpp
--rw-rw-rw-   0        0        0     1581 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/src/TextProcessor.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.542761 pyconcept-0.1.4/ccl/cclLang/unity/
--rw-rw-rw-   0        0        0      309 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/cclLang/unity/cclLang.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.613047 pyconcept-0.1.4/ccl/cmake/
--rw-rw-rw-   0        0        0     1541 2024-04-19 23:11:05.000000 pyconcept-0.1.4/ccl/cmake/CXXTargets.cmake
--rw-rw-rw-   0        0        0       93 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/conanfile.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.284581 pyconcept-0.1.4/ccl/core/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.280578 pyconcept-0.1.4/ccl/core/include/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.711263 pyconcept-0.1.4/ccl/core/include/ccl/
--rw-rw-rw-   0        0        0     2124 2024-05-06 15:23:11.000000 pyconcept-0.1.4/ccl/core/include/ccl/Operation.hpp
--rw-rw-rw-   0        0        0     5309 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/Source.hpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.719042 pyconcept-0.1.4/ccl/core/include/ccl/api/
--rw-rw-rw-   0        0        0      915 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/api/RSFormJA.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.748907 pyconcept-0.1.4/ccl/core/include/ccl/env/
--rw-rw-rw-   0        0        0     2904 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/env/SourceManager.hpp
--rw-rw-rw-   0        0        0      624 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/env/cclEnvironment.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.807402 pyconcept-0.1.4/ccl/core/include/ccl/ops/
--rw-rw-rw-   0        0        0     1998 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/ops/EquationOptions.h
--rw-rw-rw-   0        0        0      850 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/ops/RSAggregator.h
--rw-rw-rw-   0        0        0     1187 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/ops/RSEquationProcessor.h
--rw-rw-rw-   0        0        0     3525 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/ops/RSOperations.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.845495 pyconcept-0.1.4/ccl/core/include/ccl/oss/
--rw-rw-rw-   0        0        0     4161 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/OSSchema.h
--rw-rw-rw-   0        0        0     1658 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/OperationProcessor.hpp
--rw-rw-rw-   0        0        0      903 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/Pict.hpp
--rw-rw-rw-   0        0        0      934 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/RSSynthesProcessor.h
--rw-rw-rw-   0        0        0     1363 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/ossGraphFacet.h
--rw-rw-rw-   0        0        0     2334 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/ossGridFacet.h
--rw-rw-rw-   0        0        0     2979 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/ossOperationsFacet.h
--rw-rw-rw-   0        0        0     2469 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/oss/ossSourceFacet.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.897611 pyconcept-0.1.4/ccl/core/include/ccl/semantic/
--rw-rw-rw-   0        0        0      622 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/ConceptRecord.h
--rw-rw-rw-   0        0        0     1473 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstFilters.hpp
--rw-rw-rw-   0        0        0     2367 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstList.h
--rw-rw-rw-   0        0        0     2523 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstType.hpp
--rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/IdentityManager.h
--rw-rw-rw-   0        0        0      962 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/InterpretationStorage.h
--rw-rw-rw-   0        0        0     1095 2024-05-06 14:59:52.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSConcept.h
--rw-rw-rw-   0        0        0     3584 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSCore.h
--rw-rw-rw-   0        0        0     3430 2024-05-06 15:04:15.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSForm.h
--rw-rw-rw-   0        0        0     3012 2024-05-06 15:04:05.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSModel.h
--rw-rw-rw-   0        0        0     5074 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/Schema.h
--rw-rw-rw-   0        0        0     1122 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/TextConcept.h
--rw-rw-rw-   0        0        0     2603 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/TextData.hpp
--rw-rw-rw-   0        0        0     3988 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/Thesaurus.h
--rw-rw-rw-   0        0        0     1577 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsCalculationFacet.h
--rw-rw-rw-   0        0        0     1648 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsModificationFacet.h
--rw-rw-rw-   0        0        0     1099 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsOperationFacet.h
--rw-rw-rw-   0        0        0     1867 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsValuesFacet.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.903148 pyconcept-0.1.4/ccl/core/include/ccl/tools/
--rw-rw-rw-   0        0        0      894 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/tools/CstNameGenerator.h
--rw-rw-rw-   0        0        0      523 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/tools/EntityGenerator.h
--rw-rw-rw-   0        0        0     2935 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/tools/EnumJSON.hpp
--rw-rw-rw-   0        0        0     3871 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/ccl/tools/JSON.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.904151 pyconcept-0.1.4/ccl/core/include/nlohmann/
--rw-rw-rw-   0        0        0   945021 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/include/nlohmann/json.hpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.907148 pyconcept-0.1.4/ccl/core/src/
--rw-rw-rw-   0        0        0    18448 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/JSON.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.909153 pyconcept-0.1.4/ccl/core/src/api/
--rw-rw-rw-   0        0        0     3026 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/api/RSFormJA.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.911152 pyconcept-0.1.4/ccl/core/src/env/
--rw-rw-rw-   0        0        0      636 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/env/cclEnvironment.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.915148 pyconcept-0.1.4/ccl/core/src/ops/
--rw-rw-rw-   0        0        0     1772 2024-05-06 14:58:07.000000 pyconcept-0.1.4/ccl/core/src/ops/EquationOptions.cpp
--rw-rw-rw-   0        0        0     4124 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/ops/RSAggregator.cpp
--rw-rw-rw-   0        0        0     4290 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/ops/RSEquationProcessor.cpp
--rw-rw-rw-   0        0        0    16240 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/ops/RSOperations.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.978670 pyconcept-0.1.4/ccl/core/src/oss/
--rw-rw-rw-   0        0        0     7258 2024-05-06 15:10:47.000000 pyconcept-0.1.4/ccl/core/src/oss/OSSchema.cpp
--rw-rw-rw-   0        0        0     2812 2024-05-06 15:23:33.000000 pyconcept-0.1.4/ccl/core/src/oss/RSSynthesProcessor.cpp
--rw-rw-rw-   0        0        0     4305 2024-05-06 15:06:48.000000 pyconcept-0.1.4/ccl/core/src/oss/ossGraphFacet.cpp
--rw-rw-rw-   0        0        0     3023 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/oss/ossGridFacet.cpp
--rw-rw-rw-   0        0        0    11652 2024-05-06 15:05:23.000000 pyconcept-0.1.4/ccl/core/src/oss/ossOperationsFacet.cpp
--rw-rw-rw-   0        0        0    10397 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/oss/ossSourceFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.283578 pyconcept-0.1.4/ccl/core/src/semantic/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.982669 pyconcept-0.1.4/ccl/core/src/semantic/rscore/
--rw-rw-rw-   0        0        0      588 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rscore/ConceptRecord.cpp
--rw-rw-rw-   0        0        0     3957 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rscore/CstList.cpp
--rw-rw-rw-   0        0        0     1950 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rscore/IdentityManager.cpp
--rw-rw-rw-   0        0        0    10403 2024-05-06 15:01:20.000000 pyconcept-0.1.4/ccl/core/src/semantic/rscore/RSCore.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.985670 pyconcept-0.1.4/ccl/core/src/semantic/rsform/
--rw-rw-rw-   0        0        0     8112 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsform/RSForm.cpp
--rw-rw-rw-   0        0        0     1573 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsform/rsModificationFacet.cpp
--rw-rw-rw-   0        0        0     2431 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsform/rsOperationFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.016669 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/
--rw-rw-rw-   0        0        0     1591 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp
--rw-rw-rw-   0        0        0     4755 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/RSModel.cpp
--rw-rw-rw-   0        0        0     3954 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp
--rw-rw-rw-   0        0        0     6866 2024-05-06 13:08:18.000000 pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.052732 pyconcept-0.1.4/ccl/core/src/semantic/schema/
--rw-rw-rw-   0        0        0      830 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/schema/RSConcept.cpp
--rw-rw-rw-   0        0        0    13468 2024-05-08 08:09:16.000000 pyconcept-0.1.4/ccl/core/src/semantic/schema/Schema.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.060736 pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/
--rw-rw-rw-   0        0        0      919 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/TextConcept.cpp
--rw-rw-rw-   0        0        0    10089 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/Thesaurus.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.086732 pyconcept-0.1.4/ccl/core/src/tools/
--rw-rw-rw-   0        0        0     2682 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/tools/CstNameGenerator.cpp
--rw-rw-rw-   0        0        0      773 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/src/tools/EntityGenerator.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.087734 pyconcept-0.1.4/ccl/core/unity/
--rw-rw-rw-   0        0        0     1448 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/core/unity/CCL.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.288579 pyconcept-0.1.4/ccl/rslang/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.138787 pyconcept-0.1.4/ccl/rslang/header/
--rw-rw-rw-   0        0        0     1363 2024-05-06 10:35:16.000000 pyconcept-0.1.4/ccl/rslang/header/ASTNormalizer.h
--rw-rw-rw-   0        0        0    34735 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/header/AsciiLexerImpl.hpp
--rw-rw-rw-   0        0        0     2424 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/header/GeneratorImplAST.h
--rw-rw-rw-   0        0        0    35507 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/header/MathLexerImpl.hpp
--rw-rw-rw-   0        0        0      994 2024-05-09 22:59:05.000000 pyconcept-0.1.4/ccl/rslang/header/NameCollector.h
--rw-rw-rw-   0        0        0    31974 2024-05-09 23:07:18.000000 pyconcept-0.1.4/ccl/rslang/header/RSParserImpl.h
--rw-rw-rw-   0        0        0     5446 2024-05-05 13:20:57.000000 pyconcept-0.1.4/ccl/rslang/header/SDImplementation.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.285579 pyconcept-0.1.4/ccl/rslang/import/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.286578 pyconcept-0.1.4/ccl/rslang/import/reflex/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.285579 pyconcept-0.1.4/ccl/rslang/import/reflex/include/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.211667 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/
--rw-rw-rw-   0        0        0    16072 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/abslexer.h
--rw-rw-rw-   0        0        0    69252 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/absmatcher.h
--rw-rw-rw-   0        0        0    18001 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/bits.h
--rw-rw-rw-   0        0        0    19348 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/boostmatcher.h
--rw-rw-rw-   0        0        0    11147 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/convert.h
--rw-rw-rw-   0        0        0     6862 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/debug.h
--rw-rw-rw-   0        0        0     6978 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/error.h
--rw-rw-rw-   0        0        0    24462 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/flexlexer.h
--rw-rw-rw-   0        0        0    38598 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/input.h
--rw-rw-rw-   0        0        0     6354 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/linematcher.h
--rw-rw-rw-   0        0        0    15401 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/matcher.h
--rw-rw-rw-   0        0        0    45834 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/pattern.h
--rw-rw-rw-   0        0        0    20060 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h
--rw-rw-rw-   0        0        0     2948 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/posix.h
--rw-rw-rw-   0        0        0    37159 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/ranges.h
--rw-rw-rw-   0        0        0    12093 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/setop.h
--rw-rw-rw-   0        0        0     4594 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/simd.h
--rw-rw-rw-   0        0        0    22985 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/stdmatcher.h
--rw-rw-rw-   0        0        0     4244 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/timer.h
--rw-rw-rw-   0        0        0     3159 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/traits.h
--rw-rw-rw-   0        0        0     2997 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/unicode.h
--rw-rw-rw-   0        0        0     9522 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/utf8.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.305788 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/
--rw-rw-rw-   0        0        0    78708 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/convert.cpp
--rw-rw-rw-   0        0        0     3792 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/debug.cpp
--rw-rw-rw-   0        0        0     5896 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/error.cpp
--rw-rw-rw-   0        0        0    84320 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/input.cpp
--rw-rw-rw-   0        0        0   116725 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher.cpp
--rw-rw-rw-   0        0        0     2693 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher_avx2.cpp
--rw-rw-rw-   0        0        0     2715 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp
--rw-rw-rw-   0        0        0   155001 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/pattern.cpp
--rw-rw-rw-   0        0        0     4261 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/posix.cpp
--rw-rw-rw-   0        0        0     5046 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/simd_avx2.cpp
--rw-rw-rw-   0        0        0     3478 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp
--rw-rw-rw-   0        0        0     5118 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/unicode.cpp
--rw-rw-rw-   0        0        0     8872 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/lib/utf8.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:40.310782 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/
--rw-rw-rw-   0        0        0    38187 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/block_scripts.cpp
--rw-rw-rw-   0        0        0    30273 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/composer.cpp
--rw-rw-rw-   0        0        0   223308 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/language_scripts.cpp
--rw-rw-rw-   0        0        0    23072 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/letter_scripts.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.287578 pyconcept-0.1.4/ccl/rslang/include/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:39.287578 pyconcept-0.1.4/ccl/rslang/include/ccl/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.251388 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/
--rw-rw-rw-   0        0        0     3659 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ASTInterpreter.h
--rw-rw-rw-   0        0        0     1048 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/AsciiLexer.h
--rw-rw-rw-   0        0        0      963 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Auditor.h
--rw-rw-rw-   0        0        0      317 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/DataContext.hpp
--rw-rw-rw-   0        0        0     1120 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Error.hpp
--rw-rw-rw-   0        0        0      555 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ErrorLogger.h
--rw-rw-rw-   0        0        0      848 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Interpreter.h
--rw-rw-rw-   0        0        0     2192 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/LexerBase.hpp
--rw-rw-rw-   0        0        0      254 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Literals.h
--rw-rw-rw-   0        0        0      998 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/MathLexer.h
--rw-rw-rw-   0        0        0      927 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Parser.h
--rw-rw-rw-   0        0        0     1667 2024-05-05 09:01:01.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ParserState.hpp
--rw-rw-rw-   0        0        0     6503 2024-05-07 22:51:03.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp
--rw-rw-rw-   0        0        0     1102 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSExpr.h
--rw-rw-rw-   0        0        0     1651 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSGenerator.h
--rw-rw-rw-   0        0        0      869 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSParser.h
--rw-rw-rw-   0        0        0     4722 2024-05-06 14:48:08.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSToken.h
--rw-rw-rw-   0        0        0     1117 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/SDataCompact.h
--rw-rw-rw-   0        0        0     1953 2024-05-08 07:33:13.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Structure.hpp
--rw-rw-rw-   0        0        0     4776 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/StructuredData.h
--rw-rw-rw-   0        0        0    13165 2024-05-09 23:25:09.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/SyntaxTree.h
--rw-rw-rw-   0        0        0     5534 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/TypeAuditor.h
--rw-rw-rw-   0        0        0     1520 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/TypeContext.hpp
--rw-rw-rw-   0        0        0     3927 2024-05-08 07:34:11.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Typification.h
--rw-rw-rw-   0        0        0     4379 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ValueAuditor.h
--rw-rw-rw-   0        0        0      314 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ValueClass.hpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.452579 pyconcept-0.1.4/ccl/rslang/src/
--rw-rw-rw-   0        0        0    19591 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/src/ASTInterpreter.cpp
--rw-rw-rw-   0        0        0     5991 2024-05-06 14:51:18.000000 pyconcept-0.1.4/ccl/rslang/src/ASTNormalizer.cpp
--rw-rw-rw-   0        0        0     2219 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/AsciiLexer.cpp
--rw-rw-rw-   0        0        0     1222 2024-05-06 14:50:47.000000 pyconcept-0.1.4/ccl/rslang/src/Auditor.cpp
--rw-rw-rw-   0        0        0     1375 2024-05-06 10:40:35.000000 pyconcept-0.1.4/ccl/rslang/src/ErrorLogger.cpp
--rw-rw-rw-   0        0        0     7222 2024-05-09 23:22:30.000000 pyconcept-0.1.4/ccl/rslang/src/GeneratorImplAST.cpp
--rw-rw-rw-   0        0        0     1122 2024-05-06 13:10:50.000000 pyconcept-0.1.4/ccl/rslang/src/Interpreter.cpp
--rw-rw-rw-   0        0        0     2067 2024-05-07 15:44:11.000000 pyconcept-0.1.4/ccl/rslang/src/Literals.cpp
--rw-rw-rw-   0        0        0     2316 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/MathLexer.cpp
--rw-rw-rw-   0        0        0     3267 2024-05-09 22:58:58.000000 pyconcept-0.1.4/ccl/rslang/src/NameCollector.cpp
--rw-rw-rw-   0        0        0     3891 2024-05-09 23:09:18.000000 pyconcept-0.1.4/ccl/rslang/src/Parser.cpp
--rw-rw-rw-   0        0        0     3409 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/RSExpr.cpp
--rw-rw-rw-   0        0        0     7626 2024-05-06 14:51:49.000000 pyconcept-0.1.4/ccl/rslang/src/RSGenerator.cpp
--rw-rw-rw-   0        0        0     8365 2024-05-05 12:24:50.000000 pyconcept-0.1.4/ccl/rslang/src/RSParser.cpp
--rw-rw-rw-   0        0        0    63677 2024-05-09 23:07:18.000000 pyconcept-0.1.4/ccl/rslang/src/RSParserImpl.cpp
--rw-rw-rw-   0        0        0    11051 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/RSToken.cpp
--rw-rw-rw-   0        0        0     6872 2024-05-05 13:20:57.000000 pyconcept-0.1.4/ccl/rslang/src/SDImplementation.cpp
--rw-rw-rw-   0        0        0     7639 2024-05-08 08:09:16.000000 pyconcept-0.1.4/ccl/rslang/src/SDataCompact.cpp
--rw-rw-rw-   0        0        0    10421 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/src/StructuredData.cpp
--rw-rw-rw-   0        0        0     6348 2024-05-06 14:51:57.000000 pyconcept-0.1.4/ccl/rslang/src/SyntaxTree.cpp
--rw-rw-rw-   0        0        0    32177 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/src/TypeAuditor.cpp
--rw-rw-rw-   0        0        0     4114 2024-05-08 07:34:32.000000 pyconcept-0.1.4/ccl/rslang/src/Typification.cpp
--rw-rw-rw-   0        0        0     6081 2024-05-09 23:22:53.000000 pyconcept-0.1.4/ccl/rslang/src/ValueAuditor.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.458580 pyconcept-0.1.4/ccl/rslang/unity/
--rw-rw-rw-   0        0        0      399 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/unity/RSlang.cpp
--rw-rw-rw-   0        0        0      458 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/unity/RSlang2.cpp
--rw-rw-rw-   0        0        0     1195 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/unity/reflex_unity1.cpp
--rw-rw-rw-   0        0        0     1776 2024-04-15 19:05:00.000000 pyconcept-0.1.4/ccl/rslang/unity/reflex_unity2.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.460584 pyconcept-0.1.4/cmake/
--rw-rw-rw-   0        0        0     1490 2024-04-19 23:11:03.000000 pyconcept-0.1.4/cmake/CXXTargets.cmake
--rw-rw-rw-   0        0        0       96 2024-04-16 20:20:08.000000 pyconcept-0.1.4/conanfile.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.461578 pyconcept-0.1.4/include/
--rw-rw-rw-   0        0        0     1216 2024-04-15 19:05:00.000000 pyconcept-0.1.4/include/pyconcept.h
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.552449 pyconcept-0.1.4/pyconcept.egg-info/
--rw-rw-rw-   0        0        0      953 2024-05-09 23:28:39.000000 pyconcept-0.1.4/pyconcept.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8509 2024-05-09 23:28:39.000000 pyconcept-0.1.4/pyconcept.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 23:28:39.000000 pyconcept-0.1.4/pyconcept.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-09 23:28:39.000000 pyconcept-0.1.4/pyconcept.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      146 2024-04-17 11:29:28.000000 pyconcept-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      860 2024-05-09 23:28:41.556446 pyconcept-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     3916 2024-04-17 17:59:03.000000 pyconcept-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.469994 pyconcept-0.1.4/src/
--rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.4/src/pyconcept.cpp
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.471997 pyconcept-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-15 19:05:00.000000 pyconcept-0.1.4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.474998 pyconcept-0.1.4/tests/__pycache__/
--rw-rw-rw-   0        0        0      148 2024-04-16 20:55:54.000000 pyconcept-0.1.4/tests/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     5032 2024-04-17 18:55:51.000000 pyconcept-0.1.4/tests/__pycache__/testBinding.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-09 23:28:41.520703 pyconcept-0.1.4/tests/data/
--rw-rw-rw-   0        0        0     2486 2024-04-15 19:05:00.000000 pyconcept-0.1.4/tests/data/Schema1.trs
--rw-rw-rw-   0        0        0     2606 2024-04-17 16:14:46.000000 pyconcept-0.1.4/tests/testBinding.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.942400 pyconcept-0.1.5/
+-rw-rw-rw-   0        0        0     1035 2024-05-13 09:02:27.000000 pyconcept-0.1.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0      955 2024-04-19 23:54:16.000000 pyconcept-0.1.5/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1101 2024-04-15 19:05:00.000000 pyconcept-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      162 2024-04-18 08:33:28.000000 pyconcept-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      953 2024-05-13 09:03:59.941411 pyconcept-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2024-04-17 11:33:45.000000 pyconcept-0.1.5/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-13 09:02:35.000000 pyconcept-0.1.5/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.407977 pyconcept-0.1.5/ccl/
+-rw-rw-rw-   0        0        0     2133 2024-04-17 08:48:56.000000 pyconcept-0.1.5/ccl/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.355832 pyconcept-0.1.5/ccl/cclCommons/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.355832 pyconcept-0.1.5/ccl/cclCommons/include/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.416041 pyconcept-0.1.5/ccl/cclCommons/include/ccl/
+-rw-rw-rw-   0        0        0    10473 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclCommons/include/ccl/Strings.hpp
+-rw-rw-rw-   0        0        0      895 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclCommons/include/ccl/Substitutes.hpp
+-rw-rw-rw-   0        0        0     1506 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclCommons/include/ccl/cclChange.hpp
+-rw-rw-rw-   0        0        0    11710 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclCommons/include/ccl/cclMeta.hpp
+-rw-rw-rw-   0        0        0     6078 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclCommons/include/ccl/cclTypes.hpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.358465 pyconcept-0.1.5/ccl/cclGraph/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.357576 pyconcept-0.1.5/ccl/cclGraph/include/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.417709 pyconcept-0.1.5/ccl/cclGraph/include/ccl/
+-rw-rw-rw-   0        0        0     2749 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclGraph/include/ccl/Entity.hpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.419384 pyconcept-0.1.5/ccl/cclGraph/include/ccl/graph/
+-rw-rw-rw-   0        0        0     2907 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclGraph/include/ccl/graph/CGraph.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.421363 pyconcept-0.1.5/ccl/cclGraph/src/
+-rw-rw-rw-   0        0        0     9187 2024-05-06 12:39:34.000000 pyconcept-0.1.5/ccl/cclGraph/src/CGraph.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.361319 pyconcept-0.1.5/ccl/cclLang/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.360259 pyconcept-0.1.5/ccl/cclLang/include/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.360788 pyconcept-0.1.5/ccl/cclLang/include/ccl/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.437978 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/
+-rw-rw-rw-   0        0        0     1191 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp
+-rw-rw-rw-   0        0        0     1941 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/LexicalTerm.h
+-rw-rw-rw-   0        0        0      345 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/Literals.h
+-rw-rw-rw-   0        0        0     1327 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/ManagedText.h
+-rw-rw-rw-   0        0        0     8108 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/Morphology.h
+-rw-rw-rw-   0        0        0     2748 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/Reference.h
+-rw-rw-rw-   0        0        0     2766 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/RefsManager.h
+-rw-rw-rw-   0        0        0      514 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/TextEnvironment.h
+-rw-rw-rw-   0        0        0     1278 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/TextProcessor.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.450964 pyconcept-0.1.5/ccl/cclLang/src/
+-rw-rw-rw-   0        0        0     2111 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/src/LexicalTerm.cpp
+-rw-rw-rw-   0        0        0      307 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/src/Literals.cpp
+-rw-rw-rw-   0        0        0     2016 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/src/ManagedText.cpp
+-rw-rw-rw-   0        0        0     2239 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/src/Morphology.cpp
+-rw-rw-rw-   0        0        0     7475 2024-05-06 12:47:43.000000 pyconcept-0.1.5/ccl/cclLang/src/Reference.cpp
+-rw-rw-rw-   0        0        0     6529 2024-05-06 12:48:14.000000 pyconcept-0.1.5/ccl/cclLang/src/RefsManager.cpp
+-rw-rw-rw-   0        0        0      452 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/src/TextEnvironment.cpp
+-rw-rw-rw-   0        0        0     1581 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/src/TextProcessor.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.452965 pyconcept-0.1.5/ccl/cclLang/unity/
+-rw-rw-rw-   0        0        0      309 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/cclLang/unity/cclLang.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.453968 pyconcept-0.1.5/ccl/cmake/
+-rw-rw-rw-   0        0        0     1541 2024-04-19 23:11:05.000000 pyconcept-0.1.5/ccl/cmake/CXXTargets.cmake
+-rw-rw-rw-   0        0        0       93 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/conanfile.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.375976 pyconcept-0.1.5/ccl/core/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.367436 pyconcept-0.1.5/ccl/core/include/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.457973 pyconcept-0.1.5/ccl/core/include/ccl/
+-rw-rw-rw-   0        0        0     2124 2024-05-06 15:23:11.000000 pyconcept-0.1.5/ccl/core/include/ccl/Operation.hpp
+-rw-rw-rw-   0        0        0     5309 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/Source.hpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.458977 pyconcept-0.1.5/ccl/core/include/ccl/api/
+-rw-rw-rw-   0        0        0      915 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/api/RSFormJA.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.462128 pyconcept-0.1.5/ccl/core/include/ccl/env/
+-rw-rw-rw-   0        0        0     2904 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/env/SourceManager.hpp
+-rw-rw-rw-   0        0        0      624 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/env/cclEnvironment.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.468970 pyconcept-0.1.5/ccl/core/include/ccl/ops/
+-rw-rw-rw-   0        0        0     1998 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/ops/EquationOptions.h
+-rw-rw-rw-   0        0        0      850 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/ops/RSAggregator.h
+-rw-rw-rw-   0        0        0     1187 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/ops/RSEquationProcessor.h
+-rw-rw-rw-   0        0        0     3525 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/ops/RSOperations.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.483977 pyconcept-0.1.5/ccl/core/include/ccl/oss/
+-rw-rw-rw-   0        0        0     4161 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/oss/OSSchema.h
+-rw-rw-rw-   0        0        0     1658 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/oss/OperationProcessor.hpp
+-rw-rw-rw-   0        0        0      903 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/oss/Pict.hpp
+-rw-rw-rw-   0        0        0      934 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/oss/RSSynthesProcessor.h
+-rw-rw-rw-   0        0        0     1363 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/oss/ossGraphFacet.h
+-rw-rw-rw-   0        0        0     2334 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/oss/ossGridFacet.h
+-rw-rw-rw-   0        0        0     2979 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/oss/ossOperationsFacet.h
+-rw-rw-rw-   0        0        0     2469 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/oss/ossSourceFacet.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.541596 pyconcept-0.1.5/ccl/core/include/ccl/semantic/
+-rw-rw-rw-   0        0        0      622 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/ConceptRecord.h
+-rw-rw-rw-   0        0        0     1473 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/CstFilters.hpp
+-rw-rw-rw-   0        0        0     2367 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/CstList.h
+-rw-rw-rw-   0        0        0     2523 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/CstType.hpp
+-rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/IdentityManager.h
+-rw-rw-rw-   0        0        0      962 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/InterpretationStorage.h
+-rw-rw-rw-   0        0        0     1095 2024-05-06 14:59:52.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/RSConcept.h
+-rw-rw-rw-   0        0        0     3584 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/RSCore.h
+-rw-rw-rw-   0        0        0     3430 2024-05-06 15:04:15.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/RSForm.h
+-rw-rw-rw-   0        0        0     3012 2024-05-06 15:04:05.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/RSModel.h
+-rw-rw-rw-   0        0        0     5074 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/Schema.h
+-rw-rw-rw-   0        0        0     1122 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/TextConcept.h
+-rw-rw-rw-   0        0        0     2603 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/TextData.hpp
+-rw-rw-rw-   0        0        0     3988 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/Thesaurus.h
+-rw-rw-rw-   0        0        0     1577 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/rsCalculationFacet.h
+-rw-rw-rw-   0        0        0     1648 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/rsModificationFacet.h
+-rw-rw-rw-   0        0        0     1099 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/rsOperationFacet.h
+-rw-rw-rw-   0        0        0     1867 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/semantic/rsValuesFacet.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.549152 pyconcept-0.1.5/ccl/core/include/ccl/tools/
+-rw-rw-rw-   0        0        0      894 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/tools/CstNameGenerator.h
+-rw-rw-rw-   0        0        0      523 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/tools/EntityGenerator.h
+-rw-rw-rw-   0        0        0     2935 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/tools/EnumJSON.hpp
+-rw-rw-rw-   0        0        0     3871 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/ccl/tools/JSON.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.550226 pyconcept-0.1.5/ccl/core/include/nlohmann/
+-rw-rw-rw-   0        0        0   945021 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/include/nlohmann/json.hpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.555288 pyconcept-0.1.5/ccl/core/src/
+-rw-rw-rw-   0        0        0    18448 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/JSON.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.557053 pyconcept-0.1.5/ccl/core/src/api/
+-rw-rw-rw-   0        0        0     3026 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/api/RSFormJA.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.559046 pyconcept-0.1.5/ccl/core/src/env/
+-rw-rw-rw-   0        0        0      636 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/env/cclEnvironment.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.564708 pyconcept-0.1.5/ccl/core/src/ops/
+-rw-rw-rw-   0        0        0     1772 2024-05-06 14:58:07.000000 pyconcept-0.1.5/ccl/core/src/ops/EquationOptions.cpp
+-rw-rw-rw-   0        0        0     4124 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/ops/RSAggregator.cpp
+-rw-rw-rw-   0        0        0     4290 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/ops/RSEquationProcessor.cpp
+-rw-rw-rw-   0        0        0    16220 2024-05-10 11:53:57.000000 pyconcept-0.1.5/ccl/core/src/ops/RSOperations.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.575695 pyconcept-0.1.5/ccl/core/src/oss/
+-rw-rw-rw-   0        0        0     7258 2024-05-06 15:10:47.000000 pyconcept-0.1.5/ccl/core/src/oss/OSSchema.cpp
+-rw-rw-rw-   0        0        0     2812 2024-05-06 15:23:33.000000 pyconcept-0.1.5/ccl/core/src/oss/RSSynthesProcessor.cpp
+-rw-rw-rw-   0        0        0     4305 2024-05-06 15:06:48.000000 pyconcept-0.1.5/ccl/core/src/oss/ossGraphFacet.cpp
+-rw-rw-rw-   0        0        0     3023 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/oss/ossGridFacet.cpp
+-rw-rw-rw-   0        0        0    11652 2024-05-06 15:05:23.000000 pyconcept-0.1.5/ccl/core/src/oss/ossOperationsFacet.cpp
+-rw-rw-rw-   0        0        0    10397 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/oss/ossSourceFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.374977 pyconcept-0.1.5/ccl/core/src/semantic/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.581707 pyconcept-0.1.5/ccl/core/src/semantic/rscore/
+-rw-rw-rw-   0        0        0      588 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/rscore/ConceptRecord.cpp
+-rw-rw-rw-   0        0        0     3957 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/rscore/CstList.cpp
+-rw-rw-rw-   0        0        0     1950 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/rscore/IdentityManager.cpp
+-rw-rw-rw-   0        0        0    10403 2024-05-06 15:01:20.000000 pyconcept-0.1.5/ccl/core/src/semantic/rscore/RSCore.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.586699 pyconcept-0.1.5/ccl/core/src/semantic/rsform/
+-rw-rw-rw-   0        0        0     8112 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/rsform/RSForm.cpp
+-rw-rw-rw-   0        0        0     1573 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/rsform/rsModificationFacet.cpp
+-rw-rw-rw-   0        0        0     2431 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/rsform/rsOperationFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.591698 pyconcept-0.1.5/ccl/core/src/semantic/rsmodel/
+-rw-rw-rw-   0        0        0     1591 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp
+-rw-rw-rw-   0        0        0     4755 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/rsmodel/RSModel.cpp
+-rw-rw-rw-   0        0        0     3954 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp
+-rw-rw-rw-   0        0        0     6866 2024-05-06 13:08:18.000000 pyconcept-0.1.5/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.593695 pyconcept-0.1.5/ccl/core/src/semantic/schema/
+-rw-rw-rw-   0        0        0      830 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/schema/RSConcept.cpp
+-rw-rw-rw-   0        0        0    13468 2024-05-08 08:09:16.000000 pyconcept-0.1.5/ccl/core/src/semantic/schema/Schema.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.643594 pyconcept-0.1.5/ccl/core/src/semantic/thesaurus/
+-rw-rw-rw-   0        0        0      919 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/thesaurus/TextConcept.cpp
+-rw-rw-rw-   0        0        0    10089 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/semantic/thesaurus/Thesaurus.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.646611 pyconcept-0.1.5/ccl/core/src/tools/
+-rw-rw-rw-   0        0        0     2682 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/tools/CstNameGenerator.cpp
+-rw-rw-rw-   0        0        0      773 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/src/tools/EntityGenerator.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.648608 pyconcept-0.1.5/ccl/core/unity/
+-rw-rw-rw-   0        0        0     1448 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/core/unity/CCL.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.381965 pyconcept-0.1.5/ccl/rslang/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.670604 pyconcept-0.1.5/ccl/rslang/header/
+-rw-rw-rw-   0        0        0     1511 2024-05-12 22:52:36.000000 pyconcept-0.1.5/ccl/rslang/header/ASTNormalizer.h
+-rw-rw-rw-   0        0        0    34737 2024-05-10 11:57:55.000000 pyconcept-0.1.5/ccl/rslang/header/AsciiLexerImpl.hpp
+-rw-rw-rw-   0        0        0     2525 2024-05-12 11:39:13.000000 pyconcept-0.1.5/ccl/rslang/header/GeneratorImplAST.h
+-rw-rw-rw-   0        0        0    35509 2024-05-10 11:57:56.000000 pyconcept-0.1.5/ccl/rslang/header/MathLexerImpl.hpp
+-rw-rw-rw-   0        0        0      994 2024-05-09 22:59:05.000000 pyconcept-0.1.5/ccl/rslang/header/NameCollector.h
+-rw-rw-rw-   0        0        0    31805 2024-05-11 08:11:59.000000 pyconcept-0.1.5/ccl/rslang/header/RSParserImpl.h
+-rw-rw-rw-   0        0        0     5446 2024-05-05 13:20:57.000000 pyconcept-0.1.5/ccl/rslang/header/SDImplementation.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.377977 pyconcept-0.1.5/ccl/rslang/import/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.379968 pyconcept-0.1.5/ccl/rslang/import/reflex/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.378977 pyconcept-0.1.5/ccl/rslang/import/reflex/include/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.716672 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/
+-rw-rw-rw-   0        0        0    16072 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/abslexer.h
+-rw-rw-rw-   0        0        0    69252 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/absmatcher.h
+-rw-rw-rw-   0        0        0    18001 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/bits.h
+-rw-rw-rw-   0        0        0    19348 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/boostmatcher.h
+-rw-rw-rw-   0        0        0    11147 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/convert.h
+-rw-rw-rw-   0        0        0     6862 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/debug.h
+-rw-rw-rw-   0        0        0     6978 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/error.h
+-rw-rw-rw-   0        0        0    24462 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/flexlexer.h
+-rw-rw-rw-   0        0        0    38598 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/input.h
+-rw-rw-rw-   0        0        0     6354 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/linematcher.h
+-rw-rw-rw-   0        0        0    15401 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/matcher.h
+-rw-rw-rw-   0        0        0    45834 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/pattern.h
+-rw-rw-rw-   0        0        0    20060 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h
+-rw-rw-rw-   0        0        0     2948 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/posix.h
+-rw-rw-rw-   0        0        0    37159 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/ranges.h
+-rw-rw-rw-   0        0        0    12093 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/setop.h
+-rw-rw-rw-   0        0        0     4594 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/simd.h
+-rw-rw-rw-   0        0        0    22985 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/stdmatcher.h
+-rw-rw-rw-   0        0        0     4244 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/timer.h
+-rw-rw-rw-   0        0        0     3159 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/traits.h
+-rw-rw-rw-   0        0        0     2997 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/unicode.h
+-rw-rw-rw-   0        0        0     9522 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/utf8.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.741909 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/
+-rw-rw-rw-   0        0        0    78708 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/convert.cpp
+-rw-rw-rw-   0        0        0     3792 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/debug.cpp
+-rw-rw-rw-   0        0        0     5896 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/error.cpp
+-rw-rw-rw-   0        0        0    84320 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/input.cpp
+-rw-rw-rw-   0        0        0   116725 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/matcher.cpp
+-rw-rw-rw-   0        0        0     2693 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/matcher_avx2.cpp
+-rw-rw-rw-   0        0        0     2715 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp
+-rw-rw-rw-   0        0        0   155001 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/pattern.cpp
+-rw-rw-rw-   0        0        0     4261 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/posix.cpp
+-rw-rw-rw-   0        0        0     5046 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/simd_avx2.cpp
+-rw-rw-rw-   0        0        0     3478 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp
+-rw-rw-rw-   0        0        0     5118 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/unicode.cpp
+-rw-rw-rw-   0        0        0     8872 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/lib/utf8.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.748916 pyconcept-0.1.5/ccl/rslang/import/reflex/unicode/
+-rw-rw-rw-   0        0        0    38187 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/unicode/block_scripts.cpp
+-rw-rw-rw-   0        0        0    30273 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/unicode/composer.cpp
+-rw-rw-rw-   0        0        0   223308 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/unicode/language_scripts.cpp
+-rw-rw-rw-   0        0        0    23072 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/import/reflex/unicode/letter_scripts.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.380966 pyconcept-0.1.5/ccl/rslang/include/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.380966 pyconcept-0.1.5/ccl/rslang/include/ccl/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.796893 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/
+-rw-rw-rw-   0        0        0     3618 2024-05-12 23:46:56.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/ASTInterpreter.h
+-rw-rw-rw-   0        0        0     1048 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/AsciiLexer.h
+-rw-rw-rw-   0        0        0      963 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Auditor.h
+-rw-rw-rw-   0        0        0      317 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/DataContext.hpp
+-rw-rw-rw-   0        0        0     1120 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Error.hpp
+-rw-rw-rw-   0        0        0      555 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/ErrorLogger.h
+-rw-rw-rw-   0        0        0      848 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Interpreter.h
+-rw-rw-rw-   0        0        0     2195 2024-05-10 15:22:43.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/LexerBase.hpp
+-rw-rw-rw-   0        0        0      254 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Literals.h
+-rw-rw-rw-   0        0        0      998 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/MathLexer.h
+-rw-rw-rw-   0        0        0      927 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Parser.h
+-rw-rw-rw-   0        0        0     1667 2024-05-11 08:03:02.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/ParserState.hpp
+-rw-rw-rw-   0        0        0     6663 2024-05-11 07:56:58.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp
+-rw-rw-rw-   0        0        0     1102 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSExpr.h
+-rw-rw-rw-   0        0        0     1651 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSGenerator.h
+-rw-rw-rw-   0        0        0      869 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSParser.h
+-rw-rw-rw-   0        0        0     4588 2024-05-10 15:36:06.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSToken.h
+-rw-rw-rw-   0        0        0     1117 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/SDataCompact.h
+-rw-rw-rw-   0        0        0     1953 2024-05-08 07:33:13.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Structure.hpp
+-rw-rw-rw-   0        0        0     4776 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/StructuredData.h
+-rw-rw-rw-   0        0        0    12947 2024-05-12 22:30:56.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/SyntaxTree.h
+-rw-rw-rw-   0        0        0     5446 2024-05-10 15:05:19.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/TypeAuditor.h
+-rw-rw-rw-   0        0        0     1520 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/TypeContext.hpp
+-rw-rw-rw-   0        0        0     3927 2024-05-08 07:34:11.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Typification.h
+-rw-rw-rw-   0        0        0     4282 2024-05-10 14:55:13.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/ValueAuditor.h
+-rw-rw-rw-   0        0        0      314 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/ValueClass.hpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.848725 pyconcept-0.1.5/ccl/rslang/src/
+-rw-rw-rw-   0        0        0    19735 2024-05-13 00:02:46.000000 pyconcept-0.1.5/ccl/rslang/src/ASTInterpreter.cpp
+-rw-rw-rw-   0        0        0     6885 2024-05-13 08:36:27.000000 pyconcept-0.1.5/ccl/rslang/src/ASTNormalizer.cpp
+-rw-rw-rw-   0        0        0     2219 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/src/AsciiLexer.cpp
+-rw-rw-rw-   0        0        0     1222 2024-05-06 14:50:47.000000 pyconcept-0.1.5/ccl/rslang/src/Auditor.cpp
+-rw-rw-rw-   0        0        0     1375 2024-05-06 10:40:35.000000 pyconcept-0.1.5/ccl/rslang/src/ErrorLogger.cpp
+-rw-rw-rw-   0        0        0     6808 2024-05-12 11:39:21.000000 pyconcept-0.1.5/ccl/rslang/src/GeneratorImplAST.cpp
+-rw-rw-rw-   0        0        0     1122 2024-05-06 13:10:50.000000 pyconcept-0.1.5/ccl/rslang/src/Interpreter.cpp
+-rw-rw-rw-   0        0        0     2067 2024-05-07 15:44:11.000000 pyconcept-0.1.5/ccl/rslang/src/Literals.cpp
+-rw-rw-rw-   0        0        0     2316 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/src/MathLexer.cpp
+-rw-rw-rw-   0        0        0     3250 2024-05-10 15:01:10.000000 pyconcept-0.1.5/ccl/rslang/src/NameCollector.cpp
+-rw-rw-rw-   0        0        0     3891 2024-05-09 23:09:18.000000 pyconcept-0.1.5/ccl/rslang/src/Parser.cpp
+-rw-rw-rw-   0        0        0     3409 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/src/RSExpr.cpp
+-rw-rw-rw-   0        0        0     7626 2024-05-06 14:51:49.000000 pyconcept-0.1.5/ccl/rslang/src/RSGenerator.cpp
+-rw-rw-rw-   0        0        0     9890 2024-05-11 14:55:48.000000 pyconcept-0.1.5/ccl/rslang/src/RSParser.cpp
+-rw-rw-rw-   0        0        0    62145 2024-05-11 08:11:59.000000 pyconcept-0.1.5/ccl/rslang/src/RSParserImpl.cpp
+-rw-rw-rw-   0        0        0    10856 2024-05-10 15:04:16.000000 pyconcept-0.1.5/ccl/rslang/src/RSToken.cpp
+-rw-rw-rw-   0        0        0     6872 2024-05-05 13:20:57.000000 pyconcept-0.1.5/ccl/rslang/src/SDImplementation.cpp
+-rw-rw-rw-   0        0        0     7639 2024-05-08 08:09:16.000000 pyconcept-0.1.5/ccl/rslang/src/SDataCompact.cpp
+-rw-rw-rw-   0        0        0    10421 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/src/StructuredData.cpp
+-rw-rw-rw-   0        0        0     6348 2024-05-06 14:51:57.000000 pyconcept-0.1.5/ccl/rslang/src/SyntaxTree.cpp
+-rw-rw-rw-   0        0        0    32171 2024-05-10 15:05:42.000000 pyconcept-0.1.5/ccl/rslang/src/TypeAuditor.cpp
+-rw-rw-rw-   0        0        0     4114 2024-05-08 07:34:32.000000 pyconcept-0.1.5/ccl/rslang/src/Typification.cpp
+-rw-rw-rw-   0        0        0     6081 2024-05-09 23:22:53.000000 pyconcept-0.1.5/ccl/rslang/src/ValueAuditor.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.854818 pyconcept-0.1.5/ccl/rslang/unity/
+-rw-rw-rw-   0        0        0      399 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/unity/RSlang.cpp
+-rw-rw-rw-   0        0        0      458 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/unity/RSlang2.cpp
+-rw-rw-rw-   0        0        0     1195 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/unity/reflex_unity1.cpp
+-rw-rw-rw-   0        0        0     1776 2024-04-15 19:05:00.000000 pyconcept-0.1.5/ccl/rslang/unity/reflex_unity2.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.856821 pyconcept-0.1.5/cmake/
+-rw-rw-rw-   0        0        0     1490 2024-04-19 23:11:03.000000 pyconcept-0.1.5/cmake/CXXTargets.cmake
+-rw-rw-rw-   0        0        0       96 2024-04-16 20:20:08.000000 pyconcept-0.1.5/conanfile.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.858919 pyconcept-0.1.5/include/
+-rw-rw-rw-   0        0        0     1216 2024-04-15 19:05:00.000000 pyconcept-0.1.5/include/pyconcept.h
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.938397 pyconcept-0.1.5/pyconcept.egg-info/
+-rw-rw-rw-   0        0        0      953 2024-05-13 09:03:59.000000 pyconcept-0.1.5/pyconcept.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8509 2024-05-13 09:03:59.000000 pyconcept-0.1.5/pyconcept.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 09:03:59.000000 pyconcept-0.1.5/pyconcept.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 09:03:59.000000 pyconcept-0.1.5/pyconcept.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      146 2024-04-17 11:29:28.000000 pyconcept-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      860 2024-05-13 09:03:59.944405 pyconcept-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     3916 2024-04-17 17:59:03.000000 pyconcept-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.870986 pyconcept-0.1.5/src/
+-rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.5/src/pyconcept.cpp
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.873514 pyconcept-0.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-15 19:05:00.000000 pyconcept-0.1.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.935394 pyconcept-0.1.5/tests/__pycache__/
+-rw-rw-rw-   0        0        0      148 2024-04-16 20:55:54.000000 pyconcept-0.1.5/tests/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5032 2024-04-17 18:55:51.000000 pyconcept-0.1.5/tests/__pycache__/testBinding.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-13 09:03:59.937398 pyconcept-0.1.5/tests/data/
+-rw-rw-rw-   0        0        0     2486 2024-04-15 19:05:00.000000 pyconcept-0.1.5/tests/data/Schema1.trs
+-rw-rw-rw-   0        0        0     2606 2024-04-17 16:14:46.000000 pyconcept-0.1.5/tests/testBinding.py
```

### Comparing `pyconcept-0.1.4/CHANGELOG.md` & `pyconcept-0.1.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 - [PROJECTNAME-YYYY](http://tickets.projectname.com/browse/PROJECTNAME-YYYY)
   PATCH Ticket title goes here.
 
 ### Changed
 
 ### Fixed
 
+## [0.1.5] - 2024-05-10
+
+### Added
+
+- Allow tuple declarations in imperative syntax
+
 ## [0.1.4] - 2024-05-10
 
 ### Fixed
 
 - EmptySet is correctly processed as argument for functions and other operations
 
 ## [0.1.3] - 2024-05-08
```

### Comparing `pyconcept-0.1.4/CMakeLists.txt` & `pyconcept-0.1.5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/LICENSE` & `pyconcept-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/PKG-INFO` & `pyconcept-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconcept
-Version: 0.1.4
+Version: 0.1.5
 Summary: Concept core Python wrapper
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Project-URL: GitHub, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept
 Project-URL: Changelog, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyconcept-0.1.4/ccl/CMakeLists.txt` & `pyconcept-0.1.5/ccl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclCommons/include/ccl/Strings.hpp` & `pyconcept-0.1.5/ccl/cclCommons/include/ccl/Strings.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclCommons/include/ccl/Substitutes.hpp` & `pyconcept-0.1.5/ccl/cclCommons/include/ccl/Substitutes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclChange.hpp` & `pyconcept-0.1.5/ccl/cclCommons/include/ccl/cclChange.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclMeta.hpp` & `pyconcept-0.1.5/ccl/cclCommons/include/ccl/cclMeta.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclCommons/include/ccl/cclTypes.hpp` & `pyconcept-0.1.5/ccl/cclCommons/include/ccl/cclTypes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclGraph/include/ccl/Entity.hpp` & `pyconcept-0.1.5/ccl/cclGraph/include/ccl/Entity.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclGraph/include/ccl/graph/CGraph.h` & `pyconcept-0.1.5/ccl/cclGraph/include/ccl/graph/CGraph.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclGraph/src/CGraph.cpp` & `pyconcept-0.1.5/ccl/cclGraph/src/CGraph.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp` & `pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/LexicalTerm.h` & `pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/LexicalTerm.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/ManagedText.h` & `pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/ManagedText.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Morphology.h` & `pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/Morphology.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/Reference.h` & `pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/Reference.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/RefsManager.h` & `pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/RefsManager.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/TextEnvironment.h` & `pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/TextEnvironment.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/include/ccl/lang/TextProcessor.h` & `pyconcept-0.1.5/ccl/cclLang/include/ccl/lang/TextProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/src/LexicalTerm.cpp` & `pyconcept-0.1.5/ccl/cclLang/src/LexicalTerm.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/src/ManagedText.cpp` & `pyconcept-0.1.5/ccl/cclLang/src/ManagedText.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/src/Morphology.cpp` & `pyconcept-0.1.5/ccl/cclLang/src/Morphology.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/src/Reference.cpp` & `pyconcept-0.1.5/ccl/cclLang/src/Reference.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/src/RefsManager.cpp` & `pyconcept-0.1.5/ccl/cclLang/src/RefsManager.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cclLang/src/TextProcessor.cpp` & `pyconcept-0.1.5/ccl/cclLang/src/TextProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/cmake/CXXTargets.cmake` & `pyconcept-0.1.5/ccl/cmake/CXXTargets.cmake`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/Operation.hpp` & `pyconcept-0.1.5/ccl/core/include/ccl/Operation.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/Source.hpp` & `pyconcept-0.1.5/ccl/core/include/ccl/Source.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/api/RSFormJA.h` & `pyconcept-0.1.5/ccl/core/include/ccl/api/RSFormJA.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/env/SourceManager.hpp` & `pyconcept-0.1.5/ccl/core/include/ccl/env/SourceManager.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/env/cclEnvironment.h` & `pyconcept-0.1.5/ccl/core/include/ccl/env/cclEnvironment.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/ops/EquationOptions.h` & `pyconcept-0.1.5/ccl/core/include/ccl/ops/EquationOptions.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/ops/RSAggregator.h` & `pyconcept-0.1.5/ccl/core/include/ccl/ops/RSAggregator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/ops/RSEquationProcessor.h` & `pyconcept-0.1.5/ccl/core/include/ccl/ops/RSEquationProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/ops/RSOperations.h` & `pyconcept-0.1.5/ccl/core/include/ccl/ops/RSOperations.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/oss/OSSchema.h` & `pyconcept-0.1.5/ccl/core/include/ccl/oss/OSSchema.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/oss/OperationProcessor.hpp` & `pyconcept-0.1.5/ccl/core/include/ccl/oss/OperationProcessor.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/oss/Pict.hpp` & `pyconcept-0.1.5/ccl/core/include/ccl/oss/Pict.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/oss/RSSynthesProcessor.h` & `pyconcept-0.1.5/ccl/core/include/ccl/oss/RSSynthesProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/oss/ossGraphFacet.h` & `pyconcept-0.1.5/ccl/core/include/ccl/oss/ossGraphFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/oss/ossGridFacet.h` & `pyconcept-0.1.5/ccl/core/include/ccl/oss/ossGridFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/oss/ossOperationsFacet.h` & `pyconcept-0.1.5/ccl/core/include/ccl/oss/ossOperationsFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/oss/ossSourceFacet.h` & `pyconcept-0.1.5/ccl/core/include/ccl/oss/ossSourceFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/ConceptRecord.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/ConceptRecord.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstFilters.hpp` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/CstFilters.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstList.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/CstList.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/CstType.hpp` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/CstType.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/IdentityManager.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/IdentityManager.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/InterpretationStorage.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/InterpretationStorage.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSConcept.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/RSConcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSCore.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/RSCore.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSForm.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/RSForm.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/RSModel.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/RSModel.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/Schema.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/Schema.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/TextConcept.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/TextConcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/TextData.hpp` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/TextData.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/Thesaurus.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/Thesaurus.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsCalculationFacet.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/rsCalculationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsModificationFacet.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/rsModificationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsOperationFacet.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/rsOperationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/semantic/rsValuesFacet.h` & `pyconcept-0.1.5/ccl/core/include/ccl/semantic/rsValuesFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/tools/CstNameGenerator.h` & `pyconcept-0.1.5/ccl/core/include/ccl/tools/CstNameGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/tools/EntityGenerator.h` & `pyconcept-0.1.5/ccl/core/include/ccl/tools/EntityGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/tools/EnumJSON.hpp` & `pyconcept-0.1.5/ccl/core/include/ccl/tools/EnumJSON.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/ccl/tools/JSON.h` & `pyconcept-0.1.5/ccl/core/include/ccl/tools/JSON.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/include/nlohmann/json.hpp` & `pyconcept-0.1.5/ccl/core/include/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/JSON.cpp` & `pyconcept-0.1.5/ccl/core/src/JSON.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/api/RSFormJA.cpp` & `pyconcept-0.1.5/ccl/core/src/api/RSFormJA.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/env/cclEnvironment.cpp` & `pyconcept-0.1.5/ccl/core/src/env/cclEnvironment.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/ops/EquationOptions.cpp` & `pyconcept-0.1.5/ccl/core/src/ops/EquationOptions.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/ops/RSAggregator.cpp` & `pyconcept-0.1.5/ccl/core/src/ops/RSAggregator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/ops/RSEquationProcessor.cpp` & `pyconcept-0.1.5/ccl/core/src/ops/RSEquationProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/ops/RSOperations.cpp` & `pyconcept-0.1.5/ccl/core/src/ops/RSOperations.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -394,23 +394,23 @@
       const auto updated = UpdatedExpression(cst.definition);
 #if !defined(__GNUC__) && !defined(__clang__)
       std::string newExpression = std::format("I{{({0}, {1}) | {0}{4}{2}; {1}{5}{3}}}",
                                        baseID,        // 0
                                        termID,        // 1
                                        baseName,      // 2
                                        updated,        // 3
-                                       Token::Str(TokenID::PUNC_ITERATE), // 4
-                                       Token::Str(TokenID::PUNC_ASSIGN)); // 5
+                                       Token::Str(TokenID::ITERATE), // 4
+                                       Token::Str(TokenID::ASSIGN)); // 5
 #else
       std::string newExpression = "I{(";
       newExpression += baseID + ", " + termID;
       newExpression += ") | ";
-      newExpression += baseID + Token::Str(TokenID::PUNC_ITERATE) + baseName;
+      newExpression += baseID + Token::Str(TokenID::ITERATE) + baseName;
       newExpression += "; ";
-      newExpression += termID + Token::Str(TokenID::PUNC_ASSIGN) + updated + "}";
+      newExpression += termID + Token::Str(TokenID::ASSIGN) + updated + "}";
 #endif
       resultSchema->SetExpressionFor(entity, newExpression);
       break;
     }
     case CstType::structured: {
       resultSchema->SetExpressionFor(entity, Token::Str(TokenID::BOOLEAN) + '(' + baseName
                                      + Token::Str(TokenID::DECART) + cst.definition + ')');
```

### Comparing `pyconcept-0.1.4/ccl/core/src/oss/OSSchema.cpp` & `pyconcept-0.1.5/ccl/core/src/oss/OSSchema.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/oss/RSSynthesProcessor.cpp` & `pyconcept-0.1.5/ccl/core/src/oss/RSSynthesProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/oss/ossGraphFacet.cpp` & `pyconcept-0.1.5/ccl/core/src/oss/ossGraphFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/oss/ossGridFacet.cpp` & `pyconcept-0.1.5/ccl/core/src/oss/ossGridFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/oss/ossOperationsFacet.cpp` & `pyconcept-0.1.5/ccl/core/src/oss/ossOperationsFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/oss/ossSourceFacet.cpp` & `pyconcept-0.1.5/ccl/core/src/oss/ossSourceFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rscore/ConceptRecord.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rscore/ConceptRecord.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rscore/CstList.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rscore/CstList.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rscore/IdentityManager.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rscore/IdentityManager.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rscore/RSCore.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rscore/RSCore.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rsform/RSForm.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rsform/RSForm.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rsform/rsModificationFacet.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rsform/rsModificationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rsform/rsOperationFacet.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rsform/rsOperationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/RSModel.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rsmodel/RSModel.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/schema/RSConcept.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/schema/RSConcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/schema/Schema.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/schema/Schema.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/TextConcept.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/thesaurus/TextConcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/semantic/thesaurus/Thesaurus.cpp` & `pyconcept-0.1.5/ccl/core/src/semantic/thesaurus/Thesaurus.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/tools/CstNameGenerator.cpp` & `pyconcept-0.1.5/ccl/core/src/tools/CstNameGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/src/tools/EntityGenerator.cpp` & `pyconcept-0.1.5/ccl/core/src/tools/EntityGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/core/unity/CCL.cpp` & `pyconcept-0.1.5/ccl/core/unity/CCL.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/header/ASTNormalizer.h` & `pyconcept-0.1.5/ccl/rslang/header/ASTNormalizer.h`

 * *Files 13% similar despite different names*

```diff
@@ -6,39 +6,42 @@
 
 namespace ccl::rslang {
 //! Converter for AST into standard form
 class Normalizer {
 public:
   using TupleSubstitutes = std::unordered_map<std::string, std::vector<Index>>;
   using NodeSubstitutes = std::unordered_map<std::string, const SyntaxTree::Node*>;
+  using NameSubstitutes = std::unordered_map<std::string, std::string>;
 
 private:
   SyntaxTreeContext termFuncs;
 
-  TupleSubstitutes tuples{};
-  NodeSubstitutes nodes{};
-
-  std::unordered_map<std::string, std::string> nameSubstitutes{};
+  TupleSubstitutes tupleSubstitutes{};
+  NodeSubstitutes nodeSubstitutes{};
+  NameSubstitutes nameSubstitutes{};
   uint32_t localVarBase{ 0 };
 
 public:
   explicit Normalizer(SyntaxTreeContext termFuncs)
     : termFuncs{ std::move(termFuncs) } {}
 
 public:
   void Normalize(SyntaxTree::Node& root);
 
 private:
   void Quantifier(SyntaxTree::Node& quant);
+  void Imperative(SyntaxTree::Node& root);
+  void Recursion(SyntaxTree::Node& root);
+  void Declarative(SyntaxTree::Node& root);
+  void Function(SyntaxTree::Node& func);
+
   static void EnumDeclaration(SyntaxTree::Node& quant);
   void TupleDeclaration(SyntaxTree::Node& declaration, SyntaxTree::Node& predicate);
-  void TupleDeclaration(SyntaxTree::Node& target);
 
-  [[nodiscard]] std::string CreateTupleName(const SyntaxTree::Node& root);
+  [[nodiscard]] std::string ProcessTupleDeclaration(SyntaxTree::Node& root);
   void SubstituteTupleVariables(SyntaxTree::Node& target, const std::string& newName);
-
-  void Function(SyntaxTree::Node& func);
+  
   [[nodiscard]] static std::vector<std::string> ArgNames(const SyntaxTree::Node& declaration);
   void SubstituteArgs(SyntaxTree::Node& target, StrRange pos);
 };
 
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.4/ccl/rslang/header/AsciiLexerImpl.hpp` & `pyconcept-0.1.5/ccl/rslang/header/AsciiLexerImpl.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-// AsciiLexerImpl.hpp generated by reflex 4.2.0 from AsciiLexerImpl.l
+// AsciiLexerImpl.hpp generated by reflex 4.2.1 from AsciiLexerImpl.l
 
-#define REFLEX_VERSION "4.2.0"
+#define REFLEX_VERSION "4.2.1"
 
 ////////////////////////////////////////////////////////////////////////////////
 //                                                                            //
 //  OPTIONS USED                                                              //
 //                                                                            //
 ////////////////////////////////////////////////////////////////////////////////
 
@@ -72,16 +72,18 @@
 namespace asciilex {
 
 class AsciiLexerImpl : public reflex::AbstractLexer<reflex::Matcher> {
 
 public:
   [[nodiscard]] StrRange Range() const {
    // Note: returning byte position, not code point! Assume input is ASCII
-    return StrRange{ static_cast<StrPos>(matcher().first()),
-            static_cast<StrPos>(matcher().last()) };
+    return StrRange{
+        static_cast<StrPos>(matcher().first()),
+        static_cast<StrPos>(matcher().last())
+    };
   }
 
  public:
   typedef reflex::AbstractLexer<reflex::Matcher> AbstractBaseLexer;
   AsciiLexerImpl(
       // a persistent source of input, empty by default
       const reflex::Input& input = reflex::Input(),
@@ -148,204 +150,204 @@
             }
             else
             {
               lexer_error("scanner jammed");
               return ccl::rslang::TokenID();
             }
             break;
-          case 1: // rule AsciiLexerImpl.l:45: "\A" :
+          case 1: // rule AsciiLexerImpl.l:47: "\A" :
 { return TokenID::FORALL; }
             break;
-          case 2: // rule AsciiLexerImpl.l:46: "\E" :
+          case 2: // rule AsciiLexerImpl.l:48: "\E" :
 { return TokenID::EXISTS; }
 
             break;
-          case 3: // rule AsciiLexerImpl.l:48: "\neg" :
+          case 3: // rule AsciiLexerImpl.l:50: "\neg" :
 { return TokenID::NOT; }
             break;
-          case 4: // rule AsciiLexerImpl.l:49: "\and" :
+          case 4: // rule AsciiLexerImpl.l:51: "\and" :
 { return TokenID::AND; }
             break;
-          case 5: // rule AsciiLexerImpl.l:50: "\or" :
+          case 5: // rule AsciiLexerImpl.l:52: "\or" :
 { return TokenID::OR; }
             break;
-          case 6: // rule AsciiLexerImpl.l:51: "\impl" :
+          case 6: // rule AsciiLexerImpl.l:53: "\impl" :
 { return TokenID::IMPLICATION; }
             break;
-          case 7: // rule AsciiLexerImpl.l:52: "\equiv" :
+          case 7: // rule AsciiLexerImpl.l:54: "\equiv" :
 { return TokenID::EQUIVALENT; }
 
             break;
-          case 8: // rule AsciiLexerImpl.l:54: "\plus" :
+          case 8: // rule AsciiLexerImpl.l:56: "\plus" :
 { return TokenID::PLUS; }
             break;
-          case 9: // rule AsciiLexerImpl.l:55: "\minus" :
+          case 9: // rule AsciiLexerImpl.l:57: "\minus" :
 { return TokenID::MINUS; }
             break;
-          case 10: // rule AsciiLexerImpl.l:56: "\multiply" :
+          case 10: // rule AsciiLexerImpl.l:58: "\multiply" :
 { return TokenID::MULTIPLY; }
             break;
-          case 11: // rule AsciiLexerImpl.l:57: "\gr" :
+          case 11: // rule AsciiLexerImpl.l:59: "\gr" :
 { return TokenID::GREATER; }
             break;
-          case 12: // rule AsciiLexerImpl.l:58: "\ls" :
+          case 12: // rule AsciiLexerImpl.l:60: "\ls" :
 { return TokenID::LESSER; }
             break;
-          case 13: // rule AsciiLexerImpl.l:59: "\ge" :
+          case 13: // rule AsciiLexerImpl.l:61: "\ge" :
 { return TokenID::GREATER_OR_EQ; }
             break;
-          case 14: // rule AsciiLexerImpl.l:60: "\le" :
+          case 14: // rule AsciiLexerImpl.l:62: "\le" :
 { return TokenID::LESSER_OR_EQ; }
 
             break;
-          case 15: // rule AsciiLexerImpl.l:62: "\eq" :
+          case 15: // rule AsciiLexerImpl.l:64: "\eq" :
 { return TokenID::EQUAL; }
             break;
-          case 16: // rule AsciiLexerImpl.l:63: "\noteq" :
+          case 16: // rule AsciiLexerImpl.l:65: "\noteq" :
 { return TokenID::NOTEQUAL; }
 
             break;
-          case 17: // rule AsciiLexerImpl.l:65: "\in" :
+          case 17: // rule AsciiLexerImpl.l:67: "\in" :
 { return TokenID::IN; }
             break;
-          case 18: // rule AsciiLexerImpl.l:66: "\notin" :
+          case 18: // rule AsciiLexerImpl.l:68: "\notin" :
 { return TokenID::NOTIN; }
             break;
-          case 19: // rule AsciiLexerImpl.l:67: "\subseteq" :
+          case 19: // rule AsciiLexerImpl.l:69: "\subseteq" :
 { return TokenID::SUBSET_OR_EQ; }
             break;
-          case 20: // rule AsciiLexerImpl.l:68: "\subset" :
+          case 20: // rule AsciiLexerImpl.l:70: "\subset" :
 { return TokenID::SUBSET; }
             break;
-          case 21: // rule AsciiLexerImpl.l:69: "\notsubset" :
+          case 21: // rule AsciiLexerImpl.l:71: "\notsubset" :
 { return TokenID::NOTSUBSET; }
 
             break;
-          case 22: // rule AsciiLexerImpl.l:71: "*" :
+          case 22: // rule AsciiLexerImpl.l:73: "*" :
 { return TokenID::DECART; }
             break;
-          case 23: // rule AsciiLexerImpl.l:72: "\union" :
+          case 23: // rule AsciiLexerImpl.l:74: "\union" :
 { return TokenID::UNION; }
             break;
-          case 24: // rule AsciiLexerImpl.l:73: "\intersect" :
+          case 24: // rule AsciiLexerImpl.l:75: "\intersect" :
 { return TokenID::INTERSECTION; }
             break;
-          case 25: // rule AsciiLexerImpl.l:74: "\setminus" :
+          case 25: // rule AsciiLexerImpl.l:76: "\setminus" :
 { return TokenID::SET_MINUS; }
             break;
-          case 26: // rule AsciiLexerImpl.l:75: "\symmdiff" :
+          case 26: // rule AsciiLexerImpl.l:77: "\symmdiff" :
 { return TokenID::SYMMINUS; }
             break;
-          case 27: // rule AsciiLexerImpl.l:76: "B" :
+          case 27: // rule AsciiLexerImpl.l:78: "B" :
 { return TokenID::BOOLEAN; }
 
             break;
-          case 28: // rule AsciiLexerImpl.l:78: pr{index} :
+          case 28: // rule AsciiLexerImpl.l:80: pr{index} :
 { return TokenID::SMALLPR; }
             break;
-          case 29: // rule AsciiLexerImpl.l:79: Pr{index} :
+          case 29: // rule AsciiLexerImpl.l:81: Pr{index} :
 { return TokenID::BIGPR; }
             break;
-          case 30: // rule AsciiLexerImpl.l:80: Fi{index} :
+          case 30: // rule AsciiLexerImpl.l:82: Fi{index} :
 { return TokenID::FILTER; }
             break;
-          case 31: // rule AsciiLexerImpl.l:81: card :
+          case 31: // rule AsciiLexerImpl.l:83: card :
 { return TokenID::CARD; }
             break;
-          case 32: // rule AsciiLexerImpl.l:82: bool :
+          case 32: // rule AsciiLexerImpl.l:84: bool :
 { return TokenID::BOOL; }
             break;
-          case 33: // rule AsciiLexerImpl.l:83: red :
+          case 33: // rule AsciiLexerImpl.l:85: red :
 { return TokenID::REDUCE; }
             break;
-          case 34: // rule AsciiLexerImpl.l:84: debool :
+          case 34: // rule AsciiLexerImpl.l:86: debool :
 { return TokenID::DEBOOL; }
 
             break;
-          case 35: // rule AsciiLexerImpl.l:86: D :
+          case 35: // rule AsciiLexerImpl.l:88: D :
 { return TokenID::DECLARATIVE; }
             break;
-          case 36: // rule AsciiLexerImpl.l:87: R :
+          case 36: // rule AsciiLexerImpl.l:89: R :
 { return TokenID::RECURSIVE; }
             break;
-          case 37: // rule AsciiLexerImpl.l:88: I :
+          case 37: // rule AsciiLexerImpl.l:90: I :
 { return TokenID::IMPERATIVE; }
 
             break;
-          case 38: // rule AsciiLexerImpl.l:90: Z :
+          case 38: // rule AsciiLexerImpl.l:92: Z :
 { return TokenID::LIT_INTSET; }
             break;
-          case 39: // rule AsciiLexerImpl.l:91: "{}" :
+          case 39: // rule AsciiLexerImpl.l:93: "{}" :
 { return TokenID::LIT_EMPTYSET; }
             break;
-          case 40: // rule AsciiLexerImpl.l:92: {number} :
+          case 40: // rule AsciiLexerImpl.l:94: {number} :
 { return TokenID::LIT_INTEGER; }
 
             break;
-          case 41: // rule AsciiLexerImpl.l:94: F{number} :
+          case 41: // rule AsciiLexerImpl.l:96: F{number} :
 { return TokenID::ID_FUNCTION; }
             break;
-          case 42: // rule AsciiLexerImpl.l:95: P{number} :
+          case 42: // rule AsciiLexerImpl.l:97: P{number} :
 { return TokenID::ID_PREDICATE; }
             break;
-          case 43: // rule AsciiLexerImpl.l:96: R{number} :
+          case 43: // rule AsciiLexerImpl.l:98: R{number} :
 { return TokenID::ID_RADICAL; }
 
             break;
-          case 44: // rule AsciiLexerImpl.l:98: {global_id} :
+          case 44: // rule AsciiLexerImpl.l:100: {global_id} :
 { return TokenID::ID_GLOBAL; }
             break;
-          case 45: // rule AsciiLexerImpl.l:99: {local_id} :
+          case 45: // rule AsciiLexerImpl.l:101: {local_id} :
 { return TokenID::ID_LOCAL; }
 
             break;
-          case 46: // rule AsciiLexerImpl.l:101: "\assign" :
-{ return TokenID::PUNC_ASSIGN; }
+          case 46: // rule AsciiLexerImpl.l:103: "\assign" :
+{ return TokenID::ASSIGN; }
             break;
-          case 47: // rule AsciiLexerImpl.l:102: "\from" :
-{ return TokenID::PUNC_ITERATE; }
+          case 47: // rule AsciiLexerImpl.l:104: "\from" :
+{ return TokenID::ITERATE; }
             break;
-          case 48: // rule AsciiLexerImpl.l:103: "\defexpr" :
+          case 48: // rule AsciiLexerImpl.l:105: "\defexpr" :
 { return TokenID::PUNC_DEFINE; }
             break;
-          case 49: // rule AsciiLexerImpl.l:104: "\deftype" :
+          case 49: // rule AsciiLexerImpl.l:106: "\deftype" :
 { return TokenID::PUNC_STRUCT; }
             break;
-          case 50: // rule AsciiLexerImpl.l:105: "(" :
+          case 50: // rule AsciiLexerImpl.l:107: "(" :
 { return TokenID::PUNC_PL; }
             break;
-          case 51: // rule AsciiLexerImpl.l:106: ")" :
+          case 51: // rule AsciiLexerImpl.l:108: ")" :
 { return TokenID::PUNC_PR; }
             break;
-          case 52: // rule AsciiLexerImpl.l:107: "{" :
+          case 52: // rule AsciiLexerImpl.l:109: "{" :
 { return TokenID::PUNC_CL; }
             break;
-          case 53: // rule AsciiLexerImpl.l:108: "}" :
+          case 53: // rule AsciiLexerImpl.l:110: "}" :
 { return TokenID::PUNC_CR; }
             break;
-          case 54: // rule AsciiLexerImpl.l:109: "[" :
+          case 54: // rule AsciiLexerImpl.l:111: "[" :
 { return TokenID::PUNC_SL; }
             break;
-          case 55: // rule AsciiLexerImpl.l:110: "]" :
+          case 55: // rule AsciiLexerImpl.l:112: "]" :
 { return TokenID::PUNC_SR; }
             break;
-          case 56: // rule AsciiLexerImpl.l:111: "|" :
+          case 56: // rule AsciiLexerImpl.l:113: "|" :
 { return TokenID::PUNC_BAR; }
             break;
-          case 57: // rule AsciiLexerImpl.l:112: "," :
+          case 57: // rule AsciiLexerImpl.l:114: "," :
 { return TokenID::PUNC_COMMA; }
             break;
-          case 58: // rule AsciiLexerImpl.l:113: ";" :
+          case 58: // rule AsciiLexerImpl.l:115: ";" :
 { return TokenID::PUNC_SEMICOLON; }
 
             break;
-          case 59: // rule AsciiLexerImpl.l:115: {ws} :
+          case 59: // rule AsciiLexerImpl.l:117: {ws} :
 ;
             break;
-          case 60: // rule AsciiLexerImpl.l:117: . :
+          case 60: // rule AsciiLexerImpl.l:119: . :
 { return TokenID::INTERRUPT; }
 
             break;
         }
   }
 }
```

### Comparing `pyconcept-0.1.4/ccl/rslang/header/GeneratorImplAST.h` & `pyconcept-0.1.5/ccl/rslang/header/GeneratorImplAST.h`

 * *Files 10% similar despite different names*

```diff
@@ -37,24 +37,23 @@
 
   bool ViArithmetic(Cursor iter);
   bool ViCard(Cursor iter);
 
   bool ViQuantifier(Cursor iter);
   bool ViNegation(Cursor iter);
   bool ViLogicBinary(Cursor iter);
-  bool ViEquals(Cursor iter);
-  bool ViIntegerPredicate(Cursor iter) { return ViEquals(iter); }
-  bool ViSetexprPredicate(Cursor iter) { return ViEquals(iter); }
+  bool ViEquals(Cursor iter) { return OutputBinary(iter); }
+  bool ViIntegerPredicate(Cursor iter) { return OutputBinary(iter); }
+  bool ViSetexprPredicate(Cursor iter) { return OutputBinary(iter); }
 
   bool ViDeclarative(Cursor iter);
-  bool ViImperative(Cursor iter);
-  bool ViImpDeclare(Cursor iter);
-  bool ViImpAssign(Cursor iter);
-  bool ViImpCheck(Cursor iter);
   bool ViRecursion(Cursor iter);
+  bool ViImperative(Cursor iter);
+  bool ViIterate(Cursor iter) { return OutputBinary(iter); }
+  bool ViAssign(Cursor iter) { return OutputBinary(iter); }
 
   bool ViDecart(Cursor iter);
   bool ViBoolean(Cursor iter);
 
   bool ViTuple(Cursor iter);
   bool ViEnumeration(Cursor iter);
   bool ViBool(Cursor iter) { return ViCard(iter); }
@@ -67,13 +66,14 @@
   bool ViReduce(Cursor iter) { return ViCard(iter); }
 
 private:
   void SetSyntax(const Syntax newSyntax) noexcept { syntax = newSyntax; }
   void Clear() noexcept;
 
   void OutputChild(const Cursor& iter, Index index, bool addBrackets = false);
+  bool OutputBinary(const Cursor& iter);
 
-  void EnumChildren(const Cursor& iter, const std::string& separator);
-  void EnumChildren(const Cursor& iter, char left, char right, const std::string& separator);
+  bool EnumChildren(const Cursor& iter, const std::string& separator);
+  bool EnumChildren(const Cursor& iter, char left, char right, const std::string& separator);
 };
 
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.4/ccl/rslang/header/MathLexerImpl.hpp` & `pyconcept-0.1.5/ccl/rslang/header/MathLexerImpl.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-// MathLexerImpl.hpp generated by reflex 4.2.0 from MathLexerImpl.l
+// MathLexerImpl.hpp generated by reflex 4.2.1 from MathLexerImpl.l
 
-#define REFLEX_VERSION "4.2.0"
+#define REFLEX_VERSION "4.2.1"
 
 ////////////////////////////////////////////////////////////////////////////////
 //                                                                            //
 //  OPTIONS USED                                                              //
 //                                                                            //
 ////////////////////////////////////////////////////////////////////////////////
 
@@ -77,16 +77,18 @@
 
 class MathLexerImpl : public reflex::AbstractLexer<reflex::Matcher> {
 
 public:
   StrPos lineBase{ 0 };
 
   [[nodiscard]] StrRange Range() const {
-    return StrRange{ static_cast<StrPos>(lineBase + columno()),
-            static_cast<StrPos>(lineBase + columno() + columns()) };
+    return StrRange{
+        static_cast<StrPos>(lineBase + columno()),
+        static_cast<StrPos>(lineBase + columno() + columns())
+    };
   }
 
 
  public:
   typedef reflex::AbstractLexer<reflex::Matcher> AbstractBaseLexer;
   MathLexerImpl(
       // a persistent source of input, empty by default
@@ -154,207 +156,207 @@
             }
             else
             {
               lexer_error("scanner jammed");
               return ccl::rslang::TokenID();
             }
             break;
-          case 1: // rule MathLexerImpl.l:48: "+" :
+          case 1: // rule MathLexerImpl.l:50: "+" :
 { return TokenID::PLUS; }
             break;
-          case 2: // rule MathLexerImpl.l:49: "-" :
+          case 2: // rule MathLexerImpl.l:51: "-" :
 { return TokenID::MINUS; }
             break;
-          case 3: // rule MathLexerImpl.l:50: "*" :
+          case 3: // rule MathLexerImpl.l:52: "*" :
 { return TokenID::MULTIPLY; }
             break;
-          case 4: // rule MathLexerImpl.l:51: ">" :
+          case 4: // rule MathLexerImpl.l:53: ">" :
 { return TokenID::GREATER; }
             break;
-          case 5: // rule MathLexerImpl.l:52: "<" :
+          case 5: // rule MathLexerImpl.l:54: "<" :
 { return TokenID::LESSER; }
             break;
-          case 6: // rule MathLexerImpl.l:53: \x{2265} :
+          case 6: // rule MathLexerImpl.l:55: \x{2265} :
 { return TokenID::GREATER_OR_EQ; }
             break;
-          case 7: // rule MathLexerImpl.l:54: \x{2264} :
+          case 7: // rule MathLexerImpl.l:56: \x{2264} :
 { return TokenID::LESSER_OR_EQ; }
 
             break;
-          case 8: // rule MathLexerImpl.l:56: "=" :
+          case 8: // rule MathLexerImpl.l:58: "=" :
 { return TokenID::EQUAL; }
             break;
-          case 9: // rule MathLexerImpl.l:57: \x{2260} :
+          case 9: // rule MathLexerImpl.l:59: \x{2260} :
 { return TokenID::NOTEQUAL; }
 
             break;
-          case 10: // rule MathLexerImpl.l:59: \x{2200} :
+          case 10: // rule MathLexerImpl.l:61: \x{2200} :
 { return TokenID::FORALL; }
             break;
-          case 11: // rule MathLexerImpl.l:60: \x{2203} :
+          case 11: // rule MathLexerImpl.l:62: \x{2203} :
 { return TokenID::EXISTS; }
 
             break;
-          case 12: // rule MathLexerImpl.l:62: \x{00AC} :
+          case 12: // rule MathLexerImpl.l:64: \x{00AC} :
 { return TokenID::NOT; }
             break;
-          case 13: // rule MathLexerImpl.l:63: "&" :
+          case 13: // rule MathLexerImpl.l:65: "&" :
 { return TokenID::AND; }
             break;
-          case 14: // rule MathLexerImpl.l:64: \x{2228} :
+          case 14: // rule MathLexerImpl.l:66: \x{2228} :
 { return TokenID::OR; }
             break;
-          case 15: // rule MathLexerImpl.l:65: \x{21D2} :
+          case 15: // rule MathLexerImpl.l:67: \x{21D2} :
 { return TokenID::IMPLICATION; }
             break;
-          case 16: // rule MathLexerImpl.l:66: \x{21D4} :
+          case 16: // rule MathLexerImpl.l:68: \x{21D4} :
 { return TokenID::EQUIVALENT; }
 
             break;
-          case 17: // rule MathLexerImpl.l:68: :\x{2208} :
-{ return TokenID::PUNC_ITERATE; }
+          case 17: // rule MathLexerImpl.l:70: :\x{2208} :
+{ return TokenID::ITERATE; }
             break;
-          case 18: // rule MathLexerImpl.l:69: \x{2208} :
+          case 18: // rule MathLexerImpl.l:71: \x{2208} :
 { return TokenID::IN; }
             break;
-          case 19: // rule MathLexerImpl.l:70: \x{2209} :
+          case 19: // rule MathLexerImpl.l:72: \x{2209} :
 { return TokenID::NOTIN; }
             break;
-          case 20: // rule MathLexerImpl.l:71: \x{2286} :
+          case 20: // rule MathLexerImpl.l:73: \x{2286} :
 { return TokenID::SUBSET_OR_EQ; }
             break;
-          case 21: // rule MathLexerImpl.l:72: \x{2282} :
+          case 21: // rule MathLexerImpl.l:74: \x{2282} :
 { return TokenID::SUBSET; }
             break;
-          case 22: // rule MathLexerImpl.l:73: \x{2284} :
+          case 22: // rule MathLexerImpl.l:75: \x{2284} :
 { return TokenID::NOTSUBSET; }
 
             break;
-          case 23: // rule MathLexerImpl.l:75: \x{00D7} :
+          case 23: // rule MathLexerImpl.l:77: \x{00D7} :
 { return TokenID::DECART; }
             break;
-          case 24: // rule MathLexerImpl.l:76: \x{222A} :
+          case 24: // rule MathLexerImpl.l:78: \x{222A} :
 { return TokenID::UNION; }
             break;
-          case 25: // rule MathLexerImpl.l:77: \x{2229} :
+          case 25: // rule MathLexerImpl.l:79: \x{2229} :
 { return TokenID::INTERSECTION; }
             break;
-          case 26: // rule MathLexerImpl.l:78: \x{005C} :
+          case 26: // rule MathLexerImpl.l:80: \x{005C} :
 { return TokenID::SET_MINUS; }
             break;
-          case 27: // rule MathLexerImpl.l:79: \x{2206} :
+          case 27: // rule MathLexerImpl.l:81: \x{2206} :
 { return TokenID::SYMMINUS; }
             break;
-          case 28: // rule MathLexerImpl.l:80: \x{212C} :
+          case 28: // rule MathLexerImpl.l:82: \x{212C} :
 { return TokenID::BOOLEAN; }
 
             break;
-          case 29: // rule MathLexerImpl.l:82: pr{index} :
+          case 29: // rule MathLexerImpl.l:84: pr{index} :
 { return TokenID::SMALLPR; }
             break;
-          case 30: // rule MathLexerImpl.l:83: Pr{index} :
+          case 30: // rule MathLexerImpl.l:85: Pr{index} :
 { return TokenID::BIGPR; }
             break;
-          case 31: // rule MathLexerImpl.l:84: Fi{index} :
+          case 31: // rule MathLexerImpl.l:86: Fi{index} :
 { return TokenID::FILTER; }
             break;
-          case 32: // rule MathLexerImpl.l:85: card :
+          case 32: // rule MathLexerImpl.l:87: card :
 { return TokenID::CARD; }
             break;
-          case 33: // rule MathLexerImpl.l:86: bool :
+          case 33: // rule MathLexerImpl.l:88: bool :
 { return TokenID::BOOL; }
             break;
-          case 34: // rule MathLexerImpl.l:87: red :
+          case 34: // rule MathLexerImpl.l:89: red :
 { return TokenID::REDUCE; }
             break;
-          case 35: // rule MathLexerImpl.l:88: debool :
+          case 35: // rule MathLexerImpl.l:90: debool :
 { return TokenID::DEBOOL; }
 
             break;
-          case 36: // rule MathLexerImpl.l:90: D :
+          case 36: // rule MathLexerImpl.l:92: D :
 { return TokenID::DECLARATIVE; }
             break;
-          case 37: // rule MathLexerImpl.l:91: R :
+          case 37: // rule MathLexerImpl.l:93: R :
 { return TokenID::RECURSIVE; }
             break;
-          case 38: // rule MathLexerImpl.l:92: I :
+          case 38: // rule MathLexerImpl.l:94: I :
 { return TokenID::IMPERATIVE; }
 
             break;
-          case 39: // rule MathLexerImpl.l:94: Z :
+          case 39: // rule MathLexerImpl.l:96: Z :
 { return TokenID::LIT_INTSET; }
             break;
-          case 40: // rule MathLexerImpl.l:95: \x{2205} :
+          case 40: // rule MathLexerImpl.l:97: \x{2205} :
 { return TokenID::LIT_EMPTYSET; }
             break;
-          case 41: // rule MathLexerImpl.l:96: {number} :
+          case 41: // rule MathLexerImpl.l:98: {number} :
 { return TokenID::LIT_INTEGER; }
 
             break;
-          case 42: // rule MathLexerImpl.l:98: F{number} :
+          case 42: // rule MathLexerImpl.l:100: F{number} :
 { return TokenID::ID_FUNCTION; }
             break;
-          case 43: // rule MathLexerImpl.l:99: P{number} :
+          case 43: // rule MathLexerImpl.l:101: P{number} :
 { return TokenID::ID_PREDICATE; }
             break;
-          case 44: // rule MathLexerImpl.l:100: R{number} :
+          case 44: // rule MathLexerImpl.l:102: R{number} :
 { return TokenID::ID_RADICAL; }
 
             break;
-          case 45: // rule MathLexerImpl.l:102: {global_id} :
+          case 45: // rule MathLexerImpl.l:104: {global_id} :
 { return TokenID::ID_GLOBAL; }
             break;
-          case 46: // rule MathLexerImpl.l:103: {local_id} :
+          case 46: // rule MathLexerImpl.l:105: {local_id} :
 { return TokenID::ID_LOCAL; }
 
             break;
-          case 47: // rule MathLexerImpl.l:105: ":=" :
-{ return TokenID::PUNC_ASSIGN; }
+          case 47: // rule MathLexerImpl.l:107: ":=" :
+{ return TokenID::ASSIGN; }
             break;
-          case 48: // rule MathLexerImpl.l:106: ":==" :
+          case 48: // rule MathLexerImpl.l:108: ":==" :
 { return TokenID::PUNC_DEFINE; }
             break;
-          case 49: // rule MathLexerImpl.l:107: "::=" :
+          case 49: // rule MathLexerImpl.l:109: "::=" :
 { return TokenID::PUNC_STRUCT; }
             break;
-          case 50: // rule MathLexerImpl.l:108: "(" :
+          case 50: // rule MathLexerImpl.l:110: "(" :
 { return TokenID::PUNC_PL; }
             break;
-          case 51: // rule MathLexerImpl.l:109: ")" :
+          case 51: // rule MathLexerImpl.l:111: ")" :
 { return TokenID::PUNC_PR; }
             break;
-          case 52: // rule MathLexerImpl.l:110: "{" :
+          case 52: // rule MathLexerImpl.l:112: "{" :
 { return TokenID::PUNC_CL; }
             break;
-          case 53: // rule MathLexerImpl.l:111: "}" :
+          case 53: // rule MathLexerImpl.l:113: "}" :
 { return TokenID::PUNC_CR; }
             break;
-          case 54: // rule MathLexerImpl.l:112: "[" :
+          case 54: // rule MathLexerImpl.l:114: "[" :
 { return TokenID::PUNC_SL; }
             break;
-          case 55: // rule MathLexerImpl.l:113: "]" :
+          case 55: // rule MathLexerImpl.l:115: "]" :
 { return TokenID::PUNC_SR; }
             break;
-          case 56: // rule MathLexerImpl.l:114: "|" :
+          case 56: // rule MathLexerImpl.l:116: "|" :
 { return TokenID::PUNC_BAR; }
             break;
-          case 57: // rule MathLexerImpl.l:115: "," :
+          case 57: // rule MathLexerImpl.l:117: "," :
 { return TokenID::PUNC_COMMA; }
             break;
-          case 58: // rule MathLexerImpl.l:116: ";" :
+          case 58: // rule MathLexerImpl.l:118: ";" :
 { return TokenID::PUNC_SEMICOLON; }
 
             break;
-          case 59: // rule MathLexerImpl.l:118: \n :
+          case 59: // rule MathLexerImpl.l:120: \n :
 { lineBase += static_cast<StrPos>(columno() + 1); }
             break;
-          case 60: // rule MathLexerImpl.l:119: [ \t]+ :
+          case 60: // rule MathLexerImpl.l:121: [ \t]+ :
 ;
             break;
-          case 61: // rule MathLexerImpl.l:121: . :
+          case 61: // rule MathLexerImpl.l:123: . :
 { return TokenID::INTERRUPT; }
 
             break;
         }
   }
 }
```

### Comparing `pyconcept-0.1.4/ccl/rslang/header/NameCollector.h` & `pyconcept-0.1.5/ccl/rslang/header/NameCollector.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/header/RSParserImpl.h` & `pyconcept-0.1.5/ccl/rslang/header/RSParserImpl.h`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
     RawNode start,
     RawNode argumentsDeclaration,
     RawNode expr
 );
 
 RawNode FunctionCall(
     RawNode function,
-    RawNode args, RawNode
-    rs
+    RawNode args,
+    RawNode rs
 );
 
 RawNode FilterCall(
     RawNode filter,
     RawNode params,
     RawNode argument,
     RawNode rp
@@ -105,15 +105,20 @@
 );
 
 RawNode TermDeclaration(
     RawNode lc,
     RawNode declaration,
     RawNode domain,
     RawNode predicate,
-    RawNode rc);
+    RawNode rc
+);
+RawNode TupleDeclaration(
+    ParserState* state,
+    RawNode tuple
+);
 
 RawNode FullRecursion(
     RawNode rec,
     RawNode declaration,
     RawNode domain,
     RawNode condition,
     RawNode iteration,
@@ -133,15 +138,15 @@
     RawNode value,
     RawNode actions,
     RawNode rc
 );
 
 } // namespace ccl::rslang::detail
 
-#line 141 "../header/RSParserImpl.h"
+#line 146 "../header/RSParserImpl.h"
 
 # include <cassert>
 # include <cstdlib> // std::abort
 # include <iostream>
 # include <stdexcept>
 # include <string>
 # include <vector>
@@ -263,15 +268,15 @@
 /* Debug traces.  */
 #ifndef YYDEBUG
 # define YYDEBUG 0
 #endif
 
 #line 15 "RSParserImpl.y"
 namespace ccl { namespace rslang { namespace detail {
-#line 271 "../header/RSParserImpl.h"
+#line 276 "../header/RSParserImpl.h"
 
 
 
 
   /// A Bison parser.
   class RSParserImpl
   {
@@ -347,18 +352,18 @@
     RST_CARD = 296,                // CARD
     RST_BOOL = 297,                // BOOL
     RST_DEBOOL = 298,              // DEBOOL
     RST_RED = 299,                 // RED
     RST_DECLARATIVE = 300,         // DECLARATIVE
     RST_RECURSIVE = 301,           // RECURSIVE
     RST_IMPERATIVE = 302,          // IMPERATIVE
-    RST_DEFINE = 303,              // DEFINE
-    RST_STRUCT = 304,              // STRUCT
-    RST_ASSIGN = 305,              // ASSIGN
-    RST_ITERATE = 306,             // ITERATE
+    RST_ITERATE = 303,             // ITERATE
+    RST_ASSIGN = 304,              // ASSIGN
+    RST_DEFINE = 305,              // DEFINE
+    RST_STRUCT = 306,              // STRUCT
     RST_LP = 307,                  // LP
     RST_RP = 308,                  // RP
     RST_LC = 309,                  // LC
     RST_RC = 310,                  // RC
     RST_LS = 311,                  // LS
     RST_RS = 312,                  // RS
     RST_BAR = 313,                 // BAR
@@ -426,18 +431,18 @@
         S_CARD = 41,                             // CARD
         S_BOOL = 42,                             // BOOL
         S_DEBOOL = 43,                           // DEBOOL
         S_RED = 44,                              // RED
         S_DECLARATIVE = 45,                      // DECLARATIVE
         S_RECURSIVE = 46,                        // RECURSIVE
         S_IMPERATIVE = 47,                       // IMPERATIVE
-        S_DEFINE = 48,                           // DEFINE
-        S_STRUCT = 49,                           // STRUCT
-        S_ASSIGN = 50,                           // ASSIGN
-        S_ITERATE = 51,                          // ITERATE
+        S_ITERATE = 48,                          // ITERATE
+        S_ASSIGN = 49,                           // ASSIGN
+        S_DEFINE = 50,                           // DEFINE
+        S_STRUCT = 51,                           // STRUCT
         S_LP = 52,                               // LP
         S_RP = 53,                               // RP
         S_LC = 54,                               // LC
         S_RC = 55,                               // RC
         S_LS = 56,                               // LS
         S_RS = 57,                               // RS
         S_BAR = 58,                              // BAR
@@ -447,46 +452,42 @@
         S_expression = 62,                       // expression
         S_global_declaration = 63,               // global_declaration
         S_logic_or_setexpr = 64,                 // logic_or_setexpr
         S_function_definition = 65,              // function_definition
         S_arguments = 66,                        // arguments
         S_declaration = 67,                      // declaration
         S_variable = 68,                         // variable
-        S_var_enum = 69,                         // var_enum
-        S_var_all = 70,                          // var_all
-        S_logic = 71,                            // logic
+        S_variable_pack = 69,                    // variable_pack
+        S_logic = 70,                            // logic
+        S_logic_no_binary = 71,                  // logic_no_binary
         S_logic_all = 72,                        // logic_all
         S_logic_par = 73,                        // logic_par
         S_logic_predicates = 74,                 // logic_predicates
         S_binary_predicate = 75,                 // binary_predicate
         S_logic_unary = 76,                      // logic_unary
-        S_logic_no_binary = 77,                  // logic_no_binary
-        S_quantifier = 78,                       // quantifier
-        S_quant_var = 79,                        // quant_var
-        S_quant_var_enum = 80,                   // quant_var_enum
-        S_logic_binary = 81,                     // logic_binary
-        S_setexpr = 82,                          // setexpr
-        S_text_function = 83,                    // text_function
-        S_setexpr_enum = 84,                     // setexpr_enum
-        S_setexpr_enum_min2 = 85,                // setexpr_enum_min2
-        S_literal = 86,                          // literal
-        S_identifier = 87,                       // identifier
-        S_setexpr_binary = 88,                   // setexpr_binary
-        S_setexpr_generators = 89,               // setexpr_generators
-        S_enumeration = 90,                      // enumeration
-        S_tuple = 91,                            // tuple
-        S_boolean = 92,                          // boolean
-        S_filter_expression = 93,                // filter_expression
-        S_declarative = 94,                      // declarative
-        S_recursion = 95,                        // recursion
-        S_imperative = 96,                       // imperative
-        S_imp_blocks = 97,                       // imp_blocks
-        S_imp_block = 98,                        // imp_block
-        S_RPE = 99,                              // RPE
-        S_RCE = 100                              // RCE
+        S_quantifier = 77,                       // quantifier
+        S_logic_binary = 78,                     // logic_binary
+        S_setexpr = 79,                          // setexpr
+        S_text_function = 80,                    // text_function
+        S_setexpr_enum = 81,                     // setexpr_enum
+        S_setexpr_enum_min2 = 82,                // setexpr_enum_min2
+        S_literal = 83,                          // literal
+        S_identifier = 84,                       // identifier
+        S_setexpr_binary = 85,                   // setexpr_binary
+        S_setexpr_generators = 86,               // setexpr_generators
+        S_enumeration = 87,                      // enumeration
+        S_tuple = 88,                            // tuple
+        S_boolean = 89,                          // boolean
+        S_filter_expression = 90,                // filter_expression
+        S_declarative = 91,                      // declarative
+        S_recursion = 92,                        // recursion
+        S_imperative = 93,                       // imperative
+        S_imp_blocks = 94,                       // imp_blocks
+        S_RPE = 95,                              // RPE
+        S_RCE = 96                               // RCE
       };
     };
 
     /// (Internal) symbol kind.
     typedef symbol_kind::symbol_kind_type symbol_kind_type;
 
     /// The number of tokens.
@@ -976,27 +977,27 @@
 
     /// Pop \a n symbols from the stack.
     void yypop_ (int n = 1);
 
     /// Constants.
     enum
     {
-      yylast_ = 640,     ///< Last index in yytable_.
-      yynnts_ = 40,  ///< Number of nonterminal symbols.
-      yyfinal_ = 87 ///< Termination state number.
+      yylast_ = 620,     ///< Last index in yytable_.
+      yynnts_ = 36,  ///< Number of nonterminal symbols.
+      yyfinal_ = 89 ///< Termination state number.
     };
 
 
     // User arguments.
     ParserState* state;
 
   };
 
 
 #line 15 "RSParserImpl.y"
 } } } // ccl::rslang::detail
-#line 998 "../header/RSParserImpl.h"
+#line 999 "../header/RSParserImpl.h"
 
 
 
 
 #endif // !YY_YY_HEADER_RSPARSERIMPL_H_INCLUDED
```

### Comparing `pyconcept-0.1.4/ccl/rslang/header/SDImplementation.h` & `pyconcept-0.1.5/ccl/rslang/header/SDImplementation.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/abslexer.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/abslexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/absmatcher.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/absmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/bits.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/bits.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/boostmatcher.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/boostmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/convert.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/convert.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/debug.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/debug.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/error.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/error.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/flexlexer.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/flexlexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/input.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/input.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/linematcher.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/linematcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/matcher.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/matcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/pattern.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/pattern.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/posix.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/posix.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/ranges.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/ranges.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/setop.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/setop.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/simd.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/simd.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/stdmatcher.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/stdmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/timer.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/timer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/traits.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/traits.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/unicode.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/unicode.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/include/reflex/utf8.h` & `pyconcept-0.1.5/ccl/rslang/import/reflex/include/reflex/utf8.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/convert.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/convert.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/debug.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/debug.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/error.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/error.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/input.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/input.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/matcher.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher_avx2.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/matcher_avx2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/pattern.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/pattern.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/posix.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/posix.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/simd_avx2.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/simd_avx2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/unicode.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/unicode.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/lib/utf8.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/lib/utf8.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/block_scripts.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/unicode/block_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/composer.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/unicode/composer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/language_scripts.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/unicode/language_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/import/reflex/unicode/letter_scripts.cpp` & `pyconcept-0.1.5/ccl/rslang/import/reflex/unicode/letter_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ASTInterpreter.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/ASTInterpreter.h`

 * *Files 2% similar despite different names*

```diff
@@ -77,19 +77,18 @@
   bool ViIntegerPredicate(Cursor iter);
   bool ViSetexprPredicate(Cursor iter) { return ViSetexprBinary(iter); }
 
   bool ViDecart(Cursor iter);
   bool ViBoolean(Cursor iter);
 
   bool ViDeclarative(Cursor iter);
-  bool ViImperative(Cursor iter);
-  //bool ViImpDeclare(Cursor iter);
-  //bool ViImpAssign(Cursor iter);
-  //bool ViImpCheck(Cursor iter);
   bool ViRecursion(Cursor iter);
+  bool ViImperative(Cursor iter);
+  //bool ViIterate(Cursor iter);
+  //bool ViAssign(Cursor iter);
 
   bool ViTuple(Cursor iter);
   bool ViEnumeration(Cursor iter);
   bool ViBool(Cursor iter);
   bool ViDebool(Cursor iter);
 
   bool ViSetexprBinary(Cursor iter);
```

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/AsciiLexer.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/AsciiLexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Auditor.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Auditor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Error.hpp` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Error.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ErrorLogger.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/ErrorLogger.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Interpreter.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Interpreter.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/LexerBase.hpp` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/LexerBase.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,19 @@
   }
 
   [[nodiscard]] TokenStream Stream() {
     return[lex = this]() {
       lex->lex();
       auto token = lex->MakeToken();
       if (token.id == TokenID::INTERRUPT && lex->reporter.has_value()) {
-        lex->reporter.value()(Error{ static_cast<uint32_t>(LexerEID::unknownSymbol),
-                                      token.pos.start, { lex->Text() } });
+        lex->reporter.value()(Error{
+          static_cast<uint32_t>(LexerEID::unknownSymbol),
+          token.pos.start,
+          { lex->Text() }
+        });
       }
       return token;
     };
   }
 
   [[nodiscard]] std::string Text() const {
     return this->BaseT().GetText();
```

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/MathLexer.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/MathLexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Parser.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Parser.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ParserState.hpp` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/ParserState.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -53,14 +53,14 @@
       ++countCriticalErrors;
     }
     if (reporter.has_value()) {
       reporter.value()(err);
     }
   }
 
-  void CreateSyntaxTree(RawNode root);
-  void FinalizeExpression(RawNode expr);
-  void FinalizeCstEmpty(RawNode cst, RawNode mode);
-  void FinalizeCstExpression(RawNode cst, RawNode mode, RawNode data);
+  bool CreateSyntaxTree(RawNode root);
+  bool FinalizeExpression(RawNode expr);
+  bool FinalizeCstEmpty(RawNode cst, RawNode mode);
+  bool FinalizeCstExpression(RawNode cst, RawNode mode, RawNode data);
 };
 
 } // namespace ccl::rslang::detail
```

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 //! Syntactic errors enumeration
 enum class ParseEID : uint32_t {
   syntax = 0x8400, // Неизвестная синтаксическая ошибка
   missingParenthesis = 0x8406,      // Пропущена скобка ')'
   missingCurlyBrace = 0x8407,       // Пропущена скобка '}'
   invalidQuantifier = 0x8408,       // Некорректная кванторная декларация
+  invalidImperative = 0x8409,       // Использование императивного синтаксиса вне императивного блока
   expectedDeclaration = 0x8414,     // Ожидалось объявление аргументов
   expectedLocal = 0x8415,           // Ожидалось имя локальной переменной
 };
 
 //! Semantic errors enumeration
 enum class SemanticEID : uint32_t {
   localDoubleDeclare = 0x2801,      // Повторное использование одного и того же имени переменной
```

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSExpr.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSExpr.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSGenerator.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSParser.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSParser.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/RSToken.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/RSToken.h`

 * *Files 4% similar despite different names*

```diff
@@ -78,19 +78,21 @@
   REDUCE,
 
   // Term constructions prefixes
   DECLARATIVE,
   RECURSIVE,
   IMPERATIVE,
 
+  // Imperative operators
+  ITERATE,
+  ASSIGN,
+
   // Punctuation
   PUNC_DEFINE,
   PUNC_STRUCT,
-  PUNC_ASSIGN,
-  PUNC_ITERATE,
   PUNC_PL,
   PUNC_PR,
   PUNC_CL,
   PUNC_CR,
   PUNC_SL,
   PUNC_SR,
   PUNC_BAR,
@@ -109,18 +111,14 @@
   NT_FUNC_CALL, // Вызов функции
   
   NT_DECLARATIVE_EXPR, // Задание множества с помощью выражения D{x из H | A(x) }
   NT_IMPERATIVE_EXPR, // Императивное определение
   NT_RECURSIVE_FULL, // Полная рекурсия
   NT_RECURSIVE_SHORT, // Сокращенная рекурсия
 
-  NT_IMP_DECLARE, // Блок декларации
-  NT_IMP_ASSIGN, // Блок присвоения
-  NT_IMP_LOGIC, // Блок проверки
-  
   // ======= Helper tokens ========
   INTERRUPT,
   END,
 };
 
 //! RS token payload data
 class TokenData {
```

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/SDataCompact.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/SDataCompact.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Structure.hpp` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Structure.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/StructuredData.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/StructuredData.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/SyntaxTree.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/SyntaxTree.h`

 * *Files 1% similar despite different names*

```diff
@@ -228,29 +228,27 @@
       case TokenID::NOTIN:
       case TokenID::SUBSET:
       case TokenID::SUBSET_OR_EQ:
       case TokenID::NOTSUBSET:
         assert(ChildrenCount() == 2);
         return visitor.ViSetexprPredicate(*this);
 
+      case TokenID::ITERATE:
+        assert(ChildrenCount() == 2);
+        return visitor.ViIterate(*this);
+      case TokenID::ASSIGN:
+        assert(ChildrenCount() == 2);
+        return visitor.ViAssign(*this);
+
       case TokenID::NT_DECLARATIVE_EXPR:
         assert(ChildrenCount() == 3);
         return visitor.ViDeclarative(*this);
       case TokenID::NT_IMPERATIVE_EXPR:
         assert(ChildrenCount() > 1);
         return visitor.ViImperative(*this);
-      case TokenID::NT_IMP_DECLARE:
-        assert(ChildrenCount() == 2);
-        return visitor.ViImpDeclare(*this);
-      case TokenID::NT_IMP_ASSIGN:
-        assert(ChildrenCount() == 2);
-        return visitor.ViImpAssign(*this);
-      case TokenID::NT_IMP_LOGIC:
-        assert(ChildrenCount() == 1);
-        return visitor.ViImpCheck(*this);
 
       case TokenID::DECART:
         assert(ChildrenCount() > 1);
         return visitor.ViDecart(*this);
       case TokenID::BOOLEAN:
         assert(ChildrenCount() == 1);
         return visitor.ViBoolean(*this);
@@ -345,19 +343,18 @@
   bool ViNegation(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViLogicBinary(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViEquals(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViIntegerPredicate(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViSetexprPredicate(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViDeclarative(Cursor iter) { return this->BaseT().VisitDefault(iter); }
-  bool ViImperative(Cursor iter) { return this->BaseT().VisitDefault(iter); }
-  bool ViImpDeclare(Cursor iter) { return this->BaseT().VisitDefault(iter); }
-  bool ViImpAssign(Cursor iter) { return this->BaseT().VisitDefault(iter); }
-  bool ViImpCheck(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViRecursion(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViImperative(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViIterate(Cursor iter) { return this->BaseT().VisitDefault(iter); }
+  bool ViAssign(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViDecart(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViBoolean(Cursor iter) { return this->BaseT().VisitDefault(iter); }
 
   bool ViTuple(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViEnumeration(Cursor iter) { return this->BaseT().VisitDefault(iter); }
   bool ViBool(Cursor iter) { return this->BaseT().VisitDefault(iter); }
```

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/TypeAuditor.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/TypeAuditor.h`

 * *Files 0% similar despite different names*

```diff
@@ -100,19 +100,18 @@
   bool ViIntegerPredicate(Cursor iter);
   bool ViSetexprPredicate(Cursor iter);
 
   bool ViDecart(Cursor iter);
   bool ViBoolean(Cursor iter);
 
   bool ViDeclarative(Cursor iter);
-  bool ViImperative(Cursor iter);
-  bool ViImpDeclare(Cursor iter);
-  bool ViImpAssign(Cursor iter);
-  bool ViImpCheck(Cursor iter) { return VisitAllAndSetCurrent(iter, LogicT{}); }
   bool ViRecursion(Cursor iter);
+  bool ViImperative(Cursor iter);
+  bool ViIterate(Cursor iter);
+  bool ViAssign(Cursor iter);
 
   bool ViTuple(Cursor iter);
   bool ViEnumeration(Cursor iter);
   bool ViBool(Cursor iter) { return ViEnumeration(iter); }
   bool ViDebool(Cursor iter);
 
   bool ViSetexprBinary(Cursor iter);
```

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/TypeContext.hpp` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/TypeContext.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/Typification.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/Typification.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/include/ccl/rslang/ValueAuditor.h` & `pyconcept-0.1.5/ccl/rslang/include/ccl/rslang/ValueAuditor.h`

 * *Files 1% similar despite different names*

```diff
@@ -61,18 +61,17 @@
   bool ViSetexprPredicate(Cursor iter);
 
   bool ViDecart(Cursor iter);
   bool ViBoolean(Cursor iter);
 
   bool ViDeclarative(Cursor iter);
   bool ViImperative(Cursor iter);
-  bool ViImpDeclare(Cursor iter) { return AssertChildIsValue(iter, 1); }
-  bool ViImpAssign(Cursor iter) { return AssertChildIsValue(iter, 1); }
-  bool ViImpCheck(Cursor iter) { return VisitAllAndSetCurrent(iter, ValueClass::value); }
   bool ViRecursion(Cursor iter) { return AssertAllValues(iter); }
+  bool ViIterate(Cursor iter) { return AssertChildIsValue(iter, 1); }
+  bool ViAssign(Cursor iter) { return AssertChildIsValue(iter, 1); }
 
   bool ViTuple(Cursor iter) { return AssertAllValues(iter); }
   bool ViEnumeration(Cursor iter) { return AssertAllValues(iter); }
   bool ViBool(Cursor iter) { return AssertChildIsValue(iter, 0); }
   bool ViDebool(Cursor iter) { return AssertChildIsValue(iter, 0); }
 
   bool ViSetexprBinary(Cursor iter);
```

### Comparing `pyconcept-0.1.4/ccl/rslang/src/ASTInterpreter.cpp` & `pyconcept-0.1.5/ccl/rslang/src/ASTInterpreter.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     : parent{ parent }, imperative{ imperative } {}
 
 public:
   StructuredData value{ Factory::EmptySet() };
   
 private:
   struct BlockMeta {
-    TokenID type{ TokenID::NT_IMP_LOGIC };
+    TokenID rootID{};
     uint32_t arg{};
     std::optional<object::StructuredData> domain{};
   };
 
   ASTInterpreter& parent;
   const Cursor imperative;
 
@@ -40,58 +40,58 @@
   bool incrementIter{};
 
 public:
   [[nodiscard]] bool Evaluate() {
     CreateBlockMetadata();
     for (current = 0; ; ++current) {
       incrementIter = false;
-      if (IsDone()) {
+      if (HasReachedEnd()) {
         if (!SaveElement()) {
           return false;
         }
-      } else {
-        if (!ProcessBlock()) {
-          return false;
-        }
+      } else if (!ProcessBlock()) {
+        return false;
       }
       if (incrementIter && !PrepareNextIteration()) {
         return true;
       }
       if (++parent.iterationCounter > MAX_ITERATIONS) {
-        parent.OnError(ValueEID::iterationsLimit, imperative->pos.start,
-                       std::to_string(MAX_ITERATIONS));
+        parent.OnError(
+          ValueEID::iterationsLimit,
+          imperative->pos.start,
+          std::to_string(MAX_ITERATIONS)
+        );
         return false;
       }
     }
   }
 
 private:
   void CreateBlockMetadata() {
     auto iter = imperative;
     iter.MoveToChild(1);
     do {
       BlockMeta newBlock{};
-      newBlock.type = iter->id;
-      switch (newBlock.type) {
-      case TokenID::NT_IMP_DECLARE: {
+      newBlock.rootID = iter->id;
+      switch (newBlock.rootID) {
+      case TokenID::ITERATE: {
         newBlock.arg = *begin(parent.nodeVars[iter.Child(0).get()]);
         break;
       }
-      case TokenID::NT_IMP_ASSIGN: {
+      case TokenID::ASSIGN: {
         newBlock.arg = *begin(parent.nodeVars[iter.Child(0).get()]);
         break;
       }
-      default:
-      case TokenID::NT_IMP_LOGIC: break;
+      default: break;
       }
       metaData.emplace_back(std::move(newBlock));
     } while (iter.MoveToNextSibling());
   }
 
-  [[nodiscard]] bool IsDone() const noexcept {
+  [[nodiscard]] bool HasReachedEnd() const noexcept {
     return current + 1 >= imperative.ChildrenCount();
   }
 
   [[nodiscard]] bool SaveElement() {
     auto element = parent.EvaluateChild(imperative, 0);
     if (!element.has_value()) {
       return false;
@@ -103,50 +103,46 @@
   }
 
   [[nodiscard]] bool ProcessBlock() {
     auto child = imperative;
     child.MoveToChild(static_cast<Index>(current + 1));
     auto& meta = metaData.at(static_cast<size_t>(current));
 
-    switch (meta.type) {
-    default:
-    case TokenID::NT_IMP_LOGIC: {
-      const auto predicatValue = parent.EvaluateChild(child, 0);
-      if (!predicatValue.has_value()) {
+    switch (meta.rootID) {
+    default: {
+      const auto predicatValue = parent.EvaluateChild(imperative, static_cast<Index>(current + 1));
+      if (!predicatValue.has_value() || !std::holds_alternative<bool>(predicatValue.value())) {
         return false;
-      } else {
-        incrementIter = !std::get<bool>(predicatValue.value());
-        return true;
       }
+      incrementIter = !std::get<bool>(predicatValue.value());
+      return true;
     }
-    case TokenID::NT_IMP_DECLARE: {
+    case TokenID::ITERATE: {
       const auto domain = parent.ExtractDomain(child);
       if (!domain.has_value()) {
         return false;
-      } else if (domain->B().IsEmpty()) {
+      } 
+      if (domain->B().IsEmpty()) {
         incrementIter = true;
-        return true;
       } else {
         meta.domain = domain.value();
-
         auto element = std::begin(meta.domain->B());
         parent.idsData[meta.arg] = *element;
         blockStack.emplace(current);
         iterStack.emplace(element);
-        return true;
       }
+      return true;
     }
-    case TokenID::NT_IMP_ASSIGN: {
+    case TokenID::ASSIGN: {
       const auto localValue = parent.ExtractDomain(child);
       if (!localValue.has_value()) {
         return false;
-      } else {
-        parent.idsData[meta.arg] = localValue.value();
-        return true;
       }
+      parent.idsData[meta.arg] = localValue.value();
+      return true;
     }
     }
   }
 
   [[nodiscard]] bool PrepareNextIteration() {
     while (!empty(blockStack)) {
       object::SDIterator element = iterStack.top();
@@ -271,15 +267,19 @@
 bool ASTInterpreter::ViCard(Cursor iter) {
   const auto base = EvaluateChild(iter, 0);
   if (!base.has_value()) {
     return false;
   }
   const auto size = std::get<StructuredData>(base.value()).B().Cardinality();
   if (size == StructuredData::SET_INFINITY) {
-    OnError(ValueEID::typedOverflow, iter->pos.start, std::to_string(StructuredData::SET_INFINITY));
+    OnError(
+      ValueEID::typedOverflow,
+      iter->pos.start,
+      std::to_string(StructuredData::SET_INFINITY)
+    );
     return false;
   }
   return SetCurrent(Factory::Val(size));
 }
 
 bool ASTInterpreter::ViQuantifier(Cursor iter) {
   const auto domain = ExtractDomain(iter);
@@ -287,21 +287,27 @@
     return false;
   }
 
   const auto varID = *begin(nodeVars[iter.Child(0).get()]);
   const auto isUniversal = iter->id == TokenID::FORALL;
   for (const auto& child : domain->B()) {
     if (++iterationCounter > MAX_ITERATIONS) {
-      OnError(ValueEID::iterationsLimit, iter->pos.start, std::to_string(MAX_ITERATIONS));
+      OnError(
+        ValueEID::iterationsLimit,
+        iter->pos.start,
+        std::to_string(MAX_ITERATIONS)
+      );
       return false;
     }
     idsData[varID] = child;
-    if (const auto iterationValue = EvaluateChild(iter, 2); !iterationValue.has_value()) {
+    const auto iterationValue = EvaluateChild(iter, 2);
+    if (!iterationValue.has_value()) {
       return false;
-    } else if (std::get<bool>(iterationValue.value()) != isUniversal) {
+    }
+    if (std::get<bool>(iterationValue.value()) != isUniversal) {
       return SetCurrent(!isUniversal);
     }
   }
   return SetCurrent(isUniversal);
 }
 
 std::optional<StructuredData> ASTInterpreter::ExtractDomain(Cursor iter) {
@@ -341,16 +347,15 @@
     case TokenID::OR: curValue = op1 || op2;  return true;
     case TokenID::IMPLICATION: curValue = !op1 || op2;  return true;
     case TokenID::EQUIVALENT: curValue = op1 == op2; return true;
   }
 }
 
 bool ASTInterpreter::TryEvaluateFromFirstArg(TokenID operation, bool firstArgValue) noexcept {
-  if ((operation == TokenID::AND && !firstArgValue) ||
-    (operation == TokenID::OR && firstArgValue)) {
+  if ((operation == TokenID::AND && !firstArgValue) || (operation == TokenID::OR && firstArgValue)) {
     return SetCurrent(firstArgValue);
   } else if (operation == TokenID::IMPLICATION && !firstArgValue) {
     return SetCurrent(!firstArgValue);
   } else {
     return false;
   }
 }
@@ -392,15 +397,19 @@
   if (!setDomain.has_value()) {
     return false;
   }
   const auto varID = *begin(nodeVars[iter.Child(0).get()]);
   auto result = Factory::EmptySet();
   for (const auto& child : setDomain->B()) {
     if (++iterationCounter > MAX_ITERATIONS) {
-      OnError(ValueEID::iterationsLimit, iter->pos.start, std::to_string(MAX_ITERATIONS));
+      OnError(
+        ValueEID::iterationsLimit,
+        iter->pos.start,
+        std::to_string(MAX_ITERATIONS)
+      );
       return false;
     }
     idsData[varID] = child;
     const auto predicatValue = EvaluateChild(iter, 2);
     if (!predicatValue.has_value()) {
       return false;
     }
@@ -424,15 +433,19 @@
   if (!initial.has_value()) {
     return false;
   }
   const auto varID = *begin(nodeVars[iter.Child(0).get()]);
   StructuredData current = initial.value();
   do {
     if (++iterationCounter > MAX_ITERATIONS) {
-      OnError(ValueEID::iterationsLimit, iter->pos.start, std::to_string(MAX_ITERATIONS));
+      OnError(
+        ValueEID::iterationsLimit,
+        iter->pos.start,
+        std::to_string(MAX_ITERATIONS)
+      );
       return false;
     }
 
     idsData[varID] = current;
     if (iter->id == TokenID::NT_RECURSIVE_FULL) {
       const auto predicat = EvaluateChild(iter, 2);
       if (!predicat.has_value()) {
@@ -450,24 +463,29 @@
   } while (idsData[varID] != current);
   return SetCurrent(std::move(current));
 }
 
 bool ASTInterpreter::ViDecart(Cursor iter) {
   std::vector<StructuredData> args{};
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
-    if (const auto childValue = EvaluateChild(iter, child); !childValue.has_value()) {
+    const auto childValue = EvaluateChild(iter, child);
+    if (!childValue.has_value()) {
       return false;
-    } else {
-      args.emplace_back(std::get<StructuredData>(childValue.value()));
-    }
+    } 
+     args.emplace_back(std::get<StructuredData>(childValue.value()));
   }
 
   curValue = Factory::Decartian(args);
-  if (std::get<StructuredData>(curValue).B().Cardinality() == StructuredData::SET_INFINITY) {
-    OnError(ValueEID::typedOverflow, iter->pos.start, std::to_string(StructuredData::SET_INFINITY));
+  const auto cardinality = std::get<StructuredData>(curValue).B().Cardinality();
+  if (cardinality == StructuredData::SET_INFINITY) {
+    OnError(
+      ValueEID::typedOverflow,
+      iter->pos.start,
+      std::to_string(StructuredData::SET_INFINITY)
+    );
     return false;
   }
   return true;
 }
 
 bool ASTInterpreter::ViBoolean(Cursor iter) {
   const auto childValue = EvaluateChild(iter, 0);
@@ -623,15 +641,18 @@
 bool ASTInterpreter::ViDebool(Cursor iter) {
   const auto childValue = EvaluateChild(iter, 0);
   if (!childValue.has_value()) {
     return false;
   }
   const auto value = std::get<StructuredData>(childValue.value());
   if (value.B().Cardinality() != 1) {
-    OnError(ValueEID::invalidDebool, iter->pos.start);
+    OnError(
+      ValueEID::invalidDebool,
+      iter->pos.start
+    );
     return false;
   }
   return SetCurrent(std::get<StructuredData>(childValue.value()).B().Debool());
 }
 
 std::optional<ExpressionValue> ASTInterpreter::EvaluateChild(Cursor iter, const Index index) {
   assert(iter.ChildrenCount() > index);
```

### Comparing `pyconcept-0.1.4/ccl/rslang/src/ASTNormalizer.cpp` & `pyconcept-0.1.5/ccl/rslang/src/ASTNormalizer.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -11,19 +11,24 @@
   default: break;
   case TokenID::FORALL:
   case TokenID::EXISTS: {
     Quantifier(root);
     break;
   }
   case TokenID::NT_RECURSIVE_FULL:
-  case TokenID::NT_RECURSIVE_SHORT:
+  case TokenID::NT_RECURSIVE_SHORT: {
+    Recursion(root);
+    break;
+  }
   case TokenID::NT_DECLARATIVE_EXPR: {
-    if (root(0).token.id == TokenID::NT_TUPLE_DECL) {
-      TupleDeclaration(root);
-    }
+    Declarative(root);
+    break;
+  }
+  case TokenID::NT_IMPERATIVE_EXPR: {
+    Imperative(root);
     break;
   }
   case TokenID::NT_FUNC_CALL: {
     Function(root);
     break;
   }
   }
@@ -38,14 +43,54 @@
   if (declToken == TokenID::NT_TUPLE_DECL) {
     TupleDeclaration(quant(0), quant(2));
   } else if (declToken == TokenID::NT_ENUM_DECL) {
     EnumDeclaration(quant);
   }
 }
 
+void Normalizer::Declarative(SyntaxTree::Node& root) {
+  if (root(0).token.id != TokenID::NT_TUPLE_DECL) {
+    return;
+  }
+  const auto newName = ProcessTupleDeclaration(root(0));
+  SubstituteTupleVariables(root(1), newName);
+  SubstituteTupleVariables(root(2), newName);
+}
+
+void Normalizer::Recursion(SyntaxTree::Node& root) {
+  if (root(0).token.id != TokenID::NT_TUPLE_DECL) {
+    return;
+  }
+  const auto newName = ProcessTupleDeclaration(root(0));
+  SubstituteTupleVariables(root(2), newName);
+  if (root.token.id == TokenID::NT_RECURSIVE_FULL) {
+    SubstituteTupleVariables(root(3), newName);
+  }
+}
+
+void Normalizer::Imperative(SyntaxTree::Node& root) {
+  for (Index child = 1; child < root.ChildrenCount(); ++child) {
+    const auto childID = root(child).token.id;
+    if (childID != TokenID::ITERATE && childID != TokenID::ASSIGN) {
+      continue;
+    }
+    auto& declRoot = root(child);
+    if (declRoot(0).token.id != TokenID::NT_TUPLE_DECL) {
+      continue;
+    }
+    const auto newName = ProcessTupleDeclaration(declRoot(0));
+    for (Index child2 = 0; child2 < root.ChildrenCount(); ++child2) {
+      if (child2 != child) {
+        SubstituteTupleVariables(root(child2), newName);
+      }
+    }
+    SubstituteTupleVariables(root, newName);
+  }
+}
+
 void Normalizer::EnumDeclaration(SyntaxTree::Node& quant) {
   auto newQuant = std::make_unique<SyntaxTree::Node>(quant.token);
   newQuant->AddChildCopy(quant(0));
   newQuant->AddChildCopy(quant(1));
   newQuant->AdoptChild(quant.ExtractChild(2));
 
   if (quant(0).ChildrenCount() > 2) {
@@ -57,95 +102,78 @@
   quant(0) = quant(0)(0);
 }
 
 void Normalizer::TupleDeclaration(
   SyntaxTree::Node& declaration,
   SyntaxTree::Node& predicate
 ) {
-  const auto newName = CreateTupleName(declaration);
-  declaration.RemoveAll();
-  declaration.token.data = TokenData{ newName };
-  declaration.token.id = TokenID::ID_LOCAL;
+  const auto newName = ProcessTupleDeclaration(declaration);
   SubstituteTupleVariables(predicate, newName);
 }
 
-void Normalizer::TupleDeclaration(SyntaxTree::Node& target) {
-  const auto token = target.token.id;
-  auto newName = CreateTupleName(target(0));
-
-  target(0).RemoveAll();
-  target(0).token.id = TokenID::ID_LOCAL;
-  target(0).token.data = TokenData{ newName };
-
-  if (token == TokenID::NT_DECLARATIVE_EXPR) {
-    SubstituteTupleVariables(target(1), newName);
-  }
-  SubstituteTupleVariables(target(2), newName);
-  if (token == TokenID::NT_RECURSIVE_FULL) {
-    SubstituteTupleVariables(target(3), newName);
-  }
-}
-
-std::string Normalizer::CreateTupleName(const SyntaxTree::Node& root) {
-  tuples.clear();
+std::string Normalizer::ProcessTupleDeclaration(SyntaxTree::Node& root) {
+  tupleSubstitutes.clear();
   std::string newName{ '@' };
 
   std::stack<const SyntaxTree::Node*> nodeStack{};
   std::stack<std::vector<Index>> pathStack{};
   nodeStack.push(&root);
   pathStack.emplace();
   while (!std::empty(nodeStack)) {
     auto curPath = pathStack.top();
     pathStack.pop();
     const auto* curNode = nodeStack.top();
     nodeStack.pop();
     if (curNode->token.id == TokenID::ID_LOCAL) {
       const auto& name = curNode->token.data.ToText();
       newName += name;
-      tuples.insert({ name, curPath });
+      tupleSubstitutes.insert({ name, curPath });
     } else if (const auto childCount = curNode->ChildrenCount(); childCount > 0) {
       for (auto child = static_cast<Index>(childCount - 1); child >= 0; --child) {
         curPath.emplace_back(static_cast<Index>(child + 1));
         pathStack.push(curPath);
         nodeStack.push(&curNode->At(child));
         curPath.pop_back();
       }
     }
   }
+  root.RemoveAll();
+  root.token.data = TokenData{ newName };
+  root.token.id = TokenID::ID_LOCAL;
   return newName;
 }
 
 void Normalizer::SubstituteTupleVariables(SyntaxTree::Node& target, const std::string& newName) {
   for (Index child = 0; child < target.ChildrenCount(); ++child) {
-    if (target(child).token.id == TokenID::ID_LOCAL) {
+    if (target(child).token.id != TokenID::ID_LOCAL) {
+      SubstituteTupleVariables(target(child), newName);
+    } else {
       const auto& localName = target(child).token.data.ToText();
-      if (tuples.contains(localName)) {
-        const auto& indexes = tuples.at(localName);
+      if (tupleSubstitutes.contains(localName)) {
+        const auto& indexes = tupleSubstitutes.at(localName);
         target(child).token.data = TokenData{ newName };
         for (const auto prIndex : indexes) {
           target.ExtendChild(child, TokenID::SMALLPR);
           target(child).token.pos = target(child)(0).token.pos;
           target(child).token.data = TokenData{ std::vector<Index>{ prIndex } };
         }
       }
-    } else {
-      SubstituteTupleVariables(target(child), newName);
     }
   }
 }
 
 void Normalizer::Function(SyntaxTree::Node& func) {
-  nodes.clear();
+  nodeSubstitutes.clear();
   nameSubstitutes.clear();
   
   const auto* funcTree = termFuncs(func(0).token.data.ToText());
   if (funcTree != nullptr) {
     const auto argNames = ArgNames(funcTree->root->At(1).At(0));
     for (Index child = 1; child < func.ChildrenCount(); ++child) {
-      nodes.insert({ argNames.at(static_cast<size_t>(child) - 1), &func(child) });
+      nodeSubstitutes.insert({ argNames.at(static_cast<size_t>(child) - 1), &func(child) });
     }
     SyntaxTree newTree = *funcTree;
     SubstituteArgs(newTree.root->At(1).At(1), func.token.pos);
     func = newTree.root->At(1).At(1);
     Normalize(func);
   }
 }
@@ -163,16 +191,16 @@
   target.token.pos = pos;
   if (target.token.id != TokenID::ID_LOCAL) {
     for (Index child = 0; child < target.ChildrenCount(); ++child) {
       SubstituteArgs(target(child), pos);
     }
   } else {
     const auto& localName = target.token.ToString();
-    if (nodes.contains(localName)) {
-      target = *nodes.at(localName);
+    if (nodeSubstitutes.contains(localName)) {
+      target = *nodeSubstitutes.at(localName);
     } else {
       const auto& oldName = target.token.ToString();
       std::string newName{};
       const auto iter = nameSubstitutes.find(oldName);
       if (iter == std::end(nameSubstitutes)) {
         ++localVarBase;
         newName = R"(__var)" + std::to_string(localVarBase);
```

### Comparing `pyconcept-0.1.4/ccl/rslang/src/AsciiLexer.cpp` & `pyconcept-0.1.5/ccl/rslang/src/AsciiLexer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/Auditor.cpp` & `pyconcept-0.1.5/ccl/rslang/src/Auditor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/ErrorLogger.cpp` & `pyconcept-0.1.5/ccl/rslang/src/ErrorLogger.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/GeneratorImplAST.cpp` & `pyconcept-0.1.5/ccl/rslang/src/GeneratorImplAST.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -143,21 +143,14 @@
   rsText += ' ';
   rsText += iter->ToString(syntax);
   rsText += ' ';
   OutputChild(iter, 1, needRightBrackets);
   return true;
 }
 
-bool GeneratorImplAST::ViEquals(Cursor iter) {
-  OutputChild(iter, 0);
-  rsText += iter->ToString(syntax);
-  OutputChild(iter, 1);
-  return true;
-}
-
 bool GeneratorImplAST::ViDeclarative(Cursor iter) {
   rsText += Token::Str(TokenID::DECLARATIVE, syntax);
   rsText += '{';
   OutputChild(iter, 0);
   rsText += Token::Str(TokenID::IN, syntax);
   OutputChild(iter, 1);
   rsText += R"( | )";
@@ -177,38 +170,19 @@
     }
     OutputChild(iter, child);
   }
   rsText += '}';
   return true;
 }
 
-bool GeneratorImplAST::ViImpDeclare(Cursor iter) {
-  OutputChild(iter, 0);
-  rsText += Token::Str(TokenID::PUNC_ITERATE, syntax);
-  OutputChild(iter, 1);
-  return true;
-}
-
-bool GeneratorImplAST::ViImpAssign(Cursor iter) {
-  OutputChild(iter, 0);
-  rsText += Token::Str(TokenID::PUNC_ASSIGN, syntax);
-  OutputChild(iter, 1);
-  return true;
-}
-
-bool GeneratorImplAST::ViImpCheck(Cursor iter) {
-  OutputChild(iter, 0);
-  return true;
-}
-
 bool GeneratorImplAST::ViRecursion(Cursor iter) {
   rsText += Token::Str(TokenID::RECURSIVE, syntax);
   rsText += '{';
   OutputChild(iter, 0);
-  rsText += Token::Str(TokenID::PUNC_ASSIGN);
+  rsText += Token::Str(TokenID::ASSIGN);
   OutputChild(iter, 1);
   rsText += R"( | )";
   OutputChild(iter, 2);
   if (iter->id == TokenID::NT_RECURSIVE_FULL) {
     rsText += R"( | )";
     OutputChild(iter, 3);
   }
@@ -248,23 +222,32 @@
   }
   VisitChild(iter, index);
   if (addBrackets) {
     rsText += ')';
   }
 }
 
-void GeneratorImplAST::EnumChildren(const Cursor& iter, const std::string& separator) {
+bool GeneratorImplAST::OutputBinary(const Cursor& iter) {
+  OutputChild(iter, 0);
+  rsText += iter->ToString(syntax);
+  OutputChild(iter, 1);
+  return true;
+}
+
+bool GeneratorImplAST::EnumChildren(const Cursor& iter, const std::string& separator) {
   for (Index child = 0; child < iter.ChildrenCount(); ++child) {
     if (child > 0) {
       rsText += separator;
     }
     OutputChild(iter, child);
   }
+  return true;
 }
 
-void GeneratorImplAST::EnumChildren(const Cursor& iter, const char left, const char right, const std::string& separator) {
+bool GeneratorImplAST::EnumChildren(const Cursor& iter, const char left, const char right, const std::string& separator) {
   rsText += left;
   EnumChildren(iter, separator);
   rsText += right;
+  return true;
 }
 
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.4/ccl/rslang/src/Interpreter.cpp` & `pyconcept-0.1.5/ccl/rslang/src/Interpreter.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/Literals.cpp` & `pyconcept-0.1.5/ccl/rslang/src/Literals.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/MathLexer.cpp` & `pyconcept-0.1.5/ccl/rslang/src/MathLexer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/NameCollector.cpp` & `pyconcept-0.1.5/ccl/rslang/src/NameCollector.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 }
 
 bool ASTInterpreter::NameCollector::ViGlobalDeclaration(Cursor iter) {
   if (iter->id == TokenID::PUNC_STRUCT) {
     return false; // TODO: specify error
   }
   switch (iter(0).id) {
-  default:
-  case TokenID::ID_FUNCTION:
-  case TokenID::ID_PREDICATE: {
-    return false; // TODO: specify error
-  }
-  case TokenID::ID_GLOBAL: {
-    return iter.ChildrenCount() == 2 && VisitChild(iter, 1);
-  }
+    default:
+    case TokenID::ID_FUNCTION:
+    case TokenID::ID_PREDICATE: {
+      return false; // TODO: specify error
+    }
+    case TokenID::ID_GLOBAL: {
+      return iter.ChildrenCount() == 2 && VisitChild(iter, 1);
+    }
   }
 }
 
 bool ASTInterpreter::NameCollector::ViGlobal(Cursor iter) {
   const auto& idName = iter->data.ToText();
   if (parent.idsBase.contains(idName)) {
     parent.nodeVars[iter.get()] = { parent.idsBase[idName] };
@@ -89,22 +89,21 @@
   }
 
   auto& vars = parent.nodeVars[iter.get()];
   auto child = iter;
   child.MoveToChild(1);
   do {
     switch (child->id) {
-    case TokenID::NT_IMP_ASSIGN:
-    case TokenID::NT_IMP_DECLARE: {
-      const auto varID = *begin(parent.nodeVars[iter.Child(0).get()]);
-      vars.erase(std::remove(begin(vars), end(vars), varID), end(vars));
-      break;
-    }
-    default:
-    case TokenID::NT_IMP_LOGIC: break;
+      case TokenID::ITERATE:
+      case TokenID::ASSIGN: {
+        const auto varID = *begin(parent.nodeVars[iter.Child(0).get()]);
+        vars.erase(std::remove(begin(vars), end(vars), varID), end(vars));
+        break;
+      }
+      default: break;
     }
   } while (child.MoveToNextSibling());
   return true;
 }
 
 } // namespace ccl::rslang
```

### Comparing `pyconcept-0.1.4/ccl/rslang/src/Parser.cpp` & `pyconcept-0.1.5/ccl/rslang/src/Parser.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/RSExpr.cpp` & `pyconcept-0.1.5/ccl/rslang/src/RSExpr.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/RSGenerator.cpp` & `pyconcept-0.1.5/ccl/rslang/src/RSGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/RSParser.cpp` & `pyconcept-0.1.5/ccl/rslang/src/RSParser.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 #ifdef _MSC_VER
   #pragma warning( push )
   #pragma warning( disable : 26418 26415 26440 )
 #endif
 
 #include <optional>
+#include <unordered_map>
 
 namespace ccl::rslang::detail {
 
 RSParser::RSParser(std::optional<ErrorReporter> reporter)
   : state{ reporter }, impl{ std::make_unique<RSParserImpl>(&state) } {}
 
 RSParser::~RSParser() = default;
@@ -182,14 +183,34 @@
   );
   result->children.emplace_back(declaration);
   result->children.emplace_back(domain);
   result->children.emplace_back(predicate);
   return result;
 }
 
+RawNode TupleDeclaration(ParserState* state, RawNode tuple) {
+  // TODO: check tuple contains only local variables, ParseEID::expectedLocal
+  std::vector<Node*> stack{ tuple.get()};
+  while (!stack.empty()) {
+    auto node = stack.back();
+    const auto id = node->token.id;
+    stack.pop_back();
+    if (id == TokenID::NT_TUPLE) {
+      node->token.id = TokenID::NT_TUPLE_DECL;
+    } else if (id != TokenID::ID_LOCAL) {
+      state->OnError(ParseEID::expectedLocal, node->token.pos.start);
+      return nullptr;
+    }
+    for (const auto& child: node->children) {
+      stack.emplace_back(child.get());
+    }
+  }
+  return tuple;
+}
+
 RawNode FullRecursion(
   RawNode rec,
   RawNode declaration, 
   RawNode domain,
   RawNode condition,
   RawNode iteration,
   RawNode rc
@@ -228,45 +249,73 @@
     StrRange{ imp->token.pos.start, rc->token.pos.finish }
   );
   result->children.emplace_back(value);
   result->children.insert(end(result->children), begin(actions->children), end(actions->children));
   return result;
 }
 
+bool SemanticCheck(ParserState* state, RawNode root) {
+  std::vector<Node*> stack{ root.get() };
+  std::vector<Node*> parents{ nullptr };
+  while (!stack.empty()) {
+    const auto node = stack.back();
+    stack.pop_back();
+    const auto parent = parents.back();
+    parents.pop_back();
+
+    const auto id = node->token.id;
+    if (id == TokenID::ASSIGN || id == TokenID::ITERATE) {
+      if (parent == nullptr || parent->token.id != TokenID::NT_IMPERATIVE_EXPR) {
+        state->OnError(ParseEID::invalidImperative, node->token.pos.start);
+        return false;
+      }
+    }
+    for (const auto& child: node->children) {
+      stack.emplace_back(child.get());
+      parents.emplace_back(node);
+    }
+  }
+  return true;
+}
+
 SyntaxTree::RawNode CreateNodeRecursive(Node& astNode) {
   if (astNode.token.id == TokenID::PUNC_PL) {
     return CreateNodeRecursive(*astNode.children.at(0));
   } else {
     auto result = std::make_unique<SyntaxTree::Node>(std::move(astNode.token));
     for (const auto& child : astNode.children) {
       result->AdoptChild(CreateNodeRecursive(*child));
     }
     return result;
   }
 }
 
-void ParserState::CreateSyntaxTree(RawNode root) {
+bool ParserState::CreateSyntaxTree(RawNode root) {
+  if (!SemanticCheck(this, root)) {
+    return false;
+  }
   parsedTree = std::make_unique<SyntaxTree>(CreateNodeRecursive(*root));
+  return true;
 }
 
-void ParserState::FinalizeExpression(RawNode expr) {
-  CreateSyntaxTree(expr);
+bool ParserState::FinalizeExpression(RawNode expr) {
+  return CreateSyntaxTree(expr);
 }
 
-void ParserState::FinalizeCstEmpty(RawNode cst, RawNode mode) {
+bool ParserState::FinalizeCstEmpty(RawNode cst, RawNode mode) {
   mode->token.pos = StrRange{ cst->token.pos.start, mode->token.pos.finish };
   mode->children.emplace_back(cst);
-  CreateSyntaxTree(mode);
+  return CreateSyntaxTree(mode);
 }
 
-void ParserState::FinalizeCstExpression(RawNode cst, RawNode mode, RawNode data) {
+bool ParserState::FinalizeCstExpression(RawNode cst, RawNode mode, RawNode data) {
   mode->token.pos = StrRange{ cst->token.pos.start, data->token.pos.finish };
   mode->children.emplace_back(cst);
   mode->children.emplace_back(data);
-  CreateSyntaxTree(mode);
+  return CreateSyntaxTree(mode);
 }
 
 } // namespace ccl::rslang::detail
 
 #ifdef _MSC_VER
   #pragma warning( pop )
 #endif
```

### Comparing `pyconcept-0.1.4/ccl/rslang/src/RSParserImpl.cpp` & `pyconcept-0.1.5/ccl/rslang/src/RSParserImpl.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -581,381 +581,357 @@
 #if YY_EXCEPTIONS
       try
 #endif // YY_EXCEPTIONS
         {
           switch (yyn)
             {
   case 3: // expression: logic_or_setexpr
-#line 263 "RSParserImpl.y"
-                                            { state->FinalizeExpression(yystack_[0].value); }
+#line 271 "RSParserImpl.y"
+                                            { if(!state->FinalizeExpression(yystack_[0].value)) YYABORT; }
 #line 591 "RSParserImpl.cpp"
     break;
 
   case 4: // expression: function_definition
-#line 264 "RSParserImpl.y"
-                                            { state->FinalizeExpression(yystack_[0].value); }
+#line 272 "RSParserImpl.y"
+                                            { if(!state->FinalizeExpression(yystack_[0].value)) YYABORT; }
 #line 597 "RSParserImpl.cpp"
     break;
 
   case 5: // global_declaration: GLOBAL DEFINE
-#line 268 "RSParserImpl.y"
-                                            { state->FinalizeCstEmpty(yystack_[1].value, yystack_[0].value); }
+#line 276 "RSParserImpl.y"
+                                            { if(!state->FinalizeCstEmpty(yystack_[1].value, yystack_[0].value)) YYABORT; }
 #line 603 "RSParserImpl.cpp"
     break;
 
   case 6: // global_declaration: GLOBAL STRUCT setexpr
-#line 269 "RSParserImpl.y"
-                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 277 "RSParserImpl.y"
+                                            { if(!state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value)) YYABORT; }
 #line 609 "RSParserImpl.cpp"
     break;
 
   case 7: // global_declaration: GLOBAL DEFINE logic_or_setexpr
-#line 270 "RSParserImpl.y"
-                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 278 "RSParserImpl.y"
+                                            { if(!state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value)) YYABORT; }
 #line 615 "RSParserImpl.cpp"
     break;
 
   case 8: // global_declaration: FUNCTION DEFINE function_definition
-#line 271 "RSParserImpl.y"
-                                            { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 279 "RSParserImpl.y"
+                                            { if(!state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value)) YYABORT; }
 #line 621 "RSParserImpl.cpp"
     break;
 
   case 9: // global_declaration: PREDICATE DEFINE function_definition
-#line 272 "RSParserImpl.y"
-                                                { state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+#line 280 "RSParserImpl.y"
+                                                { if(!state->FinalizeCstExpression(yystack_[2].value, yystack_[1].value, yystack_[0].value)) YYABORT; }
 #line 627 "RSParserImpl.cpp"
     break;
 
   case 12: // function_definition: LS arguments RS logic_or_setexpr
-#line 281 "RSParserImpl.y"
+#line 289 "RSParserImpl.y"
                                             { yylhs.value = FunctionDeclaration(yystack_[3].value, yystack_[2].value, yystack_[0].value); }
 #line 633 "RSParserImpl.cpp"
     break;
 
   case 13: // function_definition: LS error
-#line 282 "RSParserImpl.y"
+#line 290 "RSParserImpl.y"
                                             { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
 #line 639 "RSParserImpl.cpp"
     break;
 
   case 14: // arguments: declaration
-#line 287 "RSParserImpl.y"
+#line 295 "RSParserImpl.y"
                                             { yylhs.value = AddNode(TokenID::NT_ARGUMENTS, yystack_[0].value); }
 #line 645 "RSParserImpl.cpp"
     break;
 
   case 15: // arguments: arguments COMMA declaration
-#line 288 "RSParserImpl.y"
+#line 296 "RSParserImpl.y"
                                             { yylhs.value = Enumeration(TokenID::NT_ARGUMENTS, yystack_[2].value, yystack_[0].value); }
 #line 651 "RSParserImpl.cpp"
     break;
 
   case 16: // arguments: arguments COMMA error
-#line 289 "RSParserImpl.y"
+#line 297 "RSParserImpl.y"
                                             { state->OnError(ParseEID::expectedLocal); YYABORT; }
 #line 657 "RSParserImpl.cpp"
     break;
 
   case 17: // declaration: LOCAL IN setexpr
-#line 292 "RSParserImpl.y"
+#line 300 "RSParserImpl.y"
                                             { yylhs.value = AddNode(TokenID::NT_ARG_DECL, yystack_[2].value, yystack_[0].value); }
 #line 663 "RSParserImpl.cpp"
     break;
 
   case 18: // declaration: LOCAL error
-#line 293 "RSParserImpl.y"
+#line 301 "RSParserImpl.y"
                                             { state->OnError(ParseEID::expectedDeclaration); YYABORT; }
 #line 669 "RSParserImpl.cpp"
     break;
 
-  case 20: // variable: LP var_enum RPE
-#line 298 "RSParserImpl.y"
-                                            { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE_DECL, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+  case 20: // variable: tuple
+#line 306 "RSParserImpl.y"
+                                            { yylhs.value = TupleDeclaration(state, yystack_[0].value); if (!yylhs.value) YYABORT; }
 #line 675 "RSParserImpl.cpp"
     break;
 
-  case 21: // var_enum: var_all COMMA var_all
-#line 301 "RSParserImpl.y"
-                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
+  case 22: // variable_pack: variable_pack COMMA variable_pack
+#line 310 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::NT_ENUM_DECL, yystack_[2].value, yystack_[0].value); }
 #line 681 "RSParserImpl.cpp"
     break;
 
-  case 22: // var_enum: var_all COMMA error
-#line 302 "RSParserImpl.y"
+  case 23: // variable_pack: variable_pack COMMA error
+#line 311 "RSParserImpl.y"
                                             { state->OnError(ParseEID::expectedLocal); YYABORT; }
 #line 687 "RSParserImpl.cpp"
     break;
 
-  case 30: // logic_par: LP logic_binary RPE
-#line 320 "RSParserImpl.y"
+  case 32: // logic_par: LP logic_binary RPE
+#line 330 "RSParserImpl.y"
                                             { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 693 "RSParserImpl.cpp"
     break;
 
-  case 31: // logic_par: LP logic_predicates RPE
-#line 321 "RSParserImpl.y"
+  case 33: // logic_par: LP logic_predicates RPE
+#line 331 "RSParserImpl.y"
                                             { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 699 "RSParserImpl.cpp"
     break;
 
-  case 32: // logic_predicates: setexpr binary_predicate setexpr
-#line 325 "RSParserImpl.y"
+  case 34: // logic_predicates: setexpr binary_predicate setexpr
+#line 335 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 705 "RSParserImpl.cpp"
     break;
 
-  case 44: // logic_unary: NOT logic_no_binary
-#line 342 "RSParserImpl.y"
-                                            { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value);}
+  case 35: // logic_predicates: variable ITERATE setexpr
+#line 336 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 711 "RSParserImpl.cpp"
     break;
 
-  case 45: // logic_unary: quantifier quant_var IN setexpr logic_no_binary
-#line 343 "RSParserImpl.y"
-                                                      { yylhs.value = Quantifier(yystack_[4].value, yystack_[3].value, yystack_[1].value, yystack_[0].value);}
+  case 36: // logic_predicates: variable ASSIGN setexpr
+#line 337 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 717 "RSParserImpl.cpp"
     break;
 
-  case 46: // logic_unary: quantifier error
-#line 344 "RSParserImpl.y"
-                                            { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
+  case 48: // logic_unary: NOT logic_no_binary
+#line 354 "RSParserImpl.y"
+                                            { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value);}
 #line 723 "RSParserImpl.cpp"
     break;
 
-  case 47: // logic_unary: PREDICATE LS setexpr_enum RS
-#line 345 "RSParserImpl.y"
-                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+  case 49: // logic_unary: quantifier variable_pack IN setexpr logic_no_binary
+#line 355 "RSParserImpl.y"
+                                                          { yylhs.value = Quantifier(yystack_[4].value, yystack_[3].value, yystack_[1].value, yystack_[0].value);}
 #line 729 "RSParserImpl.cpp"
     break;
 
-  case 55: // quant_var: LP error
-#line 359 "RSParserImpl.y"
+  case 50: // logic_unary: quantifier error
+#line 356 "RSParserImpl.y"
                                             { state->OnError(ParseEID::invalidQuantifier); YYABORT; }
 #line 735 "RSParserImpl.cpp"
     break;
 
-  case 56: // quant_var_enum: quant_var COMMA quant_var
-#line 362 "RSParserImpl.y"
-                                            { yylhs.value = Enumeration(TokenID::NT_ENUM_DECL, yystack_[2].value, yystack_[0].value); }
+  case 51: // logic_unary: PREDICATE LS setexpr_enum RS
+#line 357 "RSParserImpl.y"
+                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
 #line 741 "RSParserImpl.cpp"
     break;
 
-  case 57: // quant_var_enum: quant_var COMMA error
-#line 363 "RSParserImpl.y"
-                                            { state->OnError(ParseEID::expectedLocal); YYABORT; }
+  case 54: // logic_binary: logic_all EQUIVALENT logic_all
+#line 365 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 747 "RSParserImpl.cpp"
     break;
 
-  case 58: // logic_binary: logic_all EQUIVALENT logic_all
-#line 367 "RSParserImpl.y"
+  case 55: // logic_binary: logic_all IMPLICATION logic_all
+#line 366 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 753 "RSParserImpl.cpp"
     break;
 
-  case 59: // logic_binary: logic_all IMPLICATION logic_all
-#line 368 "RSParserImpl.y"
+  case 56: // logic_binary: logic_all OR logic_all
+#line 367 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 759 "RSParserImpl.cpp"
     break;
 
-  case 60: // logic_binary: logic_all OR logic_all
-#line 369 "RSParserImpl.y"
+  case 57: // logic_binary: logic_all AND logic_all
+#line 368 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 765 "RSParserImpl.cpp"
     break;
 
-  case 61: // logic_binary: logic_all AND logic_all
-#line 370 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
+  case 62: // setexpr: FUNCTION LS setexpr_enum RS
+#line 378 "RSParserImpl.y"
+                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
 #line 771 "RSParserImpl.cpp"
     break;
 
-  case 66: // setexpr: FUNCTION LS setexpr_enum RS
-#line 380 "RSParserImpl.y"
-                                            { yylhs.value = FunctionCall(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+  case 63: // setexpr: text_function LP setexpr RPE
+#line 379 "RSParserImpl.y"
+                                            { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
 #line 777 "RSParserImpl.cpp"
     break;
 
-  case 67: // setexpr: text_function LP setexpr RPE
-#line 381 "RSParserImpl.y"
-                                            { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
+  case 70: // setexpr_enum: setexpr
+#line 390 "RSParserImpl.y"
+                                            { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
 #line 783 "RSParserImpl.cpp"
     break;
 
-  case 74: // setexpr_enum: setexpr
-#line 392 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
+  case 72: // setexpr_enum_min2: setexpr_enum COMMA setexpr
+#line 394 "RSParserImpl.y"
+                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
 #line 789 "RSParserImpl.cpp"
     break;
 
-  case 76: // setexpr_enum_min2: setexpr_enum COMMA setexpr
-#line 396 "RSParserImpl.y"
-                                            { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
+  case 81: // setexpr_binary: setexpr PLUS setexpr
+#line 412 "RSParserImpl.y"
+                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 795 "RSParserImpl.cpp"
     break;
 
-  case 85: // setexpr_binary: setexpr PLUS setexpr
-#line 414 "RSParserImpl.y"
+  case 82: // setexpr_binary: setexpr MINUS setexpr
+#line 413 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 801 "RSParserImpl.cpp"
     break;
 
-  case 86: // setexpr_binary: setexpr MINUS setexpr
-#line 415 "RSParserImpl.y"
+  case 83: // setexpr_binary: setexpr MULTIPLY setexpr
+#line 414 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 807 "RSParserImpl.cpp"
     break;
 
-  case 87: // setexpr_binary: setexpr MULTIPLY setexpr
-#line 416 "RSParserImpl.y"
+  case 84: // setexpr_binary: setexpr UNION setexpr
+#line 415 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 813 "RSParserImpl.cpp"
     break;
 
-  case 88: // setexpr_binary: setexpr UNION setexpr
-#line 417 "RSParserImpl.y"
+  case 85: // setexpr_binary: setexpr SET_MINUS setexpr
+#line 416 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 819 "RSParserImpl.cpp"
     break;
 
-  case 89: // setexpr_binary: setexpr SET_MINUS setexpr
-#line 418 "RSParserImpl.y"
+  case 86: // setexpr_binary: setexpr SYMMINUS setexpr
+#line 417 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 825 "RSParserImpl.cpp"
     break;
 
-  case 90: // setexpr_binary: setexpr SYMMINUS setexpr
-#line 419 "RSParserImpl.y"
+  case 87: // setexpr_binary: setexpr INTERSECTION setexpr
+#line 418 "RSParserImpl.y"
                                             { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
 #line 831 "RSParserImpl.cpp"
     break;
 
-  case 91: // setexpr_binary: setexpr INTERSECTION setexpr
-#line 420 "RSParserImpl.y"
-                                            { yylhs.value = BinaryOperation(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 837 "RSParserImpl.cpp"
-    break;
-
-  case 92: // setexpr_binary: setexpr DECART setexpr
-#line 421 "RSParserImpl.y"
+  case 88: // setexpr_binary: setexpr DECART setexpr
+#line 419 "RSParserImpl.y"
                                             { yylhs.value = Decartian(yystack_[2].value, yystack_[1].value, yystack_[0].value);}
-#line 843 "RSParserImpl.cpp"
+#line 837 "RSParserImpl.cpp"
     break;
 
-  case 93: // setexpr_binary: LP setexpr_binary RPE
-#line 422 "RSParserImpl.y"
+  case 89: // setexpr_binary: LP setexpr_binary RPE
+#line 420 "RSParserImpl.y"
                                             { yylhs.value = RemoveBrackets(yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 849 "RSParserImpl.cpp"
+#line 843 "RSParserImpl.cpp"
     break;
 
-  case 101: // enumeration: LC setexpr_enum RC
-#line 435 "RSParserImpl.y"
+  case 97: // enumeration: LC setexpr_enum RC
+#line 433 "RSParserImpl.y"
                                             { yylhs.value = ReplaceBrackets(TokenID::NT_ENUMERATION, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 855 "RSParserImpl.cpp"
+#line 849 "RSParserImpl.cpp"
     break;
 
-  case 102: // tuple: LP setexpr_enum_min2 RPE
-#line 438 "RSParserImpl.y"
+  case 98: // tuple: LP setexpr_enum_min2 RPE
+#line 436 "RSParserImpl.y"
                                             { yylhs.value = ReplaceBrackets(TokenID::NT_TUPLE, yystack_[2].value, yystack_[1].value, yystack_[0].value); }
-#line 861 "RSParserImpl.cpp"
+#line 855 "RSParserImpl.cpp"
     break;
 
-  case 103: // boolean: BOOLEAN LP setexpr RPE
-#line 441 "RSParserImpl.y"
+  case 99: // boolean: BOOLEAN LP setexpr RPE
+#line 439 "RSParserImpl.y"
                                             { yylhs.value = TextOperator(yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 867 "RSParserImpl.cpp"
+#line 861 "RSParserImpl.cpp"
     break;
 
-  case 104: // boolean: BOOLEAN boolean
-#line 442 "RSParserImpl.y"
+  case 100: // boolean: BOOLEAN boolean
+#line 440 "RSParserImpl.y"
                                             { yylhs.value = UnaryOperation(yystack_[1].value, yystack_[0].value); }
-#line 873 "RSParserImpl.cpp"
+#line 867 "RSParserImpl.cpp"
     break;
 
-  case 105: // filter_expression: FILTER LS setexpr_enum RS LP setexpr RPE
-#line 445 "RSParserImpl.y"
+  case 101: // filter_expression: FILTER LS setexpr_enum RS LP setexpr RPE
+#line 443 "RSParserImpl.y"
                                                { yylhs.value = FilterCall(yystack_[6].value, yystack_[4].value, yystack_[1].value, yystack_[0].value); }
-#line 879 "RSParserImpl.cpp"
+#line 873 "RSParserImpl.cpp"
     break;
 
-  case 106: // declarative: LC LOCAL IN setexpr BAR logic RCE
-#line 449 "RSParserImpl.y"
+  case 102: // declarative: LC LOCAL IN setexpr BAR logic RCE
+#line 447 "RSParserImpl.y"
                                             { yylhs.value = TermDeclaration(yystack_[6].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 885 "RSParserImpl.cpp"
+#line 879 "RSParserImpl.cpp"
     break;
 
-  case 107: // declarative: DECLARATIVE LC variable IN setexpr BAR logic RCE
-#line 450 "RSParserImpl.y"
+  case 103: // declarative: DECLARATIVE LC variable IN setexpr BAR logic RCE
+#line 448 "RSParserImpl.y"
                                                        { yylhs.value = TermDeclaration(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 891 "RSParserImpl.cpp"
+#line 885 "RSParserImpl.cpp"
     break;
 
-  case 108: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR logic BAR setexpr RCE
-#line 453 "RSParserImpl.y"
+  case 104: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR logic BAR setexpr RCE
+#line 451 "RSParserImpl.y"
                                                                      { yylhs.value = FullRecursion(yystack_[9].value, yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 897 "RSParserImpl.cpp"
+#line 891 "RSParserImpl.cpp"
     break;
 
-  case 109: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR setexpr RCE
-#line 454 "RSParserImpl.y"
+  case 105: // recursion: RECURSIVE LC variable ASSIGN setexpr BAR setexpr RCE
+#line 452 "RSParserImpl.y"
                                                            { yylhs.value = ShortRecursion(yystack_[7].value, yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 903 "RSParserImpl.cpp"
+#line 897 "RSParserImpl.cpp"
     break;
 
-  case 110: // imperative: IMPERATIVE LC setexpr BAR imp_blocks RCE
-#line 457 "RSParserImpl.y"
+  case 106: // imperative: IMPERATIVE LC setexpr BAR imp_blocks RCE
+#line 455 "RSParserImpl.y"
                                                { yylhs.value = Imperative(yystack_[5].value, yystack_[3].value, yystack_[1].value, yystack_[0].value); }
-#line 909 "RSParserImpl.cpp"
+#line 903 "RSParserImpl.cpp"
     break;
 
-  case 111: // imp_blocks: imp_block
-#line 460 "RSParserImpl.y"
+  case 107: // imp_blocks: logic
+#line 458 "RSParserImpl.y"
                                             { yylhs.value = AddNode(TokenID::INTERRUPT, yystack_[0].value); }
-#line 915 "RSParserImpl.cpp"
+#line 909 "RSParserImpl.cpp"
     break;
 
-  case 112: // imp_blocks: imp_blocks SEMICOLON imp_blocks
-#line 461 "RSParserImpl.y"
+  case 108: // imp_blocks: imp_blocks SEMICOLON imp_blocks
+#line 459 "RSParserImpl.y"
                                             { yylhs.value = Enumeration(TokenID::INTERRUPT, yystack_[2].value, yystack_[0].value); }
-#line 921 "RSParserImpl.cpp"
-    break;
-
-  case 113: // imp_block: LOCAL ITERATE setexpr
-#line 464 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::NT_IMP_DECLARE, yystack_[2].value, yystack_[0].value); }
-#line 927 "RSParserImpl.cpp"
-    break;
-
-  case 114: // imp_block: LOCAL ASSIGN setexpr
-#line 465 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::NT_IMP_ASSIGN, yystack_[2].value, yystack_[0].value); }
-#line 933 "RSParserImpl.cpp"
+#line 915 "RSParserImpl.cpp"
     break;
 
-  case 115: // imp_block: logic
+  case 110: // RPE: error
 #line 466 "RSParserImpl.y"
-                                            { yylhs.value = AddNode(TokenID::NT_IMP_LOGIC, yystack_[0].value); }
-#line 939 "RSParserImpl.cpp"
-    break;
-
-  case 117: // RPE: error
-#line 473 "RSParserImpl.y"
             { state->OnError(ParseEID::missingParenthesis); YYABORT; }
-#line 945 "RSParserImpl.cpp"
+#line 921 "RSParserImpl.cpp"
     break;
 
-  case 119: // RCE: error
-#line 477 "RSParserImpl.y"
+  case 112: // RCE: error
+#line 470 "RSParserImpl.y"
             { state->OnError(ParseEID::missingCurlyBrace); YYABORT; }
-#line 951 "RSParserImpl.cpp"
+#line 927 "RSParserImpl.cpp"
     break;
 
 
-#line 955 "RSParserImpl.cpp"
+#line 931 "RSParserImpl.cpp"
 
             default:
               break;
             }
         }
 #if YY_EXCEPTIONS
       catch (const syntax_error& yyexc)
@@ -1292,207 +1268,201 @@
         }
       else
         yyres += *yyp;
     return yyres;
   }
 
 
-  const signed char RSParserImpl::yypact_ninf_ = -115;
+  const signed char RSParserImpl::yypact_ninf_ = -60;
 
-  const signed char RSParserImpl::yytable_ninf_ = -116;
+  const signed char RSParserImpl::yytable_ninf_ = -108;
 
   const short
   RSParserImpl::yypact_[] =
   {
-     289,  -115,    83,   -21,     1,  -115,  -115,  -115,  -115,  -115,
-    -115,   395,     8,  -115,  -115,   -20,  -115,  -115,  -115,  -115,
-     -36,    -2,    42,   395,   467,    36,    46,  -115,  -115,  -115,
-      61,   161,  -115,  -115,  -115,    25,  -115,   604,    30,  -115,
-    -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,
-     395,   519,    65,   519,    65,   519,  -115,    71,    78,  -115,
-    -115,  -115,  -115,   604,   519,  -115,   519,    22,    22,   519,
-    -115,   100,   135,   604,    81,    12,   204,   140,  -115,   519,
-     326,   -38,  -115,  -115,    21,    -1,  -115,  -115,   395,   395,
-     395,   395,  -115,  -115,    28,  -115,   -12,  -115,   519,   519,
-     519,  -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,  -115,
-    -115,  -115,   519,   519,   519,   519,   519,   519,   519,  -115,
-     326,  -115,    26,  -115,    86,   143,   123,    22,   145,   107,
-     215,  -115,  -115,  -115,  -115,   519,  -115,  -115,   519,  -115,
-    -115,   519,   395,    92,    80,   177,   155,  -115,  -115,  -115,
-      19,   134,   519,    29,   115,   115,   130,  -115,  -115,  -115,
-    -115,  -115,   326,   143,  -115,  -115,  -115,   152,   519,   519,
-     447,   326,   542,   326,  -115,  -115,  -115,  -115,    37,   343,
-    -115,  -115,  -115,   519,   556,   569,   157,     7,    15,  -115,
-     395,  -115,  -115,  -115,  -115,   143,   395,   395,   519,   519,
-    -115,  -115,   447,  -115,    18,  -115,    18,   137,   253,   326,
-     326,  -115,  -115,  -115,   519,  -115,    75,  -115
+     321,    66,    22,   -29,   -28,   -60,   -60,   -60,   -60,   -60,
+     -60,   427,   -21,   -60,   -60,   -36,   -60,   -60,   -60,   -60,
+      -9,     8,    42,   427,   447,    36,    86,   -60,   -60,   -60,
+     119,   107,   156,   -60,   -60,   -60,    43,   -60,   584,    82,
+     -60,   -60,   -60,   -60,   -60,   128,   -60,   -60,   -60,   -60,
+     -60,   427,   499,    88,   499,    88,   499,   -60,   108,   129,
+     -60,   -60,   -60,   -60,   584,   499,   -60,   499,    23,    23,
+     499,   -60,    10,   112,   584,   116,     5,   217,   157,   -60,
+     499,   276,    26,   -60,   -60,   -60,    11,    40,   -60,   -60,
+     499,   499,   427,   427,   427,   427,   -60,   -60,   499,   -60,
+     -19,   -60,   499,   499,   499,   -60,   -60,   -60,   -60,   -60,
+     -60,   -60,   -60,   -60,   -60,   -60,   499,   499,   499,   499,
+     499,   499,   499,   -60,   -60,   276,   -60,    73,   -60,    84,
+      76,    93,   159,   139,   228,   -60,   -60,   -60,   -60,   499,
+     -60,   -60,   499,   -60,   -60,   499,   427,    56,   276,   276,
+      68,     4,   163,   -60,   499,    81,   127,   127,   166,   -60,
+     -60,   -60,   -60,   -60,   276,    76,   -60,   -60,   -60,   143,
+     499,   499,   427,   276,   522,   276,   -60,   -60,   -60,   375,
+     -60,   -60,   -60,   499,   536,   549,     6,    14,   427,   -60,
+      76,   427,   427,   -60,   -60,   427,   -60,    24,   -60,    24,
+     133,   266,   -60,   -60,   -60,   499,   -60,   302,   -60
   };
 
   const signed char
   RSParserImpl::yydefact_[] =
   {
-       0,    83,    80,    81,    82,    84,    77,    79,    78,    51,
-      52,     0,     0,    71,    72,     0,    73,    68,    69,    70,
+       0,    79,    76,    77,    78,    80,    73,    75,    74,    52,
+      53,     0,     0,    67,    68,     0,    69,    64,    65,    66,
        0,     0,     0,     0,     0,     0,     0,     2,     3,     4,
-      28,     0,    29,    25,    26,     0,    27,    11,     0,    62,
-      63,    64,    65,    94,    95,    96,    97,    98,   100,    99,
-       5,     0,     0,     0,     0,     0,    80,    81,    82,    50,
-      48,    49,    44,     0,     0,   104,     0,     0,     0,     0,
-      28,     0,     0,    74,     0,     0,     0,    83,    82,     0,
-      74,     0,    75,    13,     0,     0,    14,     1,     0,     0,
-       0,     0,    46,    19,     0,    53,     0,    54,     0,     0,
-       0,    40,    41,    42,    43,    39,    38,    33,    34,    35,
-      36,    37,     0,     0,     0,     0,     0,     0,     0,     7,
-       6,     8,     0,     9,     0,     0,     0,     0,     0,     0,
-       0,   117,   116,    31,    30,     0,   102,    93,     0,   101,
-      18,     0,     0,     0,    58,    59,    60,    61,    55,    23,
-       0,     0,     0,     0,    85,    86,    87,    92,    88,    91,
-      89,    90,    32,     0,    66,    47,   103,     0,     0,     0,
-       0,    76,     0,    17,    12,    16,    15,    20,     0,     0,
-      57,    56,    67,     0,     0,     0,    83,    28,     0,   111,
-       0,    22,    24,    21,    45,     0,     0,     0,     0,     0,
-     119,   118,     0,   110,     0,   105,     0,    28,     0,   114,
-     113,   112,   106,   107,     0,   109,     0,   108
+       0,    30,     0,    31,    24,    25,     0,    26,    11,     0,
+      58,    59,    60,    61,    90,    91,    92,    93,    94,    96,
+      95,     5,     0,     0,     0,     0,     0,    76,    77,    78,
+      48,    29,    27,    28,     0,     0,   100,     0,     0,     0,
+       0,    30,     0,     0,    70,     0,     0,     0,    79,    78,
+       0,    70,     0,    71,    91,    13,     0,     0,    14,     1,
+       0,     0,     0,     0,     0,     0,    50,    19,     0,    21,
+       0,    20,     0,     0,     0,    44,    45,    46,    47,    43,
+      42,    37,    38,    39,    40,    41,     0,     0,     0,     0,
+       0,     0,     0,     7,    79,     6,     8,     0,     9,     0,
+       0,     0,     0,     0,     0,   110,   109,    33,    32,     0,
+      98,    89,     0,    97,    18,     0,     0,     0,    35,    36,
+      54,    55,    56,    57,     0,     0,    81,    82,    83,    88,
+      84,    87,    85,    86,    34,     0,    62,    51,    99,     0,
+       0,     0,     0,    72,     0,    17,    12,    16,    15,     0,
+      23,    22,    63,     0,     0,     0,    30,     0,     0,    49,
+       0,     0,     0,   112,   111,     0,   106,     0,   101,     0,
+      30,     0,   108,   102,   103,     0,   105,     0,   104
   };
 
   const short
   RSParserImpl::yypgoto_[] =
   {
-    -115,  -115,  -115,   -39,    85,  -115,    66,   -34,    32,    33,
-       4,   101,    -8,    -9,  -115,    -6,    34,  -115,    59,  -115,
-     201,     0,  -115,    67,   -16,  -115,  -115,   -11,  -115,  -115,
-    -115,   213,  -115,  -115,  -115,  -115,    27,  -115,   -66,  -114
+     -60,   -60,   -60,   -41,   103,   -60,    49,   -27,    48,     2,
+      31,   114,    -7,   -10,   -60,    -6,   -60,   189,     0,   -60,
+      99,   -20,   -60,   -60,    -4,   -60,   -60,    32,   201,   -60,
+     -60,   -60,   -60,    19,   -59,   -50
   };
 
   const short
   RSParserImpl::yydefgoto_[] =
   {
-      -1,    26,    27,    28,    29,    85,    86,   149,   150,   151,
-      70,    31,    32,    33,   117,    34,    62,    35,    96,    97,
-      36,    63,    38,    74,    82,    39,    40,    41,    42,    43,
-      44,    45,    46,    47,    48,    49,   188,   189,   133,   203
+      -1,    26,    27,    28,    29,    87,    88,    30,   100,    71,
+      60,    32,    33,    34,   121,    35,    36,    37,    64,    39,
+      75,    83,    40,    41,    42,    43,    44,    84,    46,    47,
+      48,    49,    50,   187,   137,   196
   };
 
   const short
   RSParserImpl::yytable_[] =
   {
-      37,    95,    60,    59,    30,    61,   134,    75,  -115,   136,
-     137,   119,    76,   131,    71,   152,   200,   139,    67,   200,
-     131,   135,   140,    73,    80,    93,    92,    52,    93,   148,
-     180,    93,    93,   128,   129,    53,    66,    83,   191,    84,
-      93,   -28,   -28,   -28,   -28,    12,    87,   153,   141,    54,
-      37,   120,    68,    80,    30,    80,   142,    55,   143,   166,
-      64,   -10,  -115,    75,   125,   132,    80,  -115,    76,   130,
-     201,   -75,   132,   201,   127,   202,   200,    94,   -24,    80,
-     127,    94,   118,   164,   177,   135,    98,    99,   100,   127,
-     212,    81,   213,   175,   215,    84,    69,   182,   154,   155,
-     156,   131,   217,   174,    89,    90,    91,   112,   113,   114,
-     115,   116,   157,   158,   159,   160,   161,   162,   163,    95,
-     122,    25,   124,   -25,   -25,   -25,   -25,    53,   100,   205,
-     201,    50,    51,   126,    55,   171,   131,   121,   172,   123,
-     135,   173,    37,   165,   131,   135,    30,   112,   113,   114,
-     115,   116,   179,   132,    98,    99,   100,   169,   -27,   -27,
-     -27,   -27,   112,   113,   114,   115,   116,   138,   184,   185,
-      60,    59,   168,    61,   187,   112,   113,   114,   115,   116,
-     167,    91,   135,   195,    88,    89,    90,    91,   132,   144,
-     145,   146,   147,   178,   204,   214,   132,   208,   209,   210,
-     206,   207,    90,    91,   183,   131,   187,   198,   199,   176,
-     192,   193,   181,   194,   216,   -64,   -64,   -64,   -64,   -64,
-     -64,   -64,   -64,   -64,    72,    65,    98,    99,   100,   211,
-       0,   -64,   -64,   -64,   -64,   -64,   -64,   -64,   -64,   -64,
-     -64,     0,     0,     0,     0,     0,     0,   112,   113,   114,
-     115,   116,     0,     0,   200,     0,     0,   132,     0,     0,
-       0,     0,     0,   -64,    98,    99,   100,   101,   102,   103,
-     104,   105,   106,   170,     0,     0,     0,     0,     0,     0,
-     107,   108,   109,   110,   111,   112,   113,   114,   115,   116,
-       0,     0,     1,     2,     3,     4,     5,     6,     7,     8,
-       0,     0,     0,     0,     0,     0,     0,     0,   201,     9,
-      10,    11,     0,     0,     0,     0,     0,     0,     0,     0,
-       0,     0,     0,     0,     0,     0,    12,    13,    14,    15,
-      16,    17,    18,    19,    20,    21,    22,    98,    99,   100,
-       0,    23,     0,    24,     0,    25,     1,    56,    57,    58,
-       5,     6,     7,     8,    98,    99,   100,     0,   112,   113,
-     114,   115,   116,     9,    10,    11,     0,     0,     0,     0,
-       0,     0,     0,     0,     0,   112,   113,   114,   115,   116,
-      12,    13,    14,    15,    16,    17,    18,    19,    20,    21,
-      22,     0,     0,     0,     0,    23,     0,    24,     1,    56,
-      57,    58,     5,     6,     7,     8,     0,     0,     0,     0,
+      38,    62,    31,    76,    61,    63,   135,  -107,   154,    99,
+     123,   135,   144,    72,   138,   193,    12,   140,   141,    77,
+      67,    53,    55,    74,    81,   193,    97,    54,    56,    94,
+      95,    65,    45,   -24,   -24,   -24,   -24,    85,   145,    86,
+     155,   132,   133,    45,    96,    68,    97,   -30,   -30,   -30,
+     -30,    38,   125,    31,    81,    45,    81,   177,   136,    86,
+      76,  -107,    69,   136,   -71,   130,  -107,    81,   101,   194,
+     134,   168,    51,    52,   195,    98,    77,   135,    76,   194,
+      81,   143,   180,    45,    97,   139,    89,   102,   103,   104,
+     148,   149,    93,    94,    95,    98,    70,   146,    81,   147,
+     101,   101,   156,   157,   158,   176,   182,   -10,   116,   117,
+     118,   119,   120,   135,   -19,   -19,   159,   160,   161,   162,
+     163,   164,   165,    82,    45,    45,    45,    45,    99,   136,
+     166,   198,   139,    98,   122,   -26,   -26,   -26,   -26,   173,
+     104,   167,   174,   139,    25,   175,    38,   203,    31,   204,
+     169,   206,   139,   127,   179,   129,   126,   208,   128,   116,
+     117,   118,   119,   120,    54,   136,   131,    90,    91,    62,
+     184,   185,    61,    63,   186,   139,   -20,   -20,    45,    92,
+      93,    94,    95,   190,   142,    56,   170,   101,   171,    95,
+     197,   205,   201,   199,   200,   183,   178,   186,   116,   117,
+     118,   119,   120,   181,    45,   207,   150,   151,   152,   153,
+     189,    45,    73,    66,   202,     0,     0,     0,   135,     0,
+      45,     0,     0,    45,    45,     0,     0,    45,   -60,   -60,
+     -60,   -60,   -60,   -60,   -60,   -60,   -60,     0,     0,   102,
+     103,   104,     0,     0,   -60,   -60,   -60,   -60,   -60,   -60,
+     -60,   -60,   -60,   -60,     0,     0,     0,     0,     0,     0,
+     116,   117,   118,   119,   120,     0,     0,   193,     0,     0,
+     136,     0,     0,     0,     0,     0,   -60,   102,   103,   104,
+     105,   106,   107,   108,   109,   110,   172,   102,   103,   104,
+       0,     0,     0,   111,   112,   113,   114,   115,   116,   117,
+     118,   119,   120,   193,     0,     0,     0,     0,   116,   117,
+     118,   119,   120,   102,   103,   104,     0,     0,     0,     0,
+       0,   194,     0,     0,     1,     2,     3,     4,     5,     6,
+       7,     8,     0,     0,   116,   117,   118,   119,   120,     0,
+       0,     9,    10,    11,     0,     0,     0,     0,     0,     0,
+       0,     0,     0,     0,     0,     0,     0,   194,    12,    13,
+      14,    15,    16,    17,    18,    19,    20,    21,    22,     0,
+       0,     0,     0,    23,     0,    24,     0,    25,     1,    57,
+      58,    59,     5,     6,     7,     8,   102,   103,   104,     0,
        0,     0,     0,     0,     0,     9,    10,    11,     0,     0,
-       0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
-       0,     0,    12,    13,    14,    15,    16,    17,    18,    19,
+       0,     0,     0,     0,     0,     0,     0,   116,   117,   118,
+     119,   120,    12,    13,    14,    15,    16,    17,    18,    19,
       20,    21,    22,     0,     0,     0,     0,    23,     0,    24,
-     186,    56,    57,    58,     5,     6,     7,     8,     0,     0,
+       1,    57,    58,    59,     5,     6,     7,     8,     0,     0,
        0,     0,     0,     0,     0,     0,     0,     9,    10,    11,
-      77,    56,    57,    78,     5,     6,     7,     8,     0,     0,
+      78,    57,    58,    79,     5,     6,     7,     8,     0,     0,
        0,     0,     0,     0,    12,    13,    14,    15,    16,    17,
       18,    19,    20,    21,    22,     0,     0,     0,     0,    23,
        0,    24,     0,     0,    12,    13,    14,    15,    16,    17,
-      18,    19,    20,    21,    22,     0,     0,     0,     0,    79,
-       0,    24,     1,    56,    57,    78,     5,     6,     7,     8,
+      18,    19,    20,    21,    22,     0,     0,     0,     0,    80,
+       0,    24,   124,    57,    58,    79,     5,     6,     7,     8,
        0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
        0,     0,     0,     0,     0,     0,     0,     0,     0,     0,
-       0,     0,     0,    98,    99,   100,    12,    13,    14,    15,
-      16,    17,    18,    19,    20,    21,    22,    98,    99,   100,
-       0,    79,     0,    24,   112,   113,   114,   115,   116,     0,
-      98,    99,   100,     0,     0,     0,     0,     0,   112,   113,
-     114,   115,   116,     0,     0,     0,     0,     0,     0,     0,
-     190,   112,   113,   114,   115,   116,     0,     0,     0,     0,
-       0,     0,     0,     0,   196,    98,    99,   100,   101,   102,
-     103,   104,   105,   106,     0,     0,     0,   197,     0,     0,
-       0,   107,   108,   109,   110,   111,   112,   113,   114,   115,
-     116
+       0,     0,     0,   102,   103,   104,    12,    13,    14,    15,
+      16,    17,    18,    19,    20,    21,    22,   102,   103,   104,
+       0,    80,     0,    24,   116,   117,   118,   119,   120,     0,
+     102,   103,   104,     0,     0,     0,     0,     0,   116,   117,
+     118,   119,   120,     0,     0,     0,     0,     0,     0,     0,
+     188,   116,   117,   118,   119,   120,     0,     0,     0,     0,
+       0,     0,     0,     0,   191,   102,   103,   104,   105,   106,
+     107,   108,   109,   110,     0,     0,     0,   192,     0,     0,
+       0,   111,   112,   113,   114,   115,   116,   117,   118,   119,
+     120
   };
 
   const short
   RSParserImpl::yycheck_[] =
   {
-       0,    35,    11,    11,     0,    11,    72,    23,     1,    75,
-      76,    50,    23,     1,    23,    27,     1,    55,    54,     1,
-       1,    59,     1,    23,    24,     3,     1,    48,     3,     1,
-       1,     3,     3,    67,    68,    56,    56,     1,     1,     3,
-       3,    23,    24,    25,    26,    37,     0,    59,    27,    48,
-      50,    51,    54,    53,    50,    55,    57,    56,    59,   125,
-      52,     0,    55,    79,    64,    53,    66,    60,    79,    69,
-      55,    59,    53,    55,    52,    60,     1,    52,    59,    79,
-      52,    52,    52,    57,   150,    59,    11,    12,    13,    52,
-     204,    24,   206,     1,   208,     3,    54,   163,    98,    99,
-     100,     1,   216,   142,    24,    25,    26,    32,    33,    34,
-      35,    36,   112,   113,   114,   115,   116,   117,   118,   153,
-      53,    56,    55,    23,    24,    25,    26,    56,    13,   195,
-      55,    48,    49,    66,    56,   135,     1,    52,   138,    54,
-      59,   141,   142,    57,     1,    59,   142,    32,    33,    34,
-      35,    36,   152,    53,    11,    12,    13,    50,    23,    24,
-      25,    26,    32,    33,    34,    35,    36,    27,   168,   169,
-     179,   179,    27,   179,   170,    32,    33,    34,    35,    36,
-      57,    26,    59,   183,    23,    24,    25,    26,    53,    88,
-      89,    90,    91,    59,   190,    58,    53,   197,   198,   199,
-     196,   197,    25,    26,    52,     1,   202,    50,    51,   143,
-     178,   178,   153,   179,   214,    11,    12,    13,    14,    15,
-      16,    17,    18,    19,    23,    12,    11,    12,    13,   202,
-      -1,    27,    28,    29,    30,    31,    32,    33,    34,    35,
-      36,    -1,    -1,    -1,    -1,    -1,    -1,    32,    33,    34,
-      35,    36,    -1,    -1,     1,    -1,    -1,    53,    -1,    -1,
-      -1,    -1,    -1,    59,    11,    12,    13,    14,    15,    16,
-      17,    18,    19,    58,    -1,    -1,    -1,    -1,    -1,    -1,
-      27,    28,    29,    30,    31,    32,    33,    34,    35,    36,
-      -1,    -1,     3,     4,     5,     6,     7,     8,     9,    10,
-      -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    55,    20,
-      21,    22,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
-      -1,    -1,    -1,    -1,    -1,    -1,    37,    38,    39,    40,
-      41,    42,    43,    44,    45,    46,    47,    11,    12,    13,
-      -1,    52,    -1,    54,    -1,    56,     3,     4,     5,     6,
-       7,     8,     9,    10,    11,    12,    13,    -1,    32,    33,
-      34,    35,    36,    20,    21,    22,    -1,    -1,    -1,    -1,
-      -1,    -1,    -1,    -1,    -1,    32,    33,    34,    35,    36,
-      37,    38,    39,    40,    41,    42,    43,    44,    45,    46,
-      47,    -1,    -1,    -1,    -1,    52,    -1,    54,     3,     4,
-       5,     6,     7,     8,     9,    10,    -1,    -1,    -1,    -1,
+       0,    11,     0,    23,    11,    11,     1,     1,    27,    36,
+      51,     1,     1,    23,    73,     1,    37,    76,    77,    23,
+      56,    50,    50,    23,    24,     1,     3,    56,    56,    25,
+      26,    52,     0,    23,    24,    25,    26,     1,    27,     3,
+      59,    68,    69,    11,     1,    54,     3,    23,    24,    25,
+      26,    51,    52,    51,    54,    23,    56,     1,    53,     3,
+      80,    55,    54,    53,    59,    65,    60,    67,    36,    55,
+      70,   130,    50,    51,    60,    52,    80,     1,    98,    55,
+      80,    55,     1,    51,     3,    59,     0,    11,    12,    13,
+      90,    91,    24,    25,    26,    52,    54,    57,    98,    59,
+      68,    69,   102,   103,   104,   146,   165,     0,    32,    33,
+      34,    35,    36,     1,    48,    49,   116,   117,   118,   119,
+     120,   121,   122,    24,    92,    93,    94,    95,   155,    53,
+      57,   190,    59,    52,    52,    23,    24,    25,    26,   139,
+      13,    57,   142,    59,    56,   145,   146,   197,   146,   199,
+      57,   201,    59,    54,   154,    56,    53,   207,    55,    32,
+      33,    34,    35,    36,    56,    53,    67,    48,    49,   179,
+     170,   171,   179,   179,   172,    59,    48,    49,   146,    23,
+      24,    25,    26,   183,    27,    56,    27,   155,    49,    26,
+     188,    58,   192,   191,   192,    52,   147,   195,    32,    33,
+      34,    35,    36,   155,   172,   205,    92,    93,    94,    95,
+     179,   179,    23,    12,   195,    -1,    -1,    -1,     1,    -1,
+     188,    -1,    -1,   191,   192,    -1,    -1,   195,    11,    12,
+      13,    14,    15,    16,    17,    18,    19,    -1,    -1,    11,
+      12,    13,    -1,    -1,    27,    28,    29,    30,    31,    32,
+      33,    34,    35,    36,    -1,    -1,    -1,    -1,    -1,    -1,
+      32,    33,    34,    35,    36,    -1,    -1,     1,    -1,    -1,
+      53,    -1,    -1,    -1,    -1,    -1,    59,    11,    12,    13,
+      14,    15,    16,    17,    18,    19,    58,    11,    12,    13,
+      -1,    -1,    -1,    27,    28,    29,    30,    31,    32,    33,
+      34,    35,    36,     1,    -1,    -1,    -1,    -1,    32,    33,
+      34,    35,    36,    11,    12,    13,    -1,    -1,    -1,    -1,
+      -1,    55,    -1,    -1,     3,     4,     5,     6,     7,     8,
+       9,    10,    -1,    -1,    32,    33,    34,    35,    36,    -1,
+      -1,    20,    21,    22,    -1,    -1,    -1,    -1,    -1,    -1,
+      -1,    -1,    -1,    -1,    -1,    -1,    -1,    55,    37,    38,
+      39,    40,    41,    42,    43,    44,    45,    46,    47,    -1,
+      -1,    -1,    -1,    52,    -1,    54,    -1,    56,     3,     4,
+       5,     6,     7,     8,     9,    10,    11,    12,    13,    -1,
       -1,    -1,    -1,    -1,    -1,    20,    21,    22,    -1,    -1,
-      -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,    -1,
-      -1,    -1,    37,    38,    39,    40,    41,    42,    43,    44,
+      -1,    -1,    -1,    -1,    -1,    -1,    -1,    32,    33,    34,
+      35,    36,    37,    38,    39,    40,    41,    42,    43,    44,
       45,    46,    47,    -1,    -1,    -1,    -1,    52,    -1,    54,
        3,     4,     5,     6,     7,     8,     9,    10,    -1,    -1,
       -1,    -1,    -1,    -1,    -1,    -1,    -1,    20,    21,    22,
        3,     4,     5,     6,     7,     8,     9,    10,    -1,    -1,
       -1,    -1,    -1,    -1,    37,    38,    39,    40,    41,    42,
       43,    44,    45,    46,    47,    -1,    -1,    -1,    -1,    52,
       -1,    54,    -1,    -1,    37,    38,    39,    40,    41,    42,
@@ -1514,67 +1484,66 @@
 
   const signed char
   RSParserImpl::yystos_[] =
   {
        0,     3,     4,     5,     6,     7,     8,     9,    10,    20,
       21,    22,    37,    38,    39,    40,    41,    42,    43,    44,
       45,    46,    47,    52,    54,    56,    62,    63,    64,    65,
-      71,    72,    73,    74,    76,    78,    81,    82,    83,    86,
-      87,    88,    89,    90,    91,    92,    93,    94,    95,    96,
-      48,    49,    48,    56,    48,    56,     4,     5,     6,    73,
-      74,    76,    77,    82,    52,    92,    56,    54,    54,    54,
-      71,    74,    81,    82,    84,    85,    88,     3,     6,    52,
-      82,    84,    85,     1,     3,    66,    67,     0,    23,    24,
-      25,    26,     1,     3,    52,    68,    79,    80,    11,    12,
-      13,    14,    15,    16,    17,    18,    19,    27,    28,    29,
-      30,    31,    32,    33,    34,    35,    36,    75,    52,    64,
-      82,    65,    84,    65,    84,    82,    84,    52,    68,    68,
-      82,     1,    53,    99,    99,    59,    99,    99,    27,    55,
-       1,    27,    57,    59,    72,    72,    72,    72,     1,    68,
-      69,    70,    27,    59,    82,    82,    82,    82,    82,    82,
-      82,    82,    82,    82,    57,    57,    99,    57,    27,    50,
-      58,    82,    82,    82,    64,     1,    67,    99,    59,    82,
-       1,    79,    99,    52,    82,    82,     3,    71,    97,    98,
-      58,     1,    69,    70,    77,    82,    58,    58,    50,    51,
-       1,    55,    60,   100,    71,    99,    71,    71,    82,    82,
-      82,    97,   100,   100,    58,   100,    82,   100
+      68,    70,    72,    73,    74,    76,    77,    78,    79,    80,
+      83,    84,    85,    86,    87,    88,    89,    90,    91,    92,
+      93,    50,    51,    50,    56,    50,    56,     4,     5,     6,
+      71,    73,    74,    76,    79,    52,    89,    56,    54,    54,
+      54,    70,    74,    78,    79,    81,    82,    85,     3,     6,
+      52,    79,    81,    82,    88,     1,     3,    66,    67,     0,
+      48,    49,    23,    24,    25,    26,     1,     3,    52,    68,
+      69,    88,    11,    12,    13,    14,    15,    16,    17,    18,
+      19,    27,    28,    29,    30,    31,    32,    33,    34,    35,
+      36,    75,    52,    64,     3,    79,    65,    81,    65,    81,
+      79,    81,    68,    68,    79,     1,    53,    95,    95,    59,
+      95,    95,    27,    55,     1,    27,    57,    59,    79,    79,
+      72,    72,    72,    72,    27,    59,    79,    79,    79,    79,
+      79,    79,    79,    79,    79,    79,    57,    57,    95,    57,
+      27,    49,    58,    79,    79,    79,    64,     1,    67,    79,
+       1,    69,    95,    52,    79,    79,    70,    94,    58,    71,
+      79,    58,    58,     1,    55,    60,    96,    70,    95,    70,
+      70,    79,    94,    96,    96,    58,    96,    79,    96
   };
 
   const signed char
   RSParserImpl::yyr1_[] =
   {
        0,    61,    62,    62,    62,    63,    63,    63,    63,    63,
       64,    64,    65,    65,    66,    66,    66,    67,    67,    68,
-      68,    69,    69,    70,    70,    71,    71,    71,    72,    72,
-      73,    73,    74,    75,    75,    75,    75,    75,    75,    75,
-      75,    75,    75,    75,    76,    76,    76,    76,    77,    77,
-      77,    78,    78,    79,    79,    79,    80,    80,    81,    81,
-      81,    81,    82,    82,    82,    82,    82,    82,    83,    83,
-      83,    83,    83,    83,    84,    84,    85,    86,    86,    86,
-      87,    87,    87,    87,    87,    88,    88,    88,    88,    88,
-      88,    88,    88,    88,    89,    89,    89,    89,    89,    89,
-      89,    90,    91,    92,    92,    93,    94,    94,    95,    95,
-      96,    97,    97,    98,    98,    98,    99,    99,   100,   100
+      68,    69,    69,    69,    70,    70,    70,    71,    71,    71,
+      72,    72,    73,    73,    74,    74,    74,    75,    75,    75,
+      75,    75,    75,    75,    75,    75,    75,    75,    76,    76,
+      76,    76,    77,    77,    78,    78,    78,    78,    79,    79,
+      79,    79,    79,    79,    80,    80,    80,    80,    80,    80,
+      81,    81,    82,    83,    83,    83,    84,    84,    84,    84,
+      84,    85,    85,    85,    85,    85,    85,    85,    85,    85,
+      86,    86,    86,    86,    86,    86,    86,    87,    88,    89,
+      89,    90,    91,    91,    92,    92,    93,    94,    94,    95,
+      95,    96,    96
   };
 
   const signed char
   RSParserImpl::yyr2_[] =
   {
        0,     2,     1,     1,     1,     2,     3,     3,     3,     3,
        1,     1,     4,     2,     1,     3,     3,     3,     2,     1,
-       3,     3,     3,     1,     1,     1,     1,     1,     1,     1,
-       3,     3,     3,     1,     1,     1,     1,     1,     1,     1,
-       1,     1,     1,     1,     2,     5,     2,     4,     1,     1,
-       1,     1,     1,     1,     1,     2,     3,     3,     3,     3,
-       3,     3,     1,     1,     1,     1,     4,     4,     1,     1,
-       1,     1,     1,     1,     1,     1,     3,     1,     1,     1,
-       1,     1,     1,     1,     1,     3,     3,     3,     3,     3,
-       3,     3,     3,     3,     1,     1,     1,     1,     1,     1,
-       1,     3,     3,     4,     2,     7,     7,     8,    10,     8,
-       6,     1,     3,     3,     3,     1,     1,     1,     1,     1
+       1,     1,     3,     3,     1,     1,     1,     1,     1,     1,
+       1,     1,     3,     3,     3,     3,     3,     1,     1,     1,
+       1,     1,     1,     1,     1,     1,     1,     1,     2,     5,
+       2,     4,     1,     1,     3,     3,     3,     3,     1,     1,
+       1,     1,     4,     4,     1,     1,     1,     1,     1,     1,
+       1,     1,     3,     1,     1,     1,     1,     1,     1,     1,
+       1,     3,     3,     3,     3,     3,     3,     3,     3,     3,
+       1,     1,     1,     1,     1,     1,     1,     3,     3,     4,
+       2,     7,     7,     8,    10,     8,     6,     1,     3,     1,
+       1,     1,     1
   };
 
 
 #if YYDEBUG || 1
   // YYTNAME[SYMBOL-NUM] -- String name of the symbol SYMBOL-NUM.
   // First, the terminals, then, starting at \a YYNTOKENS, nonterminals.
   const char*
@@ -1584,45 +1553,44 @@
   "FUNCTION", "PREDICATE", "RADICAL", "INTEGER", "INTSET", "EMPTYSET",
   "PLUS", "MINUS", "MULTIPLY", "GREATER", "LESSER", "GREATER_OR_EQ",
   "LESSER_OR_EQ", "EQUAL", "NOTEQUAL", "FORALL", "EXISTS", "NOT",
   "EQUIVALENT", "IMPLICATION", "OR", "AND", "IN", "NOTIN", "SUBSET",
   "SUBSET_OR_EQ", "NOTSUBSET", "DECART", "UNION", "INTERSECTION",
   "SET_MINUS", "SYMMINUS", "BOOLEAN", "BIGPR", "SMALLPR", "FILTER", "CARD",
   "BOOL", "DEBOOL", "RED", "DECLARATIVE", "RECURSIVE", "IMPERATIVE",
-  "DEFINE", "STRUCT", "ASSIGN", "ITERATE", "LP", "RP", "LC", "RC", "LS",
+  "ITERATE", "ASSIGN", "DEFINE", "STRUCT", "LP", "RP", "LC", "RC", "LS",
   "RS", "BAR", "COMMA", "SEMICOLON", "$accept", "expression",
   "global_declaration", "logic_or_setexpr", "function_definition",
-  "arguments", "declaration", "variable", "var_enum", "var_all", "logic",
-  "logic_all", "logic_par", "logic_predicates", "binary_predicate",
-  "logic_unary", "logic_no_binary", "quantifier", "quant_var",
-  "quant_var_enum", "logic_binary", "setexpr", "text_function",
-  "setexpr_enum", "setexpr_enum_min2", "literal", "identifier",
-  "setexpr_binary", "setexpr_generators", "enumeration", "tuple",
-  "boolean", "filter_expression", "declarative", "recursion", "imperative",
-  "imp_blocks", "imp_block", "RPE", "RCE", YY_NULLPTR
+  "arguments", "declaration", "variable", "variable_pack", "logic",
+  "logic_no_binary", "logic_all", "logic_par", "logic_predicates",
+  "binary_predicate", "logic_unary", "quantifier", "logic_binary",
+  "setexpr", "text_function", "setexpr_enum", "setexpr_enum_min2",
+  "literal", "identifier", "setexpr_binary", "setexpr_generators",
+  "enumeration", "tuple", "boolean", "filter_expression", "declarative",
+  "recursion", "imperative", "imp_blocks", "RPE", "RCE", YY_NULLPTR
   };
 #endif
 
 
 #if YYDEBUG
   const short
   RSParserImpl::yyrline_[] =
   {
-       0,   262,   262,   263,   264,   268,   269,   270,   271,   272,
-     276,   277,   281,   282,   287,   288,   289,   292,   293,   297,
-     298,   301,   302,   305,   306,   311,   312,   313,   316,   317,
-     320,   321,   325,   328,   329,   330,   331,   332,   333,   334,
-     335,   336,   337,   338,   342,   343,   344,   345,   348,   349,
-     350,   353,   354,   357,   358,   359,   362,   363,   367,   368,
-     369,   370,   376,   377,   378,   379,   380,   381,   384,   385,
-     386,   387,   388,   389,   392,   393,   396,   400,   401,   402,
-     406,   407,   408,   409,   410,   414,   415,   416,   417,   418,
-     419,   420,   421,   422,   426,   427,   428,   429,   430,   431,
-     432,   435,   438,   441,   442,   445,   449,   450,   453,   454,
-     457,   460,   461,   464,   465,   466,   472,   473,   476,   477
+       0,   270,   270,   271,   272,   276,   277,   278,   279,   280,
+     284,   285,   289,   290,   295,   296,   297,   300,   301,   305,
+     306,   309,   310,   311,   316,   317,   318,   321,   322,   323,
+     326,   327,   330,   331,   335,   336,   337,   340,   341,   342,
+     343,   344,   345,   346,   347,   348,   349,   350,   354,   355,
+     356,   357,   360,   361,   365,   366,   367,   368,   374,   375,
+     376,   377,   378,   379,   382,   383,   384,   385,   386,   387,
+     390,   391,   394,   398,   399,   400,   404,   405,   406,   407,
+     408,   412,   413,   414,   415,   416,   417,   418,   419,   420,
+     424,   425,   426,   427,   428,   429,   430,   433,   436,   439,
+     440,   443,   447,   448,   451,   452,   455,   458,   459,   465,
+     466,   469,   470
   };
 
   void
   RSParserImpl::yy_stack_print_ () const
   {
     *yycdebug_ << "Stack now";
     for (stack_type::const_iterator
@@ -1699,17 +1667,17 @@
       return YY_CAST (symbol_kind_type, translate_table[t]);
     else
       return symbol_kind::S_YYUNDEF;
   }
 
 #line 15 "RSParserImpl.y"
 } } } // ccl::rslang::detail
-#line 1707 "RSParserImpl.cpp"
+#line 1675 "RSParserImpl.cpp"
 
-#line 484 "RSParserImpl.y"
+#line 477 "RSParserImpl.y"
 
 
 #ifdef _MSC_VER
   #pragma warning( pop )
 #endif
 
 #ifdef __clang__
```

### Comparing `pyconcept-0.1.4/ccl/rslang/src/RSToken.cpp` & `pyconcept-0.1.5/ccl/rslang/src/RSToken.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -89,18 +89,14 @@
   case TokenID::NT_ARGUMENTS: return "ARGS";
   case TokenID::NT_FUNC_DEFINITION: return "FUNCTION_DEFINITION";
 
   case TokenID::NT_DECLARATIVE_EXPR: return "DECLARATIVE";
   case TokenID::NT_IMPERATIVE_EXPR: return "IMPERATIVE";
   case TokenID::NT_RECURSIVE_FULL: return "REC_FULL";
   case TokenID::NT_RECURSIVE_SHORT: return "REC_SHORT";
-
-  case TokenID::NT_IMP_DECLARE: return "IDECLARE";
-  case TokenID::NT_IMP_ASSIGN: return "IASSIGN";
-  case TokenID::NT_IMP_LOGIC: return "ICHECK";
   }
 }
 
 [[nodiscard]] std::string AsciiStr(const TokenID id) {
   switch (id) {
   default: return SharedStr(id);
 
@@ -129,26 +125,27 @@
 
   case TokenID::IN: return R"( \in )";
   case TokenID::NOTIN: return R"( \notin )";
   case TokenID::SUBSET: return R"( \subset )";
   case TokenID::SUBSET_OR_EQ: return R"( \subseteq )";
   case TokenID::NOTSUBSET: return R"( \notsubset )";
 
+  case TokenID::ASSIGN: return R"( \assign )";
+  case TokenID::ITERATE: return R"( \from )";
+
   case TokenID::UNION: return R"( \union )";
   case TokenID::INTERSECTION: return R"( \intersect )";
   case TokenID::SET_MINUS: return R"( \setminus )";
   case TokenID::SYMMINUS: return R"( \symmdiff )";
   case TokenID::DECART: return "*";
 
   case TokenID::BOOLEAN: return "B";
 
   case TokenID::PUNC_DEFINE: return R"( \defexpr )";
   case TokenID::PUNC_STRUCT: return R"( \deftype )";
-  case TokenID::PUNC_ASSIGN: return R"( \assign )";
-  case TokenID::PUNC_ITERATE: return R"( \from )";
   }
 }
 
 [[nodiscard]] std::string RSStr(const TokenID id) {
   switch (id) {
   default: return SharedStr(id);
 
@@ -170,32 +167,33 @@
   case TokenID::EXISTS: return "\xE2\x88\x83"; // \u2203
   case TokenID::NOT: return "\xC2\xAC"; // \u00AC
   case TokenID::AND: return "&";
   case TokenID::OR: return "\xE2\x88\xA8"; // \u2228
   case TokenID::IMPLICATION: return "\xE2\x87\x92"; // \u21D2
   case TokenID::EQUIVALENT: return "\xE2\x87\x94"; // \u21D4
 
-  case TokenID::PUNC_DEFINE: return ":==";
-  case TokenID::PUNC_STRUCT: return "::=";
-  case TokenID::PUNC_ASSIGN: return ":=";
-  case TokenID::PUNC_ITERATE: return ":\xE2\x88\x88"; // \u2208
+  case TokenID::ASSIGN: return ":=";
+  case TokenID::ITERATE: return ":\xE2\x88\x88"; // \u2208
 
   case TokenID::IN: return "\xE2\x88\x88"; // \u2208
   case TokenID::NOTIN: return "\xE2\x88\x89"; // \u2209
   case TokenID::SUBSET: return "\xE2\x8A\x82"; // \u2282
   case TokenID::SUBSET_OR_EQ: return "\xE2\x8A\x86"; // \u2286
   case TokenID::NOTSUBSET: return "\xE2\x8A\x84"; // \u2284
 
   case TokenID::UNION: return "\xE2\x88\xAA"; // \u222A
   case TokenID::INTERSECTION: return "\xE2\x88\xA9"; // \u2229
   case TokenID::SET_MINUS: return R"(\)";
   case TokenID::SYMMINUS: return "\xE2\x88\x86"; // \u2206
   case TokenID::DECART: return "\xC3\x97"; // \u00D7
 
   case TokenID::BOOLEAN: return "\xE2\x84\xAC"; // \u212C
+
+  case TokenID::PUNC_DEFINE: return ":==";
+  case TokenID::PUNC_STRUCT: return "::=";
   }
 }
 
 } // namespace
 
 bool TokenData::operator==(const TokenData& rhs) const {
   if (!HasValue()) {
@@ -235,40 +233,44 @@
   return id == rhs.id &&
     pos == rhs.pos &&
     data == rhs.data;
 }
 
 std::string Token::ToString(const Syntax syntax) const {
   switch (id) {
-  default: {
-    return Str(id, syntax);
-  }
-  case TokenID::ID_LOCAL: {
-    return ConvertID(data.ToText(), syntax);
-  }
-  case TokenID::ID_GLOBAL:
-  case TokenID::ID_FUNCTION:
-  case TokenID::ID_PREDICATE:
-  case TokenID::ID_RADICAL: {
-    return data.ToText();
-  }
-  case TokenID::LIT_INTEGER: {
-    return std::to_string(data.ToInt());
-  }
-  case TokenID::BIGPR:
-  case TokenID::SMALLPR:
-  case TokenID::FILTER: {
-    const auto& indicies = data.ToTuple();
-    std::string result = Str(id) + std::to_string(*begin(indicies));
-    result += std::accumulate(next(begin(indicies)), end(indicies), std::string{},
-                             [](std::string text, const Index index) -> decltype(auto) {
-                               text += ',';
-                               text += std::to_string(index);
-                               return text;
-                             });
+    default: {
+      return Str(id, syntax);
+    }
+    case TokenID::ID_LOCAL: {
+      return ConvertID(data.ToText(), syntax);
+    }
+    case TokenID::ID_GLOBAL:
+    case TokenID::ID_FUNCTION:
+    case TokenID::ID_PREDICATE:
+    case TokenID::ID_RADICAL: {
+      return data.ToText();
+    }
+    case TokenID::LIT_INTEGER: {
+      return std::to_string(data.ToInt());
+    }
+    case TokenID::BIGPR:
+    case TokenID::SMALLPR:
+    case TokenID::FILTER: {
+      const auto& indicies = data.ToTuple();
+      std::string result = Str(id) + std::to_string(*begin(indicies));
+      result += std::accumulate(
+        next(begin(indicies)),
+        end(indicies),
+        std::string{},
+        [](std::string text, const Index index) -> decltype(auto) {
+          text += ',';
+          text += std::to_string(index);
+          return text;
+        }
+      );
     return result;
   }
   }
 }
 
 std::string Token::Str(const TokenID id, const Syntax syntax) {
   if (syntax == Syntax::MATH) {
```

### Comparing `pyconcept-0.1.4/ccl/rslang/src/SDImplementation.cpp` & `pyconcept-0.1.5/ccl/rslang/src/SDImplementation.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/SDataCompact.cpp` & `pyconcept-0.1.5/ccl/rslang/src/SDataCompact.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/StructuredData.cpp` & `pyconcept-0.1.5/ccl/rslang/src/StructuredData.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/SyntaxTree.cpp` & `pyconcept-0.1.5/ccl/rslang/src/SyntaxTree.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/TypeAuditor.cpp` & `pyconcept-0.1.5/ccl/rslang/src/TypeAuditor.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -694,21 +694,21 @@
     return false;
   }
 
   EndScope(iter->pos.start);
   return SetCurrent(std::get<Typification>(type.value()).Bool());
 }
 
-bool TypeAuditor::ViImpDeclare(Cursor iter) {
+bool TypeAuditor::ViIterate(Cursor iter) {
   const auto domain = ChildTypeDebool(iter, 1, SemanticEID::invalidTypeOperation);
   return domain.has_value() 
     && VisitChildDeclaration(iter, 0, domain.value());
 }
 
-bool TypeAuditor::ViImpAssign(Cursor iter) {
+bool TypeAuditor::ViAssign(Cursor iter) {
   const auto domain = ChildType(iter, 1);
   return domain.has_value()
     && VisitChildDeclaration(iter, 0, std::get<Typification>(domain.value()));
 }
 
 bool TypeAuditor::ViRecursion(Cursor iter) {
   StartScope();
```

### Comparing `pyconcept-0.1.4/ccl/rslang/src/Typification.cpp` & `pyconcept-0.1.5/ccl/rslang/src/Typification.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/src/ValueAuditor.cpp` & `pyconcept-0.1.5/ccl/rslang/src/ValueAuditor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/unity/reflex_unity1.cpp` & `pyconcept-0.1.5/ccl/rslang/unity/reflex_unity1.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/ccl/rslang/unity/reflex_unity2.cpp` & `pyconcept-0.1.5/ccl/rslang/unity/reflex_unity2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/cmake/CXXTargets.cmake` & `pyconcept-0.1.5/cmake/CXXTargets.cmake`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/include/pyconcept.h` & `pyconcept-0.1.5/include/pyconcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/pyconcept.egg-info/PKG-INFO` & `pyconcept-0.1.5/pyconcept.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconcept
-Version: 0.1.4
+Version: 0.1.5
 Summary: Concept core Python wrapper
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Project-URL: GitHub, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept
 Project-URL: Changelog, https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyconcept-0.1.4/pyconcept.egg-info/SOURCES.txt` & `pyconcept-0.1.5/pyconcept.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/setup.cfg` & `pyconcept-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/setup.py` & `pyconcept-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/src/pyconcept.cpp` & `pyconcept-0.1.5/src/pyconcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/tests/__pycache__/testBinding.cpython-312.pyc` & `pyconcept-0.1.5/tests/__pycache__/testBinding.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/tests/data/Schema1.trs` & `pyconcept-0.1.5/tests/data/Schema1.trs`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.4/tests/testBinding.py` & `pyconcept-0.1.5/tests/testBinding.py`

 * *Files identical despite different names*

