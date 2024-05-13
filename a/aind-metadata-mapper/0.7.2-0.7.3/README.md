# Comparing `tmp/aind_metadata_mapper-0.7.2.tar.gz` & `tmp/aind_metadata_mapper-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_mapper-0.7.2.tar", last modified: Fri May 10 19:09:02 2024, max compression
+gzip compressed data, was "aind_metadata_mapper-0.7.3.tar", last modified: Mon May 13 16:56:29 2024, max compression
```

## Comparing `aind_metadata_mapper-0.7.2.tar` & `aind_metadata_mapper-0.7.3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.610274 aind_metadata_mapper-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.586274 aind_metadata_mapper-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.590274 aind_metadata_mapper-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.590274 aind_metadata_mapper-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-10 19:09:02.610274 aind_metadata_mapper-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.594274 aind_metadata_mapper-0.7.2/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.594274 aind_metadata_mapper-0.7.2/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.594274 aind_metadata_mapper-0.7.2/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.594274 aind_metadata_mapper-0.7.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.594274 aind_metadata_mapper-0.7.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/scripts/singularity_build.def
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:09:02.610274 aind_metadata_mapper-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.586274 aind_metadata_mapper-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.594274 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.594274 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.598274 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.598274 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.598274 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/fib/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/fib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/fib/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/gather_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.598274 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.606274 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-10 19:09:02.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-10 19:09:02.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:09:02.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-10 19:09:02.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 19:09:02.000000 aind_metadata_mapper-0.7.2/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.598274 aind_metadata_mapper-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.590274 aind_metadata_mapper-0.7.2/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.598274 aind_metadata_mapper-0.7.2/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.602274 aind_metadata_mapper-0.7.2/tests/resources/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.602274 aind_metadata_mapper-0.7.2/tests/resources/fib/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/fib/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/fib/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/fib/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.602274 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/example_funding_multiple_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/example_funding_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/example_procedures_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/example_subject_response.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.602274 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/metadata_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/metadata_files/data_description.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/metadata_files/procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/metadata_files/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/metadata_files/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.602274 aind_metadata_mapper-0.7.2/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/mesoscope/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.606274 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/base-missing-probe_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/base_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/mvr.ini
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/mvr_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/open-ephys-inferred_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/open-ephys_rig.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/sync.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/resources/neuropixels/sync_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_bergamo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:02.606274 aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/test_mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/test_neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/test_open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/test_sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_fib.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_gather_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_legacy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-10 19:08:48.000000 aind_metadata_mapper-0.7.2/tests/test_mesoscope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.190538 aind_metadata_mapper-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.166538 aind_metadata_mapper-0.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.170538 aind_metadata_mapper-0.7.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.170538 aind_metadata_mapper-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-13 16:56:29.190538 aind_metadata_mapper-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.170538 aind_metadata_mapper-0.7.3/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.170538 aind_metadata_mapper-0.7.3/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.174538 aind_metadata_mapper-0.7.3/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.174538 aind_metadata_mapper-0.7.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.174538 aind_metadata_mapper-0.7.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/scripts/singularity_build.def
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:56:29.190538 aind_metadata_mapper-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.166538 aind_metadata_mapper-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.174538 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.174538 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.174538 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.174538 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.178538 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/fib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/fib/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/gather_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.178538 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.186538 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-13 16:56:29.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-13 16:56:29.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:56:29.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 16:56:29.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 16:56:29.000000 aind_metadata_mapper-0.7.3/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.178538 aind_metadata_mapper-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.170538 aind_metadata_mapper-0.7.3/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.178538 aind_metadata_mapper-0.7.3/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.178538 aind_metadata_mapper-0.7.3/tests/resources/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.182538 aind_metadata_mapper-0.7.3/tests/resources/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/fib/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/fib/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/fib/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.182538 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/example_funding_multiple_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/example_funding_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/example_procedures_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/example_subject_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.182538 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/metadata_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/metadata_files/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/metadata_files/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/metadata_files/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/metadata_files/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.182538 aind_metadata_mapper-0.7.3/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.186538 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/resources/neuropixels/sync_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_bergamo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:56:29.186538 aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/test_open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_ephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_fib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18222 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_gather_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_legacy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-13 16:56:15.000000 aind_metadata_mapper-0.7.3/tests/test_mesoscope.py
```

### Comparing `aind_metadata_mapper-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_mapper-0.7.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_mapper-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_mapper-0.7.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/.github/workflows/tag_and_publish.yml` & `aind_metadata_mapper-0.7.3/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/.github/workflows/test_and_lint.yml` & `aind_metadata_mapper-0.7.3/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/.gitignore` & `aind_metadata_mapper-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/LICENSE` & `aind_metadata_mapper-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/PKG-INFO` & `aind_metadata_mapper-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.7.2
+Version: 0.7.3
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aind-data-schema==0.33.3
+Requires-Dist: aind-data-schema==0.36.0
+Requires-Dist: aind-data-schema-models==0.1.1
 Requires-Dist: scanimage-tiff-reader==1.4.1.4
 Requires-Dist: tifffile==2024.2.12
 Requires-Dist: pydantic-settings>=2.0
 Requires-Dist: requests
 Requires-Dist: pillow
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `aind_metadata_mapper-0.7.2/README.md` & `aind_metadata_mapper-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/doc_template/Makefile` & `aind_metadata_mapper-0.7.3/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/doc_template/make.bat` & `aind_metadata_mapper-0.7.3/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/doc_template/source/_static/dark-logo.svg` & `aind_metadata_mapper-0.7.3/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/doc_template/source/_static/favicon.ico` & `aind_metadata_mapper-0.7.3/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/doc_template/source/_static/light-logo.svg` & `aind_metadata_mapper-0.7.3/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/doc_template/source/conf.py` & `aind_metadata_mapper-0.7.3/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/examples/bergamo_session.py` & `aind_metadata_mapper-0.7.3/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/pyproject.toml` & `aind_metadata_mapper-0.7.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
-    "aind-data-schema==0.33.3",
+    "aind-data-schema==0.36.0",
+    "aind-data-schema-models==0.1.1",
     "scanimage-tiff-reader==1.4.1.4",
     "tifffile==2024.2.12",
     "pydantic-settings>=2.0",
     "requests",
     "pillow"
 ]
```

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/bergamo/session.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/bergamo/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 import sys
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
+from aind_data_schema.components.stimulus import (
+    PhotoStimulation,
+    PhotoStimulationGroup,
+)
 from aind_data_schema.core.session import (
     DetectorConfig,
     FieldOfView,
     LaserConfig,
     Modality,
     Session,
     StimulusEpoch,
     StimulusModality,
     Stream,
 )
-from aind_data_schema.models.stimulus import (
-    PhotoStimulation,
-    PhotoStimulationGroup,
-)
-from aind_data_schema.models.units import PowerUnit, SizeUnit
+from aind_data_schema_models.units import PowerUnit, SizeUnit
 from pydantic import Field
 from pydantic_settings import BaseSettings
 from ScanImageTiffReader import ScanImageTiffReader
 
 from aind_metadata_mapper.core import GenericEtl, JobResponse
```

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/core.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ETL for the MVR config."""
 
 import logging
 from pathlib import Path
 from typing import Dict, List, Tuple
 
+from aind_data_schema.components.devices import Software  # type: ignore
 from aind_data_schema.core.rig import Rig  # type: ignore
-from aind_data_schema.models.devices import Software  # type: ignore
 
 from aind_metadata_mapper.dynamic_routing import utils
 from aind_metadata_mapper.dynamic_routing.neuropixels_rig import (
     NeuropixelsRigContext,
     NeuropixelsRigEtl,
 )
```

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/open_ephys_rig.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/open_ephys_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/sync_rig.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/sync_rig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ETL for the Sync config."""
 
 from pathlib import Path
 
+from aind_data_schema.components.devices import DAQChannel  # type: ignore
 from aind_data_schema.core.rig import Rig  # type: ignore
-from aind_data_schema.models.devices import DAQChannel  # type: ignore
 from pydantic import BaseModel
 
 from aind_metadata_mapper.dynamic_routing import utils
 from aind_metadata_mapper.dynamic_routing.neuropixels_rig import (
     NeuropixelsRigContext,
     NeuropixelsRigEtl,
 )
```

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/dynamic_routing/utils.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/dynamic_routing/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/ephys/session.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/ephys/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module to write valid ephys schemas"""
 
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 
 from aind_data_schema.core.session import Session
-from aind_data_schema.models.modalities import Modality
+from aind_data_schema_models.modalities import Modality
 
 from aind_metadata_mapper.core import BaseEtl
 
 
 @dataclass(frozen=True)
 class ParsedInformation:
     """RawImageInfo gets parsed into this data"""
```

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/fib/session.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/fib/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import re
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import List, Optional, Union
 
+from aind_data_schema.components.stimulus import OptoStimulation, PulseShape
 from aind_data_schema.core.session import (
     DetectorConfig,
     FiberConnectionConfig,
     LightEmittingDiodeConfig,
     Session,
     StimulusEpoch,
     StimulusModality,
     Stream,
 )
-from aind_data_schema.models.modalities import Modality
-from aind_data_schema.models.stimulus import OptoStimulation, PulseShape
+from aind_data_schema_models.modalities import Modality
 from pydantic import Field
 from pydantic_settings import BaseSettings
 
 from aind_metadata_mapper.core import GenericEtl, JobResponse
 
 
 class JobSettings(BaseSettings):
```

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/gather_metadata.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/gather_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from aind_data_schema.core.instrument import Instrument
 from aind_data_schema.core.metadata import Metadata
 from aind_data_schema.core.procedures import Procedures
 from aind_data_schema.core.processing import PipelineProcess, Processing
 from aind_data_schema.core.rig import Rig
 from aind_data_schema.core.session import Session
 from aind_data_schema.core.subject import Subject
-from aind_data_schema.models.modalities import Modality
-from aind_data_schema.models.organizations import Organization
-from aind_data_schema.models.pid_names import PIDName
+from aind_data_schema_models.modalities import Modality
+from aind_data_schema_models.organizations import Organization
+from aind_data_schema_models.pid_names import PIDName
 from pydantic import ValidationError
 from pydantic_settings import BaseSettings
 
 
 class SubjectSettings(BaseSettings):
     """Fields needed to retrieve subject metadata"""
```

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper/mesoscope/session.py` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from datetime import datetime
 from pathlib import Path
 from typing import List, Union
 
 import tifffile
 from aind_data_schema.core.session import FieldOfView, Session, Stream
-from aind_data_schema.models.modalities import Modality
+from aind_data_schema_models.modalities import Modality
 from PIL import Image
 from PIL.TiffTags import TAGS
 from pydantic import Field
 from pydantic_settings import BaseSettings
 
 from aind_metadata_mapper.core import GenericEtl
```

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.7.2
+Version: 0.7.3
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aind-data-schema==0.33.3
+Requires-Dist: aind-data-schema==0.36.0
+Requires-Dist: aind-data-schema-models==0.1.1
 Requires-Dist: scanimage-tiff-reader==1.4.1.4
 Requires-Dist: tifffile==2024.2.12
 Requires-Dist: pydantic-settings>=2.0
 Requires-Dist: requests
 Requires-Dist: pillow
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
```

### Comparing `aind_metadata_mapper-0.7.2/src/aind_metadata_mapper.egg-info/SOURCES.txt` & `aind_metadata_mapper-0.7.3/src/aind_metadata_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind_metadata_mapper-0.7.3/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/bergamo/example_description0.txt` & `aind_metadata_mapper-0.7.3/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/bergamo/example_metadata.txt.gz` & `aind_metadata_mapper-0.7.3/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/bergamo/expected_session.json` & `aind_metadata_mapper-0.7.3/tests/resources/bergamo/expected_session.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9351610725308642%*

 * *Differences: {"'anaesthesia'": 'None',*

 * * "'data_streams'": "{0: {'ophys_fovs': {0: {'power_ratio': None}}, 'mri_scans': [], 'software': "*

 * *                   '[]}}',*

 * * "'schema_version'": "'0.2.6'"}*

```diff
@@ -1,9 +1,10 @@
 {
     "active_mouse_platform": true,
+    "anaesthesia": null,
     "animal_weight_post": null,
     "animal_weight_prior": null,
     "calibrations": [],
     "data_streams": [
         {
             "camera_names": [
                 "Side Camera"
@@ -27,14 +28,15 @@
                     "excitation_power_unit": "percent",
                     "name": "Laser A",
                     "wavelength": 920,
                     "wavelength_unit": "nanometer"
                 }
             ],
             "manipulator_modules": [],
+            "mri_scans": [],
             "notes": null,
             "ophys_fovs": [
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -48,22 +50,24 @@
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 150,
                     "imaging_depth_unit": "micrometer",
                     "index": 0,
                     "magnification": "16x",
                     "notes": null,
                     "power": null,
+                    "power_ratio": null,
                     "power_unit": "percent",
                     "scanfield_z": null,
                     "scanfield_z_unit": "micrometer",
                     "scanimage_roi_index": null,
                     "targeted_structure": "M1"
                 }
             ],
             "slap_fovs": null,
+            "software": [],
             "stack_parameters": null,
             "stick_microscopes": [],
             "stream_end_time": "2023-10-10T16:00:00Z",
             "stream_modalities": [
                 {
                     "abbreviation": "ophys",
                     "name": "Planar optical physiology"
@@ -82,15 +86,15 @@
     "mouse_platform_name": "some_mouse_platform_name",
     "notes": null,
     "protocol_id": [],
     "reward_consumed_total": null,
     "reward_consumed_unit": "microliter",
     "reward_delivery": null,
     "rig_id": "Bergamo photostim.",
-    "schema_version": "0.2.1",
+    "schema_version": "0.2.6",
     "session_end_time": "2023-10-10T17:00:00Z",
     "session_start_time": "2023-10-10T14:00:00Z",
     "session_type": "BCI",
     "stimulus_epochs": [
         {
             "light_source_config": null,
             "notes": null,
```

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/ephys/ephys_session.json` & `aind_metadata_mapper-0.7.3/tests/resources/ephys/ephys_session.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'schema_version'": "'0.2.6'"}*

```diff
@@ -280,15 +280,15 @@
     "mouse_platform_name": "Running Wheel",
     "notes": null,
     "protocol_id": [],
     "reward_consumed_total": null,
     "reward_consumed_unit": "microliter",
     "reward_delivery": null,
     "rig_id": "323_EPHYS2-RF_2024-01-18_01",
-    "schema_version": "0.2.1",
+    "schema_version": "0.2.6",
     "session_end_time": "2023-04-06T13:47:57.558000Z",
     "session_start_time": "2023-04-04T10:37:28Z",
     "session_type": "Receptive field mapping",
     "stimulus_epochs": [],
     "subject_id": "699889",
     "weight_unit": "gram"
 }
```

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/ephys/newscale_main.csv` & `aind_metadata_mapper-0.7.3/tests/resources/ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/ephys/newscale_surface_finding.csv` & `aind_metadata_mapper-0.7.3/tests/resources/ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/ephys/settings_main.xml` & `aind_metadata_mapper-0.7.3/tests/resources/ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/ephys/settings_surface_finding.xml` & `aind_metadata_mapper-0.7.3/tests/resources/ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/fib/000000_ophys_rig.json` & `aind_metadata_mapper-0.7.3/tests/resources/fib/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/fib/000000_ophys_session.json` & `aind_metadata_mapper-0.7.3/tests/resources/fib/000000_ophys_session.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'schema_version'": "'0.2.6'"}*

```diff
@@ -70,15 +70,15 @@
     "mouse_platform_name": "Disc",
     "notes": "brabrabrabra....",
     "protocol_id": [],
     "reward_consumed_total": null,
     "reward_consumed_unit": "microliter",
     "reward_delivery": null,
     "rig_id": "ophys_rig",
-    "schema_version": "0.2.1",
+    "schema_version": "0.2.6",
     "session_end_time": "1999-10-04T00:00:48Z",
     "session_start_time": "1999-10-04T00:00:00Z",
     "session_type": "Foraging_Photometry",
     "stimulus_epochs": [
         {
             "light_source_config": null,
             "notes": null,
```

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/example_funding_multiple_response.json` & `aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/example_funding_multiple_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/example_procedures_response.json` & `aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/example_procedures_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/example_subject_response.json` & `aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/example_subject_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/metadata_files/data_description.json` & `aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/metadata_files/data_description.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/metadata_files/procedures.json` & `aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/metadata_files/procedures.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/metadata_files/processing.json` & `aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/metadata_files/processing.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/gather_metadata_job/metadata_files/subject.json` & `aind_metadata_mapper-0.7.3/tests/resources/gather_metadata_job/metadata_files/subject.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind_metadata_mapper-0.7.3/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind_metadata_mapper-0.7.3/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind_metadata_mapper-0.7.3/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/mesoscope/example_extract.json` & `aind_metadata_mapper-0.7.3/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/mesoscope/example_platform.json` & `aind_metadata_mapper-0.7.3/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/mesoscope/expected_session.json` & `aind_metadata_mapper-0.7.3/tests/resources/mesoscope/expected_session.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.935180362654321%*

 * *Differences: {"'anaesthesia'": 'None',*

 * * "'data_streams'": "{0: {'ophys_fovs': {0: {'power_ratio': None}, 1: {'power_ratio': None}, 2: "*

 * *                   "{'power_ratio': None}, 3: {'power_ratio': None}, 4: {'power_ratio': None}, 5: "*

 * *                   "{'power_ratio': None}, 6: {'power_ratio': None}, 7: {'power_ratio': None}}, "*

 * *                   "'mri_scans': [], 'software': []}, 1: {'mri_scans': [], 'software': []}, 2: "*

 * *                   "{'mri_scans': [], 'software': []}, 3: {'mri_scans': [], 'software': []}, 4 […]*

```diff
@@ -1,9 +1,10 @@
 {
     "active_mouse_platform": true,
+    "anaesthesia": null,
     "animal_weight_post": null,
     "animal_weight_prior": null,
     "calibrations": [],
     "data_streams": [
         {
             "camera_names": [
                 "Mesoscope"
@@ -11,14 +12,15 @@
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
+            "mri_scans": [],
             "notes": null,
             "ophys_fovs": [
                 {
                     "coupled_fov_index": null,
                     "fov_coordinate_ap": "1.5",
                     "fov_coordinate_ml": "1.5",
                     "fov_coordinate_unit": "micrometer",
@@ -32,14 +34,15 @@
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 190,
                     "imaging_depth_unit": "micrometer",
                     "index": 0,
                     "magnification": "16x",
                     "notes": null,
                     "power": null,
+                    "power_ratio": null,
                     "power_unit": "percent",
                     "scanfield_z": null,
                     "scanfield_z_unit": "micrometer",
                     "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
@@ -57,14 +60,15 @@
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 232,
                     "imaging_depth_unit": "micrometer",
                     "index": 0,
                     "magnification": "16x",
                     "notes": null,
                     "power": null,
+                    "power_ratio": null,
                     "power_unit": "percent",
                     "scanfield_z": null,
                     "scanfield_z_unit": "micrometer",
                     "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
@@ -82,14 +86,15 @@
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 136,
                     "imaging_depth_unit": "micrometer",
                     "index": 1,
                     "magnification": "16x",
                     "notes": null,
                     "power": null,
+                    "power_ratio": null,
                     "power_unit": "percent",
                     "scanfield_z": null,
                     "scanfield_z_unit": "micrometer",
                     "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
@@ -107,14 +112,15 @@
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 282,
                     "imaging_depth_unit": "micrometer",
                     "index": 1,
                     "magnification": "16x",
                     "notes": null,
                     "power": null,
+                    "power_ratio": null,
                     "power_unit": "percent",
                     "scanfield_z": null,
                     "scanfield_z_unit": "micrometer",
                     "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
@@ -132,14 +138,15 @@
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 72,
                     "imaging_depth_unit": "micrometer",
                     "index": 2,
                     "magnification": "16x",
                     "notes": null,
                     "power": null,
+                    "power_ratio": null,
                     "power_unit": "percent",
                     "scanfield_z": null,
                     "scanfield_z_unit": "micrometer",
                     "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
@@ -157,14 +164,15 @@
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 326,
                     "imaging_depth_unit": "micrometer",
                     "index": 2,
                     "magnification": "16x",
                     "notes": null,
                     "power": null,
+                    "power_ratio": null,
                     "power_unit": "percent",
                     "scanfield_z": null,
                     "scanfield_z_unit": "micrometer",
                     "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
@@ -182,14 +190,15 @@
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 30,
                     "imaging_depth_unit": "micrometer",
                     "index": 3,
                     "magnification": "16x",
                     "notes": null,
                     "power": null,
+                    "power_ratio": null,
                     "power_unit": "percent",
                     "scanfield_z": null,
                     "scanfield_z_unit": "micrometer",
                     "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 },
                 {
@@ -207,22 +216,24 @@
                     "frame_rate_unit": "hertz",
                     "imaging_depth": 364,
                     "imaging_depth_unit": "micrometer",
                     "index": 3,
                     "magnification": "16x",
                     "notes": null,
                     "power": null,
+                    "power_ratio": null,
                     "power_unit": "percent",
                     "scanfield_z": null,
                     "scanfield_z_unit": "micrometer",
                     "scanimage_roi_index": null,
                     "targeted_structure": "VISp"
                 }
             ],
             "slap_fovs": null,
+            "software": [],
             "stack_parameters": null,
             "stick_microscopes": [],
             "stream_end_time": "2024-02-22T17:30:00Z",
             "stream_modalities": [
                 {
                     "abbreviation": "ophys",
                     "name": "Planar optical physiology"
@@ -237,17 +248,19 @@
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
+            "mri_scans": [],
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
+            "software": [],
             "stack_parameters": null,
             "stick_microscopes": [],
             "stream_end_time": "2024-02-12T10:30:54Z",
             "stream_modalities": [
                 {
                     "abbreviation": "behavior-videos",
                     "name": "Behavior videos"
@@ -262,17 +275,19 @@
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
+            "mri_scans": [],
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
+            "software": [],
             "stack_parameters": null,
             "stick_microscopes": [],
             "stream_end_time": "2024-02-12T10:30:55Z",
             "stream_modalities": [
                 {
                     "abbreviation": "behavior-videos",
                     "name": "Behavior videos"
@@ -287,17 +302,19 @@
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
+            "mri_scans": [],
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
+            "software": [],
             "stack_parameters": null,
             "stick_microscopes": [],
             "stream_end_time": "2024-02-12T10:30:55Z",
             "stream_modalities": [
                 {
                     "abbreviation": "behavior-videos",
                     "name": "Behavior videos"
@@ -312,17 +329,19 @@
             "daq_names": [],
             "detectors": [],
             "ephys_modules": [],
             "fiber_connections": [],
             "fiber_modules": [],
             "light_sources": [],
             "manipulator_modules": [],
+            "mri_scans": [],
             "notes": null,
             "ophys_fovs": [],
             "slap_fovs": null,
+            "software": [],
             "stack_parameters": null,
             "stick_microscopes": [],
             "stream_end_time": "2024-02-12T11:02:22Z",
             "stream_modalities": [
                 {
                     "abbreviation": "confocal",
                     "name": "Confocal microscopy"
@@ -340,15 +359,15 @@
     "mouse_platform_name": "disc",
     "notes": null,
     "protocol_id": [],
     "reward_consumed_total": null,
     "reward_consumed_unit": "microliter",
     "reward_delivery": null,
     "rig_id": "MESO.1",
-    "schema_version": "0.2.1",
+    "schema_version": "0.2.6",
     "session_end_time": "2024-02-22T17:30:00Z",
     "session_start_time": "2024-02-22T15:30:00Z",
     "session_type": "Mesoscope",
     "stimulus_epochs": [],
     "subject_id": "12345",
     "weight_unit": "gram"
 }
```

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/base-missing-probe_rig.json` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/base-missing-probe_rig.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827586206896551%*

 * *Differences: {"'schema_version'": "'0.3.8'"}*

```diff
@@ -1012,15 +1012,15 @@
         },
         {
             "direction": "Positive pointing up.",
             "name": "Z"
         }
     ],
     "rig_id": "327_NP2_240401",
-    "schema_version": "0.3.2",
+    "schema_version": "0.3.8",
     "stick_microscopes": [],
     "stimulus_devices": [
         {
             "additional_settings": {},
             "brightness": 43,
             "contrast": 50,
             "device_type": "Monitor",
```

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/base_rig.json` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/base_rig.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827586206896551%*

 * *Differences: {"'schema_version'": "'0.3.8'"}*

```diff
@@ -1055,15 +1055,15 @@
         },
         {
             "direction": "Positive pointing up.",
             "name": "Z"
         }
     ],
     "rig_id": "327_NP2_240401",
-    "schema_version": "0.3.2",
+    "schema_version": "0.3.8",
     "stick_microscopes": [],
     "stimulus_devices": [
         {
             "additional_settings": {},
             "brightness": 43,
             "contrast": 50,
             "device_type": "Monitor",
```

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/mvr.ini` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/mvr.ini`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/mvr_rig.json` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/mvr_rig.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827586206896551%*

 * *Differences: {"'schema_version'": "'0.3.8'"}*

```diff
@@ -1070,15 +1070,15 @@
         },
         {
             "direction": "Positive pointing up.",
             "name": "Z"
         }
     ],
     "rig_id": "327_NP2_240401",
-    "schema_version": "0.3.2",
+    "schema_version": "0.3.8",
     "stick_microscopes": [],
     "stimulus_devices": [
         {
             "additional_settings": {},
             "brightness": 43,
             "contrast": 50,
             "device_type": "Monitor",
```

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/open-ephys-inferred_rig.json` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/open-ephys-inferred_rig.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827586206896551%*

 * *Differences: {"'schema_version'": "'0.3.8'"}*

```diff
@@ -1055,15 +1055,15 @@
         },
         {
             "direction": "Positive pointing up.",
             "name": "Z"
         }
     ],
     "rig_id": "327_NP2_240401",
-    "schema_version": "0.3.2",
+    "schema_version": "0.3.8",
     "stick_microscopes": [],
     "stimulus_devices": [
         {
             "additional_settings": {},
             "brightness": 43,
             "contrast": 50,
             "device_type": "Monitor",
```

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/open-ephys_rig.json` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/open-ephys_rig.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827586206896551%*

 * *Differences: {"'schema_version'": "'0.3.8'"}*

```diff
@@ -1055,15 +1055,15 @@
         },
         {
             "direction": "Positive pointing up.",
             "name": "Z"
         }
     ],
     "rig_id": "327_NP2_240401",
-    "schema_version": "0.3.2",
+    "schema_version": "0.3.8",
     "stick_microscopes": [],
     "stimulus_devices": [
         {
             "additional_settings": {},
             "brightness": 43,
             "contrast": 50,
             "device_type": "Monitor",
```

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/settings.mislabeled-probes-0.xml` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/settings.mislabeled-probes-0.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/settings.mislabeled-probes-1.xml` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/settings.mislabeled-probes-1.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/settings.xml` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/settings.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/sync.yml` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/sync.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/resources/neuropixels/sync_rig.json` & `aind_metadata_mapper-0.7.3/tests/resources/neuropixels/sync_rig.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827586206896551%*

 * *Differences: {"'schema_version'": "'0.3.8'"}*

```diff
@@ -1216,15 +1216,15 @@
         },
         {
             "direction": "Positive pointing up.",
             "name": "Z"
         }
     ],
     "rig_id": "327_NP2_240401",
-    "schema_version": "0.3.2",
+    "schema_version": "0.3.8",
     "stick_microscopes": [],
     "stimulus_devices": [
         {
             "additional_settings": {},
             "brightness": 43,
             "contrast": 50,
             "device_type": "Monitor",
```

### Comparing `aind_metadata_mapper-0.7.2/tests/test_bergamo.py` & `aind_metadata_mapper-0.7.3/tests/test_bergamo.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/test_mvr_rig.py` & `aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/test_mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/test_neuropixels_rig.py` & `aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/test_neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/test_open_ephys_rig.py` & `aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/test_open_ephys_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/test_sync_rig.py` & `aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/test_sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/test_dynamic_routing/utils.py` & `aind_metadata_mapper-0.7.3/tests/test_dynamic_routing/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/test_ephys.py` & `aind_metadata_mapper-0.7.3/tests/test_ephys.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/test_fib.py` & `aind_metadata_mapper-0.7.3/tests/test_fib.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.2/tests/test_gather_metadata.py` & `aind_metadata_mapper-0.7.3/tests/test_gather_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import os
 import unittest
 from datetime import datetime, timezone
 from pathlib import Path
 from unittest.mock import MagicMock, mock_open, patch
 
 from aind_data_schema.core.processing import DataProcess, PipelineProcess
-from aind_data_schema.models.modalities import Modality
-from aind_data_schema.models.process_names import ProcessName
+from aind_data_schema_models.modalities import Modality
+from aind_data_schema_models.process_names import ProcessName
 from requests import Response
 
 from aind_metadata_mapper.gather_metadata import (
     GatherMetadataJob,
     JobSettings,
     MetadataSettings,
     ProceduresSettings,
@@ -307,23 +307,28 @@
         )
         metadata_job = GatherMetadataJob(settings=job_settings)
         with self.assertWarns(UserWarning) as w:
             main_metadata = metadata_job.get_main_metadata()
         # Issues with incomplete Procedures model raises warnings
         expected_warnings = (
             "Pydantic serializer warnings:\n"
-            "  Expected `Union[Surgery, TrainingProtocol, WaterRestriction,"
-            " definition-ref]` but got `dict` -"
-            " serialized value may not be as expected\n"
-            "  Expected `Union[Surgery, TrainingProtocol, WaterRestriction,"
-            " definition-ref]` but got `dict` -"
-            " serialized value may not be as expected"
+            "  Expected `date` but got `str`"
+            " - serialized value may not be as expected\n"
+            "  Expected `Union[CallithrixJacchus, HomoSapiens, MacacaMulatta, "
+            "MusMusculus, RattusNorvegicus]` but got `dict`"
+            " - serialized value may not be as expected\n"
+            "  Expected `BreedingInfo` but got `dict`"
+            " - serialized value may not be as expected\n"
+            "  Expected `Union[AllenInstitute, ColumbiaUniversity,"
+            " HuazhongUniversityOfScienceAndTechnology, JacksonLaboratory,"
+            " NewYorkUniversity, Other]` but got `dict`"
+            " - serialized value may not be as expected"
         )
-        self.assertEqual(expected_warnings, str(w.warning))
 
+        self.assertEqual(expected_warnings, str(w.warning))
         self.assertEqual(
             "s3://some-bucket/ecephys_632269_2023-10-10_10-10-10",
             main_metadata.location,
         )
         self.assertEqual("Invalid", main_metadata.metadata_status.value)
         self.assertEqual("632269", main_metadata.subject.subject_id)
```

### Comparing `aind_metadata_mapper-0.7.2/tests/test_legacy_core.py` & `aind_metadata_mapper-0.7.3/tests/test_legacy_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pathlib import Path
 from typing import Any
 from unittest import TestCase
 from unittest import main as unittest_main
 from unittest.mock import MagicMock, patch
 
 from aind_data_schema.core.subject import BreedingInfo, Housing, Sex, Subject
-from aind_data_schema.models.organizations import Organization
-from aind_data_schema.models.species import Species
+from aind_data_schema_models.organizations import Organization
+from aind_data_schema_models.species import Species
 
 from aind_metadata_mapper.core import BaseEtl
 
 
 class TestBaseEtl(TestCase):
     """Tests methods in the legacy BaseEtl class."""
```

### Comparing `aind_metadata_mapper-0.7.2/tests/test_mesoscope.py` & `aind_metadata_mapper-0.7.3/tests/test_mesoscope.py`

 * *Files identical despite different names*

