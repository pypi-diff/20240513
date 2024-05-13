# Comparing `tmp/nanomotif-0.4.0.tar.gz` & `tmp/nanomotif-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomotif-0.4.0.tar", last modified: Fri May 10 11:39:11 2024, max compression
+gzip compressed data, was "nanomotif-0.4.1.tar", last modified: Mon May 13 08:59:14 2024, max compression
```

## Comparing `nanomotif-0.4.0.tar` & `nanomotif-0.4.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/
--rw-rw-r--   0 shei      (1000) shei      (1000)     1084 2023-11-30 15:56:56.000000 nanomotif-0.4.0/LICENSE
--rw-r--r--   0 shei      (1000) shei      (1000)     7424 2024-05-10 11:39:11.674436 nanomotif-0.4.0/PKG-INFO
--rw-rw-r--   0 shei      (1000) shei      (1000)     6868 2024-05-10 11:37:33.000000 nanomotif-0.4.0/README.md
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.646436 nanomotif-0.4.0/nanomotif/
--rw-rw-r--   0 shei      (1000) shei      (1000)      278 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)       22 2024-05-10 11:37:33.000000 nanomotif-0.4.0/nanomotif/_version.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    11266 2024-05-10 11:37:33.000000 nanomotif-0.4.0/nanomotif/argparser.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     6016 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/bin_consensus.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.650436 nanomotif-0.4.0/nanomotif/binnary/
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/binnary/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    13167 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/binnary/analysis.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    15629 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/binnary/data_processing.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     3729 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/binnary/detect_contamination.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     3014 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/binnary/include_contigs.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      890 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/binnary/logging.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     9127 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/binnary/scoring.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      522 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/binnary/utils.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    14165 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/candidate.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1078 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/constants.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1698 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/dataload.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.650436 nanomotif-0.4.0/nanomotif/datasets/
--rw-rw-r--   0 shei      (1000) shei      (1000)       27 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/datasets/geobacillus-contig-bin.tsv
--rw-rw-r--   0 shei      (1000) shei      (1000)   176247 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
--rw-rw-r--   0 shei      (1000) shei      (1000) 26479844 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed
--rw-rw-r--   0 shei      (1000) shei      (1000)     1106 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/datasets.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    28603 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/evaluate.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      539 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/feature.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      321 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/logger.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    19809 2024-05-10 11:37:33.000000 nanomotif-0.4.0/nanomotif/main.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1037 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/model.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/nanomotif/mtase_linker/
--rw-rw-r--   0 shei      (1000) shei      (1000)       47 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/mtase_linker/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     5051 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/mtase_linker/command.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     3615 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/mtase_linker/dependencies.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     5639 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/old_search_method.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      850 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/parallel.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     6202 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/postprocess.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     7193 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/scoremotifs.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      197 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/seed.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    20090 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/seq.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2677 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/utils.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/nanomotif.egg-info/
--rw-r--r--   0 shei      (1000) shei      (1000)     7424 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/PKG-INFO
--rw-rw-r--   0 shei      (1000) shei      (1000)     1714 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/SOURCES.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)        1 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/dependency_links.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)       50 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/entry_points.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)        1 2023-11-30 15:56:57.000000 nanomotif-0.4.0/nanomotif.egg-info/not-zip-safe
--rw-rw-r--   0 shei      (1000) shei      (1000)      150 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/requires.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)       16 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/top_level.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)       38 2024-05-10 11:39:11.678436 nanomotif-0.4.0/setup.cfg
--rw-rw-r--   0 shei      (1000) shei      (1000)      947 2024-05-10 09:55:21.000000 nanomotif-0.4.0/setup.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/tests/
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2023-11-30 15:56:56.000000 nanomotif-0.4.0/tests/__init__.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/tests/binnary/
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2089 2024-05-10 09:55:21.000000 nanomotif-0.4.0/tests/binnary/conftest.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1019 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_arg_parser.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    11132 2024-05-10 09:55:21.000000 nanomotif-0.4.0/tests/binnary/test_cli_commands.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     6352 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_data_processing_functions.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2585 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_detect_contamination.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1404 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_generate_output.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2132 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_include_contigs.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     3317 2024-05-10 09:55:21.000000 nanomotif-0.4.0/tests/binnary/test_scoring.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      744 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_utils.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     5405 2024-05-10 09:55:21.000000 nanomotif-0.4.0/tests/binnary/test_write_bins.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     7236 2023-11-30 15:56:57.000000 nanomotif-0.4.0/tests/test_candidate.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1365 2024-03-29 11:56:23.000000 nanomotif-0.4.0/tests/test_dataload.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2933 2024-03-29 11:56:23.000000 nanomotif-0.4.0/tests/test_motif_find.py
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 11:56:23.000000 nanomotif-0.4.0/tests/test_motif_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:14.266636 nanomotif-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 08:59:10.000000 nanomotif-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-05-13 08:59:14.266636 nanomotif-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-13 08:59:10.000000 nanomotif-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:14.226636 nanomotif-0.4.1/nanomotif/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/bin_consensus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:14.230636 nanomotif-0.4.1/nanomotif/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/binnary/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/binnary/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/binnary/detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/binnary/include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/binnary/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/binnary/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/binnary/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/dataload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:14.230636 nanomotif-0.4.1/nanomotif/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/datasets/geobacillus-contig-bin.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   176247 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
+-rw-r--r--   0 runner    (1001) docker     (127) 26479844 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28603 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:14.262636 nanomotif-0.4.1/nanomotif/mtase_linker/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/mtase_linker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/mtase_linker/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/mtase_linker/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/old_search_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/scoremotifs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-13 08:59:10.000000 nanomotif-0.4.1/nanomotif/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:14.266636 nanomotif-0.4.1/nanomotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-05-13 08:59:14.000000 nanomotif-0.4.1/nanomotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-13 08:59:14.000000 nanomotif-0.4.1/nanomotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:59:14.000000 nanomotif-0.4.1/nanomotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 08:59:14.000000 nanomotif-0.4.1/nanomotif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:59:14.000000 nanomotif-0.4.1/nanomotif.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 08:59:14.000000 nanomotif-0.4.1/nanomotif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 08:59:14.000000 nanomotif-0.4.1/nanomotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:59:14.266636 nanomotif-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-13 08:59:10.000000 nanomotif-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:14.262636 nanomotif-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:14.266636 nanomotif-0.4.1/tests/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/test_arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/test_cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/test_data_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/test_detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/test_generate_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/test_include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/test_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/binnary/test_write_bins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/test_candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/test_dataload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/test_motif_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:59:10.000000 nanomotif-0.4.1/tests/test_motif_score.py
```

### Comparing `nanomotif-0.4.0/LICENSE` & `nanomotif-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/PKG-INFO` & `nanomotif-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.4.0
+Version: 0.4.1
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -69,40 +69,40 @@
 #### Required files
 
 To identify methylated motifs, the following files are required: 
 - Assembly (fasta file)
 - [modkit](https://github.com/nanoporetech/modkit/blob/master/book/src/advanced_usage.md#pileup) methylation pileup
 - tab-separated file describing `contig-bin` relationship.
 
-For further details, check out the [required files]() documentation.
+For further details, check out the [required files](https://nanomotif.readthedocs.io/en/latest/required_files.html) documentation.
 
 
 #### Motif discovery
 
 Whether you are interested in finding methylated motifs in monoculture samples or metagenomic samples, we recomment just running `motif_discovery`
 
 ```
 nanomotif motif_discovery ASSEMBLY.fasta PILEUP.bed CONTIG_BIN.tsv -t THREADS --out OUT
 ```
 
 This will create three files: `motifs.tsv`,`motif-scored.tsv`, and `bin-motifs.tsv`. Highly methylated motifs are found in `bin-motifs.tsv`.
 
-See [usage]() and [output]() for detailed usage and output information.
+See [usage](https://nanomotif.readthedocs.io/en/latest/usage.html) and [output](https://nanomotif.readthedocs.io/en/latest/output.html) for detailed usage and output information.
 
 #### Bin contamination
 After motif identification it is possible to identify contamination in bins using the `bin-motifs.tsv`, `contig-bin.tsv` and `motif-scored.tsv` files.
 
 ```
 nanomotif detect_contamination --motifs_scored MOTIFS_SCORED.tsv --bin_motifs BIN_MOTIFS.tsv --contig_bins CONTIG_BINS.tsv -t THREADS --out OUT
 ```
 This will generate a bin_contamination.tsv specifying the contigs, which is flagged as contamination.
 
 If the --write_bins and the --assembly_file flags are specified new de-contaminated bins will be written to a bins folder.
 
-See [usage]() and [output]() for detailed usage and output information.
+See [usage](https://nanomotif.readthedocs.io/en/latest/usage.html) and [output](https://nanomotif.readthedocs.io/en/latest/output.html) for detailed usage and output information.
 
 #### Include unbinned contigs
 The `include_contigs` command assigns unbinned contigs in the assembly file to bins by comparing the methylation pattern of the contig to the bin consensus pattern. The contig must have a unique perfect match to the bin consensus pattern to be assigned to a bin. Additionally, the `include_contigs` assigns all the contigs in the `bin_contamination.tsv` file as unbinned. 
 
 ```
 nanomotif include_contigs --motifs_scored MOTIFS_SCORED.tsv --bin_motifs BIN_MOTIFS.tsv --contig_bins CONTIG_BINS.tsv --run_detect_contamination -t THREADS --out OUT
 ```
@@ -133,15 +133,15 @@
 
 Running the nanomotif MTase-linker run command will generate two primary output files: mtase_assignment_table.tsv and nanomotif_assignment_table.tsv. The first file lists all predicted MTase genes in the genome along with their predicted methylation characteristics and whether the module was able to unambiguously assign any detected motifs to the MTase (`linked` = (True/False)).
 The second file includes data from the bin-motifs.tsv of the nanomotif output with two additional columns `linked` and `candidate_genes`. The `linked` variable is a boolean indicator if the motif could be unambiguously linked to a MTase in the bin/genome (TRUE/FALSE). If True the gene_id of the MTase is provided in `candidate_gene`. If False, the `candidate_gene` variable lists feasible candidate facilitators of the modification based on motif type and modification type predictions.
 
 ## Citation
 
 Nanomotif: Identification and Exploitation of DNA Methylation Motifs in Metagenomes using Oxford Nanopore Sequencing
-SØren Heidelbach, Sebastian Mølvang Dall, Jeppe Støtt Bøjer, Jacob Nissen, Lucas Nicolaas Ludovic van der Maas, Mantas Sereika, Rasmus Kirkegaard, Sabrina Just Kousgaard, Ole Thorlacius-Ussing, Sheila I Jensen, Katja Hose, Thomas Dyhre Nielsen, Mads Albertsen. Preprint at *bioRxiv* https://doi.org/10.1101/2024.04.29.591623 (2024)
+Søren Heidelbach, Sebastian Mølvang Dall, Jeppe Støtt Bøjer, Jacob Nissen, Lucas Nicolaas Ludovic van der Maas, Mantas Sereika, Rasmus Kirkegaard, Sabrina Just Kousgaard, Ole Thorlacius-Ussing, Sheila I Jensen, Katja Hose, Thomas Dyhre Nielsen, Mads Albertsen. Preprint at *bioRxiv* https://doi.org/10.1101/2024.04.29.591623 (2024)
 
 ## License
 
 Nanomotif is released under the [MIT License](https://github.com/your-username/nanomotif/blob/main/LICENSE). Feel free to use, modify, and distribute the package in accordance with the terms of the license.
 
 ## Acknowledgments
```

### Comparing `nanomotif-0.4.0/README.md` & `nanomotif-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,40 +48,40 @@
 #### Required files
 
 To identify methylated motifs, the following files are required: 
 - Assembly (fasta file)
 - [modkit](https://github.com/nanoporetech/modkit/blob/master/book/src/advanced_usage.md#pileup) methylation pileup
 - tab-separated file describing `contig-bin` relationship.
 
-For further details, check out the [required files]() documentation.
+For further details, check out the [required files](https://nanomotif.readthedocs.io/en/latest/required_files.html) documentation.
 
 
 #### Motif discovery
 
 Whether you are interested in finding methylated motifs in monoculture samples or metagenomic samples, we recomment just running `motif_discovery`
 
 ```
 nanomotif motif_discovery ASSEMBLY.fasta PILEUP.bed CONTIG_BIN.tsv -t THREADS --out OUT
 ```
 
 This will create three files: `motifs.tsv`,`motif-scored.tsv`, and `bin-motifs.tsv`. Highly methylated motifs are found in `bin-motifs.tsv`.
 
-See [usage]() and [output]() for detailed usage and output information.
+See [usage](https://nanomotif.readthedocs.io/en/latest/usage.html) and [output](https://nanomotif.readthedocs.io/en/latest/output.html) for detailed usage and output information.
 
 #### Bin contamination
 After motif identification it is possible to identify contamination in bins using the `bin-motifs.tsv`, `contig-bin.tsv` and `motif-scored.tsv` files.
 
 ```
 nanomotif detect_contamination --motifs_scored MOTIFS_SCORED.tsv --bin_motifs BIN_MOTIFS.tsv --contig_bins CONTIG_BINS.tsv -t THREADS --out OUT
 ```
 This will generate a bin_contamination.tsv specifying the contigs, which is flagged as contamination.
 
 If the --write_bins and the --assembly_file flags are specified new de-contaminated bins will be written to a bins folder.
 
-See [usage]() and [output]() for detailed usage and output information.
+See [usage](https://nanomotif.readthedocs.io/en/latest/usage.html) and [output](https://nanomotif.readthedocs.io/en/latest/output.html) for detailed usage and output information.
 
 #### Include unbinned contigs
 The `include_contigs` command assigns unbinned contigs in the assembly file to bins by comparing the methylation pattern of the contig to the bin consensus pattern. The contig must have a unique perfect match to the bin consensus pattern to be assigned to a bin. Additionally, the `include_contigs` assigns all the contigs in the `bin_contamination.tsv` file as unbinned. 
 
 ```
 nanomotif include_contigs --motifs_scored MOTIFS_SCORED.tsv --bin_motifs BIN_MOTIFS.tsv --contig_bins CONTIG_BINS.tsv --run_detect_contamination -t THREADS --out OUT
 ```
@@ -112,15 +112,15 @@
 
 Running the nanomotif MTase-linker run command will generate two primary output files: mtase_assignment_table.tsv and nanomotif_assignment_table.tsv. The first file lists all predicted MTase genes in the genome along with their predicted methylation characteristics and whether the module was able to unambiguously assign any detected motifs to the MTase (`linked` = (True/False)).
 The second file includes data from the bin-motifs.tsv of the nanomotif output with two additional columns `linked` and `candidate_genes`. The `linked` variable is a boolean indicator if the motif could be unambiguously linked to a MTase in the bin/genome (TRUE/FALSE). If True the gene_id of the MTase is provided in `candidate_gene`. If False, the `candidate_gene` variable lists feasible candidate facilitators of the modification based on motif type and modification type predictions.
 
 ## Citation
 
 Nanomotif: Identification and Exploitation of DNA Methylation Motifs in Metagenomes using Oxford Nanopore Sequencing
-SØren Heidelbach, Sebastian Mølvang Dall, Jeppe Støtt Bøjer, Jacob Nissen, Lucas Nicolaas Ludovic van der Maas, Mantas Sereika, Rasmus Kirkegaard, Sabrina Just Kousgaard, Ole Thorlacius-Ussing, Sheila I Jensen, Katja Hose, Thomas Dyhre Nielsen, Mads Albertsen. Preprint at *bioRxiv* https://doi.org/10.1101/2024.04.29.591623 (2024)
+Søren Heidelbach, Sebastian Mølvang Dall, Jeppe Støtt Bøjer, Jacob Nissen, Lucas Nicolaas Ludovic van der Maas, Mantas Sereika, Rasmus Kirkegaard, Sabrina Just Kousgaard, Ole Thorlacius-Ussing, Sheila I Jensen, Katja Hose, Thomas Dyhre Nielsen, Mads Albertsen. Preprint at *bioRxiv* https://doi.org/10.1101/2024.04.29.591623 (2024)
 
 ## License
 
 Nanomotif is released under the [MIT License](https://github.com/your-username/nanomotif/blob/main/LICENSE). Feel free to use, modify, and distribute the package in accordance with the terms of the license.
 
 ## Acknowledgments
```

### Comparing `nanomotif-0.4.0/nanomotif/argparser.py` & `nanomotif-0.4.1/nanomotif/argparser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/bin_consensus.py` & `nanomotif-0.4.1/nanomotif/bin_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/binnary/analysis.py` & `nanomotif-0.4.1/nanomotif/binnary/analysis.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/binnary/data_processing.py` & `nanomotif-0.4.1/nanomotif/binnary/data_processing.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/binnary/detect_contamination.py` & `nanomotif-0.4.1/nanomotif/binnary/detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/binnary/include_contigs.py` & `nanomotif-0.4.1/nanomotif/binnary/include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/binnary/logging.py` & `nanomotif-0.4.1/nanomotif/binnary/logging.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/binnary/scoring.py` & `nanomotif-0.4.1/nanomotif/binnary/scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/binnary/utils.py` & `nanomotif-0.4.1/nanomotif/binnary/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/candidate.py` & `nanomotif-0.4.1/nanomotif/candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/constants.py` & `nanomotif-0.4.1/nanomotif/constants.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/dataload.py` & `nanomotif-0.4.1/nanomotif/dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta` & `nanomotif-0.4.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed` & `nanomotif-0.4.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/datasets.py` & `nanomotif-0.4.1/nanomotif/datasets.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/evaluate.py` & `nanomotif-0.4.1/nanomotif/evaluate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/feature.py` & `nanomotif-0.4.1/nanomotif/feature.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/main.py` & `nanomotif-0.4.1/nanomotif/main.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/model.py` & `nanomotif-0.4.1/nanomotif/model.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/mtase_linker/command.py` & `nanomotif-0.4.1/nanomotif/mtase_linker/command.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/mtase_linker/dependencies.py` & `nanomotif-0.4.1/nanomotif/mtase_linker/dependencies.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/old_search_method.py` & `nanomotif-0.4.1/nanomotif/old_search_method.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/parallel.py` & `nanomotif-0.4.1/nanomotif/parallel.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/postprocess.py` & `nanomotif-0.4.1/nanomotif/postprocess.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/scoremotifs.py` & `nanomotif-0.4.1/nanomotif/scoremotifs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/seq.py` & `nanomotif-0.4.1/nanomotif/seq.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif/utils.py` & `nanomotif-0.4.1/nanomotif/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/nanomotif.egg-info/PKG-INFO` & `nanomotif-0.4.1/nanomotif.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.4.0
+Version: 0.4.1
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -69,40 +69,40 @@
 #### Required files
 
 To identify methylated motifs, the following files are required: 
 - Assembly (fasta file)
 - [modkit](https://github.com/nanoporetech/modkit/blob/master/book/src/advanced_usage.md#pileup) methylation pileup
 - tab-separated file describing `contig-bin` relationship.
 
-For further details, check out the [required files]() documentation.
+For further details, check out the [required files](https://nanomotif.readthedocs.io/en/latest/required_files.html) documentation.
 
 
 #### Motif discovery
 
 Whether you are interested in finding methylated motifs in monoculture samples or metagenomic samples, we recomment just running `motif_discovery`
 
 ```
 nanomotif motif_discovery ASSEMBLY.fasta PILEUP.bed CONTIG_BIN.tsv -t THREADS --out OUT
 ```
 
 This will create three files: `motifs.tsv`,`motif-scored.tsv`, and `bin-motifs.tsv`. Highly methylated motifs are found in `bin-motifs.tsv`.
 
-See [usage]() and [output]() for detailed usage and output information.
+See [usage](https://nanomotif.readthedocs.io/en/latest/usage.html) and [output](https://nanomotif.readthedocs.io/en/latest/output.html) for detailed usage and output information.
 
 #### Bin contamination
 After motif identification it is possible to identify contamination in bins using the `bin-motifs.tsv`, `contig-bin.tsv` and `motif-scored.tsv` files.
 
 ```
 nanomotif detect_contamination --motifs_scored MOTIFS_SCORED.tsv --bin_motifs BIN_MOTIFS.tsv --contig_bins CONTIG_BINS.tsv -t THREADS --out OUT
 ```
 This will generate a bin_contamination.tsv specifying the contigs, which is flagged as contamination.
 
 If the --write_bins and the --assembly_file flags are specified new de-contaminated bins will be written to a bins folder.
 
-See [usage]() and [output]() for detailed usage and output information.
+See [usage](https://nanomotif.readthedocs.io/en/latest/usage.html) and [output](https://nanomotif.readthedocs.io/en/latest/output.html) for detailed usage and output information.
 
 #### Include unbinned contigs
 The `include_contigs` command assigns unbinned contigs in the assembly file to bins by comparing the methylation pattern of the contig to the bin consensus pattern. The contig must have a unique perfect match to the bin consensus pattern to be assigned to a bin. Additionally, the `include_contigs` assigns all the contigs in the `bin_contamination.tsv` file as unbinned. 
 
 ```
 nanomotif include_contigs --motifs_scored MOTIFS_SCORED.tsv --bin_motifs BIN_MOTIFS.tsv --contig_bins CONTIG_BINS.tsv --run_detect_contamination -t THREADS --out OUT
 ```
@@ -133,15 +133,15 @@
 
 Running the nanomotif MTase-linker run command will generate two primary output files: mtase_assignment_table.tsv and nanomotif_assignment_table.tsv. The first file lists all predicted MTase genes in the genome along with their predicted methylation characteristics and whether the module was able to unambiguously assign any detected motifs to the MTase (`linked` = (True/False)).
 The second file includes data from the bin-motifs.tsv of the nanomotif output with two additional columns `linked` and `candidate_genes`. The `linked` variable is a boolean indicator if the motif could be unambiguously linked to a MTase in the bin/genome (TRUE/FALSE). If True the gene_id of the MTase is provided in `candidate_gene`. If False, the `candidate_gene` variable lists feasible candidate facilitators of the modification based on motif type and modification type predictions.
 
 ## Citation
 
 Nanomotif: Identification and Exploitation of DNA Methylation Motifs in Metagenomes using Oxford Nanopore Sequencing
-SØren Heidelbach, Sebastian Mølvang Dall, Jeppe Støtt Bøjer, Jacob Nissen, Lucas Nicolaas Ludovic van der Maas, Mantas Sereika, Rasmus Kirkegaard, Sabrina Just Kousgaard, Ole Thorlacius-Ussing, Sheila I Jensen, Katja Hose, Thomas Dyhre Nielsen, Mads Albertsen. Preprint at *bioRxiv* https://doi.org/10.1101/2024.04.29.591623 (2024)
+Søren Heidelbach, Sebastian Mølvang Dall, Jeppe Støtt Bøjer, Jacob Nissen, Lucas Nicolaas Ludovic van der Maas, Mantas Sereika, Rasmus Kirkegaard, Sabrina Just Kousgaard, Ole Thorlacius-Ussing, Sheila I Jensen, Katja Hose, Thomas Dyhre Nielsen, Mads Albertsen. Preprint at *bioRxiv* https://doi.org/10.1101/2024.04.29.591623 (2024)
 
 ## License
 
 Nanomotif is released under the [MIT License](https://github.com/your-username/nanomotif/blob/main/LICENSE). Feel free to use, modify, and distribute the package in accordance with the terms of the license.
 
 ## Acknowledgments
```

### Comparing `nanomotif-0.4.0/nanomotif.egg-info/SOURCES.txt` & `nanomotif-0.4.1/nanomotif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/setup.py` & `nanomotif-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/conftest.py` & `nanomotif-0.4.1/tests/binnary/conftest.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/test_arg_parser.py` & `nanomotif-0.4.1/tests/binnary/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/test_cli_commands.py` & `nanomotif-0.4.1/tests/binnary/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/test_data_processing_functions.py` & `nanomotif-0.4.1/tests/binnary/test_data_processing_functions.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/test_detect_contamination.py` & `nanomotif-0.4.1/tests/binnary/test_detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/test_generate_output.py` & `nanomotif-0.4.1/tests/binnary/test_generate_output.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/test_include_contigs.py` & `nanomotif-0.4.1/tests/binnary/test_include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/test_scoring.py` & `nanomotif-0.4.1/tests/binnary/test_scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/test_utils.py` & `nanomotif-0.4.1/tests/binnary/test_utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/binnary/test_write_bins.py` & `nanomotif-0.4.1/tests/binnary/test_write_bins.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/test_candidate.py` & `nanomotif-0.4.1/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/test_dataload.py` & `nanomotif-0.4.1/tests/test_dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.0/tests/test_motif_find.py` & `nanomotif-0.4.1/tests/test_motif_find.py`

 * *Files identical despite different names*

