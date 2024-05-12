# Comparing `tmp/hyped-0.1.0a1.tar.gz` & `tmp/hyped-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyped-0.1.0a1.tar", last modified: Wed May  1 14:22:00 2024, max compression
+gzip compressed data, was "hyped-0.1.0a2.tar", last modified: Sun May 12 23:12:14 2024, max compression
```

## Comparing `hyped-0.1.0a1.tar` & `hyped-0.1.0a2.tar`

### file list

```diff
@@ -1,191 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.692628 hyped-0.1.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.656629 hyped-0.1.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-01 14:21:33.000000 hyped-0.1.0a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 14:21:33.000000 hyped-0.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-01 14:22:00.692628 hyped-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-01 14:21:33.000000 hyped-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/add_ons.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/api/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/costum_data_processors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/feature_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/statistic_processors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-01 14:21:33.000000 hyped-0.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-01 14:21:33.000000 hyped-0.1.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:22:00.692628 hyped-0.1.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.656629 hyped-0.1.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/src/hyped/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.668629 hyped-0.1.0a1/src/hyped/base/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.668629 hyped-0.1.0a1/src/hyped/common/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/feature_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/feature_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.668629 hyped-0.1.0a1/src/hyped/data/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.668629 hyped-0.1.0a1/src/hyped/data/io/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/io/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/datasets/cas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/datasets/typed_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/io/writers/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/writers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/writers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/writers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/processors/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21294 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/processors/features/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/features/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/features/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/features/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/processors/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/apply_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/join_str_seq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/spans/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/apply_idx_spans.py
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/from_bio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/from_word_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/idx_spans.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/loc_to_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/overlaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/disc_seq_val_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/seq_len_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/seq_val_hist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/disc_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/mean_and_std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/taggers/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/taggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/taggers/bio.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/taggers/relex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/tokenizers/hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/src/hyped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/base/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/base/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/base/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_feature_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17355 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_feature_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/data/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/data/io/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/datasets/test_cas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/datasets/test_typed_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.684629 hyped-0.1.0a1/tests/hyped/data/io/writers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/writers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/writers/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/writers/test_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.684629 hyped-0.1.0a1/tests/hyped/data/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.684629 hyped-0.1.0a1/tests/hyped/data/processors/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/features/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/features/test_flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/features/test_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.684629 hyped-0.1.0a1/tests/hyped/data/processors/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_apply_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_join_str_seq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/spans/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_apply_idx_spans.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_from_bio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_from_word_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_idx_spans.py
--rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_loc_to_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_overlaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/test_disc_seq_val_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/test_seq_len_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/test_seq_val_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/test_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_disc_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_mean_and_std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/taggers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/taggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/taggers/test_bio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/taggers/test_relex.py
--rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/tokenizers/test_hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12943 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/test_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.729608 hyped-0.1.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.693607 hyped-0.1.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.701607 hyped-0.1.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-12 23:11:35.000000 hyped-0.1.0a2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-12 23:11:35.000000 hyped-0.1.0a2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-12 23:11:35.000000 hyped-0.1.0a2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-12 23:11:35.000000 hyped-0.1.0a2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-12 23:11:35.000000 hyped-0.1.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-12 23:11:35.000000 hyped-0.1.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-12 23:11:35.000000 hyped-0.1.0a2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 23:11:35.000000 hyped-0.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-05-12 23:12:14.729608 hyped-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-12 23:11:35.000000 hyped-0.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.701607 hyped-0.1.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.701607 hyped-0.1.0a2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/source/add_ons.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.701607 hyped-0.1.0a2/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/source/api/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/source/data_pipe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/source/data_processors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/source/feature_access.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-12 23:11:35.000000 hyped-0.1.0a2/docs/source/statistic_processors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-12 23:11:35.000000 hyped-0.1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 23:12:14.729608 hyped-0.1.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.693607 hyped-0.1.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.701607 hyped-0.1.0a2/src/hyped/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-12 23:12:14.000000 hyped-0.1.0a2/src/hyped/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.705608 hyped-0.1.0a2/src/hyped/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/base/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/base/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/base/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.705608 hyped-0.1.0a2/src/hyped/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/common/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/common/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/common/feature_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/common/feature_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/common/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/common/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.705608 hyped-0.1.0a2/src/hyped/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.705608 hyped-0.1.0a2/src/hyped/data/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.705608 hyped-0.1.0a2/src/hyped/data/io/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/io/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/io/datasets/cas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/io/datasets/typed_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.709607 hyped-0.1.0a2/src/hyped/data/io/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/io/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/io/writers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/io/writers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/io/writers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.709607 hyped-0.1.0a2/src/hyped/data/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.709607 hyped-0.1.0a2/src/hyped/data/processors/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16735 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/api/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21674 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.709607 hyped-0.1.0a2/src/hyped/data/processors/features/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/features/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/features/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/features/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.709607 hyped-0.1.0a2/src/hyped/data/processors/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/parsers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/parsers/repair_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.709607 hyped-0.1.0a2/src/hyped/data/processors/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/sequence/apply_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/sequence/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/sequence/extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/sequence/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/sequence/join_str_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.713607 hyped-0.1.0a2/src/hyped/data/processors/spans/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/spans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/spans/apply_idx_spans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/spans/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/spans/from_bio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/spans/from_word_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/spans/idx_spans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/spans/loc_to_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/spans/overlaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.713607 hyped-0.1.0a2/src/hyped/data/processors/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.713607 hyped-0.1.0a2/src/hyped/data/processors/statistics/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/sequence/disc_seq_val_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/sequence/seq_len_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/sequence/seq_val_hist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.713607 hyped-0.1.0a2/src/hyped/data/processors/statistics/value/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/value/disc_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/value/hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/statistics/value/mean_and_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.713607 hyped-0.1.0a2/src/hyped/data/processors/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/taggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/taggers/bio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/taggers/relex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.717608 hyped-0.1.0a2/src/hyped/data/processors/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/templates/jinja2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.717608 hyped-0.1.0a2/src/hyped/data/processors/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-05-12 23:11:35.000000 hyped-0.1.0a2/src/hyped/data/processors/tokenizers/hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.729608 hyped-0.1.0a2/src/hyped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-05-12 23:12:14.000000 hyped-0.1.0a2/src/hyped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-12 23:12:14.000000 hyped-0.1.0a2/src/hyped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 23:12:14.000000 hyped-0.1.0a2/src/hyped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-12 23:12:14.000000 hyped-0.1.0a2/src/hyped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 23:12:14.000000 hyped-0.1.0a2/src/hyped.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.717608 hyped-0.1.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.717608 hyped-0.1.0a2/tests/hyped/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.717608 hyped-0.1.0a2/tests/hyped/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/base/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/base/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/base/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.717608 hyped-0.1.0a2/tests/hyped/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/common/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/common/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/common/test_feature_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17355 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/common/test_feature_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/common/test_lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.717608 hyped-0.1.0a2/tests/hyped/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.717608 hyped-0.1.0a2/tests/hyped/data/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.721608 hyped-0.1.0a2/tests/hyped/data/io/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/io/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/io/datasets/test_cas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/io/datasets/test_typed_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.721608 hyped-0.1.0a2/tests/hyped/data/io/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/io/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/io/writers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/io/writers/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/io/writers/test_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.721608 hyped-0.1.0a2/tests/hyped/data/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.721608 hyped-0.1.0a2/tests/hyped/data/processors/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/api/test_openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.721608 hyped-0.1.0a2/tests/hyped/data/processors/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/features/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/features/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/features/test_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.721608 hyped-0.1.0a2/tests/hyped/data/processors/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/parsers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/parsers/test_repair_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.725607 hyped-0.1.0a2/tests/hyped/data/processors/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_apply_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_join_str_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.725607 hyped-0.1.0a2/tests/hyped/data/processors/spans/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/spans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/spans/test_apply_idx_spans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/spans/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/spans/test_from_bio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/spans/test_from_word_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/spans/test_idx_spans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/spans/test_loc_to_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/spans/test_overlaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.725607 hyped-0.1.0a2/tests/hyped/data/processors/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.725607 hyped-0.1.0a2/tests/hyped/data/processors/statistics/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/sequence/test_disc_seq_val_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/sequence/test_seq_len_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/sequence/test_seq_val_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.729608 hyped-0.1.0a2/tests/hyped/data/processors/statistics/value/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/value/test_disc_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/value/test_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/statistics/value/test_mean_and_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.729608 hyped-0.1.0a2/tests/hyped/data/processors/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/taggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/taggers/test_bio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/taggers/test_relex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.729608 hyped-0.1.0a2/tests/hyped/data/processors/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/templates/test_jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:12:14.729608 hyped-0.1.0a2/tests/hyped/data/processors/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/processors/tokenizers/test_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14041 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-12 23:11:35.000000 hyped-0.1.0a2/tests/hyped/data/test_pipe.py
```

### Comparing `hyped-0.1.0a1/.github/workflows/docs.yml` & `hyped-0.1.0a2/.github/workflows/docs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -19,16 +19,15 @@
         with:
           python-version: '3.11'
           cache: 'pip'
       
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install -r requirements.txt
-          python -m pip install -e .[docs]
+          python -m pip install -e .[docs,cas,llm]
 
       - name: Build Sphinx Documentation
         run: |
           sphinx-apidoc -e -o docs/source/api src/hyped --tocfile hyped
           make -C docs html
 
       - name: Deploy to Github Pages
```

### Comparing `hyped-0.1.0a1/.github/workflows/linting.yml` & `hyped-0.1.0a2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/.github/workflows/publish.yml` & `hyped-0.1.0a2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/.github/workflows/tests.yml` & `hyped-0.1.0a2/.github/workflows/tests.yml`

 * *Files 11% similar despite different names*

```diff
@@ -29,19 +29,20 @@
 
       - name: Display Python version
         run: python -c "import sys; print(sys.version)"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install -r requirements.txt
-          python -m pip install -e .[tests]
+          python -m pip install -e .[tests,cas,llm]
 
       - name: Run tests
-        run: python -m pytest --cov=src tests
+        run: python -m pytest --cov=src tests -v
 
       - name: Upload coverage report
-        run: coveralls --service=github
+        run: |
+          pip install coveralls[toml]
+          coveralls --service=github
         env:
           COVERALLS_REPO_TOKEN: ${{ secrets.COVERALLS_REPO_TOKEN }}
         if: ${{ matrix.python-version == '3.10' && matrix.os == 'ubuntu-latest' }}
         continue-on-error: true
```

### Comparing `hyped-0.1.0a1/.gitignore` & `hyped-0.1.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/CONTRIBUTING.md` & `hyped-0.1.0a2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/LICENSE` & `hyped-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/PKG-INFO` & `hyped-0.1.0a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyped
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: TODO
 Author: Niclas Doll
 License: Apache 2.0
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
@@ -14,25 +14,28 @@
 Requires-Dist: fsspec<=2023.9.2
 Requires-Dist: torch>=2.2.1
 Requires-Dist: transformers>=4.36.2
 Requires-Dist: networkx>=3.1
 Requires-Dist: matplotlib>=3.8.2
 Requires-Dist: orjson>=3.9.4
 Requires-Dist: pydantic>=2.6.4
+Requires-Dist: json_repair>=0.17.0
+Requires-Dist: nest-asyncio>=1.6.0
 Provides-Extra: linting
 Requires-Dist: pre-commit; extra == "linting"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Provides-Extra: peft
-Requires-Dist: peft>=0.9.0; extra == "peft"
-Requires-Dist: bitsandbytes>=0.42.0; extra == "peft"
+Provides-Extra: cas
+Requires-Dist: dkpro-cassis>=0.8.0; extra == "cas"
+Provides-Extra: llm
+Requires-Dist: openai>=1.23.6; extra == "llm"
 
 # :boom: Hyped
 
 [![Tests](https://github.com/open-hyped/hyped/actions/workflows/tests.yml/badge.svg?branch=hyped-v2)](https://github.com/open-hyped/hyped/actions/workflows/tests.yml)
 [![Linting](https://github.com/open-hyped/hyped/actions/workflows/linting.yml/badge.svg?branch=hyped-v2)](https://github.com/open-hyped/hyped/actions/workflows/linting.yml)
 [![Coverage Status](https://coveralls.io/repos/github/open-hyped/hyped/badge.svg?branch=hyped-v2)](https://coveralls.io/github/open-hyped/hyped?branch=hyped-v2)
 [![PyPi version](https://badgen.net/pypi/v/hyped/)](https://pypi.org/project/hyped)
```

### Comparing `hyped-0.1.0a1/README.md` & `hyped-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/docs/Makefile` & `hyped-0.1.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/docs/make.bat` & `hyped-0.1.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/docs/source/add_ons.rst` & `hyped-0.1.0a2/docs/source/add_ons.rst`

 * *Files 23% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 
 Available Add-Ons
 -----------------
 
 
 Here is a list of available add-ons. Please note that add-ons are developed by the community as well, more may be added in the future:
 
-- `Hyped Serve <https://github.com/open-hyped/hyped-serve>`_: Add real-time serving capabilities to your Hyped pipelines. Serve your model predictions or data processing results via REST API endpoints with ease.
+- `Hyped Serve <https://github.com/open-hyped/hyped.serve>`_: Add real-time serving capabilities to your Hyped pipelines. Serve your model predictions or data processing results via REST API endpoints.
+- `Hyped Distributed <https://github.com/open-hyped/hyped.distributed>`_: Seamless distribution of data pipelines across a `ray <https://docs.ray.io/en/latest/>`_ cluster. Harness the power of parallel computing to optimize your data processing workflows.
```

### Comparing `hyped-0.1.0a1/docs/source/conf.py` & `hyped-0.1.0a2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,30 @@
 import hyped.data.processors.statistics.sequence.seq_len_hist
 import hyped.data.processors.statistics.sequence.seq_val_hist
 import hyped.data.processors.statistics.value.disc_hist
 import hyped.data.processors.statistics.value.hist
 import hyped.data.processors.statistics.value.mean_and_std
 import hyped.data.processors.taggers.bio
 import hyped.data.processors.taggers.relex
+import hyped.data.processors.templates.jinja2
 import hyped.data.processors.tokenizers.hf
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "hyped"
 copyright = "2024, open-hyped"
 author = "open-hyped"
 version = hyped.__version__.__version__
 release = hyped.__version__.__version__
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
-extensions = ["sphinx.ext.autodoc"]
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.autosummary"]
 
 templates_path = ["_templates"]
 exclude_patterns = []
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
```

### Comparing `hyped-0.1.0a1/docs/source/feature_access.rst` & `hyped-0.1.0a2/docs/source/feature_access.rst`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/docs/source/getting_started.rst` & `hyped-0.1.0a2/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/docs/source/index.rst` & `hyped-0.1.0a2/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
 Below is a list of key sections in this documentation, guiding you through installation, basic usage, API references, and more.
 
 .. toctree::
 
    getting_started
    feature_access
+   data_pipe
+   data_processors
    statistic_processors
-   costum_data_processors
    add_ons
 
 .. toctree::
    :maxdepth: 2
    :caption: API References
 
    api/hyped
```

### Comparing `hyped-0.1.0a1/docs/source/statistic_processors.rst` & `hyped-0.1.0a2/docs/source/statistic_processors.rst`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/pyproject.toml` & `hyped-0.1.0a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     "fsspec<=2023.9.2",
     "torch>=2.2.1",
     "transformers>=4.36.2",
     "networkx>=3.1",
     "matplotlib>=3.8.2",
     "orjson>=3.9.4",
     "pydantic>=2.6.4",
+    "json_repair>=0.17.0",
+    "nest-asyncio>=1.6.0",
 ]
 
 [project.optional-dependencies]
 linting = ["pre-commit"]
 tests = ["pytest", "pytest-cov"]
 docs = ["sphinx", "sphinx_rtd_theme"]
-peft = [
-    "peft>=0.9.0",
-    "bitsandbytes>=0.42.0"
-]
+cas = ["dkpro-cassis>=0.8.0"]
+llm = ["openai>=1.23.6"]
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "setuptools_scm>=8.0.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.coverage.run]
 concurrency = ["multiprocessing"]
```

### Comparing `hyped-0.1.0a1/src/hyped/base/auto.py` & `hyped-0.1.0a2/src/hyped/base/auto.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/base/config.py` & `hyped-0.1.0a2/src/hyped/base/config.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/base/generic.py` & `hyped-0.1.0a2/src/hyped/base/generic.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/base/registry.py` & `hyped-0.1.0a2/src/hyped/base/registry.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/common/arrow.py` & `hyped-0.1.0a2/src/hyped/common/arrow.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/common/consumer.py` & `hyped-0.1.0a2/src/hyped/common/consumer.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/common/feature_checks.py` & `hyped-0.1.0a2/src/hyped/common/feature_checks.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/common/feature_key.py` & `hyped-0.1.0a2/src/hyped/common/feature_key.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/common/lazy.py` & `hyped-0.1.0a2/src/hyped/common/lazy.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 
         Arguments:
             factory (Callable[[], T]): instance factory
         """
         self.factory = factory
         self.instance: None | T = None
 
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        """Pickle set state."""
+        self.__dict__.update(state)
+
     def __getattr__(self, name: str) -> Any:
         """Forward all requests to the instance."""
         if self.instance is None:
             self.instance = self.factory()
         # forward all requests to the instance
         return getattr(self.instance, name)
```

### Comparing `hyped-0.1.0a1/src/hyped/data/graph.py` & `hyped-0.1.0a2/src/hyped/data/graph.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/io/datasets/__init__.py` & `hyped-0.1.0a2/src/hyped/data/io/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/io/datasets/cas.py` & `hyped-0.1.0a2/src/hyped/data/io/datasets/cas.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/io/datasets/typed_json.py` & `hyped-0.1.0a2/src/hyped/data/io/datasets/typed_json.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,20 @@
 """Typed JSON Dataset Generator."""
-import datetime
 import io
 from dataclasses import dataclass, field
 from itertools import chain, count
-from typing import Literal
 
 import datasets
 import orjson
 import pyarrow as pa
 import pydantic
 from datasets.packaged_modules.json.json import Json, JsonConfig
 from datasets.utils.file_utils import readline
 
-# map datasets value dtype to
-DATASETS_VALUE_TYPE_MAPPING = {
-    "bool": bool,
-    "int8": int,
-    "int16": int,
-    "int32": int,
-    "int64": int,
-    "uint8": int,
-    "uint16": int,
-    "uint32": int,
-    "uint64": int,
-    "float16": float,
-    "float32": float,
-    "float64": float,
-    "string": str,
-    "large_string": str,
-    "date32": datetime.datetime,
-    "date64": datetime.datetime,
-    "time32": datetime.time,
-    "time64": datetime.time,
-}
-
-
-def pydantic_model_from_features(
-    features: datasets.Features,
-) -> pydantic.BaseModel:
-    """Create a pydantic model from dataset features.
-
-    Arguments:
-        features (Features): datasets features to build the pydantic model for
-
-    Returns:
-        model (pydantic.BaseModel):
-            pydantic model matching the structure of the dataset features.
-    """
-    fields = {}
-    for k, field_type in features.items():
-        if isinstance(field_type, datasets.Value):
-            # get data type for the given field
-            dtype = DATASETS_VALUE_TYPE_MAPPING.get(
-                field_type.dtype, field_type.pa_type.to_pandas_dtype()
-            )
-            # set field
-            fields[k] = (
-                dtype | None,
-                None,
-            )
-
-        elif isinstance(field_type, datasets.ClassLabel):
-            fields[k] = (Literal[tuple(field_type.names)] | None, None)
-
-        elif isinstance(field_type, datasets.Sequence):
-            # infer dtype for sequence values
-            dtype = (
-                pydantic_model_from_features({"field": field_type.feature})
-                .model_fields["field"]
-                .annotation
-            )
-            # set field
-            fields[k] = (list[dtype], pydantic.Field(default_factory=list))
-
-        elif isinstance(field_type, (dict, datasets.Features)):
-            model = pydantic_model_from_features(field_type)
-            # set field
-            fields[k] = (
-                model,
-                pydantic.Field(default_factory=model),
-            )
-
-    return pydantic.create_model(
-        "Model",
-        **fields,
-        __config__=pydantic.ConfigDict(
-            arbitrary_types_allowed=True, validate_assignment=True
-        ),
-    )
+from hyped.common.pydantic import pydantic_model_from_features
 
 
 @dataclass
 class TypedJsonDatasetConfig(JsonConfig):
     """Typed Json Dataset Configuration.
 
     Matches the huggingface datasets json dataset implementation.
```

### Comparing `hyped-0.1.0a1/src/hyped/data/io/writers/base.py` & `hyped-0.1.0a2/src/hyped/data/io/writers/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/io/writers/csv.py` & `hyped-0.1.0a2/src/hyped/data/io/writers/csv.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/io/writers/json.py` & `hyped-0.1.0a2/src/hyped/data/io/writers/json.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/pipe.py` & `hyped-0.1.0a2/src/hyped/data/pipe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 """Data Pipe."""
+from __future__ import annotations
+
 import warnings
 from collections import deque
 from copy import deepcopy
-from typing import Any, Iterable
+from itertools import chain
+from typing import Any, Iterable, Literal
 
 import datasets
 import pyarrow as pa
+from pydantic import Field
 from torch.utils.data import get_worker_info
+from typing_extensions import TypeAlias
 
 from hyped.common.arrow import convert_features_to_arrow_schema
+from hyped.common.feature_checks import check_feature_equals
+from hyped.common.feature_key import FeatureDict, FeatureKey
 from hyped.data.processors.statistics.base import BaseDataStatistic
 from hyped.data.processors.statistics.report import statistics_report_manager
 
-from .processors.base import BaseDataProcessor
+from .processors.base import BaseDataProcessor, BaseDataProcessorConfig
+
+DatasetType: TypeAlias = (
+    datasets.Dataset
+    | datasets.DatasetDict
+    | datasets.IterableDataset
+    | datasets.IterableDatasetDict
+)
+
+
+class DataPipeConfig(BaseDataProcessorConfig):
+    """Data Pipeline Configuration."""
+
+    keep_input_features: Literal[True] = Field(default=True, init_var=False)
+    output_format: Literal[None] = Field(default=None, init_var=False)
 
 
-class DataPipe(list):
+class DataPipe(list, BaseDataProcessor[DataPipeConfig]):
     """Data Pipe.
 
     A Data Pipe is a sequence of data processors. It provides useful
     functionality such as passing a batch of examples through the
     sequence or pipe.
     """
 
@@ -33,125 +54,196 @@
         if not all(isinstance(p, BaseDataProcessor) for p in processors):
             raise TypeError(
                 "All processors used in a data pipe must inherit from `%s`"
                 % BaseDataProcessor
             )
         # initialize pipe as list of processors
         list.__init__(self, processors)
+        BaseDataProcessor.__init__(self, config=DataPipeConfig())
 
-        # save input features
-        # usually the input features can be inferred from the first
-        # data processor in the pipeline, however this doesn't work
-        # in case the pipeline is empty
-        self._in_features: datasets.Features = None
-
-    def prepare(self, features: datasets.Features) -> datasets.Features:
-        """Prepare all data processors of the data pipe for execution.
+    @classmethod
+    def from_config(cls, config: DataPipeConfig) -> DataPipe:
+        """Instantiate data pipe from the given config.
 
         Arguments:
-            features (Features):
-                input dataset features available to the processor on execution
+            config (DataPipeConfig):
+                data pipe configuration
 
         Returns:
-            out_features (Features):
-                dataset features of the output of the processor
+            pipe (DataPipe):
+                data pipeline
         """
-        # save a copy of the input features
-        self._in_features = deepcopy(features)
-        # prepare all processors
-        for p in self:
-            features = p.prepare(features)
-        # return final output features
-        return self.out_features
+        raise NotImplementedError()
 
     @property
     def is_prepared(self) -> bool:
         """Check if the data pipe is prepared and ready for execution.
 
         This also verifies the feature pipe, i.e. checks that the output
         of any processor matches the input of the following one.
         """
         return (
             # check all processors of the pipe
             all(p.is_prepared for p in self)
-            and all(
-                p1.out_features == p2.in_features
-                for p1, p2 in zip(self[:-1], self[1:])
+            and (self._in_features is not None)
+            and (
+                (len(self) == 0)
+                or (
+                    check_feature_equals(
+                        self[0].in_features, self._in_features
+                    )
+                    and all(
+                        check_feature_equals(p1.out_features, p2.in_features)
+                        for p1, p2 in zip(self[:-1], self[1:])
+                    )
+                )
             )
         )
 
+    def map_features(self, features: datasets.Features) -> datasets.Features:
+        """Prepare all data processors of the data pipe for execution.
+
+        Arguments:
+            features (Features):
+                input dataset features available to the processor on execution
+
+        Returns:
+            out_features (Features):
+                dataset features of the output of the processor
+        """
+        # prepare all processors
+        for p in self:
+            features = p.prepare(features)
+        # return final output features
+        return features
+
     @property
-    def in_features(self) -> datasets.Features:
-        """Input dataset features available to data pipe."""
-        return self[0].in_features if len(self) > 0 else self._in_features
+    def required_feature_keys(self) -> list[FeatureKey]:
+        """List of all required feature keys."""
+        if not self.is_prepared:
+            raise RuntimeError("Data pipe not prepared")
+
+        required_keys = set()
+        new_features = datasets.Features()
+
+        def _feature_exists(
+            key: FeatureKey, features: datasets.Features
+        ) -> bool:
+            """Check whether a feature at a key exists."""
+            try:
+                key.index_features(features)
+                return True
+            except (KeyError, IndexError):
+                return False
+
+        for proc in self:
+            # update required feature keys with all feature keys that are not
+            # present in the features up to this point
+            required_keys.update(
+                {
+                    k
+                    for k in proc.required_feature_keys
+                    if not _feature_exists(k, new_features)
+                }
+            )
+            # keep track of features created within the data pipe
+            new_features = new_features | proc.new_features
+
+        return required_keys
 
     @property
-    def new_features(self) -> datasets.Features:
-        """New dataset features generated by data pipe."""
+    def raw_features(self) -> datasets.Features:
+        """Raw dataset features generated by data pipe."""
         # aggregate all new features created through the pipe
         # TODO: this only accumulates all generated features
         #       but does not handle the removal of features
         #       throughout the pipeline by for example a filter
         #       features processor
         features = datasets.Features()
         for p in self:
             features.update(p.new_features)
 
         return features
 
     @property
-    def out_features(self) -> datasets.Features:
-        """All output features of the processor.
+    def new_features(self) -> datasets.Features:
+        """New dataset features generated by data pipe."""
+        return self.raw_features
 
-        Includes both input features and new features generated by the data
-        pipe. On conflicts, the new features are prioritized.
-        """
-        return self[-1].out_features if len(self) > 0 else self.in_features
+    @property
+    def out_features(self) -> datasets.Features:
+        """All output dataset features."""
+        return self.in_features if len(self) == 0 else self[-1].out_features
 
     def batch_process(
         self,
         examples: dict[str, list[Any]],
         index: list[int],
         rank: None | int = None,
-    ) -> dict[str, list[Any]]:
+        return_index: bool = False,
+    ) -> dict[str, list[Any]] | tuple[dict[str, list[Any]], list[int]]:
         """Process a batch of examples.
 
         Arguments:
-            examples (dict[str, list[Any]]): batch of examples to process
-            index (list[int]): dataset indices of the examples
-            rank (int): execution process rank
+            examples (dict[str, list[Any]]):
+                batch of examples to process
+            index (list[int]):
+                dataset indices of the examples
+            rank (int):
+                execution process rank
+            return_index (bool):
+                whether to return the source index for each output example
 
         Returns:
-            out (dict[str, list[Any]]): processed examples
+            out_batch (dict[str, list[Any]]):
+                processed examples
+            index (list[int]):
+                the source indices to each example. Only returned when
+                `return_index` is set to true.
         """
         iterable = self.iter_batch_process(
-            examples=examples, index=index, rank=rank
+            examples=examples,
+            index=index,
+            rank=rank,
+            return_index=return_index,
         )
         # return the last item of the iterable which corresponds
         # to the output of the last data processor
         return deque(iterable, maxlen=1).pop()
 
     def iter_batch_process(
         self,
         examples: dict[str, list[Any]],
         index: list[int],
         rank: None | int = None,
-    ) -> Iterable[dict[str, list[Any]]]:
+        return_index: bool = False,
+    ) -> Iterable[
+        dict[str, list[Any]] | tuple[dict[str, list[Any]], list[int]]
+    ]:
         """Apply each data processor to the batch of examples.
 
         Yields the output of each data processor when ready.
 
         Arguments:
-            examples (dict[str, list[Any]]): batch of examples to process
-            index (list[int]): dataset indices of the examples
-            rank (int): execution process rank
+            examples (dict[str, list[Any]]):
+                batch of examples to process
+            index (list[int]):
+                dataset indices of the examples
+            rank (int):
+                execution process rank
+            return_index (bool):
+                whether to return the source index for each output example
 
         Returns:
-            out_iter (Iterable[dict[str, list[Any]]]):
-                iterator over output batch from each processor
+            out_iter (
+                Iterable[dict[str, list[Any]]
+                | tuple[dict[str, list[Any]], list[int]]]
+            ):
+                iterator over output batch from each processor, includes
+                the source indices when `return_index=True`
         """
         if rank is None:
             # try to get multiprocessing rank from pytorch worker info
             worker_info = get_worker_info()
             rank = None if worker_info is None else worker_info.id
 
         # make sure the pipeline is prepared
@@ -163,15 +255,27 @@
             )
         # apply each processor
         for p in self:
             examples, index = p.batch_process(
                 examples, index, rank, return_index=True
             )
             # yield the output of the current data processor
-            yield examples
+            yield (examples, index) if return_index else examples
+
+    def internal_batch_process(
+        self, examples: dict[str, list[Any]], index: list[int], rank: int
+    ) -> tuple[dict[str, list[Any]], list[int]]:
+        """Internal Batch Process."""
+        raise NotImplementedError()
+
+    def process(
+        self, example: dict[str, Any], index: int, rank: int
+    ) -> dict[str, Any] | Generator[dict[str, Any], None, None]:
+        """Process a single example."""
+        raise NotImplementedError()
 
     def _batch_process_to_pyarrow(
         self,
         examples: dict[str, list[Any]],
         index: list[int],
         rank: None | int = None,
     ) -> pa.Table:
@@ -179,32 +283,28 @@
         return pa.table(
             data=self.batch_process(examples, index, rank),
             schema=convert_features_to_arrow_schema(self.out_features),
         )
 
     def apply(
         self,
-        data: (
-            datasets.Dataset
-            | datasets.DatasetDict
-            | datasets.IterableDataset
-            | datasets.IterableDatasetDict
-        ),
+        data: DatasetType,
         **kwargs,
     ) -> datasets.Dataset | datasets.DatasetDict:
         """Apply the data pipe to a dataset.
 
         Arguments:
-            data (Dataset|DatasetDict|IterableDataset|IterableDatasetDict):
+            data (DatasetType):
                 source dataset(s)
             **kwargs (dict[str, Any]):
                 arguments forwarded to datasets `.map` function
 
         Returns:
-            out (datasets.Dataset|datasets.DatasetDict): processed dataset(s)
+            out (DatasetType):
+                processed dataset(s)
         """
         # get the dataset features
         if isinstance(data, (datasets.Dataset, datasets.IterableDataset)):
             features = data.features
         elif isinstance(
             data, (datasets.DatasetDict, datasets.IterableDatasetDict)
         ):
@@ -243,40 +343,67 @@
                 warnings.warn(
                     "Loading map result from cache file will not compute "
                     "statistics, set `load_from_cache_file=False` to avoid "
                     "this behavior.",
                     UserWarning,
                 )
 
+        # apply data pipe to dataset
+        data = self.internal_apply(data, **kwargs)
+
+        if isinstance(
+            data, (datasets.IterableDataset, datasets.IterableDatasetDict)
+        ):
+            # set output features for lazy datasets manually
+            if isinstance(data, datasets.IterableDataset):
+                data.info.features = self.out_features
+            elif isinstance(data, datasets.IterableDatasetDict):
+                for split in data.values():
+                    split.info.features = self.out_features
+
+        return data
+
+    def internal_apply(
+        self,
+        data: DatasetType,
+        **kwargs,
+    ) -> DatasetType:
+        """Internal apply function.
+
+        Arguments:
+            data (DatasetType):
+                source dataset(s)
+            **kwargs:
+                keyword arguments passed to the map function
+                appropriate for the given dataset type
+
+        Returns:
+            out (DatasetType):
+                processed dataset(s)
+        """
         # required settings
         kwargs["batched"] = True
         kwargs["with_indices"] = True
-        # for in-memory datasets let the map function provide the rank
+        # for non-iterable datasets the map function provide the rank
         if isinstance(data, (datasets.Dataset, datasets.DatasetDict)):
             kwargs["with_rank"] = True
 
         if isinstance(data, (datasets.Dataset, datasets.DatasetDict)):
             # use pyarrow table as output format for in-memory
             # datasets that support caching since it includes
             # the output feature information
-            data = data.map(self._batch_process_to_pyarrow, **kwargs)
+            return data.map(self._batch_process_to_pyarrow, **kwargs)
 
         elif isinstance(
             data, (datasets.IterableDataset, datasets.IterableDatasetDict)
         ):
             # iterable dataset class doesn't support pyarrow
             # outputs in map function, but it also doesn't cache
             # and thus doesn't need the features while processing
-            data = data.map(
+            return data.map(
                 self.batch_process,
                 remove_columns=set(self.in_features.keys())
                 - set(self.out_features.keys()),
                 **kwargs,
             )
-            # set output features for lazy datasets manually
-            if isinstance(data, datasets.IterableDataset):
-                data.info.features = self.out_features
-            elif isinstance(data, datasets.IterableDatasetDict):
-                for split in data.values():
-                    split.info.features = self.out_features
 
-        return data
+        raise ValueError("Unexpected Dataset type, got %s" % data)
```

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/base.py` & `hyped-0.1.0a2/src/hyped/data/processors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """Base Data Processor."""
 from __future__ import annotations
 
 import asyncio
 import inspect
 from abc import ABC, abstractmethod
+from copy import deepcopy
 from itertools import chain, repeat
 from types import GeneratorType
 from typing import Any, ClassVar, Generator, Iterable, TypeVar
 
+import nest_asyncio
 from datasets import Features
 from datasets.iterable_dataset import _batch_to_examples, _examples_to_batch
 
 from hyped.base.config import BaseConfig, BaseConfigurable
 from hyped.common.feature_key import FeatureCollection, FeatureDict, FeatureKey
 
+# patch asyncio if running in an async environment, such as jupyter notebook
+# this fixes #26
+nest_asyncio.apply()
+
 
 class BaseDataProcessorConfig(BaseConfig):
     """Base Data Processor Config.
 
     Attributes:
         keep_input_features (bool):
             whether to pipe input features to output or only output
@@ -101,15 +107,20 @@
         self._is_process_async_gen = inspect.isasyncgenfunction(self.process)
 
     @classmethod
     def from_config(cls, config: T) -> BaseDataProcessor:
         """Instantiate data processor from the given config.
 
         Arguments:
-            config (BaseDataProcessorConfig): data processor configuration
+            config (BaseDataProcessorConfig):
+                data processor configuration
+
+        Returns:
+            processor (BaseDataProcessor):
+                data processor
         """
         return cls(config)
 
     @property
     def config(self) -> T:
         """Get the processor configuration.
 
@@ -137,38 +148,37 @@
                 input dataset features available to the processor on execution
 
         Returns:
             out_features (Features):
                 dataset features of the output of the processor
         """
         # save input features
-        self._in_features = features
+        self._in_features = deepcopy(features)
         # map input features to output features
         # copy as preparation might disturb features inplace
-        self._raw_features = Features(self.map_features(features.copy()))
+        self._raw_features = Features(self.map_features(deepcopy(features)))
         # apply output scheme to new features
         if self.config.output_format is not None:
             self._new_features = self.config.output_format.index_features(
                 self._raw_features
             )
             assert isinstance(self._new_features, Features)
         # return output features
         return self.out_features
 
     @property
-    def required_feature_keys(self) -> list[FeatureKey]:
+    def required_feature_keys(self) -> set[FeatureKey]:
         """Input dataset feature keys required for execution of the processor.
 
         These must be contained in the `in_features`.
 
         Returns:
             feature_keys (list[FeatureKey]): list of required feature keys
         """
-        # TODO: make list unique
-        return list(self.config.required_feature_keys)
+        return set(list(self.config.required_feature_keys))
 
     @property
     def in_features(self) -> Features:
         """Input dataset features available to processor.
 
         Returns:
             features (Features): input dataset features
@@ -248,22 +258,26 @@
         index: list[int],
         rank: int,
         return_index: bool = False,
     ) -> dict[str, list[Any]] | tuple[dict[str, list[Any]], list[int]]:
         """Process a batch of examples.
 
         Arguments:
-            examples (dict[str, list[Any]]): batch of examples to process
-            index (list[int]): dataset indices of the examples
-            rank (int): execution process rank
+            examples (dict[str, list[Any]]):
+                batch of examples to process
+            index (list[int]):
+                dataset indices of the examples
+            rank (int):
+                execution process rank
             return_index (bool):
                 whether to return the source index for each output example
 
         Returns:
-            out_batch (dict[str, list[Any]]): processed examples
+            out_batch (dict[str, list[Any]]):
+                processed examples
             index (list[int]):
                 the source indices to each example. Only returned when
                 `return_index` is set to true.
         """
         # process batch
         out_batch, src_index = self.internal_batch_process(
             examples, index, rank
@@ -502,15 +516,16 @@
             # apply coroutine appropriate to the process function type
             future = (
                 self._async_gen_batch_process
                 if self._is_process_async_gen
                 else self._async_batch_process
             )(examples, index, rank)
             # get the event loop to run the async function
-            loop = asyncio.get_event_loop()
+            loop = asyncio.new_event_loop()
+            # run the event loop and return coroutine results
             return loop.run_until_complete(future)
 
         # run sync
         return (
             self._sync_gen_batch_process
             if self._is_process_gen
             else self._sync_batch_process
```

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/features/filter.py` & `hyped-0.1.0a2/src/hyped/data/processors/features/filter.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/features/flatten.py` & `hyped-0.1.0a2/src/hyped/data/processors/features/flatten.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/features/format.py` & `hyped-0.1.0a2/src/hyped/data/processors/features/format.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/sequence/apply_mask.py` & `hyped-0.1.0a2/src/hyped/data/processors/sequence/apply_mask.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/sequence/chunk.py` & `hyped-0.1.0a2/src/hyped/data/processors/sequence/chunk.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/sequence/extend.py` & `hyped-0.1.0a2/src/hyped/data/processors/sequence/extend.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/sequence/filter.py` & `hyped-0.1.0a2/src/hyped/data/processors/sequence/filter.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/sequence/join_str_seq.py` & `hyped-0.1.0a2/src/hyped/data/processors/sequence/join_str_seq.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/spans/apply_idx_spans.py` & `hyped-0.1.0a2/src/hyped/data/processors/spans/apply_idx_spans.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/spans/common.py` & `hyped-0.1.0a2/src/hyped/data/processors/spans/common.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/spans/from_bio.py` & `hyped-0.1.0a2/src/hyped/data/processors/spans/from_bio.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/spans/from_word_ids.py` & `hyped-0.1.0a2/src/hyped/data/processors/spans/from_word_ids.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/spans/idx_spans.py` & `hyped-0.1.0a2/src/hyped/data/processors/spans/idx_spans.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/spans/loc_to_glob.py` & `hyped-0.1.0a2/src/hyped/data/processors/spans/loc_to_glob.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/spans/overlaps.py` & `hyped-0.1.0a2/src/hyped/data/processors/spans/overlaps.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/statistics/base.py` & `hyped-0.1.0a2/src/hyped/data/processors/statistics/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/statistics/report.py` & `hyped-0.1.0a2/src/hyped/data/processors/statistics/report.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/disc_seq_val_hist.py` & `hyped-0.1.0a2/src/hyped/data/processors/statistics/sequence/disc_seq_val_hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/seq_len_hist.py` & `hyped-0.1.0a2/src/hyped/data/processors/statistics/sequence/seq_len_hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/seq_val_hist.py` & `hyped-0.1.0a2/src/hyped/data/processors/statistics/sequence/seq_val_hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/statistics/value/disc_hist.py` & `hyped-0.1.0a2/src/hyped/data/processors/statistics/value/disc_hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/statistics/value/hist.py` & `hyped-0.1.0a2/src/hyped/data/processors/statistics/value/hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/statistics/value/mean_and_std.py` & `hyped-0.1.0a2/src/hyped/data/processors/statistics/value/mean_and_std.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/taggers/bio.py` & `hyped-0.1.0a2/src/hyped/data/processors/taggers/bio.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/taggers/relex.py` & `hyped-0.1.0a2/src/hyped/data/processors/taggers/relex.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped/data/processors/tokenizers/hf.py` & `hyped-0.1.0a2/src/hyped/data/processors/tokenizers/hf.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/src/hyped.egg-info/PKG-INFO` & `hyped-0.1.0a2/src/hyped.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyped
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: TODO
 Author: Niclas Doll
 License: Apache 2.0
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
@@ -14,25 +14,28 @@
 Requires-Dist: fsspec<=2023.9.2
 Requires-Dist: torch>=2.2.1
 Requires-Dist: transformers>=4.36.2
 Requires-Dist: networkx>=3.1
 Requires-Dist: matplotlib>=3.8.2
 Requires-Dist: orjson>=3.9.4
 Requires-Dist: pydantic>=2.6.4
+Requires-Dist: json_repair>=0.17.0
+Requires-Dist: nest-asyncio>=1.6.0
 Provides-Extra: linting
 Requires-Dist: pre-commit; extra == "linting"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Provides-Extra: peft
-Requires-Dist: peft>=0.9.0; extra == "peft"
-Requires-Dist: bitsandbytes>=0.42.0; extra == "peft"
+Provides-Extra: cas
+Requires-Dist: dkpro-cassis>=0.8.0; extra == "cas"
+Provides-Extra: llm
+Requires-Dist: openai>=1.23.6; extra == "llm"
 
 # :boom: Hyped
 
 [![Tests](https://github.com/open-hyped/hyped/actions/workflows/tests.yml/badge.svg?branch=hyped-v2)](https://github.com/open-hyped/hyped/actions/workflows/tests.yml)
 [![Linting](https://github.com/open-hyped/hyped/actions/workflows/linting.yml/badge.svg?branch=hyped-v2)](https://github.com/open-hyped/hyped/actions/workflows/linting.yml)
 [![Coverage Status](https://coveralls.io/repos/github/open-hyped/hyped/badge.svg?branch=hyped-v2)](https://coveralls.io/github/open-hyped/hyped?branch=hyped-v2)
 [![PyPi version](https://badgen.net/pypi/v/hyped/)](https://pypi.org/project/hyped)
```

### Comparing `hyped-0.1.0a1/src/hyped.egg-info/SOURCES.txt` & `hyped-0.1.0a2/src/hyped.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
-requirements.txt
 .github/workflows/docs.yml
 .github/workflows/linting.yml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/build.sh
 docs/make.bat
 docs/source/add_ons.rst
 docs/source/conf.py
-docs/source/costum_data_processors.rst
+docs/source/data_pipe.rst
+docs/source/data_processors.rst
 docs/source/feature_access.rst
 docs/source/getting_started.rst
 docs/source/index.rst
 docs/source/statistic_processors.rst
 docs/source/api/.gitkeep
 src/hyped/__version__.py
 src/hyped.egg-info/PKG-INFO
@@ -33,31 +33,37 @@
 src/hyped/base/registry.py
 src/hyped/common/__init__.py
 src/hyped/common/arrow.py
 src/hyped/common/consumer.py
 src/hyped/common/feature_checks.py
 src/hyped/common/feature_key.py
 src/hyped/common/lazy.py
+src/hyped/common/pydantic.py
 src/hyped/data/__init__.py
 src/hyped/data/graph.py
 src/hyped/data/pipe.py
 src/hyped/data/io/__init__.py
 src/hyped/data/io/datasets/__init__.py
 src/hyped/data/io/datasets/cas.py
 src/hyped/data/io/datasets/typed_json.py
 src/hyped/data/io/writers/__init__.py
 src/hyped/data/io/writers/base.py
 src/hyped/data/io/writers/csv.py
 src/hyped/data/io/writers/json.py
 src/hyped/data/processors/__init__.py
 src/hyped/data/processors/base.py
+src/hyped/data/processors/api/__init__.py
+src/hyped/data/processors/api/openai_chat.py
 src/hyped/data/processors/features/__init__.py
 src/hyped/data/processors/features/filter.py
 src/hyped/data/processors/features/flatten.py
 src/hyped/data/processors/features/format.py
+src/hyped/data/processors/parsers/__init__.py
+src/hyped/data/processors/parsers/json.py
+src/hyped/data/processors/parsers/repair_json.py
 src/hyped/data/processors/sequence/__init__.py
 src/hyped/data/processors/sequence/apply_mask.py
 src/hyped/data/processors/sequence/chunk.py
 src/hyped/data/processors/sequence/extend.py
 src/hyped/data/processors/sequence/filter.py
 src/hyped/data/processors/sequence/join_str_seq.py
 src/hyped/data/processors/spans/__init__.py
@@ -78,14 +84,16 @@
 src/hyped/data/processors/statistics/value/__init__.py
 src/hyped/data/processors/statistics/value/disc_hist.py
 src/hyped/data/processors/statistics/value/hist.py
 src/hyped/data/processors/statistics/value/mean_and_std.py
 src/hyped/data/processors/taggers/__init__.py
 src/hyped/data/processors/taggers/bio.py
 src/hyped/data/processors/taggers/relex.py
+src/hyped/data/processors/templates/__init__.py
+src/hyped/data/processors/templates/jinja2.py
 src/hyped/data/processors/tokenizers/__init__.py
 src/hyped/data/processors/tokenizers/hf.py
 tests/__init__.py
 tests/conftest.py
 tests/hyped/__init__.py
 tests/hyped/base/__init__.py
 tests/hyped/base/test_config.py
@@ -107,18 +115,23 @@
 tests/hyped/data/io/writers/__init__.py
 tests/hyped/data/io/writers/base.py
 tests/hyped/data/io/writers/test_csv.py
 tests/hyped/data/io/writers/test_json.py
 tests/hyped/data/processors/__init__.py
 tests/hyped/data/processors/base.py
 tests/hyped/data/processors/test_base.py
+tests/hyped/data/processors/api/__init__.py
+tests/hyped/data/processors/api/test_openai_chat.py
 tests/hyped/data/processors/features/__init__.py
 tests/hyped/data/processors/features/test_filter.py
 tests/hyped/data/processors/features/test_flatten.py
 tests/hyped/data/processors/features/test_format.py
+tests/hyped/data/processors/parsers/__init__.py
+tests/hyped/data/processors/parsers/test_json.py
+tests/hyped/data/processors/parsers/test_repair_json.py
 tests/hyped/data/processors/sequence/__init__.py
 tests/hyped/data/processors/sequence/test_apply_mask.py
 tests/hyped/data/processors/sequence/test_chunk.py
 tests/hyped/data/processors/sequence/test_extend.py
 tests/hyped/data/processors/sequence/test_filter.py
 tests/hyped/data/processors/sequence/test_join_str_seq.py
 tests/hyped/data/processors/spans/__init__.py
@@ -140,9 +153,11 @@
 tests/hyped/data/processors/statistics/value/__init__.py
 tests/hyped/data/processors/statistics/value/test_disc_hist.py
 tests/hyped/data/processors/statistics/value/test_hist.py
 tests/hyped/data/processors/statistics/value/test_mean_and_std.py
 tests/hyped/data/processors/taggers/__init__.py
 tests/hyped/data/processors/taggers/test_bio.py
 tests/hyped/data/processors/taggers/test_relex.py
+tests/hyped/data/processors/templates/__init__.py
+tests/hyped/data/processors/templates/test_jinja2.py
 tests/hyped/data/processors/tokenizers/__init__.py
 tests/hyped/data/processors/tokenizers/test_hf.py
```

### Comparing `hyped-0.1.0a1/tests/hyped/base/test_config.py` & `hyped-0.1.0a2/tests/hyped/base/test_config.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/base/test_generic.py` & `hyped-0.1.0a2/tests/hyped/base/test_generic.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/base/test_registry.py` & `hyped-0.1.0a2/tests/hyped/base/test_registry.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/common/test_arrow.py` & `hyped-0.1.0a2/tests/hyped/common/test_arrow.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/common/test_consumer.py` & `hyped-0.1.0a2/tests/hyped/common/test_consumer.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/common/test_feature_checks.py` & `hyped-0.1.0a2/tests/hyped/common/test_feature_checks.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/common/test_feature_key.py` & `hyped-0.1.0a2/tests/hyped/common/test_feature_key.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/common/test_lazy.py` & `hyped-0.1.0a2/tests/hyped/common/test_lazy.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/io/datasets/test_cas.py` & `hyped-0.1.0a2/tests/hyped/data/io/datasets/test_cas.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,28 +57,29 @@
     )
     # save in json and xmi format
     cas.to_json(os.path.join(path, "cas.test.json"))
     cas.to_xmi(os.path.join(path, "cas.test.xmi"))
 
 
 class TestCasDataset:
-    @pytest.fixture(autouse=True)
-    def _create_resources(self, tmpdir):
+    @pytest.fixture(scope="class")
+    def data_dir(self, tmpdir_factory):
+        tmpdir = tmpdir_factory.mktemp("cas")
         # create resource files
         build_typesystem(tmpdir)
         build_examples(tmpdir)
         # run test
-        yield
+        return tmpdir
 
-    def test_load_data(self, tmpdir):
+    def test_load_data(self, data_dir, tmpdir):
         # load dataset
         ds = datasets.load_dataset(
             "hyped.data.io.datasets.cas",
-            typesystem=os.path.join(tmpdir, "typesystem.test.xml"),
-            data_files={"train": os.path.join(tmpdir, "cas.test.*")},
+            typesystem=os.path.join(data_dir, "typesystem.test.xml"),
+            data_files={"train": os.path.join(data_dir, "cas.test.*")},
             cache_dir=os.path.join(tmpdir, "cache"),
         )
 
         # check dataset length
         assert len(ds["train"]) == 2
         # check features
         assert "sofa" in ds["train"].features
@@ -128,20 +129,20 @@
             for src, tgt in zip(
                 example["cassis.Relation:source"],
                 example["cassis.Relation:target"],
             ):
                 assert example["cassis.Entity:entityType"][src] == "ORG"
                 assert example["cassis.Entity:entityType"][tgt] == "LOC"
 
-    def test_load_specific_types_only(self, tmpdir):
+    def test_load_specific_types_only(self, data_dir, tmpdir):
         # load dataset
         ds = datasets.load_dataset(
             "hyped.data.io.datasets.cas",
-            typesystem=os.path.join(tmpdir, "typesystem.test.xml"),
-            data_files={"train": os.path.join(tmpdir, "cas.test.*")},
+            typesystem=os.path.join(data_dir, "typesystem.test.xml"),
+            data_files={"train": os.path.join(data_dir, "cas.test.*")},
             annotation_types=["cassis.Label"],
             cache_dir=os.path.join(tmpdir, "cache"),
         )
 
         # check dataset length
         assert len(ds["train"]) == 2
         assert "sofa" in ds["train"].features
@@ -151,20 +152,20 @@
         assert "cassis.Entity:begin" not in ds["train"].features
         assert "cassis.Entity:end" not in ds["train"].features
         assert "cassis.Entity:entityType" not in ds["train"].features
         # relation should be excluded
         assert "cassis.Relation:source" not in ds["train"].features
         assert "cassis.Relation:target" not in ds["train"].features
 
-    def test_error_on_required_type(self, tmpdir):
+    def test_error_on_required_type(self, data_dir, tmpdir):
         with pytest.raises(RuntimeError):
             # load dataset
             datasets.load_dataset(
                 "hyped.data.io.datasets.cas",
-                typesystem=os.path.join(tmpdir, "typesystem.test.xml"),
-                data_files={"train": os.path.join(tmpdir, "cas.test.*")},
+                typesystem=os.path.join(data_dir, "typesystem.test.xml"),
+                data_files={"train": os.path.join(data_dir, "cas.test.*")},
                 annotation_types=[
                     "cassis.Label",
                     "cassis.Relation",  # relation require entities
                 ],
                 cache_dir=os.path.join(tmpdir, "cache"),
             )
```

### Comparing `hyped-0.1.0a1/tests/hyped/data/io/datasets/test_typed_json.py` & `hyped-0.1.0a2/tests/hyped/data/io/datasets/test_typed_json.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,116 +8,118 @@
 from datasets import ClassLabel, Features, Sequence, Value
 
 # register custom datasets
 import hyped.data.io.datasets  # noqa: F401
 
 
 class TestTypedJsonDataset(object):
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def features(self) -> Features:
         return Features(
             {
                 "int": Value("int32"),
                 "string": Value("string"),
                 "class": ClassLabel(names=list("ABC")),
                 "sequence": Sequence(Value("int32")),
                 "date": Value("date32"),
                 "mapping": Features(
                     {"a": Value("int32"), "b": Value("int32")}
                 ),
             }
         )
 
-    @pytest.fixture
+    @pytest.fixture(scope="class")
     def data(self) -> list[dict[str, Any]]:
         return [
             {
                 "int": n,
                 "string": "string-w\n-%i" % n,
                 "class": "ABC"[n % 3],
                 "sequence": [n, 2 * n],
                 "date": datetime(2010, 1 + n % 12, 1),
                 "mapping": {"a": n, "b": 2 * n},
             }
             for n in range(10)
         ]
 
-    @pytest.fixture
-    def data_file(self, data, tmp_path) -> str:
+    @pytest.fixture(scope="class")
+    def data_file(self, data, tmpdir_factory) -> str:
+        tmp_path = tmpdir_factory.mktemp("data")
         data_file = os.path.join(tmp_path, "file.jsonl")
         # create sample data that matches the features
         with open(data_file, "wb+") as f:
             f.write(b"\n".join(map(orjson.dumps, data)))
 
         return data_file
 
-    def test_loading(self, features, data_file):
+    def test_loading(self, features, data_file, tmpdir):
         # load data using typed json dataset
         datasets.load_dataset(
             "hyped.data.io.datasets.typed_json",
             data_files=[data_file],
             features=features,
+            cache_dir=os.path.join(tmpdir, "cache"),
         )
 
-    def test_type_error(self, features, data_file):
+    def test_type_error(self, features, data_file, tmpdir):
         # break feature type
+        features = features.copy()
         features["string"] = Value("int32")
         # string feature type shouldn't match
         with pytest.raises(datasets.exceptions.DatasetGenerationError):
             datasets.load_dataset(
                 "hyped.data.io.datasets.typed_json",
                 data_files=[data_file],
                 features=features,
+                cache_dir=os.path.join(tmpdir, "cache"),
             )
 
-    def test_fill_with_defaults(self, features, data_file):
+    def test_fill_with_defaults(self, features, data_file, tmpdir):
         # add new feature
         features["new_feature"] = Value("string")
         # load data using typed json dataset
         ds = datasets.load_dataset(
             "hyped.data.io.datasets.typed_json",
             data_files=[data_file],
             features=features,
+            cache_dir=os.path.join(tmpdir, "cache"),
         )["train"]
 
         for item in ds:
             assert "new_feature" in item
             assert item["new_feature"] is None
 
-    def test_partial_fill_with_defaults(self, features, data_file):
-        partial_data = [{"int": n} for n in range(10)]
-
-        with open(data_file, "ab") as f:
+    @pytest.mark.parametrize(
+        "partial_data",
+        [
+            [{"int": n} for n in range(10)],
+            [{"int": n, "mapping": {"b": n}} for n in range(10)],
+        ],
+    )
+    def test_partial_fill_with_defaults(
+        self, partial_data, features, data_file, tmpdir
+    ):
+        aug_data_file = os.path.join(tmpdir, "aug_data.json")
+        with open(aug_data_file, "wb+") as f, open(data_file, "rb") as f_in:
+            f.write(f_in.read())
             f.write(b"\n")
             f.write(b"\n".join(map(orjson.dumps, partial_data)))
 
         # load data using typed json dataset
         datasets.load_dataset(
             "hyped.data.io.datasets.typed_json",
-            data_files=[data_file],
-            features=features,
-        )["train"]
-
-    def test_partial_fill_with_defaults_in_nested(self, features, data_file):
-        partial_data = [{"int": n, "mapping": {"b": n}} for n in range(10)]
-
-        with open(data_file, "ab") as f:
-            f.write(b"\n")
-            f.write(b"\n".join(map(orjson.dumps, partial_data)))
-
-        # load data using typed json dataset
-        datasets.load_dataset(
-            "hyped.data.io.datasets.typed_json",
-            data_files=[data_file],
+            data_files=[aug_data_file],
             features=features,
+            cache_dir=os.path.join(tmpdir, "cache"),
         )["train"]
 
-    def test_invalid_class_label(self, features, data_file):
+    def test_invalid_class_label(self, features, data_file, tmpdir):
         # remove class name from label space
         features["class"] = ClassLabel(names=list("AB"))
         # string feature type shouldn't match
         with pytest.raises(datasets.exceptions.DatasetGenerationError):
             datasets.load_dataset(
                 "hyped.data.io.datasets.typed_json",
                 data_files=[data_file],
                 features=features,
+                cache_dir=os.path.join(tmpdir, "cache"),
             )
```

### Comparing `hyped-0.1.0a1/tests/hyped/data/io/writers/base.py` & `hyped-0.1.0a2/tests/hyped/data/io/writers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from abc import ABC, abstractmethod
 
 import datasets
 import pytest
 
 
 class BaseTestDatasetWriter(ABC):
-    @pytest.fixture(params=[2, 4, 8, 16])
+    @pytest.fixture(params=[2, 4, 8])
     def num_proc(self, request):
         return request.param
 
-    @pytest.fixture(params=[2, 4, 8, 16])
+    @pytest.fixture(params=[2, 4, 8])
     def num_shards(self, request):
         return request.param
 
     @pytest.fixture
     @abstractmethod
     def writer(self, tmpdir, num_proc):
         ...
@@ -41,14 +41,15 @@
         # load stored dataset
         stored_ds = self.load_dataset(str(tmpdir), features)
         stored_ds = stored_ds["train"].sort("id")
         # check dataset
         for i, item in enumerate(stored_ds):
             self.assert_equal({"id": i}, item)
 
+    @pytest.mark.skip(reason="Tests with real datasets take forever.")
     @pytest.mark.parametrize("dataset", ["conll2003", "imdb"])
     def test_with_actual_data(self, writer, tmpdir, dataset):
         # load dataset and add an index column to
         # recover the original order after saving
         ds = datasets.load_dataset(dataset, split="test")
         ds = ds.add_column("__index__", range(len(ds)))
         # shard and write it
```

### Comparing `hyped-0.1.0a1/tests/hyped/data/io/writers/test_csv.py` & `hyped-0.1.0a2/tests/hyped/data/io/writers/test_json.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import datasets
 import pytest
 
-from hyped.data.io.writers.csv import CsvDatasetWriter
+from hyped.data.io.writers.json import JsonDatasetWriter
 from tests.hyped.data.io.writers.base import BaseTestDatasetWriter
 
 
-class TestCsvDatasetWriter(BaseTestDatasetWriter):
+class TestJsonDatasetWriter(BaseTestDatasetWriter):
     @pytest.fixture
     def writer(self, tmpdir, num_proc):
-        return CsvDatasetWriter(
+        return JsonDatasetWriter(
             save_dir=tmpdir, exist_ok=True, num_proc=num_proc
         )
 
     def load_dataset(self, tmpdir, features):
         return datasets.load_dataset(
-            "csv", data_files="%s/*.csv" % tmpdir, features=features
-        )
-
-    def test_with_actual_data(self, writer, tmpdir):
-        super(TestCsvDatasetWriter, self).test_with_actual_data(
-            writer, tmpdir, "imdb"
+            "json", data_files="%s/*.jsonl" % tmpdir, features=features
         )
```

### Comparing `hyped-0.1.0a1/tests/hyped/data/io/writers/test_json.py` & `hyped-0.1.0a2/tests/hyped/data/io/writers/test_csv.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import datasets
 import pytest
 
-from hyped.data.io.writers.json import JsonDatasetWriter
+from hyped.data.io.writers.csv import CsvDatasetWriter
 from tests.hyped.data.io.writers.base import BaseTestDatasetWriter
 
 
-class TestJsonDatasetWriter(BaseTestDatasetWriter):
+class TestCsvDatasetWriter(BaseTestDatasetWriter):
     @pytest.fixture
     def writer(self, tmpdir, num_proc):
-        return JsonDatasetWriter(
+        return CsvDatasetWriter(
             save_dir=tmpdir, exist_ok=True, num_proc=num_proc
         )
 
     def load_dataset(self, tmpdir, features):
         return datasets.load_dataset(
-            "json", data_files="%s/*.jsonl" % tmpdir, features=features
+            "csv", data_files="%s/*.csv" % tmpdir, features=features
         )
```

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/base.py` & `hyped-0.1.0a2/tests/hyped/data/processors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from abc import ABC, abstractmethod
 from contextlib import AbstractContextManager, nullcontext
 from copy import deepcopy
 from typing import Any
 
 import pyarrow as pa
 import pytest
```

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/features/test_filter.py` & `hyped-0.1.0a2/tests/hyped/data/processors/features/test_filter.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/features/test_flatten.py` & `hyped-0.1.0a2/tests/hyped/data/processors/features/test_flatten.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/features/test_format.py` & `hyped-0.1.0a2/tests/hyped/data/processors/features/test_format.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_apply_mask.py` & `hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_apply_mask.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_chunk.py` & `hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_chunk.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_extend.py` & `hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_extend.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_filter.py` & `hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_filter.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_join_str_seq.py` & `hyped-0.1.0a2/tests/hyped/data/processors/sequence/test_join_str_seq.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_apply_idx_spans.py` & `hyped-0.1.0a2/tests/hyped/data/processors/spans/test_apply_idx_spans.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_common.py` & `hyped-0.1.0a2/tests/hyped/data/processors/spans/test_common.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_from_bio.py` & `hyped-0.1.0a2/tests/hyped/data/processors/spans/test_from_bio.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_from_word_ids.py` & `hyped-0.1.0a2/tests/hyped/data/processors/spans/test_from_word_ids.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_idx_spans.py` & `hyped-0.1.0a2/tests/hyped/data/processors/spans/test_idx_spans.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_loc_to_glob.py` & `hyped-0.1.0a2/tests/hyped/data/processors/spans/test_loc_to_glob.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_overlaps.py` & `hyped-0.1.0a2/tests/hyped/data/processors/spans/test_overlaps.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/statistics/base.py` & `hyped-0.1.0a2/tests/hyped/data/processors/statistics/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/test_disc_seq_val_hist.py` & `hyped-0.1.0a2/tests/hyped/data/processors/statistics/sequence/test_disc_seq_val_hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/test_seq_len_hist.py` & `hyped-0.1.0a2/tests/hyped/data/processors/statistics/sequence/test_seq_len_hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/test_seq_val_hist.py` & `hyped-0.1.0a2/tests/hyped/data/processors/statistics/sequence/test_seq_val_hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/statistics/test_base.py` & `hyped-0.1.0a2/tests/hyped/data/processors/statistics/test_base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/statistics/test_report.py` & `hyped-0.1.0a2/tests/hyped/data/processors/statistics/test_report.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_disc_hist.py` & `hyped-0.1.0a2/tests/hyped/data/processors/statistics/value/test_disc_hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_hist.py` & `hyped-0.1.0a2/tests/hyped/data/processors/statistics/value/test_hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_mean_and_std.py` & `hyped-0.1.0a2/tests/hyped/data/processors/statistics/value/test_mean_and_std.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/taggers/test_bio.py` & `hyped-0.1.0a2/tests/hyped/data/processors/taggers/test_bio.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/taggers/test_relex.py` & `hyped-0.1.0a2/tests/hyped/data/processors/taggers/test_relex.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/test_base.py` & `hyped-0.1.0a2/tests/hyped/data/processors/test_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -156,14 +156,40 @@
         return {"A": ["B"] * 10}
 
     def test_process_fn_type(self, processor):
         assert not processor._is_process_gen
         assert not processor._is_process_async
         assert not processor._is_process_async_gen
 
+    def test_case_nested_async(
+        self,
+        processor,
+        in_features,
+        in_batch,
+        expected_err_on_prepare,
+        expected_err_on_process,
+        kwargs_for_post_prepare_checks,
+        kwargs_for_post_process_checks,
+    ):
+        # async wrapper of the test case
+        async def run():
+            return self.test_case(
+                processor,
+                in_features,
+                in_batch,
+                expected_err_on_prepare,
+                expected_err_on_process,
+                kwargs_for_post_prepare_checks,
+                kwargs_for_post_process_checks,
+            )
+
+        # run in new event loop
+        loop = asyncio.new_event_loop()
+        loop.run_until_complete(run())
+
 
 class TestAsyncDataProcessor(TestDataProcessor):
     @pytest.fixture
     def processor(self, keep_inputs):
         # create processor and make sure it is not prepared
         # before calling prepare function
         c = ConstantDataProcessorConfig(
```

### Comparing `hyped-0.1.0a1/tests/hyped/data/processors/tokenizers/test_hf.py` & `hyped-0.1.0a2/tests/hyped/data/processors/tokenizers/test_hf.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a1/tests/hyped/data/test_graph.py` & `hyped-0.1.0a2/tests/hyped/data/test_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,14 +188,54 @@
         return 1
 
     @pytest.fixture
     def graph(self) -> nx.DiGraph:
         return nx.DiGraph([(0, 1), (1, 2), (2, 3)])
 
 
+class TestNestedDataPipe(BaseTestProcessGraph):
+    @pytest.fixture
+    def features(self) -> Features:
+        return Features({"x": Value("int32")})
+
+    @pytest.fixture
+    def pipe(self) -> DataPipe:
+        return DataPipe(
+            [
+                FormatFeatures(
+                    FormatFeaturesConfig(
+                        output_format={"y": "x"}, keep_input_features=False
+                    )
+                ),
+                DataPipe(
+                    [
+                        FormatFeatures(
+                            FormatFeaturesConfig(output_format={"a": "y"})
+                        ),
+                        FormatFeatures(
+                            FormatFeaturesConfig(output_format={"b": "y"})
+                        ),
+                    ]
+                ),
+            ]
+        )
+
+    @pytest.fixture
+    def num_layers(self) -> int:
+        return 4
+
+    @pytest.fixture
+    def max_width(self) -> int:
+        return 2
+
+    @pytest.fixture
+    def graph(self) -> nx.DiGraph:
+        return nx.DiGraph([(0, 1), (1, 2), (2, 3), (2, 4), (1, 5)])
+
+
 class TestSimpleTree(BaseTestProcessGraph):
     @pytest.fixture
     def features(self) -> Features:
         return Features({"x": Value("int32")})
 
     @pytest.fixture
     def pipe(self) -> DataPipe:
```

### Comparing `hyped-0.1.0a1/tests/hyped/data/test_pipe.py` & `hyped-0.1.0a2/tests/hyped/data/test_pipe.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,111 @@
 import datasets
 import pytest
 
+from hyped.common.feature_key import FeatureKey
 from hyped.data.pipe import DataPipe
+from hyped.data.processors.features.format import (
+    FormatFeatures,
+    FormatFeaturesConfig,
+)
 from hyped.data.processors.statistics.report import StatisticsReport
 from tests.hyped.data.processors.statistics.test_base import (
     ConstantStatistic,
     ConstantStatisticConfig,
 )
 from tests.hyped.data.processors.test_base import (
     ConstantDataProcessor,
     ConstantDataProcessorConfig,
 )
 
 
-@pytest.fixture
-def sample_data_pipe():
-    # create data processor configs
-    c1 = ConstantDataProcessorConfig(name="A", value="1")
-    c2 = ConstantDataProcessorConfig(name="B", value="2")
-    c3 = ConstantDataProcessorConfig(name="C", value="3")
-    # create data processors
-    p1 = ConstantDataProcessor(c1)
-    p2 = ConstantDataProcessor(c2)
-    p3 = ConstantDataProcessor(c3)
-    # create data pipe
-    return DataPipe([p1, p2, p3])
+@pytest.mark.parametrize(
+    "pipe,required_keys",
+    [
+        (
+            DataPipe(
+                [
+                    FormatFeatures(
+                        FormatFeaturesConfig(
+                            output_format={
+                                "X": "x",
+                                "Y": "y",
+                            }
+                        )
+                    )
+                ]
+            ),
+            [FeatureKey("x"), FeatureKey("y")],
+        ),
+        (
+            DataPipe(
+                [
+                    FormatFeatures(
+                        FormatFeaturesConfig(
+                            output_format={
+                                "X": "x",
+                                "Y": "y",
+                            }
+                        )
+                    ),
+                    FormatFeatures(
+                        FormatFeaturesConfig(
+                            output_format={
+                                "Z": "Y",
+                            }
+                        ),
+                    ),
+                ]
+            ),
+            [FeatureKey("x"), FeatureKey("y")],
+        ),
+    ],
+)
+def test_required_feature_keys(pipe, required_keys):
+    pipe.prepare(
+        datasets.Features(
+            {
+                "x": datasets.Value("int32"),
+                "y": datasets.Value("int32"),
+                "a": datasets.Value("int32"),
+                "b": datasets.Value("int32"),
+            }
+        )
+    )
+
+    pipe_required_keys = list(pipe.required_feature_keys)
+    # check
+    assert len(pipe_required_keys) == len(required_keys)
+    assert all(k in required_keys for k in pipe_required_keys)
 
 
 class TestDataPipe:
+    @pytest.fixture(params=["flat", "nested_1", "nested_2"])
+    def sample_data_pipe(self, request):
+        # create data processor configs
+        c1 = ConstantDataProcessorConfig(name="A", value="1")
+        c2 = ConstantDataProcessorConfig(name="B", value="2")
+        c3 = ConstantDataProcessorConfig(name="C", value="3")
+        # create data processors
+        p1 = ConstantDataProcessor(c1)
+        p2 = ConstantDataProcessor(c2)
+        p3 = ConstantDataProcessor(c3)
+
+        # create data pipe
+        if request.param == "flat":
+            return DataPipe([p1, p2, p3])
+        if request.param == "nested_1":
+            return DataPipe([DataPipe([p1]), DataPipe([p2, p3])])
+        if request.param == "nested_2":
+            return DataPipe(
+                [DataPipe([DataPipe([p1])]), DataPipe([p2, DataPipe([p3])])]
+            )
+
+        raise ValueError(request.param)
+
     def test_preparation_logic(self, sample_data_pipe):
         assert not sample_data_pipe.is_prepared
 
         # create different input features
         x = datasets.Features({"X": datasets.Value("int32")})
         y = datasets.Features({"Y": datasets.Value("int32")})
```

