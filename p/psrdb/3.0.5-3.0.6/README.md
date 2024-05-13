# Comparing `tmp/psrdb-3.0.5.tar.gz` & `tmp/psrdb-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psrdb-3.0.5.tar", max compression
+gzip compressed data, was "psrdb-3.0.6.tar", max compression
```

## Comparing `psrdb-3.0.5.tar` & `psrdb-3.0.6.tar`

### file list

```diff
@@ -1,91 +1,39 @@
--rw-r--r--   0        0        0    35149 2023-05-30 05:15:57.018989 psrdb-3.0.5/LICENSE
--rw-r--r--   0        0        0        0 2023-05-30 05:15:57.018989 psrdb-3.0.5/psrdb/__init__.py
--rw-r--r--   0        0        0    14969 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/l_band_gain_calibrators.csv
--rw-r--r--   0        0        0     3147 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/molonglo_phasing.txt
--rw-r--r--   0        0        0     1782 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/polarisation_calibrators.csv
--rw-r--r--   0        0        0     5680 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/s_band_gain_calibrators.csv
--rw-r--r--   0        0        0     5441 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/data/uhf_band_gain_calibrators.csv
--rw-r--r--   0        0        0     2758 2024-04-08 04:00:36.591981 psrdb-3.0.5/psrdb/graphql_client.py
--rw-r--r--   0        0        0    10552 2024-04-18 06:36:18.652677 psrdb-3.0.5/psrdb/graphql_table.py
--rw-r--r--   0        0        0      328 2023-05-30 05:16:50.098246 psrdb-3.0.5/psrdb/joins/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5549 2023-05-30 05:16:50.098246 psrdb-3.0.5/psrdb/joins/__pycache__/folded_observations.cpython-310.pyc
--rw-r--r--   0        0        0     1603 2023-05-30 05:16:50.098246 psrdb-3.0.5/psrdb/joins/__pycache__/graphql_join.cpython-310.pyc
--rw-r--r--   0        0        0     5171 2023-05-30 05:16:50.098246 psrdb-3.0.5/psrdb/joins/__pycache__/processed_observations.cpython-310.pyc
--rw-r--r--   0        0        0     5954 2023-05-30 05:16:50.102246 psrdb-3.0.5/psrdb/joins/__pycache__/toaed_observations.cpython-310.pyc
--rw-r--r--   0        0        0      924 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/load_data.py
--rw-r--r--   0        0        0        0 2023-06-02 01:54:24.872472 psrdb-3.0.5/psrdb/scripts/__init__.py
--rw-r--r--   0        0        0      140 2023-06-02 03:15:49.753919 psrdb-3.0.5/psrdb/scripts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5405 2023-12-07 08:15:08.840488 psrdb-3.0.5/psrdb/scripts/__pycache__/generate_molonglo_json.cpython-310.pyc
--rw-r--r--   0        0        0     3611 2023-06-15 01:57:40.726904 psrdb-3.0.5/psrdb/scripts/__pycache__/ingest_obs.cpython-310.pyc
--rw-r--r--   0        0        0     2182 2023-11-07 08:08:02.995828 psrdb-3.0.5/psrdb/scripts/__pycache__/psrdb.cpython-310.pyc
--rw-r--r--   0        0        0     6338 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/scripts/generate_meerkat_json.py
--rw-r--r--   0        0        0     3764 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/scripts/generate_molonglo_json.py
--rwxr-xr-x   0        0        0     4446 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/scripts/ingest_obs.py
--rwxr-xr-x   0        0        0     2613 2024-04-08 04:00:36.591981 psrdb-3.0.5/psrdb/scripts/psrdb.py
--rw-r--r--   0        0        0        0 2023-11-07 08:06:24.331662 psrdb-3.0.5/psrdb/tables/__init__.py
--rw-r--r--   0        0        0      139 2023-11-07 08:07:03.843712 psrdb-3.0.5/psrdb/tables/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4745 2023-08-30 02:33:29.094412 psrdb-3.0.5/psrdb/tables/__pycache__/basebandings.cpython-310.pyc
--rw-r--r--   0        0        0     6244 2024-04-18 06:41:23.569219 psrdb-3.0.5/psrdb/tables/__pycache__/calibration.cpython-310.pyc
--rw-r--r--   0        0        0     4786 2023-08-30 02:33:29.194416 psrdb-3.0.5/psrdb/tables/__pycache__/calibrations.cpython-310.pyc
--rw-r--r--   0        0        0     4616 2023-08-30 02:33:29.198416 psrdb-3.0.5/psrdb/tables/__pycache__/collections.cpython-310.pyc
--rw-r--r--   0        0        0     7794 2023-08-30 02:33:29.202416 psrdb-3.0.5/psrdb/tables/__pycache__/ephemerides.cpython-310.pyc
--rw-r--r--   0        0        0     8683 2024-04-18 06:41:23.541219 psrdb-3.0.5/psrdb/tables/__pycache__/ephemeris.cpython-310.pyc
--rw-r--r--   0        0        0     5806 2023-08-30 02:33:29.202416 psrdb-3.0.5/psrdb/tables/__pycache__/filterbankings.cpython-310.pyc
--rw-r--r--   0        0        0     6196 2023-08-30 02:33:29.206416 psrdb-3.0.5/psrdb/tables/__pycache__/foldings.cpython-310.pyc
--rw-r--r--   0        0        0     4823 2023-08-30 02:33:29.194416 psrdb-3.0.5/psrdb/tables/__pycache__/graphql_query.cpython-310.pyc
--rw-r--r--   0        0        0     9172 2023-08-30 02:33:29.102413 psrdb-3.0.5/psrdb/tables/__pycache__/graphql_table.cpython-310.pyc
--rw-r--r--   0        0        0     6152 2023-08-30 02:33:29.206416 psrdb-3.0.5/psrdb/tables/__pycache__/instrumentconfigs.cpython-310.pyc
--rw-r--r--   0        0        0     5325 2023-08-30 02:33:29.210417 psrdb-3.0.5/psrdb/tables/__pycache__/launches.cpython-310.pyc
--rw-r--r--   0        0        0     5806 2024-04-18 06:41:23.517219 psrdb-3.0.5/psrdb/tables/__pycache__/main_project.cpython-310.pyc
--rw-r--r--   0        0        0    20905 2024-04-18 06:41:23.581219 psrdb-3.0.5/psrdb/tables/__pycache__/observation.cpython-310.pyc
--rw-r--r--   0        0        0     9723 2023-08-30 02:33:29.214417 psrdb-3.0.5/psrdb/tables/__pycache__/observations.cpython-310.pyc
--rw-r--r--   0        0        0     4708 2024-04-18 06:41:23.701220 psrdb-3.0.5/psrdb/tables/__pycache__/pipeline_image.cpython-310.pyc
--rw-r--r--   0        0        0    13575 2024-04-18 06:41:23.669220 psrdb-3.0.5/psrdb/tables/__pycache__/pipeline_run.cpython-310.pyc
--rw-r--r--   0        0        0     5962 2023-08-30 02:33:29.218417 psrdb-3.0.5/psrdb/tables/__pycache__/pipelinefiles.cpython-310.pyc
--rw-r--r--   0        0        0     5962 2023-08-30 02:33:29.214417 psrdb-3.0.5/psrdb/tables/__pycache__/pipelineimages.cpython-310.pyc
--rw-r--r--   0        0        0     5800 2023-08-30 02:33:29.218417 psrdb-3.0.5/psrdb/tables/__pycache__/pipelines.cpython-310.pyc
--rw-r--r--   0        0        0     4960 2023-08-30 02:33:29.222417 psrdb-3.0.5/psrdb/tables/__pycache__/processingcollections.cpython-310.pyc
--rw-r--r--   0        0        0     7283 2023-08-30 02:33:29.222417 psrdb-3.0.5/psrdb/tables/__pycache__/processings.cpython-310.pyc
--rw-r--r--   0        0        0     4694 2023-08-30 02:33:29.226417 psrdb-3.0.5/psrdb/tables/__pycache__/programs.cpython-310.pyc
--rw-r--r--   0        0        0     7073 2024-04-18 06:41:23.529219 psrdb-3.0.5/psrdb/tables/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5641 2023-08-30 02:33:29.226417 psrdb-3.0.5/psrdb/tables/__pycache__/projects.cpython-310.pyc
--rw-r--r--   0        0        0     5982 2023-11-16 01:57:19.167220 psrdb-3.0.5/psrdb/tables/__pycache__/pulsar.cpython-310.pyc
--rw-r--r--   0        0        0     5588 2024-04-18 06:41:23.689220 psrdb-3.0.5/psrdb/tables/__pycache__/pulsar_fold_result.cpython-310.pyc
--rw-r--r--   0        0        0     4654 2023-08-30 02:33:29.230417 psrdb-3.0.5/psrdb/tables/__pycache__/pulsars.cpython-310.pyc
--rw-r--r--   0        0        0     5117 2023-08-30 02:33:29.230417 psrdb-3.0.5/psrdb/tables/__pycache__/pulsartargets.cpython-310.pyc
--rw-r--r--   0        0        0     5476 2024-04-18 06:41:23.741220 psrdb-3.0.5/psrdb/tables/__pycache__/residual.cpython-310.pyc
--rw-r--r--   0        0        0     5747 2023-08-30 02:33:29.234418 psrdb-3.0.5/psrdb/tables/__pycache__/sessions.cpython-310.pyc
--rw-r--r--   0        0        0     4670 2023-08-30 02:33:29.234418 psrdb-3.0.5/psrdb/tables/__pycache__/targets.cpython-310.pyc
--rw-r--r--   0        0        0     5339 2024-04-18 06:41:23.509219 psrdb-3.0.5/psrdb/tables/__pycache__/telescope.cpython-310.pyc
--rw-r--r--   0        0        0     4223 2023-08-30 02:33:29.238417 psrdb-3.0.5/psrdb/tables/__pycache__/telescopes.cpython-310.pyc
--rw-r--r--   0        0        0     4965 2024-04-18 06:41:23.553219 psrdb-3.0.5/psrdb/tables/__pycache__/template.cpython-310.pyc
--rw-r--r--   0        0        0     7037 2023-08-30 02:33:29.242418 psrdb-3.0.5/psrdb/tables/__pycache__/templates.cpython-310.pyc
--rw-r--r--   0        0        0    12044 2024-04-18 06:41:23.717220 psrdb-3.0.5/psrdb/tables/__pycache__/toa.cpython-310.pyc
--rw-r--r--   0        0        0     7754 2023-08-30 02:33:29.242418 psrdb-3.0.5/psrdb/tables/__pycache__/toas.cpython-310.pyc
--rw-r--r--   0        0        0     6182 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/calibration.py
--rw-r--r--   0        0        0    10082 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/ephemeris.py
--rw-r--r--   0        0        0     5761 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/main_project.py
--rw-r--r--   0        0        0    31662 2024-04-18 06:36:18.652677 psrdb-3.0.5/psrdb/tables/observation.py
--rw-r--r--   0        0        0     4779 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/pipeline_image.py
--rw-r--r--   0        0        0    17605 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/pipeline_run.py
--rw-r--r--   0        0        0     7390 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/project.py
--rw-r--r--   0        0        0     6119 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/pulsar.py
--rw-r--r--   0        0        0     7640 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/pulsar_fold_result.py
--rw-r--r--   0        0        0     6381 2024-04-08 04:00:36.591981 psrdb-3.0.5/psrdb/tables/residual.py
--rw-r--r--   0        0        0     5190 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/telescope.py
--rw-r--r--   0        0        0     5419 2023-11-16 01:56:57.828868 psrdb-3.0.5/psrdb/tables/template.py
--rw-r--r--   0        0        0    15643 2024-04-18 06:36:18.656677 psrdb-3.0.5/psrdb/tables/toa.py
--rw-r--r--   0        0        0        0 2023-11-07 08:06:24.335662 psrdb-3.0.5/psrdb/utils/__init__.py
--rw-r--r--   0        0        0      138 2023-11-07 08:07:05.091714 psrdb-3.0.5/psrdb/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3994 2023-12-07 08:15:08.880487 psrdb-3.0.5/psrdb/utils/__pycache__/header.cpython-310.pyc
--rw-r--r--   0        0        0     3554 2024-04-18 06:41:23.497219 psrdb-3.0.5/psrdb/utils/__pycache__/other.cpython-310.pyc
--rw-r--r--   0        0        0     1191 2023-11-07 08:08:03.863830 psrdb-3.0.5/psrdb/utils/__pycache__/residual.cpython-310.pyc
--rw-r--r--   0        0        0     1744 2024-04-18 06:41:23.717220 psrdb-3.0.5/psrdb/utils/__pycache__/toa.cpython-310.pyc
--rw-r--r--   0        0        0     2345 2023-11-07 08:06:35.143673 psrdb-3.0.5/psrdb/utils/ephemeris.py
--rw-r--r--   0        0        0     5879 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/utils/header.py
--rw-r--r--   0        0        0     4044 2024-04-08 04:00:36.591981 psrdb-3.0.5/psrdb/utils/other.py
--rw-r--r--   0        0        0     1318 2023-11-07 08:06:24.335662 psrdb-3.0.5/psrdb/utils/residual.py
--rw-r--r--   0        0        0     1944 2024-04-18 06:36:14.244686 psrdb-3.0.5/psrdb/utils/toa.py
--rw-r--r--   0        0        0      806 2024-03-21 03:33:05.768496 psrdb-3.0.5/psrdb/utils/upload.py
--rw-r--r--   0        0        0     1006 2024-04-18 06:36:18.656677 psrdb-3.0.5/pyproject.toml
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 psrdb-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-23 07:23:00.534055 psrdb-3.0.6/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-23 07:23:00.534055 psrdb-3.0.6/psrdb/__init__.py
+-rw-r--r--   0        0        0    14969 2024-04-08 03:41:36.357745 psrdb-3.0.6/psrdb/data/l_band_gain_calibrators.csv
+-rw-r--r--   0        0        0     3147 2023-12-08 02:19:31.485711 psrdb-3.0.6/psrdb/data/molonglo_phasing.txt
+-rw-r--r--   0        0        0     1782 2024-04-08 03:41:36.361745 psrdb-3.0.6/psrdb/data/polarisation_calibrators.csv
+-rw-r--r--   0        0        0     5680 2024-04-08 03:41:36.361745 psrdb-3.0.6/psrdb/data/s_band_gain_calibrators.csv
+-rw-r--r--   0        0        0     5441 2024-04-08 03:41:36.361745 psrdb-3.0.6/psrdb/data/uhf_band_gain_calibrators.csv
+-rw-r--r--   0        0        0     2829 2024-05-13 01:48:58.303218 psrdb-3.0.6/psrdb/graphql_client.py
+-rw-r--r--   0        0        0    10830 2024-05-13 01:49:04.046977 psrdb-3.0.6/psrdb/graphql_table.py
+-rw-r--r--   0        0        0     1095 2024-05-13 01:49:04.046977 psrdb-3.0.6/psrdb/load_data.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:23:00.534055 psrdb-3.0.6/psrdb/scripts/__init__.py
+-rw-r--r--   0        0        0     6338 2024-04-08 03:41:36.361745 psrdb-3.0.6/psrdb/scripts/generate_meerkat_json.py
+-rw-r--r--   0        0        0     3764 2024-04-08 03:41:36.361745 psrdb-3.0.6/psrdb/scripts/generate_molonglo_json.py
+-rwxr-xr-x   0        0        0     4446 2023-11-17 05:04:08.063479 psrdb-3.0.6/psrdb/scripts/ingest_obs.py
+-rwxr-xr-x   0        0        0     2785 2024-05-13 01:49:04.046977 psrdb-3.0.6/psrdb/scripts/psrdb.py
+-rw-r--r--   0        0        0        0 2023-11-17 05:04:08.063479 psrdb-3.0.6/psrdb/tables/__init__.py
+-rw-r--r--   0        0        0     6182 2023-11-17 05:04:08.063479 psrdb-3.0.6/psrdb/tables/calibration.py
+-rw-r--r--   0        0        0    10082 2023-11-17 05:04:08.063479 psrdb-3.0.6/psrdb/tables/ephemeris.py
+-rw-r--r--   0        0        0     5761 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/tables/main_project.py
+-rw-r--r--   0        0        0    32489 2024-05-13 01:49:04.046977 psrdb-3.0.6/psrdb/tables/observation.py
+-rw-r--r--   0        0        0     4779 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/tables/pipeline_image.py
+-rw-r--r--   0        0        0    17605 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/tables/pipeline_run.py
+-rw-r--r--   0        0        0     7390 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/tables/project.py
+-rw-r--r--   0        0        0     6119 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/tables/pulsar.py
+-rw-r--r--   0        0        0     9708 2024-05-13 01:49:04.046977 psrdb-3.0.6/psrdb/tables/pulsar_fold_result.py
+-rw-r--r--   0        0        0     4470 2024-05-13 01:49:04.046977 psrdb-3.0.6/psrdb/tables/pulsar_fold_summary.py
+-rw-r--r--   0        0        0     6564 2024-05-13 01:48:58.307217 psrdb-3.0.6/psrdb/tables/residual.py
+-rw-r--r--   0        0        0     5190 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/tables/telescope.py
+-rw-r--r--   0        0        0     5419 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/tables/template.py
+-rw-r--r--   0        0        0    16716 2024-05-13 01:49:04.050977 psrdb-3.0.6/psrdb/tables/toa.py
+-rw-r--r--   0        0        0        0 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/utils/__init__.py
+-rw-r--r--   0        0        0     2345 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/utils/ephemeris.py
+-rw-r--r--   0        0        0     5879 2024-04-08 03:41:36.365745 psrdb-3.0.6/psrdb/utils/header.py
+-rw-r--r--   0        0        0     4173 2024-05-13 01:48:58.307217 psrdb-3.0.6/psrdb/utils/other.py
+-rw-r--r--   0        0        0     1318 2023-11-17 05:04:08.067479 psrdb-3.0.6/psrdb/utils/residual.py
+-rw-r--r--   0        0        0     2003 2024-05-13 01:48:58.307217 psrdb-3.0.6/psrdb/utils/toa.py
+-rw-r--r--   0        0        0      806 2024-04-08 03:41:36.365745 psrdb-3.0.6/psrdb/utils/upload.py
+-rw-r--r--   0        0        0     1046 2024-05-13 01:49:04.050977 psrdb-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 psrdb-3.0.6/PKG-INFO
```

### Comparing `psrdb-3.0.5/LICENSE` & `psrdb-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/data/l_band_gain_calibrators.csv` & `psrdb-3.0.6/psrdb/data/l_band_gain_calibrators.csv`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/data/molonglo_phasing.txt` & `psrdb-3.0.6/psrdb/data/molonglo_phasing.txt`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/data/polarisation_calibrators.csv` & `psrdb-3.0.6/psrdb/data/polarisation_calibrators.csv`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/data/s_band_gain_calibrators.csv` & `psrdb-3.0.6/psrdb/data/s_band_gain_calibrators.csv`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/data/uhf_band_gain_calibrators.csv` & `psrdb-3.0.6/psrdb/data/uhf_band_gain_calibrators.csv`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/graphql_client.py` & `psrdb-3.0.6/psrdb/graphql_client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import json
-import logging
-import copy
-import requests as r
-from requests.packages.urllib3.util.retry import Retry
-
-
-class GraphQLClient:
-    """Provides a HTTP client connection to the GraphQL endpoint"""
-
-    def __init__(self, url, token, verbose=False, logger=None):
-        """Initialise GraphQL connection for the url."""
-        self.graphql_url = f"{url}/graphql/"
-        self.rest_api_url = f"{url}/upload/"
-        self.token = token
-        self.header = {"Authorization": f"JWT {token}"}
-        self.connect(verbose)
-
-        if logger is None:
-            self.logger = logging.getLogger(__name__)
-        else:
-            self.logger = logger
-
-    def connect(self, verbose):
-        """Connect to the GraphQL URL."""
-        if verbose:
-            try:
-                import http.client as http_client
-            except ImportError:
-                # Python 2
-                import httplib as http_client
-            http_client.HTTPConnection.debuglevel = 1
-
-        if self.graphql_url is None:
-            raise RuntimeError("GraphQL URL is required")
-
-        retry_strategy = Retry(total=3, backoff_factor=1, status_forcelist=[429, 500, 502, 503, 504])
-        adapter = r.adapters.HTTPAdapter(max_retries=retry_strategy)
-
-        self.graphql_session = r.Session()
-        self.graphql_session.mount(self.graphql_url, adapter)
-
-    def handle_error_msg(self, content):
-        """Handle logging of error messages in GraphQL response."""
-        if "errors" in content.keys():
-            message = None
-            if "message" in content["errors"][0]:
-                message = content["errors"][0]["message"]
-            self.logger.error(f"Error: {message}")
-
-    def post(self, payload):
-        """Post the payload and header to the GraphQL URL."""
-        self.logger.debug(f"Using url: {self.graphql_url}")
-        self.logger.debug(f"Using payload: {json.dumps(payload, indent=4)}")
-        header_log = copy.deepcopy(self.header)
-        if "Authorization" in self.header.keys():
-            if "JWT" in header_log["Authorization"]:
-                header_log["Authorization"] = "JWT [redacted]"
-        self.logger.debug(f"Using header: {json.dumps(header_log, indent=4)}")
-        response = self.graphql_session.post(self.graphql_url, headers=self.header, json=payload, timeout=(60, 60))
-        content = json.loads(response.content)
-
-        if response.status_code != 200:
-            self.logger.error(f"GraphQL response.status_code != {response.status_code}")
-            self.handle_error_msg(content)
-        elif "errors" in content.keys():
-            self.logger.error("GraphQL error")
-            self.handle_error_msg(content)
-        else:
-            self.logger.debug("Success")
-        return response
+import json
+import logging
+import copy
+import requests as r
+from requests.packages.urllib3.util.retry import Retry
+
+
+class GraphQLClient:
+    """Provides a HTTP client connection to the GraphQL endpoint"""
+
+    def __init__(self, url, token, verbose=False, logger=None):
+        """Initialise GraphQL connection for the url."""
+        self.graphql_url = f"{url}/graphql/"
+        self.rest_api_url = f"{url}/upload/"
+        self.token = token
+        self.header = {"Authorization": f"JWT {token}"}
+        self.connect(verbose)
+
+        if logger is None:
+            self.logger = logging.getLogger(__name__)
+        else:
+            self.logger = logger
+
+    def connect(self, verbose):
+        """Connect to the GraphQL URL."""
+        if verbose:
+            try:
+                import http.client as http_client
+            except ImportError:
+                # Python 2
+                import httplib as http_client
+            http_client.HTTPConnection.debuglevel = 1
+
+        if self.graphql_url is None:
+            raise RuntimeError("GraphQL URL is required")
+
+        retry_strategy = Retry(total=3, backoff_factor=1, status_forcelist=[429, 500, 502, 503, 504])
+        adapter = r.adapters.HTTPAdapter(max_retries=retry_strategy)
+
+        self.graphql_session = r.Session()
+        self.graphql_session.mount(self.graphql_url, adapter)
+
+    def handle_error_msg(self, content):
+        """Handle logging of error messages in GraphQL response."""
+        if "errors" in content.keys():
+            message = None
+            if "message" in content["errors"][0]:
+                message = content["errors"][0]["message"]
+            self.logger.error(f"Error: {message}")
+
+    def post(self, payload):
+        """Post the payload and header to the GraphQL URL."""
+        self.logger.debug(f"Using url: {self.graphql_url}")
+        self.logger.debug(f"Using payload: {json.dumps(payload, indent=4)}")
+        header_log = copy.deepcopy(self.header)
+        if "Authorization" in self.header.keys():
+            if "JWT" in header_log["Authorization"]:
+                header_log["Authorization"] = "JWT [redacted]"
+        self.logger.debug(f"Using header: {json.dumps(header_log, indent=4)}")
+        response = self.graphql_session.post(self.graphql_url, headers=self.header, json=payload, timeout=(60, 60))
+        content = json.loads(response.content)
+
+        if response.status_code != 200:
+            self.logger.error(f"GraphQL response.status_code != {response.status_code}")
+            self.handle_error_msg(content)
+        elif "errors" in content.keys():
+            self.logger.error("GraphQL error")
+            self.handle_error_msg(content)
+        else:
+            self.logger.debug("Success")
+        return response
```

### Comparing `psrdb-3.0.5/psrdb/graphql_table.py` & `psrdb-3.0.6/psrdb/graphql_table.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-import json
-import logging
-from base64 import b64decode
-import binascii
-from copy import copy
-
-from psrdb.utils.other import to_camel_case
-
-
-def generate_graphql_query(table_name, filters, conection_fields, node_fields):
-    """Generate a GraphQL query for a table"""
-
-    # From filter create query arguments
-    arguments = []
-    argument_definitions = []
-    for f in filters:
-        field = f["field"]
-        value = f["value"]
-        if value is not None:
-            arguments.append(f'{field}: ${field}')
-            if type(value) == str:
-                argument_definitions.append(f'${field}: String')
-            elif type(value) == bool:
-                argument_definitions.append(f"${field}: Boolean")
-            elif type(value) == list:
-                value_list = '","'.join(value)
-                argument_definitions.append(f'${field}: [String]')
-            else:
-                argument_definitions.append(f"${field}: Int")
-    # Prepare the argument definitions to the template format
-    if len(argument_definitions) > 0:
-        argument_definitions = ',\n        '.join(argument_definitions)
-        query_argument_definitions = f"(\n        {argument_definitions}\n    )"
-    else:
-        query_argument_definitions = ""
-    # Prepare the arguments to the template format
-    if len(arguments) > 0:
-        arguments = ',\n        '.join(arguments)
-        query_arguments = f"(\n        {arguments}\n    )"
-    else:
-        query_arguments = ""
-
-    # Prepare the fields to the template format
-    node_fields = "\n                ".join(node_fields)
-    conection_fields= "\n        ".join(conection_fields)
-
-    # Convert table name to camel case to match graphql query
-    query_name = to_camel_case(table_name)
-
-    # Combine everything into a query
-    query = f"""query {query_name} {query_argument_definitions} {{
-    {query_name} {query_arguments} {{
-        {conection_fields}
-        edges {{
-            node {{
-                {node_fields}
-            }}
-        }}
-    }}
-}}
-    """
-    return query
-
-
-
-class GraphQLTable:
-    """Abstract base class to perform create, update and select GraphQL queries"""
-
-    def __init__(self, client, logger=None):
-
-        # the graphQL client may also be a djangodb mock endpoint
-        self.client = client
-
-        if logger is None:
-            self.logger = logging.getLogger(__name__)
-        else:
-            self.logger = logger
-
-        self.get_dicts = False
-        self.print_stdout = False
-        self.paginate = False
-        self.quiet = False
-
-        self.mutation_name = None
-        self.mutation = None
-        self.variables = {}
-
-        # table name that should be overwritten
-        self.table_name = self.__class__.__name__.lower()
-        # List of variables to return from list queries which will be overwritten
-        self.field_names = []
-
-    def set_use_pagination(self, paginate):
-        self.paginate = paginate
-
-    def set_quiet(self, id_only):
-        if id_only:
-            self.field_names = ["id"]
-            self.quiet = True
-
-    def decode_id(self, encoded):
-        decoded = b64decode(encoded).decode("ascii")
-        return decoded.split(":")[1]
-
-    def parse_mutation_response(self, response, table_name, mutation_name):
-        """Parse the response from a create or update mutation and return the id of the record"""
-        if response.status_code == 200:
-            content = json.loads(response.content)
-            self.logger.debug(f"Response content: {content}")
-            if "errors" not in content.keys():
-                data = content["data"]
-                mutation_data = data[mutation_name]
-                created_data = mutation_data[to_camel_case(table_name)]
-                if self.print_stdout:
-                    if type(created_data) == list:
-                        for d in created_data:
-                            print(d["id"])
-                    else:
-                        print(created_data["id"])
-            else:
-                self.logger.warning(f"Errors returned in content {content['errors']}")
-        else:
-            self.logger.warning(f"Bad response status_code={response.status_code}")
-        return None
-
-    def mutation_graphql(self):
-        self.logger.debug(f"Using mutation {self.mutation}")
-        self.logger.debug(f"Using mutation vars dict {json.dumps(self.variables, indent=4)}")
-
-        payload = {"query": self.mutation, "variables": json.dumps(self.variables)}
-        response = self.client.post(payload)
-        self.parse_mutation_response(response, self.table_name, self.mutation_name)
-        return response
-
-    def list_graphql(
-        self,
-        table_name,
-        input_filters,
-        connection_fields,
-        input_node_fields,
-        paginate_num=100,
-    ):
-        """
-        Perform a list query on a table
-
-        Parameters
-        ----------
-        table_name : str
-            The name of the table to query
-        input_filters : list
-            A list of dictionaries with the fields and values to filter the query
-        connection_fields : list
-            A list of fields to return from the connection
-        input_node_fields : list
-            A list of fields to return from the node
-        paginate_num: int, optional
-            The number of records to return per page, default is 100
-        """
-        print_headers = True
-        cursor = None
-        connection_fields.append("pageInfo { hasNextPage endCursor }")
-        result = []
-        has_next_page = True
-        while has_next_page:
-            # Append page information to input filters and fields
-            filters = copy(input_filters)
-            filters.append({"field": "first", "value": paginate_num})
-            if cursor is not None:
-                filters.append({"field": "after", "value": cursor})
-            variables = {}
-            for f in filters:
-                variables[f["field"]] = f["value"]
-
-            # Generate the query
-            query = generate_graphql_query(table_name, filters, connection_fields, input_node_fields)
-            self.logger.debug(f"Using query: {query}")
-
-            # Send the query
-            payload = {"query": query, "variables": json.dumps(variables)}
-            response = self.client.post(payload)
-            has_next_page = False
-            if response.status_code == 200:
-                content = json.loads(response.content)
-                self.logger.debug(f"Response content: {content}")
-                if "errors" not in content.keys():
-                    data = content["data"][to_camel_case(table_name)]
-                    # Get next page info (if available)
-                    if data["pageInfo"]["hasNextPage"]:
-                        cursor = data["pageInfo"]["endCursor"]
-                        has_next_page = True
-
-                    for node in data["edges"]:
-                        if self.get_dicts:
-                            result.append(node["node"])
-                        self.print_record_set(node["node"], "\t", print_headers=print_headers)
-                        print_headers = cursor is None
-
-        if self.get_dicts:
-            return result
-        else:
-            return response
-
-    def print_record_set_fields(self, prefix, record_set, delim):
-        fields = []
-        if "node" in record_set.keys():
-            record_set = record_set["node"]
-        for k in record_set.keys():
-            if type(record_set[k]) is dict:
-                if prefix is None:
-                    fields.extend(self.print_record_set_fields(k, record_set[k], delim))
-                else:
-                    fields.extend(self.print_record_set_fields(prefix + "_" + k, record_set[k], delim))
-            else:
-                if prefix is None:
-                    fields.append(str(k))
-                else:
-                    fields.append(prefix + "_" + str(k))
-        if prefix is None and self.print_stdout:
-            print(delim.join(fields))
-        return fields
-
-    def get_record_set_value(self, key, value):
-        if key == "id":
-            try:
-                result = self.decode_id(value)
-            except (binascii.Error, UnicodeDecodeError):
-                result = value
-        elif type(value) is dict:
-            k = list(value.keys())[0]
-            v = list(value.values())[0]
-            result = self.get_record_set_value(k, v)
-        else:
-            result = value
-        return str(result)
-
-    def print_record_set_values(self, prefix, record_set, delim):
-        values = []
-        if "node" in record_set.keys():
-            record_set = record_set["node"]
-        for k in record_set.keys():
-            if type(record_set[k]) is dict:
-                if prefix is None:
-                    values.extend(self.print_record_set_values(k, record_set[k], delim))
-                else:
-                    values.extend(self.print_record_set_values(k + "_" + prefix, record_set[k], delim))
-            else:
-                values.append(self.get_record_set_value(k, record_set[k]))
-        if prefix is None and self.print_stdout:
-            print(delim.join(values))
-        return values
-
-    def print_record_set(self, record_set, delim, print_headers=True):
-        num_records = len(record_set)
-        if num_records == 0:
-            return
-        if type(record_set) == list:
-            if not self.quiet and print_headers:
-                self.print_record_set_fields(None, record_set[0], delim)
-            for record in record_set:
-                self.print_record_set_values(None, record, delim)
-        elif type(record_set) == dict:
-            if not self.quiet and print_headers:
-                self.print_record_set_fields(None, record_set, delim)
-            self.print_record_set_values(None, record_set, delim)
-        else:
-            raise RuntimeError("did not understand type of recordset")
-
-    @classmethod
-    def get_default_parser(cls, desc=""):
-        from argparse import ArgumentParser
-        from os import environ
-
-        parser = ArgumentParser(description=desc)
-        parser.add_argument("-t", "--token", default=environ.get("PSRDB_TOKEN"), help="JWT token")
-        parser.add_argument("-u", "--url", default=environ.get("PSRDB_URL", "https://pulsars.org.au/api/"), help="GraphQL URL")
-        parser.add_argument("-q", "--quiet", action="store_true", default=False, help="Return ID only")
-        parser.add_argument("-v", "--verbose", action="store_true", default=False, help="Increase verbosity")
-        return parser
+import json
+import logging
+from base64 import b64decode
+import binascii
+from copy import copy
+
+from psrdb.utils.other import to_camel_case
+
+
+def generate_graphql_query(table_name, filters, conection_fields, node_fields):
+    """Generate a GraphQL query for a table"""
+
+    # From filter create query arguments
+    arguments = []
+    argument_definitions = []
+    for f in filters:
+        field = f["field"]
+        value = f["value"]
+        if value is not None:
+            arguments.append(f'{field}: ${field}')
+            if type(value) == str:
+                argument_definitions.append(f'${field}: String')
+            elif type(value) == bool:
+                argument_definitions.append(f"${field}: Boolean")
+            elif type(value) == list:
+                value_list = '","'.join(value)
+                argument_definitions.append(f'${field}: [String]')
+            else:
+                argument_definitions.append(f"${field}: Int")
+    # Prepare the argument definitions to the template format
+    if len(argument_definitions) > 0:
+        argument_definitions = ',\n        '.join(argument_definitions)
+        query_argument_definitions = f"(\n        {argument_definitions}\n    )"
+    else:
+        query_argument_definitions = ""
+    # Prepare the arguments to the template format
+    if len(arguments) > 0:
+        arguments = ',\n        '.join(arguments)
+        query_arguments = f"(\n        {arguments}\n    )"
+    else:
+        query_arguments = ""
+
+    # Prepare the fields to the template format
+    node_fields = "\n                ".join(node_fields)
+    conection_fields= "\n        ".join(conection_fields)
+
+    # Convert table name to camel case to match graphql query
+    query_name = to_camel_case(table_name)
+
+    # Combine everything into a query
+    query = f"""query {query_name} {query_argument_definitions} {{
+    {query_name} {query_arguments} {{
+        {conection_fields}
+        edges {{
+            node {{
+                {node_fields}
+            }}
+        }}
+    }}
+}}
+    """
+    return query
+
+
+
+class GraphQLTable:
+    """Abstract base class to perform create, update and select GraphQL queries"""
+
+    def __init__(self, client, logger=None):
+
+        # the graphQL client may also be a djangodb mock endpoint
+        self.client = client
+
+        if logger is None:
+            self.logger = logging.getLogger(__name__)
+        else:
+            self.logger = logger
+
+        self.get_dicts = False
+        self.print_stdout = False
+        self.paginate = False
+        self.quiet = False
+
+        self.mutation_name = None
+        self.mutation = None
+        self.variables = {}
+
+        # table name that should be overwritten
+        self.table_name = self.__class__.__name__.lower()
+        # List of variables to return from list queries which will be overwritten
+        self.field_names = []
+
+    def set_use_pagination(self, paginate):
+        self.paginate = paginate
+
+    def set_quiet(self, id_only):
+        if id_only:
+            self.field_names = ["id"]
+            self.quiet = True
+
+    def decode_id(self, encoded):
+        decoded = b64decode(encoded).decode("ascii")
+        return decoded.split(":")[1]
+
+    def parse_mutation_response(self, response, table_name, mutation_name):
+        """Parse the response from a create or update mutation and return the id of the record"""
+        if response.status_code == 200:
+            content = json.loads(response.content)
+            self.logger.debug(f"Response content: {content}")
+            if "errors" not in content.keys():
+                data = content["data"]
+                mutation_data = data[mutation_name]
+                created_data = mutation_data[to_camel_case(table_name)]
+                if self.print_stdout:
+                    if type(created_data) == list:
+                        for d in created_data:
+                            print(d["id"])
+                    else:
+                        print(created_data["id"])
+            else:
+                self.logger.warning(f"Errors returned in content {content['errors']}")
+        else:
+            self.logger.warning(f"Bad response status_code={response.status_code}")
+        return None
+
+    def mutation_graphql(self):
+        self.logger.debug(f"Using mutation {self.mutation}")
+        self.logger.debug(f"Using mutation vars dict {json.dumps(self.variables, indent=4)}")
+
+        payload = {"query": self.mutation, "variables": json.dumps(self.variables)}
+        response = self.client.post(payload)
+        self.parse_mutation_response(response, self.table_name, self.mutation_name)
+        return response
+
+    def list_graphql(
+        self,
+        table_name,
+        input_filters,
+        connection_fields,
+        input_node_fields,
+        paginate_num=100,
+    ):
+        """
+        Perform a list query on a table
+
+        Parameters
+        ----------
+        table_name : str
+            The name of the table to query
+        input_filters : list
+            A list of dictionaries with the fields and values to filter the query
+        connection_fields : list
+            A list of fields to return from the connection
+        input_node_fields : list
+            A list of fields to return from the node
+        paginate_num: int, optional
+            The number of records to return per page, default is 100
+        """
+        print_headers = True
+        cursor = None
+        connection_fields.append("pageInfo { hasNextPage endCursor }")
+        result = []
+        has_next_page = True
+        while has_next_page:
+            # Append page information to input filters and fields
+            filters = copy(input_filters)
+            filters.append({"field": "first", "value": paginate_num})
+            if cursor is not None:
+                filters.append({"field": "after", "value": cursor})
+            variables = {}
+            for f in filters:
+                variables[f["field"]] = f["value"]
+
+            # Generate the query
+            query = generate_graphql_query(table_name, filters, connection_fields, input_node_fields)
+            self.logger.debug(f"Using query: {query}")
+
+            # Send the query
+            payload = {"query": query, "variables": json.dumps(variables)}
+            response = self.client.post(payload)
+            has_next_page = False
+            if response.status_code == 200:
+                content = json.loads(response.content)
+                self.logger.debug(f"Response content: {content}")
+                if "errors" not in content.keys():
+                    data = content["data"][to_camel_case(table_name)]
+                    # Get next page info (if available)
+                    if data["pageInfo"]["hasNextPage"]:
+                        cursor = data["pageInfo"]["endCursor"]
+                        has_next_page = True
+
+                    for node in data["edges"]:
+                        if self.get_dicts:
+                            result.append(node["node"])
+                        self.print_record_set(node["node"], "\t", print_headers=print_headers)
+                        print_headers = cursor is None
+
+        if self.get_dicts:
+            return result
+        else:
+            return response
+
+    def print_record_set_fields(self, prefix, record_set, delim):
+        fields = []
+        if "node" in record_set.keys():
+            record_set = record_set["node"]
+        for k in record_set.keys():
+            if type(record_set[k]) is dict:
+                if prefix is None:
+                    fields.extend(self.print_record_set_fields(k, record_set[k], delim))
+                else:
+                    fields.extend(self.print_record_set_fields(prefix + "_" + k, record_set[k], delim))
+            else:
+                if prefix is None:
+                    fields.append(str(k))
+                else:
+                    fields.append(prefix + "_" + str(k))
+        if prefix is None and self.print_stdout:
+            print(delim.join(fields))
+        return fields
+
+    def get_record_set_value(self, key, value):
+        if key == "id":
+            try:
+                result = self.decode_id(value)
+            except (binascii.Error, UnicodeDecodeError):
+                result = value
+        elif type(value) is dict:
+            k = list(value.keys())[0]
+            v = list(value.values())[0]
+            result = self.get_record_set_value(k, v)
+        else:
+            result = value
+        return str(result)
+
+    def print_record_set_values(self, prefix, record_set, delim):
+        values = []
+        if "node" in record_set.keys():
+            record_set = record_set["node"]
+        for k in record_set.keys():
+            if type(record_set[k]) is dict:
+                if prefix is None:
+                    values.extend(self.print_record_set_values(k, record_set[k], delim))
+                else:
+                    values.extend(self.print_record_set_values(k + "_" + prefix, record_set[k], delim))
+            else:
+                values.append(self.get_record_set_value(k, record_set[k]))
+        if prefix is None and self.print_stdout:
+            print(delim.join(values))
+        return values
+
+    def print_record_set(self, record_set, delim, print_headers=True):
+        num_records = len(record_set)
+        if num_records == 0:
+            return
+        if type(record_set) == list:
+            if not self.quiet and print_headers:
+                self.print_record_set_fields(None, record_set[0], delim)
+            for record in record_set:
+                self.print_record_set_values(None, record, delim)
+        elif type(record_set) == dict:
+            if not self.quiet and print_headers:
+                self.print_record_set_fields(None, record_set, delim)
+            self.print_record_set_values(None, record_set, delim)
+        else:
+            raise RuntimeError("did not understand type of recordset")
+
+    @classmethod
+    def get_default_parser(cls, desc=""):
+        from argparse import ArgumentParser
+        from os import environ
+
+        parser = ArgumentParser(description=desc)
+        parser.add_argument("-t", "--token", default=environ.get("PSRDB_TOKEN"), help="JWT token")
+        parser.add_argument("-u", "--url", default=environ.get("PSRDB_URL", "https://pulsars.org.au/api/"), help="GraphQL URL")
+        parser.add_argument("-q", "--quiet", action="store_true", default=False, help="Return ID only")
+        parser.add_argument("-v", "--verbose", action="store_true", default=False, help="Increase verbosity")
+        return parser
```

### Comparing `psrdb-3.0.5/psrdb/scripts/generate_meerkat_json.py` & `psrdb-3.0.6/psrdb/scripts/generate_meerkat_json.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/scripts/generate_molonglo_json.py` & `psrdb-3.0.6/psrdb/scripts/generate_molonglo_json.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/scripts/ingest_obs.py` & `psrdb-3.0.6/psrdb/scripts/ingest_obs.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/scripts/psrdb.py` & `psrdb-3.0.6/psrdb/scripts/psrdb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,82 @@
-#!/usr/bin/env python
-import sys
-
-from psrdb.graphql_table import GraphQLTable
-from psrdb.graphql_client import GraphQLClient
-from psrdb.utils.other import setup_logging
-
-from psrdb.tables.pulsar import Pulsar
-from psrdb.tables.telescope import Telescope
-from psrdb.tables.main_project import MainProject
-from psrdb.tables.project import Project
-from psrdb.tables.ephemeris import Ephemeris
-from psrdb.tables.template import Template
-from psrdb.tables.calibration import Calibration
-from psrdb.tables.observation import Observation
-from psrdb.tables.pipeline_run import PipelineRun
-from psrdb.tables.pulsar_fold_result import PulsarFoldResult
-from psrdb.tables.pipeline_image import PipelineImage
-from psrdb.tables.toa import Toa
-from psrdb.tables.residual import Residual
-
-
-def main():
-    logger = setup_logging()
-
-    parser = GraphQLTable.get_default_parser()
-    subparsers = parser.add_subparsers(
-        dest="command", help="Database models which can be interrogated"
-    )
-    subparsers.required = True
-
-    tables = [
-        Pulsar,
-        Telescope,
-        MainProject,
-        Project,
-        Ephemeris,
-        Template,
-        Calibration,
-        Observation,
-        PipelineRun,
-        PulsarFoldResult,
-        PipelineImage,
-        Toa,
-        Residual,
-    ]
-
-    configured = []
-    for t in tables:
-        n = t.get_name()
-        p = subparsers.add_parser(n, help=t.get_description())
-        t.configure_parsers(p)
-        configured.append({"name": n, "parser": p, "table": t})
-
-    args = parser.parse_args()
-    if args.url is None:
-        raise RuntimeError("GraphQL URL must be provided in $PSRDB_URL or via -u option")
-    if args.token is None:
-        raise RuntimeError("GraphQL Token must be provided in $PSRDB_TOKEN or via -t option")
-
-    for c in configured:
-        if args.command == c["name"]:
-            client = GraphQLClient(args.url, args.token, verbose=args.verbose)
-            table = c["table"](client)
-            table.set_quiet(args.quiet)
-            table.set_use_pagination(True)
-            response = table.process(args)
-            if 'status_code' in dir(response):
-                if response.status_code not in (200, 201):
-                    logger.error(f"Query failed with the error code {response.status_code}, error:")
-                    print(json.loads(response.content))
-                    sys.exit(response.status_code)
-                if args.verbose:
-                    import json
-                    print(response.status_code)
-                    print(json.loads(response.content))
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+import sys
+
+from psrdb.graphql_table import GraphQLTable
+from psrdb.graphql_client import GraphQLClient
+from psrdb.utils.other import setup_logging
+
+from psrdb.tables.pulsar import Pulsar
+from psrdb.tables.telescope import Telescope
+from psrdb.tables.main_project import MainProject
+from psrdb.tables.project import Project
+from psrdb.tables.ephemeris import Ephemeris
+from psrdb.tables.template import Template
+from psrdb.tables.calibration import Calibration
+from psrdb.tables.observation import Observation
+from psrdb.tables.pipeline_run import PipelineRun
+from psrdb.tables.pulsar_fold_result import PulsarFoldResult
+from psrdb.tables.pulsar_fold_summary import PulsarFoldSummary
+from psrdb.tables.pipeline_image import PipelineImage
+from psrdb.tables.toa import Toa
+from psrdb.tables.residual import Residual
+
+
+def main():
+    logger = setup_logging()
+
+    parser = GraphQLTable.get_default_parser()
+    subparsers = parser.add_subparsers(
+        dest="command", help="Database models which can be interrogated"
+    )
+    subparsers.required = True
+
+    tables = [
+        Pulsar,
+        Telescope,
+        MainProject,
+        Project,
+        Ephemeris,
+        Template,
+        Calibration,
+        Observation,
+        PipelineRun,
+        PulsarFoldResult,
+        PulsarFoldSummary,
+        PipelineImage,
+        Toa,
+        Residual,
+    ]
+
+    configured = []
+    for t in tables:
+        n = t.get_name()
+        p = subparsers.add_parser(n, help=t.get_description())
+        t.configure_parsers(p)
+        configured.append({"name": n, "parser": p, "table": t})
+
+    args = parser.parse_args()
+    if args.url is None:
+        raise RuntimeError("GraphQL URL must be provided in $PSRDB_URL or via -u option")
+    if args.token is None:
+        raise RuntimeError("GraphQL Token must be provided in $PSRDB_TOKEN or via -t option")
+
+    for c in configured:
+        if args.command == c["name"]:
+            client = GraphQLClient(args.url, args.token, verbose=args.verbose)
+            table = c["table"](client)
+            table.set_quiet(args.quiet)
+            table.set_use_pagination(True)
+            response = table.process(args)
+            if 'status_code' in dir(response):
+                if response.status_code not in (200, 201):
+                    logger.error(f"Query failed with the error code {response.status_code}, error:")
+                    print(json.loads(response.content))
+                    sys.exit(response.status_code)
+                if args.verbose:
+                    import json
+                    print(response.status_code)
+                    print(json.loads(response.content))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `psrdb-3.0.5/psrdb/tables/__pycache__/main_project.cpython-310.pyc` & `psrdb-3.0.6/psrdb/tables/template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,363 +1,339 @@
-00000000: 6f0d 0d0a 0000 0000 e976 5565 8116 0000  o........vUe....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
-00000030: 6401 6c00 6d01 5a01 0100 6402 6403 8400  d.l.m.Z...d.d...
-00000040: 5a02 4700 6404 6405 8400 6405 6501 8303  Z.G.d.d...d.e...
-00000050: 5a03 6406 5300 2907 e900 0000 0029 01da  Z.d.S.)......)..
-00000060: 0c47 7261 7068 514c 5461 626c 6563 0000  .GraphQLTablec..
-00000070: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000080: 0000 4300 0000 7318 0000 0074 00a0 0164  ..C...s....t...d
-00000090: 01a1 017d 0074 02a0 037c 00a1 0101 007c  ...}.t...|.....|
-000000a0: 0053 0029 027a 2952 6574 7572 6e73 2074  .S.).z)Returns t
-000000b0: 6865 2064 6566 6175 6c74 2070 6172 7365  he default parse
-000000c0: 7220 666f 7220 7468 6973 206d 6f64 656c  r for this model
-000000d0: 7a96 5468 6520 666f 6c6c 6f77 696e 6720  z.The following 
-000000e0: 6f70 7469 6f6e 7320 7769 6c6c 2061 6c6c  options will all
-000000f0: 6f77 2079 6f75 2074 6f20 696e 7465 7261  ow you to intera
-00000100: 6374 2077 6974 6820 7468 6520 4d61 696e  ct with the Main
-00000110: 5072 6f6a 6563 7420 6461 7461 6261 7365  Project database
-00000120: 206f 626a 6563 7420 6f6e 2074 6865 2063   object on the c
-00000130: 6f6d 6d61 6e64 206c 696e 6520 696e 2064  ommand line in d
-00000140: 6966 6665 7265 6e74 2077 6179 7320 6261  ifferent ways ba
-00000150: 7365 6420 6f6e 2074 6865 2073 7562 2d63  sed on the sub-c
-00000160: 6f6d 6d61 6e64 732e 2904 7202 0000 00da  ommands.).r.....
-00000170: 1267 6574 5f64 6566 6175 6c74 5f70 6172  .get_default_par
-00000180: 7365 72da 0b4d 6169 6e50 726f 6a65 6374  ser..MainProject
-00000190: da11 636f 6e66 6967 7572 655f 7061 7273  ..configure_pars
-000001a0: 6572 7329 01da 0670 6172 7365 72a9 0072  ers)...parser..r
-000001b0: 0700 0000 fa32 2f68 6f6d 652f 6e69 636b  .....2/home/nick
-000001c0: 2f63 6f64 652f 7073 7264 622f 7073 7264  /code/psrdb/psrd
-000001d0: 622f 7461 626c 6573 2f6d 6169 6e5f 7072  b/tables/main_pr
-000001e0: 6f6a 6563 742e 7079 da0b 6765 745f 7061  oject.py..get_pa
-000001f0: 7273 6572 7304 0000 0073 0600 0000 0a02  rsers....s......
-00000200: 0a01 0401 7209 0000 0063 0000 0000 0000  ....r....c......
-00000210: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000220: 0000 7366 0000 0065 005a 0164 005a 0264  ..sf...e.Z.d.Z.d
-00000230: 015a 0364 0264 0384 005a 0464 1564 0564  .Z.d.d...Z.d.d.d
-00000240: 0684 015a 0564 0764 0884 005a 0664 0964  ...Z.d.d...Z.d.d
-00000250: 0a84 005a 0764 0b64 0c84 005a 0864 0d64  ...Z.d.d...Z.d.d
-00000260: 0e84 005a 0965 0a64 0f64 1084 0083 015a  ...Z.e.d.d.....Z
-00000270: 0b65 0a64 1164 1284 0083 015a 0c65 0a64  .e.d.d.....Z.e.d
-00000280: 1364 1484 0083 015a 0d64 0453 0029 1672  .d.....Z.d.S.).r
-00000290: 0400 0000 7ac3 436c 6173 7320 666f 7220  ....z.Class for 
-000002a0: 696e 7465 7261 6374 696e 6720 7769 7468  interacting with
-000002b0: 2074 6865 204d 6169 6e50 726f 6a65 6374   the MainProject
-000002c0: 2064 6174 6162 6173 6520 6f62 6a65 6374   database object
-000002d0: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-000002e0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-000002f0: 0a20 2020 2063 6c69 656e 7420 3a20 4772  .    client : Gr
-00000300: 6170 6851 4c43 6c69 656e 740a 2020 2020  aphQLClient.    
-00000310: 2020 2020 4772 6170 6851 4c43 6c69 656e      GraphQLClien
-00000320: 7420 636c 6173 7320 696e 7374 616e 6365  t class instance
-00000330: 2077 6974 6820 7468 6520 5552 4c20 616e   with the URL an
-00000340: 6420 546f 6b65 6e20 616c 7265 6164 7920  d Token already 
-00000350: 7365 742e 0a20 2020 2063 0200 0000 0000  set..    c......
-00000360: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000370: 0000 7320 0000 0074 00a0 017c 007c 01a1  ..s ...t...|.|..
-00000380: 0201 0064 017c 005f 0267 0064 02a2 017c  ...d.|._.g.d...|
-00000390: 005f 0364 0053 0029 034e da0c 6d61 696e  ._.d.S.).N..main
-000003a0: 5f70 726f 6a65 6374 2903 da02 6964 7a11  _project)...idz.
-000003b0: 7465 6c65 7363 6f70 6520 7b6e 616d 657d  telescope {name}
-000003c0: 20da 046e 616d 6529 0472 0200 0000 da08   ..name).r......
-000003d0: 5f5f 696e 6974 5f5f da0a 7461 626c 655f  __init__..table_
-000003e0: 6e61 6d65 da0b 6669 656c 645f 6e61 6d65  name..field_name
-000003f0: 7329 02da 0473 656c 66da 0663 6c69 656e  s)...self..clien
-00000400: 7472 0700 0000 7207 0000 0072 0800 0000  tr....r....r....
-00000410: 720d 0000 0012 0000 0073 0600 0000 0c01  r........s......
-00000420: 0601 0e01 7a14 4d61 696e 5072 6f6a 6563  ....z.MainProjec
-00000430: 742e 5f5f 696e 6974 5f5f 4e63 0400 0000  t.__init__Nc....
-00000440: 0000 0000 0000 0000 0500 0000 0700 0000  ................
-00000450: 4300 0000 7332 0000 0064 017c 0164 029c  C...s2...d.|.d..
-00000460: 0264 037c 0264 029c 0264 047c 0364 029c  .d.|.d...d.|.d..
-00000470: 0267 037d 0474 00a0 017c 007c 006a 027c  .g.}.t...|.|.j.|
-00000480: 0467 007c 006a 03a1 0553 0029 0561 6802  .g.|.j...S.).ah.
-00000490: 0000 5265 7475 726e 2061 206c 6973 7420  ..Return a list 
-000004a0: 6f66 204d 6169 6e50 726f 6a65 6374 2069  of MainProject i
-000004b0: 6e66 6f72 6d61 7469 6f6e 2062 6173 6564  nformation based
-000004c0: 206f 6e20 7468 6520 6073 656c 662e 6669   on the `self.fi
-000004d0: 656c 645f 6e61 6d65 7360 2061 6e64 2066  eld_names` and f
-000004e0: 696c 7465 7265 6420 6279 2074 6865 2070  iltered by the p
-000004f0: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
-00000500: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000510: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00000520: 2d0a 2020 2020 2020 2020 6964 203a 2069  -.        id : i
-00000530: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
-00000540: 2020 2020 2020 2020 2046 696c 7465 7220           Filter 
-00000550: 6279 2074 6865 2064 6174 6162 6173 6520  by the database 
-00000560: 4944 2c20 6279 2064 6566 6175 6c74 204e  ID, by default N
-00000570: 6f6e 650a 2020 2020 2020 2020 7465 6c65  one.        tele
-00000580: 7363 6f70 6520 3a20 7374 722c 206f 7074  scope : str, opt
-00000590: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-000005a0: 2020 4669 6c74 6572 2062 7920 7468 6520    Filter by the 
-000005b0: 7465 6c65 7363 6f70 6520 6e61 6d65 2c20  telescope name, 
-000005c0: 6279 2064 6566 6175 6c74 204e 6f6e 650a  by default None.
-000005d0: 2020 2020 2020 2020 6e61 6d65 203a 2073          name : s
-000005e0: 7472 2c20 6f70 7469 6f6e 616c 0a20 2020  tr, optional.   
-000005f0: 2020 2020 2020 2020 2046 696c 7465 7220           Filter 
-00000600: 6279 2074 6865 206e 616d 652c 2062 7920  by the name, by 
-00000610: 6465 6661 756c 7420 4e6f 6e65 0a0a 2020  default None..  
-00000620: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00000630: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00000640: 2020 2020 2020 6c69 7374 206f 6620 6469        list of di
-00000650: 6374 730a 2020 2020 2020 2020 2020 2020  cts.            
-00000660: 4966 2060 7365 6c66 2e67 6574 5f64 6963  If `self.get_dic
-00000670: 7473 6020 6973 2060 5472 7565 602c 2061  ts` is `True`, a
-00000680: 206c 6973 7420 6f66 2064 6963 7469 6f6e   list of diction
-00000690: 6172 6965 7320 636f 6e74 6169 6e69 6e67  aries containing
-000006a0: 2074 6865 2072 6573 756c 7473 2e0a 2020   the results..  
-000006b0: 2020 2020 2020 636c 6965 6e74 5f72 6573        client_res
-000006c0: 706f 6e73 653a 0a20 2020 2020 2020 2020  ponse:.         
-000006d0: 2020 2045 6c73 6520 6120 636c 6965 6e74     Else a client
-000006e0: 2072 6573 706f 6e73 6520 6f62 6a65 6374   response object
-000006f0: 2e0a 2020 2020 2020 2020 720b 0000 0029  ..        r....)
-00000700: 02da 0566 6965 6c64 da05 7661 6c75 65da  ...field..value.
-00000710: 0974 656c 6573 636f 7065 720c 0000 0029  .telescoper....)
-00000720: 0472 0200 0000 da0c 6c69 7374 5f67 7261  .r......list_gra
-00000730: 7068 716c 720e 0000 0072 0f00 0000 2905  phqlr....r....).
-00000740: 7210 0000 0072 0b00 0000 7214 0000 0072  r....r....r....r
-00000750: 0c00 0000 da07 6669 6c74 6572 7372 0700  ......filtersr..
-00000760: 0000 7207 0000 0072 0800 0000 da04 6c69  ..r....r......li
-00000770: 7374 1700 0000 730a 0000 0008 1408 0108  st....s.........
-00000780: 0104 fd16 057a 104d 6169 6e50 726f 6a65  .....z.MainProje
-00000790: 6374 2e6c 6973 7463 0300 0000 0000 0000  ct.listc........
-000007a0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-000007b0: 7320 0000 0064 017c 005f 0064 027c 005f  s ...d.|._.d.|._
-000007c0: 017c 017c 0264 039c 027c 005f 027c 00a0  .|.|.d...|._.|..
-000007d0: 03a1 0053 0029 0461 2b01 0000 4372 6561  ...S.).a+...Crea
-000007e0: 7465 2061 206e 6577 204d 6169 6e50 726f  te a new MainPro
-000007f0: 6a65 6374 2064 6174 6162 6173 6520 6f62  ject database ob
-00000800: 6a65 6374 2e0a 0a20 2020 2020 2020 2050  ject...        P
-00000810: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00000820: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00000830: 2020 2020 2074 656c 6573 636f 7065 203a       telescope :
-00000840: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
-00000850: 2054 6865 2074 656c 6573 636f 7065 206e   The telescope n
-00000860: 616d 650a 2020 2020 2020 2020 6e61 6d65  ame.        name
-00000870: 203a 2073 7472 0a20 2020 2020 2020 2020   : str.         
-00000880: 2020 2054 6865 206e 616d 6520 6f66 2074     The name of t
-00000890: 6865 204d 6169 6e50 726f 6a65 6374 0a0a  he MainProject..
-000008a0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-000008b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-000008c0: 2020 2020 2020 2020 636c 6965 6e74 5f72          client_r
-000008d0: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-000008e0: 2020 2020 2041 2063 6c69 656e 7420 7265       A client re
-000008f0: 7370 6f6e 7365 206f 626a 6563 742e 0a20  sponse object.. 
-00000900: 2020 2020 2020 205a 1163 7265 6174 654d         Z.createM
-00000910: 6169 6e50 726f 6a65 6374 6125 0100 000a  ainProjecta%....
-00000920: 2020 2020 2020 2020 6d75 7461 7469 6f6e          mutation
-00000930: 2028 2474 656c 6573 636f 7065 3a20 5374   ($telescope: St
-00000940: 7269 6e67 212c 2024 6e61 6d65 3a20 5374  ring!, $name: St
-00000950: 7269 6e67 2129 207b 0a20 2020 2020 2020  ring!) {.       
-00000960: 2020 2020 2063 7265 6174 654d 6169 6e50       createMainP
-00000970: 726f 6a65 6374 2869 6e70 7574 3a20 7b0a  roject(input: {.
-00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000990: 7465 6c65 7363 6f70 654e 616d 653a 2024  telescopeName: $
-000009a0: 7465 6c65 7363 6f70 652c 0a20 2020 2020  telescope,.     
-000009b0: 2020 2020 2020 2020 2020 206e 616d 653a             name:
-000009c0: 2024 6e61 6d65 2c0a 2020 2020 2020 2020   $name,.        
-000009d0: 2020 2020 2020 2020 7d29 207b 0a20 2020          }) {.   
-000009e0: 2020 2020 2020 2020 2020 2020 206d 6169               mai
-000009f0: 6e70 726f 6a65 6374 207b 0a20 2020 2020  nproject {.     
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00000a10: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00000a20: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00000a30: 7d0a 2020 2020 2020 2020 7d0a 2020 2020  }.        }.    
-00000a40: 2020 2020 2902 7214 0000 0072 0c00 0000      ).r....r....
-00000a50: a904 da0d 6d75 7461 7469 6f6e 5f6e 616d  ....mutation_nam
-00000a60: 65da 086d 7574 6174 696f 6eda 0976 6172  e..mutation..var
-00000a70: 6961 626c 6573 da10 6d75 7461 7469 6f6e  iables..mutation
-00000a80: 5f67 7261 7068 716c 2903 7210 0000 0072  _graphql).r....r
-00000a90: 1400 0000 720c 0000 0072 0700 0000 7207  ....r....r....r.
-00000aa0: 0000 0072 0800 0000 da06 6372 6561 7465  ...r......create
-00000ab0: 3100 0000 730c 0000 0006 0f06 0102 0d02  1...s...........
-00000ac0: 0108 fe08 047a 124d 6169 6e50 726f 6a65  .....z.MainProje
-00000ad0: 6374 2e63 7265 6174 6563 0400 0000 0000  ct.createc......
-00000ae0: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
-00000af0: 0000 7322 0000 0064 017c 005f 0064 027c  ..s"...d.|._.d.|
-00000b00: 005f 017c 017c 027c 0364 039c 037c 005f  ._.|.|.|.d...|._
-00000b10: 027c 00a0 03a1 0053 0029 0461 5401 0000  .|.....S.).aT...
-00000b20: 5570 6461 7465 2061 204d 6169 6e50 726f  Update a MainPro
-00000b30: 6a65 6374 2064 6174 6162 6173 6520 6f62  ject database ob
-00000b40: 6a65 6374 2e0a 0a20 2020 2020 2020 2050  ject...        P
-00000b50: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00000b60: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00000b70: 2020 2020 2069 6420 3a20 696e 740a 2020       id : int.  
-00000b80: 2020 2020 2020 2020 2020 5468 6520 6461            The da
-00000b90: 7461 6261 7365 2049 440a 2020 2020 2020  tabase ID.      
-00000ba0: 2020 7465 6c65 7363 6f70 6520 3a20 7374    telescope : st
-00000bb0: 720a 2020 2020 2020 2020 2020 2020 5468  r.            Th
-00000bc0: 6520 7465 6c65 7363 6f70 6520 6e61 6d65  e telescope name
-00000bd0: 0a20 2020 2020 2020 206e 616d 6520 3a20  .        name : 
-00000be0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-00000bf0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-00000c00: 4d61 696e 5072 6f6a 6563 740a 0a20 2020  MainProject..   
-00000c10: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00000c20: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00000c30: 2020 2020 2063 6c69 656e 745f 7265 7370       client_resp
-00000c40: 6f6e 7365 3a0a 2020 2020 2020 2020 2020  onse:.          
-00000c50: 2020 4120 636c 6965 6e74 2072 6573 706f    A client respo
-00000c60: 6e73 6520 6f62 6a65 6374 2e0a 2020 2020  nse object..    
-00000c70: 2020 2020 5a11 7570 6461 7465 4d61 696e      Z.updateMain
-00000c80: 5072 6f6a 6563 7461 5401 0000 0a20 2020  ProjectaT....   
-00000c90: 2020 2020 206d 7574 6174 696f 6e20 2824       mutation ($
-00000ca0: 6964 3a20 496e 7421 2c20 2474 656c 6573  id: Int!, $teles
-00000cb0: 636f 7065 3a20 5374 7269 6e67 212c 2024  cope: String!, $
-00000cc0: 6e61 6d65 3a20 5374 7269 6e67 2129 207b  name: String!) {
-00000cd0: 0a20 2020 2020 2020 2020 2020 2075 7064  .            upd
-00000ce0: 6174 654d 6169 6e50 726f 6a65 6374 2869  ateMainProject(i
-00000cf0: 643a 2024 6964 2c20 696e 7075 743a 207b  d: $id, input: {
-00000d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d10: 2074 656c 6573 636f 7065 4e61 6d65 3a20   telescopeName: 
-00000d20: 2474 656c 6573 636f 7065 2c0a 2020 2020  $telescope,.    
-00000d30: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00000d40: 3a20 246e 616d 652c 0a20 2020 2020 2020  : $name,.       
-00000d50: 2020 2020 2020 2020 207d 2920 7b0a 2020           }) {.  
-00000d60: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00000d70: 696e 7072 6f6a 6563 7420 7b0a 2020 2020  inproject {.    
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d90: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00000da0: 2020 2020 2020 2020 6e61 6d65 2c0a 2020          name,.  
-00000db0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00000dc0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000dd0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00000de0: 2903 720b 0000 0072 1400 0000 720c 0000  ).r....r....r...
-00000df0: 0072 1800 0000 2904 7210 0000 0072 0b00  .r....).r....r..
-00000e00: 0000 7214 0000 0072 0c00 0000 7207 0000  ..r....r....r...
-00000e10: 0072 0700 0000 7208 0000 00da 0675 7064  .r....r......upd
-00000e20: 6174 6553 0000 0073 0e00 0000 0611 0601  ateS...s........
-00000e30: 020e 0201 0201 08fd 0805 7a12 4d61 696e  ..........z.Main
-00000e40: 5072 6f6a 6563 742e 7570 6461 7465 6302  Project.updatec.
-00000e50: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000e60: 0000 0043 0000 0073 1e00 0000 6401 7c00  ...C...s....d.|.
-00000e70: 5f00 6402 7c00 5f01 6403 7c01 6901 7c00  _.d.|._.d.|.i.|.
-00000e80: 5f02 7c00 a003 a100 5300 2904 7ae2 4465  _.|.....S.).z.De
-00000e90: 6c65 7465 2061 204d 6169 6e50 726f 6a65  lete a MainProje
-00000ea0: 6374 2064 6174 6162 6173 6520 6f62 6a65  ct database obje
-00000eb0: 6374 2e0a 0a20 2020 2020 2020 2050 6172  ct...        Par
-00000ec0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00000ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00000ee0: 2020 2069 6420 3a20 696e 740a 2020 2020     id : int.    
-00000ef0: 2020 2020 2020 2020 5468 6520 6461 7461          The data
-00000f00: 6261 7365 2049 440a 0a20 2020 2020 2020  base ID..       
-00000f10: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00000f20: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00000f30: 2063 6c69 656e 745f 7265 7370 6f6e 7365   client_response
-00000f40: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
-00000f50: 636c 6965 6e74 2072 6573 706f 6e73 6520  client response 
-00000f60: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-00000f70: 5a11 6465 6c65 7465 4d61 696e 5072 6f6a  Z.deleteMainProj
-00000f80: 6563 747a 7c0a 2020 2020 2020 2020 6d75  ectz|.        mu
-00000f90: 7461 7469 6f6e 2028 2469 643a 2049 6e74  tation ($id: Int
-00000fa0: 2129 207b 0a20 2020 2020 2020 2020 2020  !) {.           
-00000fb0: 2064 656c 6574 654d 6169 6e50 726f 6a65   deleteMainProje
-00000fc0: 6374 2869 643a 2024 6964 2920 7b0a 2020  ct(id: $id) {.  
-00000fd0: 2020 2020 2020 2020 2020 2020 2020 6f6b                ok
-00000fe0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00000ff0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00001000: 2072 0b00 0000 7218 0000 0029 0272 1000   r....r....).r..
-00001010: 0000 720b 0000 0072 0700 0000 7207 0000  ..r....r....r...
-00001020: 0072 0800 0000 da06 6465 6c65 7465 7900  .r......deletey.
-00001030: 0000 730a 0000 0006 0d06 0104 0806 ff08  ..s.............
-00001040: 037a 124d 6169 6e50 726f 6a65 6374 2e64  .z.MainProject.d
-00001050: 656c 6574 6563 0200 0000 0000 0000 0000  eletec..........
-00001060: 0000 0200 0000 0500 0000 4300 0000 7382  ..........C...s.
-00001070: 0000 0064 017c 005f 007c 016a 0164 026b  ...d.|._.|.j.d.k
-00001080: 0272 127c 00a0 027c 016a 037c 016a 047c  .r.|...|.j.|.j.|
-00001090: 016a 05a1 0353 007c 016a 0164 036b 0272  .j...S.|.j.d.k.r
-000010a0: 1f7c 00a0 067c 016a 047c 016a 05a1 0253  .|...|.j.|.j...S
-000010b0: 007c 016a 0164 046b 0272 2e7c 00a0 077c  .|.j.d.k.r.|...|
-000010c0: 016a 037c 016a 047c 016a 05a1 0353 007c  .j.|.j.|.j...S.|
-000010d0: 016a 0164 056b 0272 397c 00a0 087c 016a  .j.d.k.r9|...|.j
-000010e0: 03a1 0153 0074 097c 016a 019b 0064 069d  ...S.t.|.j...d..
-000010f0: 0283 0182 0129 077a 2950 6172 7365 2074  .....).z)Parse t
-00001100: 6865 2061 7267 756d 656e 7473 2063 6f6c  he arguments col
-00001110: 6c65 6374 6564 2062 7920 7468 6520 434c  lected by the CL
-00001120: 492e 5472 1700 0000 721d 0000 0072 1e00  I.Tr....r....r..
-00001130: 0000 721f 0000 007a 1b20 636f 6d6d 616e  ..r....z. comman
-00001140: 6420 6973 206e 6f74 2069 6d70 6c65 6d65  d is not impleme
-00001150: 6e74 6564 290a da0c 7072 696e 745f 7374  nted)...print_st
-00001160: 646f 7574 da0a 7375 6263 6f6d 6d61 6e64  dout..subcommand
-00001170: 7217 0000 0072 0b00 0000 7214 0000 0072  r....r....r....r
-00001180: 0c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
-00001190: 0000 00da 0c52 756e 7469 6d65 4572 726f  .....RuntimeErro
-000011a0: 7229 0272 1000 0000 da04 6172 6773 7207  r).r......argsr.
-000011b0: 0000 0072 0700 0000 7208 0000 00da 0770  ...r....r......p
-000011c0: 726f 6365 7373 9300 0000 7314 0000 0006  rocess....s.....
-000011d0: 020a 0114 010a 0110 010a 0114 010a 010c  ................
-000011e0: 0110 027a 134d 6169 6e50 726f 6a65 6374  ...z.MainProject
-000011f0: 2e70 726f 6365 7373 6301 0000 0000 0000  .processc.......
-00001200: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00001210: 00f3 0400 0000 6401 5300 2902 4e72 0a00  ......d.S.).Nr..
-00001220: 0000 7207 0000 00a9 01da 0363 6c73 7207  ..r........clsr.
-00001230: 0000 0072 0700 0000 7208 0000 00da 0867  ...r....r......g
-00001240: 6574 5f6e 616d 65a1 0000 00f3 0200 0000  et_name.........
-00001250: 0402 7a14 4d61 696e 5072 6f6a 6563 742e  ..z.MainProject.
-00001260: 6765 745f 6e61 6d65 6301 0000 0000 0000  get_namec.......
-00001270: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00001280: 0072 2500 0000 2902 4e7a 4d41 204d 6169  .r%...).NzMA Mai
-00001290: 6e50 726f 6a65 6374 2064 6566 696e 6564  nProject defined
-000012a0: 2062 7920 6120 636f 6465 2c20 7368 6f72   by a code, shor
-000012b0: 7420 6e61 6d65 2c20 656d 6261 7267 6f20  t name, embargo 
-000012c0: 7065 7269 6f64 2061 6e64 2061 2064 6573  period and a des
-000012d0: 6372 6970 7469 6f6e 7207 0000 0072 2600  criptionr....r&.
-000012e0: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000012f0: 00da 0f67 6574 5f64 6573 6372 6970 7469  ...get_descripti
-00001300: 6f6e a500 0000 7229 0000 007a 1b4d 6169  on....r)...z.Mai
-00001310: 6e50 726f 6a65 6374 2e67 6574 5f64 6573  nProject.get_des
-00001320: 6372 6970 7469 6f6e 6302 0000 0000 0000  criptionc.......
-00001330: 0000 0000 0004 0000 0006 0000 0043 0000  .............C..
-00001340: 0073 6a00 0000 7c01 6a00 7c00 a001 a100  .sj...|.j.|.....
-00001350: 6401 8d01 0100 7c01 6a02 6402 6403 8d01  d.....|.j.d.d...
-00001360: 7d02 6404 7c02 5f03 7c02 6a04 6405 6406  }.d.|._.|.j.d.d.
-00001370: 6407 8d02 7d03 7c03 6a05 6408 6409 7406  d...}.|.j.d.d.t.
-00001380: 640a 640b 8d04 0100 7c03 6a05 640c 640d  d.d.....|.j.d.d.
-00001390: 7406 640e 640b 8d04 0100 7c03 6a05 640f  t.d.d.....|.j.d.
-000013a0: 6410 7407 6411 640b 8d04 0100 6412 5300  d.t.d.d.....d.S.
-000013b0: 2913 7a2f 4164 6420 7375 622d 7061 7273  ).z/Add sub-pars
-000013c0: 6572 7320 666f 7220 6561 6368 206f 6620  ers for each of 
-000013d0: 7468 6520 7661 6c69 6420 636f 6d6d 616e  the valid comman
-000013e0: 6473 2e29 01da 0763 6f6d 6d61 6e64 7221  ds.)...commandr!
-000013f0: 0000 0029 01da 0464 6573 7454 7217 0000  ...)...destTr...
-00001400: 007a 196c 6973 7420 6578 6973 7469 6e67  .z.list existing
-00001410: 204d 6169 6e50 726f 6a65 6374 2901 da04   MainProject)...
-00001420: 6865 6c70 7a04 2d2d 6964 da02 4944 7a26  helpz.--id..IDz&
-00001430: 6c69 7374 204d 6169 6e50 726f 6a65 6374  list MainProject
-00001440: 206d 6174 6368 696e 6720 7468 6520 6964   matching the id
-00001450: 205b 696e 745d 2903 da07 6d65 7461 7661   [int])...metava
-00001460: 72da 0474 7970 6572 2d00 0000 7a0b 2d2d  r..typer-...z.--
-00001470: 7465 6c65 7363 6f70 655a 0354 454c 7a30  telescopeZ.TELz0
-00001480: 6c69 7374 204d 6169 6e50 726f 6a65 6374  list MainProject
-00001490: 206d 6174 6368 696e 6720 7468 6520 7465   matching the te
-000014a0: 6c65 7363 6f70 6520 6964 205b 696e 745d  lescope id [int]
-000014b0: 7a06 2d2d 6e61 6d65 da04 4e41 4d45 7a28  z.--name..NAMEz(
-000014c0: 6c69 7374 204d 6169 6e50 726f 6a65 6374  list MainProject
-000014d0: 206d 6174 6368 696e 6720 7468 6520 6e61   matching the na
-000014e0: 6d65 205b 7374 725d 4e29 08da 0c73 6574  me [str]N)...set
-000014f0: 5f64 6566 6175 6c74 7372 2800 0000 da0e  _defaultsr(.....
-00001500: 6164 645f 7375 6270 6172 7365 7273 da08  add_subparsers..
-00001510: 7265 7175 6972 6564 da0a 6164 645f 7061  required..add_pa
-00001520: 7273 6572 da0c 6164 645f 6172 6775 6d65  rser..add_argume
-00001530: 6e74 da03 696e 74da 0373 7472 2904 7227  nt..int..str).r'
-00001540: 0000 0072 0600 0000 da04 7375 6273 da0b  ...r......subs..
-00001550: 7061 7273 6572 5f6c 6973 7472 0700 0000  parser_listr....
-00001560: 7207 0000 0072 0800 0000 7205 0000 00a9  r....r....r.....
-00001570: 0000 0073 1200 0000 1004 0c01 0601 0e02  ...s............
-00001580: 1201 0401 0801 06ff 1603 7a1d 4d61 696e  ..........z.Main
-00001590: 5072 6f6a 6563 742e 636f 6e66 6967 7572  Project.configur
-000015a0: 655f 7061 7273 6572 7329 034e 4e4e 290e  e_parsers).NNN).
-000015b0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000015c0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000015d0: 6d65 5f5f da07 5f5f 646f 635f 5f72 0d00  me__..__doc__r..
-000015e0: 0000 7217 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000015f0: 0072 1f00 0000 7224 0000 00da 0b63 6c61  .r....r$.....cla
-00001600: 7373 6d65 7468 6f64 7228 0000 0072 2a00  ssmethodr(...r*.
-00001610: 0000 7205 0000 0072 0700 0000 7207 0000  ..r....r....r...
-00001620: 0072 0700 0000 7208 0000 0072 0400 0000  .r....r....r....
-00001630: 0a00 0000 731c 0000 0008 0004 0108 070a  ....s...........
-00001640: 0508 1a08 2208 2608 1a02 0e0a 0102 030a  ....".&.........
-00001650: 0102 030e 0172 0400 0000 4e29 04da 1370  .....r....N)...p
-00001660: 7372 6462 2e67 7261 7068 716c 5f74 6162  srdb.graphql_tab
-00001670: 6c65 7202 0000 0072 0900 0000 7204 0000  ler....r....r...
-00001680: 0072 0700 0000 7207 0000 0072 0700 0000  .r....r....r....
-00001690: 7208 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000016a0: 0000 0073 0600 0000 0c00 0803 1406       ...s..........
+00000000: 696d 706f 7274 2072 6571 7565 7374 730a  import requests.
+00000010: 0a66 726f 6d20 7073 7264 622e 6772 6170  .from psrdb.grap
+00000020: 6871 6c5f 7461 626c 6520 696d 706f 7274  hql_table import
+00000030: 2047 7261 7068 514c 5461 626c 650a 0a0a   GraphQLTable...
+00000040: 6465 6620 6765 745f 7061 7273 6572 7328  def get_parsers(
+00000050: 293a 0a20 2020 2022 2222 5265 7475 726e  ):.    """Return
+00000060: 7320 7468 6520 6465 6661 756c 7420 7061  s the default pa
+00000070: 7273 6572 2066 6f72 2074 6869 7320 6d6f  rser for this mo
+00000080: 6465 6c22 2222 0a20 2020 2070 6172 7365  del""".    parse
+00000090: 7220 3d20 4772 6170 6851 4c54 6162 6c65  r = GraphQLTable
+000000a0: 2e67 6574 5f64 6566 6175 6c74 5f70 6172  .get_default_par
+000000b0: 7365 7228 2254 6865 2066 6f6c 6c6f 7769  ser("The followi
+000000c0: 6e67 206f 7074 696f 6e73 2077 696c 6c20  ng options will 
+000000d0: 616c 6c6f 7720 796f 7520 746f 2069 6e74  allow you to int
+000000e0: 6572 6163 7420 7769 7468 2074 6865 2054  eract with the T
+000000f0: 656d 706c 6174 6520 6461 7461 6261 7365  emplate database
+00000100: 206f 626a 6563 7420 6f6e 2074 6865 2063   object on the c
+00000110: 6f6d 6d61 6e64 206c 696e 6520 696e 2064  ommand line in d
+00000120: 6966 6665 7265 6e74 2077 6179 7320 6261  ifferent ways ba
+00000130: 7365 6420 6f6e 2074 6865 2073 7562 2d63  sed on the sub-c
+00000140: 6f6d 6d61 6e64 732e 2229 0a20 2020 2054  ommands.").    T
+00000150: 656d 706c 6174 652e 636f 6e66 6967 7572  emplate.configur
+00000160: 655f 7061 7273 6572 7328 7061 7273 6572  e_parsers(parser
+00000170: 290a 2020 2020 7265 7475 726e 2070 6172  ).    return par
+00000180: 7365 720a 0a0a 636c 6173 7320 5465 6d70  ser...class Temp
+00000190: 6c61 7465 2847 7261 7068 514c 5461 626c  late(GraphQLTabl
+000001a0: 6529 3a0a 2020 2020 2222 2243 6c61 7373  e):.    """Class
+000001b0: 2066 6f72 2069 6e74 6572 6163 7469 6e67   for interacting
+000001c0: 2077 6974 6820 7468 6520 5465 6d70 6c61   with the Templa
+000001d0: 7465 2064 6174 6162 6173 6520 6f62 6a65  te database obje
+000001e0: 6374 2e0a 0a20 2020 2050 6172 616d 6574  ct...    Paramet
+000001f0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00000200: 2d2d 0a20 2020 2063 6c69 656e 7420 3a20  --.    client : 
+00000210: 4772 6170 6851 4c43 6c69 656e 740a 2020  GraphQLClient.  
+00000220: 2020 2020 2020 4772 6170 6851 4c43 6c69        GraphQLCli
+00000230: 656e 7420 636c 6173 7320 696e 7374 616e  ent class instan
+00000240: 6365 2077 6974 6820 7468 6520 5552 4c20  ce with the URL 
+00000250: 616e 6420 546f 6b65 6e20 616c 7265 6164  and Token alread
+00000260: 7920 7365 742e 0a20 2020 2022 2222 0a20  y set..    """. 
+00000270: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000280: 7365 6c66 2c20 636c 6965 6e74 293a 0a20  self, client):. 
+00000290: 2020 2020 2020 2047 7261 7068 514c 5461         GraphQLTa
+000002a0: 626c 652e 5f5f 696e 6974 5f5f 2873 656c  ble.__init__(sel
+000002b0: 662c 2063 6c69 656e 7429 0a20 2020 2020  f, client).     
+000002c0: 2020 2073 656c 662e 7461 626c 655f 6e61     self.table_na
+000002d0: 6d65 203d 2022 7465 6d70 6c61 7465 220a  me = "template".
+000002e0: 2020 2020 2020 2020 7365 6c66 2e66 6965          self.fie
+000002f0: 6c64 5f6e 616d 6573 203d 205b 0a20 2020  ld_names = [.   
+00000300: 2020 2020 2020 2020 2022 6964 222c 0a20           "id",. 
+00000310: 2020 2020 2020 2020 2020 2022 7075 6c73             "puls
+00000320: 6172 207b 6a6e 616d 657d 222c 0a20 2020  ar {jname}",.   
+00000330: 2020 2020 2020 2020 2022 6672 6571 7565           "freque
+00000340: 6e63 7922 2c0a 2020 2020 2020 2020 2020  ncy",.          
+00000350: 2020 2262 616e 6477 6964 7468 222c 0a20    "bandwidth",. 
+00000360: 2020 2020 2020 2020 2020 2022 6372 6561             "crea
+00000370: 7465 6441 7422 2c0a 2020 2020 2020 2020  tedAt",.        
+00000380: 2020 2020 2263 7265 6174 6564 4279 222c      "createdBy",
+00000390: 0a20 2020 2020 2020 2020 2020 2022 6c6f  .            "lo
+000003a0: 6361 7469 6f6e 222c 0a20 2020 2020 2020  cation",.       
+000003b0: 2020 2020 2022 6d65 7468 6f64 222c 0a20       "method",. 
+000003c0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000003d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000003e0: 636f 6d6d 656e 7422 2c0a 2020 2020 2020  comment",.      
+000003f0: 2020 5d0a 0a20 2020 2064 6566 206c 6973    ]..    def lis
+00000400: 7428 7365 6c66 2c20 6964 3d4e 6f6e 652c  t(self, id=None,
+00000410: 2070 756c 7361 725f 6e61 6d65 3d4e 6f6e   pulsar_name=Non
+00000420: 652c 2062 616e 643d 4e6f 6e65 2c20 7072  e, band=None, pr
+00000430: 6f6a 6563 745f 7368 6f72 743d 4e6f 6e65  oject_short=None
+00000440: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+00000450: 7475 726e 2061 206c 6973 7420 6f66 2054  turn a list of T
+00000460: 656d 706c 6174 6520 696e 666f 726d 6174  emplate informat
+00000470: 696f 6e20 6261 7365 6420 6f6e 2074 6865  ion based on the
+00000480: 2060 7365 6c66 2e66 6965 6c64 5f6e 616d   `self.field_nam
+00000490: 6573 6020 616e 6420 6669 6c74 6572 6564  es` and filtered
+000004a0: 2062 7920 7468 6520 7061 7261 6d65 7465   by the paramete
+000004b0: 7273 2e0a 0a20 2020 2020 2020 2050 6172  rs...        Par
+000004c0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+000004d0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+000004e0: 2020 2069 6420 3a20 696e 742c 206f 7074     id : int, opt
+000004f0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00000500: 2020 4669 6c74 6572 2062 7920 7468 6520    Filter by the 
+00000510: 6461 7461 6261 7365 2049 442c 2062 7920  database ID, by 
+00000520: 6465 6661 756c 7420 4e6f 6e65 0a20 2020  default None.   
+00000530: 2020 2020 2070 756c 7361 725f 6e61 6d65       pulsar_name
+00000540: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
+00000550: 0a20 2020 2020 2020 2020 2020 2046 696c  .            Fil
+00000560: 7465 7220 6279 2074 6865 2070 756c 7361  ter by the pulsa
+00000570: 7220 6e61 6d65 2c20 6279 2064 6566 6175  r name, by defau
+00000580: 6c74 204e 6f6e 650a 2020 2020 2020 2020  lt None.        
+00000590: 6261 6e64 203a 2073 7472 2c20 6f70 7469  band : str, opti
+000005a0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+000005b0: 2046 696c 7465 7220 6279 2074 6865 2062   Filter by the b
+000005c0: 616e 642c 2062 7920 6465 6661 756c 7420  and, by default 
+000005d0: 4e6f 6e65 0a20 2020 2020 2020 2070 726f  None.        pro
+000005e0: 6a65 6374 5f73 686f 7274 203a 2073 7472  ject_short : str
+000005f0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00000600: 2020 2020 2020 2046 696c 7465 7220 6279         Filter by
+00000610: 2074 6865 2070 726f 6a65 6374 2073 686f   the project sho
+00000620: 7274 206e 616d 652c 2062 7920 6465 6661  rt name, by defa
+00000630: 756c 7420 4e6f 6e65 0a0a 2020 2020 2020  ult None..      
+00000640: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00000650: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00000660: 2020 6c69 7374 206f 6620 6469 6374 730a    list of dicts.
+00000670: 2020 2020 2020 2020 2020 2020 4966 2060              If `
+00000680: 7365 6c66 2e67 6574 5f64 6963 7473 6020  self.get_dicts` 
+00000690: 6973 2060 5472 7565 602c 2061 206c 6973  is `True`, a lis
+000006a0: 7420 6f66 2064 6963 7469 6f6e 6172 6965  t of dictionarie
+000006b0: 7320 636f 6e74 6169 6e69 6e67 2074 6865  s containing the
+000006c0: 2072 6573 756c 7473 2e0a 2020 2020 2020   results..      
+000006d0: 2020 636c 6965 6e74 5f72 6573 706f 6e73    client_respons
+000006e0: 653a 0a20 2020 2020 2020 2020 2020 2045  e:.            E
+000006f0: 6c73 6520 6120 636c 6965 6e74 2072 6573  lse a client res
+00000700: 706f 6e73 6520 6f62 6a65 6374 2e0a 2020  ponse object..  
+00000710: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00000720: 2020 6669 6c74 6572 7320 3d20 5b0a 2020    filters = [.  
+00000730: 2020 2020 2020 2020 2020 7b22 6669 656c            {"fiel
+00000740: 6422 3a20 2269 6422 2c20 2276 616c 7565  d": "id", "value
+00000750: 223a 2069 647d 2c0a 2020 2020 2020 2020  ": id},.        
+00000760: 2020 2020 7b22 6669 656c 6422 3a20 2270      {"field": "p
+00000770: 756c 7361 725f 4e61 6d65 222c 2022 7661  ulsar_Name", "va
+00000780: 6c75 6522 3a20 7075 6c73 6172 5f6e 616d  lue": pulsar_nam
+00000790: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
+000007a0: 7b22 6669 656c 6422 3a20 2262 616e 6422  {"field": "band"
+000007b0: 2c20 2276 616c 7565 223a 2062 616e 647d  , "value": band}
+000007c0: 2c0a 2020 2020 2020 2020 2020 2020 7b22  ,.            {"
+000007d0: 6669 656c 6422 3a20 2270 726f 6a65 6374  field": "project
+000007e0: 5f53 686f 7274 222c 2022 7661 6c75 6522  _Short", "value"
+000007f0: 3a20 7072 6f6a 6563 745f 7368 6f72 747d  : project_short}
+00000800: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+00000810: 2020 2020 7265 7475 726e 2047 7261 7068      return Graph
+00000820: 514c 5461 626c 652e 6c69 7374 5f67 7261  QLTable.list_gra
+00000830: 7068 716c 2873 656c 662c 2073 656c 662e  phql(self, self.
+00000840: 7461 626c 655f 6e61 6d65 2c20 6669 6c74  table_name, filt
+00000850: 6572 732c 205b 5d2c 2073 656c 662e 6669  ers, [], self.fi
+00000860: 656c 645f 6e61 6d65 7329 0a0a 2020 2020  eld_names)..    
+00000870: 6465 6620 6372 6561 7465 280a 2020 2020  def create(.    
+00000880: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00000890: 2020 2020 2020 2020 2020 7075 6c73 6172            pulsar
+000008a0: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
+000008b0: 2020 2062 616e 642c 0a20 2020 2020 2020     band,.       
+000008c0: 2020 2020 2074 656d 706c 6174 655f 7061       template_pa
+000008d0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+000008e0: 7072 6f6a 6563 745f 636f 6465 3d4e 6f6e  project_code=Non
+000008f0: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
+00000900: 726f 6a65 6374 5f73 686f 7274 3d4e 6f6e  roject_short=Non
+00000910: 652c 0a20 2020 2020 2020 2029 3a0a 2020  e,.        ):.  
+00000920: 2020 2020 2020 2222 2243 7265 6174 6520        """Create 
+00000930: 6120 6e65 7720 5465 6d70 6c61 7465 2064  a new Template d
+00000940: 6174 6162 6173 6520 6f62 6a65 6374 2e0a  atabase object..
+00000950: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00000960: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00000970: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2070  ------.        p
+00000980: 756c 7361 725f 6e61 6d65 203a 2073 7472  ulsar_name : str
+00000990: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+000009a0: 206e 616d 6520 6f66 2074 6865 2070 756c   name of the pul
+000009b0: 7361 722e 0a20 2020 2020 2020 2062 616e  sar..        ban
+000009c0: 6420 3a20 7374 720a 2020 2020 2020 2020  d : str.        
+000009d0: 2020 2020 5468 6520 6261 6e64 206f 6620      The band of 
+000009e0: 7468 6520 7465 6d70 6c61 7465 2028 652e  the template (e.
+000009f0: 672e 2053 4241 4e44 292e 0a20 2020 2020  g. SBAND)..     
+00000a00: 2020 2074 656d 706c 6174 655f 7061 7468     template_path
+00000a10: 203a 2073 7472 0a20 2020 2020 2020 2020   : str.         
+00000a20: 2020 2054 6865 2070 6174 6820 746f 2074     The path to t
+00000a30: 6865 2074 656d 706c 6174 6520 6669 6c65  he template file
+00000a40: 2e0a 2020 2020 2020 2020 7072 6f6a 6563  ..        projec
+00000a50: 745f 636f 6465 203a 2073 7472 2c20 6f70  t_code : str, op
+00000a60: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00000a70: 2020 2054 6865 2063 6f64 6520 6f66 2074     The code of t
+00000a80: 6865 2070 726f 6a65 6374 2c20 6279 2064  he project, by d
+00000a90: 6566 6175 6c74 204e 6f6e 650a 2020 2020  efault None.    
+00000aa0: 2020 2020 7072 6f6a 6563 745f 7368 6f72      project_shor
+00000ab0: 7420 3a20 7374 722c 206f 7074 696f 6e61  t : str, optiona
+00000ac0: 6c0a 2020 2020 2020 2020 2020 2020 5468  l.            Th
+00000ad0: 6520 7368 6f72 7420 6e61 6d65 206f 6620  e short name of 
+00000ae0: 7468 6520 7072 6f6a 6563 7420 2865 2e67  the project (e.g
+00000af0: 2e20 5054 4129 2c20 6279 2064 6566 6175  . PTA), by defau
+00000b00: 6c74 204e 6f6e 650a 0a20 2020 2020 2020  lt None..       
+00000b10: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00000b20: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00000b30: 2063 6c69 656e 745f 7265 7370 6f6e 7365   client_response
+00000b40: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
+00000b50: 636c 6965 6e74 2072 6573 706f 6e73 6520  client response 
+00000b60: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+00000b70: 2222 220a 2020 2020 2020 2020 2320 4f70  """.        # Op
+00000b80: 656e 2074 6865 2066 696c 6520 696e 2062  en the file in b
+00000b90: 696e 6172 7920 6d6f 6465 0a20 2020 2020  inary mode.     
+00000ba0: 2020 2077 6974 6820 6f70 656e 2874 656d     with open(tem
+00000bb0: 706c 6174 655f 7061 7468 2c20 2772 6227  plate_path, 'rb'
+00000bc0: 2920 6173 2066 696c 653a 0a20 2020 2020  ) as file:.     
+00000bd0: 2020 2020 2020 2076 6172 6961 626c 6573         variables
+00000be0: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00000bf0: 2020 2020 2022 7075 6c73 6172 5f6e 616d       "pulsar_nam
+00000c00: 6522 3a20 7075 6c73 6172 5f6e 616d 652c  e": pulsar_name,
+00000c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c20: 2022 7072 6f6a 6563 745f 636f 6465 223a   "project_code":
+00000c30: 2070 726f 6a65 6374 5f63 6f64 652c 0a20   project_code,. 
+00000c40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000c50: 7072 6f6a 6563 745f 7368 6f72 7422 3a20  project_short": 
+00000c60: 7072 6f6a 6563 745f 7368 6f72 742c 0a20  project_short,. 
+00000c70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000c80: 6261 6e64 223a 2062 616e 642c 0a20 2020  band": band,.   
+00000c90: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00000ca0: 2020 2020 2020 2066 696c 6573 203d 207b         files = {
+00000cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000cc0: 2022 7465 6d70 6c61 7465 5f75 706c 6f61   "template_uploa
+00000cd0: 6422 3a20 6669 6c65 2c0a 2020 2020 2020  d": file,.      
+00000ce0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00000cf0: 2020 2020 2320 506f 7374 2074 6f20 7468      # Post to th
+00000d00: 6520 7265 7374 2061 7069 0a20 2020 2020  e rest api.     
+00000d10: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+00000d20: 3d20 7265 7175 6573 7473 2e70 6f73 7428  = requests.post(
+00000d30: 6627 7b73 656c 662e 636c 6965 6e74 2e72  f'{self.client.r
+00000d40: 6573 745f 6170 695f 7572 6c7d 7465 6d70  est_api_url}temp
+00000d50: 6c61 7465 2f27 2c20 6461 7461 3d76 6172  late/', data=var
+00000d60: 6961 626c 6573 2c20 6669 6c65 733d 6669  iables, files=fi
+00000d70: 6c65 7329 0a0a 2020 2020 2020 2020 7265  les)..        re
+00000d80: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+00000d90: 2020 2064 6566 2070 726f 6365 7373 2873     def process(s
+00000da0: 656c 662c 2061 7267 7329 3a0a 2020 2020  elf, args):.    
+00000db0: 2020 2020 2222 2250 6172 7365 2074 6865      """Parse the
+00000dc0: 2061 7267 756d 656e 7473 2063 6f6c 6c65   arguments colle
+00000dd0: 6374 6564 2062 7920 7468 6520 434c 492e  cted by the CLI.
+00000de0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+00000df0: 2e70 7269 6e74 5f73 7464 6f75 7420 3d20  .print_stdout = 
+00000e00: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
+00000e10: 6172 6773 2e73 7562 636f 6d6d 616e 6420  args.subcommand 
+00000e20: 3d3d 2022 6372 6561 7465 223a 0a20 2020  == "create":.   
+00000e30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000e40: 7365 6c66 2e63 7265 6174 6528 0a20 2020  self.create(.   
+00000e50: 2020 2020 2020 2020 2020 2020 2061 7267               arg
+00000e60: 732e 7075 6c73 6172 2c0a 2020 2020 2020  s.pulsar,.      
+00000e70: 2020 2020 2020 2020 2020 6172 6773 2e70            args.p
+00000e80: 726f 6a65 6374 5f63 6f64 652c 0a20 2020  roject_code,.   
+00000e90: 2020 2020 2020 2020 2020 2020 2061 7267               arg
+00000ea0: 732e 6261 6e64 2c0a 2020 2020 2020 2020  s.band,.        
+00000eb0: 2020 2020 2020 2020 6172 6773 2e74 656d          args.tem
+00000ec0: 706c 6174 655f 7061 7468 2c0a 2020 2020  plate_path,.    
+00000ed0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00000ee0: 2020 656c 6966 2061 7267 732e 7375 6263    elif args.subc
+00000ef0: 6f6d 6d61 6e64 203d 3d20 226c 6973 7422  ommand == "list"
+00000f00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000f10: 7475 726e 2073 656c 662e 6c69 7374 2861  turn self.list(a
+00000f20: 7267 732e 6964 2c20 6172 6773 2e70 756c  rgs.id, args.pul
+00000f30: 7361 722c 2061 7267 732e 6672 6571 7565  sar, args.freque
+00000f40: 6e63 792c 2061 7267 732e 6261 6e64 7769  ncy, args.bandwi
+00000f50: 6474 6829 0a20 2020 2020 2020 2065 6c73  dth).        els
+00000f60: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00000f70: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00000f80: 7228 6622 7b61 7267 732e 7375 6263 6f6d  r(f"{args.subcom
+00000f90: 6d61 6e64 7d20 636f 6d6d 616e 6420 6973  mand} command is
+00000fa0: 206e 6f74 2069 6d70 6c65 6d65 6e74 6564   not implemented
+00000fb0: 2229 0a0a 2020 2020 4063 6c61 7373 6d65  ")..    @classme
+00000fc0: 7468 6f64 0a20 2020 2064 6566 2067 6574  thod.    def get
+00000fd0: 5f6e 616d 6528 636c 7329 3a0a 2020 2020  _name(cls):.    
+00000fe0: 2020 2020 7265 7475 726e 2022 7465 6d70      return "temp
+00000ff0: 6c61 7465 220a 0a20 2020 2040 636c 6173  late"..    @clas
+00001000: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00001010: 6765 745f 6465 7363 7269 7074 696f 6e28  get_description(
+00001020: 636c 7329 3a0a 2020 2020 2020 2020 7265  cls):.        re
+00001030: 7475 726e 2022 4120 7075 6c73 6172 2074  turn "A pulsar t
+00001040: 656d 706c 6174 652f 7374 616e 6461 7264  emplate/standard
+00001050: 220a 0a20 2020 2040 636c 6173 736d 6574  "..    @classmet
+00001060: 686f 640a 2020 2020 6465 6620 6765 745f  hod.    def get_
+00001070: 7061 7273 6572 7328 636c 7329 3a0a 2020  parsers(cls):.  
+00001080: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
+00001090: 2074 6865 2064 6566 6175 6c74 2070 6172   the default par
+000010a0: 7365 7220 666f 7220 7468 6973 206d 6f64  ser for this mod
+000010b0: 656c 2222 220a 2020 2020 2020 2020 7061  el""".        pa
+000010c0: 7273 6572 203d 2047 7261 7068 514c 5461  rser = GraphQLTa
+000010d0: 626c 652e 6765 745f 6465 6661 756c 745f  ble.get_default_
+000010e0: 7061 7273 6572 2822 5465 6d70 6c61 7465  parser("Template
+000010f0: 206d 6f64 656c 2070 6172 7365 7222 290a   model parser").
+00001100: 2020 2020 2020 2020 636c 732e 636f 6e66          cls.conf
+00001110: 6967 7572 655f 7061 7273 6572 7328 7061  igure_parsers(pa
+00001120: 7273 6572 290a 2020 2020 2020 2020 7265  rser).        re
+00001130: 7475 726e 2070 6172 7365 720a 0a20 2020  turn parser..   
+00001140: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00001150: 2020 6465 6620 636f 6e66 6967 7572 655f    def configure_
+00001160: 7061 7273 6572 7328 636c 732c 2070 6172  parsers(cls, par
+00001170: 7365 7229 3a0a 2020 2020 2020 2020 2222  ser):.        ""
+00001180: 2241 6464 2073 7562 2d70 6172 7365 7273  "Add sub-parsers
+00001190: 2066 6f72 2065 6163 6820 6f66 2074 6865   for each of the
+000011a0: 2076 616c 6964 2063 6f6d 6d61 6e64 732e   valid commands.
+000011b0: 2222 220a 2020 2020 2020 2020 2320 6372  """.        # cr
+000011c0: 6561 7465 2074 6865 2070 6172 7365 7220  eate the parser 
+000011d0: 666f 7220 7468 6520 226c 6973 7422 2063  for the "list" c
+000011e0: 6f6d 6d61 6e64 0a20 2020 2020 2020 2070  ommand.        p
+000011f0: 6172 7365 722e 7365 745f 6465 6661 756c  arser.set_defaul
+00001200: 7473 2863 6f6d 6d61 6e64 3d63 6c73 2e67  ts(command=cls.g
+00001210: 6574 5f6e 616d 6528 2929 0a20 2020 2020  et_name()).     
+00001220: 2020 2073 7562 7320 3d20 7061 7273 6572     subs = parser
+00001230: 2e61 6464 5f73 7562 7061 7273 6572 7328  .add_subparsers(
+00001240: 6465 7374 3d22 7375 6263 6f6d 6d61 6e64  dest="subcommand
+00001250: 2229 0a20 2020 2020 2020 2073 7562 732e  ").        subs.
+00001260: 7265 7175 6972 6564 203d 2054 7275 650a  required = True.
+00001270: 0a20 2020 2020 2020 2070 6172 7365 725f  .        parser_
+00001280: 6c69 7374 203d 2073 7562 732e 6164 645f  list = subs.add_
+00001290: 7061 7273 6572 2822 6c69 7374 222c 2068  parser("list", h
+000012a0: 656c 703d 226c 6973 7420 6578 6973 7469  elp="list existi
+000012b0: 6e67 2065 7068 656d 6572 6964 6573 2229  ng ephemerides")
+000012c0: 0a20 2020 2020 2020 2070 6172 7365 725f  .        parser_
+000012d0: 6c69 7374 2e61 6464 5f61 7267 756d 656e  list.add_argumen
+000012e0: 7428 222d 2d69 6422 2c20 6d65 7461 7661  t("--id", metava
+000012f0: 723d 2249 4422 2c20 7479 7065 3d69 6e74  r="ID", type=int
+00001300: 2c20 6865 6c70 3d22 6c69 7374 2074 656d  , help="list tem
+00001310: 706c 6174 6520 6d61 7463 6869 6e67 2074  plate matching t
+00001320: 6865 2069 6420 5b69 6e74 5d22 290a 2020  he id [int]").  
+00001330: 2020 2020 2020 7061 7273 6572 5f6c 6973        parser_lis
+00001340: 742e 6164 645f 6172 6775 6d65 6e74 280a  t.add_argument(.
+00001350: 2020 2020 2020 2020 2020 2020 222d 2d70              "--p
+00001360: 756c 7361 7222 2c20 6d65 7461 7661 723d  ulsar", metavar=
+00001370: 2250 5352 222c 2074 7970 653d 696e 742c  "PSR", type=int,
+00001380: 2068 656c 703d 226c 6973 7420 7465 6d70   help="list temp
+00001390: 6c61 7465 206d 6174 6368 696e 6720 7468  late matching th
+000013a0: 6520 7075 6c73 6172 2069 6420 5b69 6e74  e pulsar id [int
+000013b0: 5d22 0a20 2020 2020 2020 2029 0a20 2020  ]".        ).   
+000013c0: 2020 2020 2070 6172 7365 725f 6c69 7374       parser_list
+000013d0: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
+000013e0: 2020 2020 2020 2020 2020 2022 2d2d 6672             "--fr
+000013f0: 6571 7565 6e63 7922 2c0a 2020 2020 2020  equency",.      
+00001400: 2020 2020 2020 6d65 7461 7661 723d 2246        metavar="F
+00001410: 5245 5122 2c0a 2020 2020 2020 2020 2020  REQ",.          
+00001420: 2020 7479 7065 3d66 6c6f 6174 2c0a 2020    type=float,.  
+00001430: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
+00001440: 6c69 7374 2074 656d 706c 6174 6520 6d61  list template ma
+00001450: 7463 6869 6e67 2074 6865 2070 756c 7361  tching the pulsa
+00001460: 7220 6672 6571 7565 6e63 7920 696e 204d  r frequency in M
+00001470: 487a 205b 666c 6f61 745d 5d22 2c0a 2020  Hz [float]]",.  
+00001480: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00001490: 7061 7273 6572 5f6c 6973 742e 6164 645f  parser_list.add_
+000014a0: 6172 6775 6d65 6e74 280a 2020 2020 2020  argument(.      
+000014b0: 2020 2020 2020 222d 2d62 616e 6477 6964        "--bandwid
+000014c0: 7468 222c 206d 6574 6176 6172 3d22 4257  th", metavar="BW
+000014d0: 222c 2074 7970 653d 666c 6f61 742c 2068  ", type=float, h
+000014e0: 656c 703d 226c 6973 7420 7465 6d70 6c61  elp="list templa
+000014f0: 7465 206d 6174 6368 696e 6720 7468 6520  te matching the 
+00001500: 7075 6c73 6172 2062 616e 6477 6964 7468  pulsar bandwidth
+00001510: 2069 6e20 4d48 7a20 5b66 6c6f 6174 5d5d   in MHz [float]]
+00001520: 220a 2020 2020 2020 2020 29              ".        )
```

### Comparing `psrdb-3.0.5/psrdb/tables/calibration.py` & `psrdb-3.0.6/psrdb/tables/calibration.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/tables/ephemeris.py` & `psrdb-3.0.6/psrdb/tables/ephemeris.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/tables/main_project.py` & `psrdb-3.0.6/psrdb/tables/main_project.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/tables/observation.py` & `psrdb-3.0.6/psrdb/tables/observation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,864 +1,864 @@
-from datetime import datetime
-
-from psrdb.graphql_table import GraphQLTable
-from psrdb.utils.other import decode_id
-
-
-def get_parsers():
-    """Returns the default parser for this model"""
-    parser = GraphQLTable.get_default_parser("The following options will allow you to interact with the Observation database object on the command line in different ways based on the sub-commands.")
-    Observation.configure_parsers(parser)
-    return parser
-
-
-class Observation(GraphQLTable):
-    """Class for interacting with the Observation database object.
-
-    Parameters
-    ----------
-    client : GraphQLClient
-        GraphQLClient class instance with the URL and Token already set.
-    """
-    def __init__(self, client, logger=None):
-        GraphQLTable.__init__(self, client, logger)
-        self.table_name = "observation"
-        self.field_names = [
-            "id",
-            "pulsar { name }",
-            "calibration { id }",
-            "calibration { location }",
-            "telescope { name }",
-            "project { code }",
-            "project { short }",
-            "utcStart",
-            "beam",
-            "band",
-            "duration",
-            "foldNchan",
-            "foldNbin",
-            "modeDuration"
-        ]
-
-    def list(
-        self,
-        id=None,
-        pulsar_name=None,
-        telescope_name=None,
-        project_id=None,
-        project_short=None,
-        main_project="All",
-        utcs=None,
-        utce=None,
-        obs_type='fold',
-        unprocessed=None,
-        incomplete=None,
-    ):
-        """Return a list of Observation information based on the `self.field_names` and filtered by the parameters.
-
-        Parameters
-        ----------
-        id : int, optional
-            Filter by the database ID, by default None
-        pulsar_name : str, optional
-            Filter by the pulsar name, by default None
-        telescope_name : str, optional
-            Filter by the telescope name, by default None
-        project_id : int, optional
-            Filter by the project id, by default None
-        project_short : str, optional
-            Filter by the project short name, by default None
-        utcs : str, optional
-            Filter by the utc start time greater than or equal to the timestamp in the format YYYY-MM-DDTHH:MM:SS+00:00, by default None
-        utce : str, optional
-            Filter by the utc start time less than or equal to the timestamp in the format YYYY-MM-DDTHH:MM:SS+00:00, by default None
-        obs_type : str, optional
-            Filter by the observation type (fold, search or cal), by default 'fold'
-        unprocessed : str, optional
-            Filter to only returned unprocessed observations (no PulsarFoldResult)
-        incomplete : str, optional
-            Filter to only return incomplete observations (most recent job run is not "Completed)
-
-        Returns
-        -------
-        list of dicts
-            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
-        client_response:
-            Else a client response object.
-        """
-        # Convert dates to correct format
-        if utcs == "":
-            utcs = None
-        elif utcs is not None:
-            d = datetime.strptime(utcs, '%Y-%m-%d-%H:%M:%S')
-            utcs = f"{d.date()}T{d.time()}+00:00"
-        if utce == "":
-            utce = None
-        elif utce is not None:
-            d = datetime.strptime(utce, '%Y-%m-%d-%H:%M:%S')
-            utce = f"{d.date()}T{d.time()}+00:00"
-        if project_short == "":
-            project_short = None
-        if pulsar_name == "":
-            pulsar_name = None
-        """Return a list of records matching the id and/or any of the arguments."""
-        filters = [
-            {"field": "id", "value": id},
-            {"field": "pulsar_Name", "value": pulsar_name},
-            {"field": "telescope_Name", "value": telescope_name},
-            {"field": "project_Id", "value": project_id},
-            {"field": "project_Short", "value": project_short},
-            {"field": "mainProject", "value": main_project},
-            {"field": "utcStartGte", "value": utcs},
-            {"field": "utcStartLte", "value": utce},
-            {"field": "obsType", "value": obs_type},
-        ]
-        if unprocessed is not None:
-            filters.append({"field": "unprocessed", "value": unprocessed})
-        if incomplete is not None:
-            filters.append({"field": "incomplete", "value": incomplete})
-        return GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
-
-    def download(
-        self,
-        id=None,
-        pulsar_name=None,
-        telescope_name=None,
-        project_id=None,
-        project_short=None,
-        main_project="meertime",
-        utcs=None,
-        utce=None,
-        obs_type='fold',
-        unprocessed=None,
-        incomplete=None,
-    ):
-        """Return a list of Observation information based on the `self.field_names` and filtered by the parameters.
-
-        Parameters
-        ----------
-        id : int, optional
-            Filter by the database ID, by default None
-        pulsar_name : str, optional
-            Filter by the pulsar name, by default None
-        telescope_name : str, optional
-            Filter by the telescope name, by default None
-        project_id : int, optional
-            Filter by the project id, by default None
-        project_short : str, optional
-            Filter by the project short name, by default None
-        utcs : str, optional
-            Filter by the utc start time greater than or equal to the timestamp in the format YYYY-MM-DDTHH:MM:SS+00:00, by default None
-        utce : str, optional
-            Filter by the utc start time less than or equal to the timestamp in the format YYYY-MM-DDTHH:MM:SS+00:00, by default None
-        obs_type : str, optional
-            Filter by the observation type (fold, search or cal), by default 'fold'
-        unprocessed : str, optional
-            Filter to only returned unprocessed observations (no PulsarFoldResult)
-        incomplete : str, optional
-            Filter to only return incomplete observations (most recent job run is not "Completed)
-
-        Returns
-        -------
-        list of dicts
-            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
-        client_response:
-            Else a client response object.
-        """
-        # Convert dates to correct format
-        if utcs == "":
-            utcs = None
-        elif utcs is not None:
-            d = datetime.strptime(utcs, '%Y-%m-%d-%H:%M:%S')
-            utcs = f"{d.date()}T{d.time()}+00:00"
-        if utce == "":
-            utce = None
-        elif utce is not None:
-            d = datetime.strptime(utce, '%Y-%m-%d-%H:%M:%S')
-            utce = f"{d.date()}T{d.time()}+00:00"
-        if project_short == "":
-            project_short = None
-        if pulsar_name == "":
-            pulsar_name = None
-        """Return a list of records matching the id and/or any of the arguments."""
-        filters = [
-            {"field": "id", "value": id},
-            {"field": "pulsar_Name", "value": pulsar_name},
-            {"field": "telescope_Name", "value": telescope_name},
-            {"field": "project_Id", "value": project_id},
-            {"field": "project_Short", "value": project_short},
-            {"field": "mainProject", "value": main_project},
-            {"field": "utcStartGte", "value": utcs},
-            {"field": "utcStartLte", "value": utce},
-            {"field": "obsType", "value": obs_type},
-        ]
-        if unprocessed is not None:
-            filters.append({"field": "unprocessed", "value": unprocessed})
-        if incomplete is not None:
-            filters.append({"field": "incomplete", "value": incomplete})
-
-        self.get_dicts = True
-        observations_dicts = GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
-
-        # Create the output name
-        output_name = "observations"
-        if main_project:
-            output_name += f"_{main_project}"
-        if pulsar_name:
-            output_name += f"_{'_'.join(pulsar_name)}"
-        if telescope_name:
-            output_name += f"_{telescope_name}"
-        if project_id:
-            output_name += f"_{project_id}"
-        if project_short:
-            output_name += f"_{project_short}"
-        if utcs:
-            output_name += f"_utcs{utcs}"
-        if utce:
-            output_name += f"_utce{utce}"
-        if obs_type:
-            output_name += f"_{obs_type}"
-        if unprocessed:
-            output_name += "_unprocessed"
-        if incomplete:
-            output_name += "_incomplete"
-        output_name += ".csv"
-
-        # Loop over the pulsar_fold_results and dump them as a file
-        with open(output_name, "w") as f:
-            f.write("Obs ID,Pulsar Jname,UTC Start,Project Short Name,Beam #,Observing Band,Duration (s),Mode Duration (s),Nchan,Nbin,Calibration Location\n")
-            for observations_dict in observations_dicts:
-                data_line = [
-                    str(decode_id(observations_dict["id"])),
-                    str(observations_dict["pulsar"]["name"]),
-                    str(datetime.strptime(observations_dict['utcStart'], '%Y-%m-%dT%H:%M:%S+00:00').strftime('%Y-%m-%d-%H:%M:%S')),
-                    str(observations_dict["project"]["short"]),
-                    str(observations_dict["beam"]),
-                    str(observations_dict["band"]),
-                    str(observations_dict["duration"]),
-                    str(observations_dict["modeDuration"]),
-                    str(observations_dict["foldNchan"]),
-                    str(observations_dict["foldNbin"]),
-                    str(observations_dict["calibration"]["location"]),
-                ]
-                f.write(f"{','.join(data_line)}\n")
-        return output_name
-
-    def create(
-        self,
-        pulsarName,
-        telescopeName,
-        projectCode,
-        calibrationId,
-        ephemerisText,
-        frequency,
-        bandwidth,
-        nchan,
-        beam,
-        nant,
-        nantEff,
-        npol,
-        obsType,
-        utcStart,
-        raj,
-        decj,
-        duration,
-        nbit,
-        tsamp,
-        foldNbin,
-        foldNchan,
-        foldTsubint,
-        filterbankNbit,
-        filterbankNpol,
-        filterbankNchan,
-        filterbankTsamp,
-        filterbankDm,
-    ):
-        """Create a new Observation database object.
-
-        Parameters
-        ----------
-        pulsarName : str
-            The pulsar name.
-        telescopeName : str
-            The telescope name.
-        projectCode : str
-            The project code.
-        calibrationId : int
-            The ID of the Calibration database object.
-        ephemerisText : str
-            The ephemeris text as a single string (includes new line characters).
-        frequency : float
-            The frequency of the observation in MHz.
-        bandwidth : float
-            The bandwidth of the observation in MHz.
-        nchan : int
-            The number of frequency channels.
-        beam : int
-            The beam number.
-        nant : int
-            The number of antennas used in the observation.
-        nantEff : int
-            The effective number of antennas used in the observation.
-        npol : int
-            The number of polarisations.
-        obsType : str
-            The type of observation (fold, search or cal).
-        utcStart : `datetime`
-            The UTC start time of the observation as a `datetime` object.
-        raj : str
-            The right ascension of the observation in HH:MM:SS.SS format.
-        decj : str
-            The declination of the observation in DD:MM:SS.SS format.
-        duration : float
-            The duration of the observation in seconds.
-        nbit : int
-            The number of bits per sample.
-        tsamp : float
-            The sampling time in microseconds.
-        foldNbin : int
-            The number of bins in the folded data (None for non fold observations).
-        foldNchan : int
-            The number of frequency channels in the folded data (None for non fold observations).
-        foldTsubint : int
-            The number of time samples in each sub-integration of the folded data (None for non fold observations).
-        filterbankNbit : int
-            The number of bits per sample in the filterbank data (None for non search observations).
-        filterbankNpol : int
-            The number of polarisations in the filterbank data (None for non search observations).
-        filterbankNchan : int
-            The number of frequency channels in the filterbank data (None for non search observations).
-        filterbankTsamp : float
-            The sampling time in microseconds in the filterbank data (None for non search observations).
-        filterbankDm : float
-            The dispersion measure in the filterbank data (None for non search observations).
-
-        Returns
-        -------
-        client_response:
-            A client response object.
-        """
-        # create a new record
-        self.mutation_name = "createObservation"
-        self.mutation = """
-        mutation (
-            $pulsarName: String!,
-            $telescopeName: String!,
-            $projectCode: String!,
-            $calibrationId: Int!,
-            $frequency: Float!,
-            $bandwidth: Float!,
-            $nchan: Int!,
-            $beam: Int!,
-            $nant: Int!,
-            $nantEff: Int!,
-            $npol: Int!,
-            $obsType: String!,
-            $utcStart: DateTime!,
-            $raj: String!,
-            $decj: String!,
-            $duration: Float!,
-            $nbit: Int!,
-            $tsamp: Float!,
-            # Fold options
-            $ephemerisText: String,
-            $foldNbin: Int,
-            $foldNchan: Int,
-            $foldTsubint: Int,
-            # Search options
-            $filterbankNbit: Int,
-            $filterbankNpol: Int,
-            $filterbankNchan: Int,
-            $filterbankTsamp: Float,
-            $filterbankDm: Float,
-        ) {
-            createObservation(input: {
-                pulsarName: $pulsarName,
-                telescopeName: $telescopeName,
-                projectCode: $projectCode,
-                calibrationId: $calibrationId,
-                frequency: $frequency,
-                bandwidth: $bandwidth,
-                nchan: $nchan,
-                beam: $beam,
-                nant: $nant,
-                nantEff: $nantEff,
-                npol: $npol,
-                obsType: $obsType,
-                utcStart: $utcStart,
-                raj: $raj,
-                decj: $decj,
-                duration: $duration,
-                nbit: $nbit,
-                tsamp: $tsamp,
-                ephemerisText: $ephemerisText,
-                foldNbin: $foldNbin,
-                foldNchan: $foldNchan,
-                foldTsubint: $foldTsubint,
-                filterbankNbit: $filterbankNbit,
-                filterbankNpol: $filterbankNpol,
-                filterbankNchan: $filterbankNchan,
-                filterbankTsamp: $filterbankTsamp,
-                filterbankDm: $filterbankDm,
-            }) {
-                observation {
-                    id
-                }
-            }
-        }
-        """
-        self.variables = {
-            "pulsarName": pulsarName,
-            "telescopeName": telescopeName,
-            "projectCode": projectCode,
-            "calibrationId": calibrationId,
-            "ephemerisText": ephemerisText,
-            "frequency": frequency,
-            "bandwidth": bandwidth,
-            "nchan": nchan,
-            "beam": beam,
-            "nant": nant,
-            "nantEff": nantEff,
-            "npol": npol,
-            "obsType": obsType,
-            "utcStart": utcStart,
-            "raj": raj,
-            "decj": decj,
-            "duration": duration,
-            "nbit": nbit,
-            "tsamp": tsamp,
-            "foldNbin": foldNbin,
-            "foldNchan": foldNchan,
-            "foldTsubint": foldTsubint,
-            "filterbankNbit": filterbankNbit,
-            "filterbankNpol": filterbankNpol,
-            "filterbankNchan": filterbankNchan,
-            "filterbankTsamp": filterbankTsamp,
-            "filterbankDm": filterbankDm,
-        }
-        return self.mutation_graphql()
-
-    def update(
-        self,
-        id,
-        pulsarName,
-        telescopeName,
-        projectCode,
-        calibrationId,
-        ephemerisText,
-        frequency,
-        bandwidth,
-        nchan,
-        beam,
-        nant,
-        nantEff,
-        npol,
-        obsType,
-        utcStart,
-        raj,
-        decj,
-        duration,
-        nbit,
-        tsamp,
-        foldNbin,
-        foldNchan,
-        foldTsubint,
-        filterbankNbit,
-        filterbankNpol,
-        filterbankNchan,
-        filterbankTsamp,
-        filterbankDm,
-    ):
-        """Update a Observation database object.
-
-        Parameters
-        ----------
-        id : int
-            The database ID
-        pulsarName : str
-            The pulsar name.
-        telescopeName : str
-            The telescope name.
-        projectCode : str
-            The project code.
-        calibrationId : int
-            The ID of the Calibration database object.
-        ephemerisText : str
-            The ephemeris text as a single string (includes new line characters).
-        frequency : float
-            The frequency of the observation in MHz.
-        bandwidth : float
-            The bandwidth of the observation in MHz.
-        nchan : int
-            The number of frequency channels.
-        beam : int
-            The beam number.
-        nant : int
-            The number of antennas used in the observation.
-        nantEff : int
-            The effective number of antennas used in the observation.
-        npol : int
-            The number of polarisations.
-        obsType : str
-            The type of observation (fold, search or cal).
-        utcStart : `datetime`
-            The UTC start time of the observation as a `datetime` object.
-        raj : str
-            The right ascension of the observation in HH:MM:SS.SS format.
-        decj : str
-            The declination of the observation in DD:MM:SS.SS format.
-        duration : float
-            The duration of the observation in seconds.
-        nbit : int
-            The number of bits per sample.
-        tsamp : float
-            The sampling time in microseconds.
-        foldNbin : int
-            The number of bins in the folded data (None for non fold observations).
-        foldNchan : int
-            The number of frequency channels in the folded data (None for non fold observations).
-        foldTsubint : int
-            The number of time samples in each sub-integration of the folded data (None for non fold observations).
-        filterbankNbit : int
-            The number of bits per sample in the filterbank data (None for non search observations).
-        filterbankNpol : int
-            The number of polarisations in the filterbank data (None for non search observations).
-        filterbankNchan : int
-            The number of frequency channels in the filterbank data (None for non search observations).
-        filterbankTsamp : float
-            The sampling time in microseconds in the filterbank data (None for non search observations).
-        filterbankDm : float
-            The dispersion measure in the filterbank data (None for non search observations).
-
-
-        Returns
-        -------
-        client_response:
-            A client response object.
-        """
-        self.mutation_name = "updateObservation"
-        self.mutation = """
-        mutation (
-            $id: Int!,
-            $pulsarName: String!,
-            $telescopeName: String!,
-            $projectCode: String!,
-            $calibrationId: Int!,
-            $frequency: Float!,
-            $bandwidth: Float!,
-            $nchan: Int!,
-            $beam: Int!,
-            $nant: Int!,
-            $nantEff: Int!,
-            $npol: Int!,
-            $obsType: String!,
-            $utcStart: DateTime!,
-            $raj: String!,
-            $decj: String!,
-            $duration: Float!,
-            $nbit: Int!,
-            $tsamp: Float!,
-            # Fold options
-            $ephemerisText: String,
-            $foldNbin: Int,
-            $foldNchan: Int,
-            $foldTsubint: Int,
-            # Search options
-            $filterbankNbit: Int,
-            $filterbankNpol: Int,
-            $filterbankNchan: Int,
-            $filterbankTsamp: Float,
-            $filterbankDm: Float,
-        ) {
-            updateObservation(input: {
-                id: $id,
-                pulsarName: $pulsarName,
-                telescopeName: $telescopeName,
-                projectCode: $projectCode,
-                calibrationId: $calibrationId,
-                frequency: $frequency,
-                bandwidth: $bandwidth,
-                nchan: $nchan,
-                beam: $beam,
-                nant: $nant,
-                nantEff: $nantEff,
-                npol: $npol,
-                obsType: $obsType,
-                utcStart: $utcStart,
-                raj: $raj,
-                decj: $decj,
-                duration: $duration,
-                nbit: $nbit,
-                tsamp: $tsamp,
-                ephemerisText: $ephemerisText,
-                foldNbin: $foldNbin,
-                foldNchan: $foldNchan,
-                foldTsubint: $foldTsubint,
-                filterbankNbit: $filterbankNbit,
-                filterbankNpol: $filterbankNpol,
-                filterbankNchan: $filterbankNchan,
-                filterbankTsamp: $filterbankTsamp,
-                filterbankDm: $filterbankDm,
-            }) {
-                observation {
-                    id
-                }
-            }
-        }
-        """
-        self.variables = {
-            "id": id,
-            "pulsarName": pulsarName,
-            "telescopeName": telescopeName,
-            "projectCode": projectCode,
-            "calibrationId": calibrationId,
-            "ephemerisText": ephemerisText,
-            "frequency": frequency,
-            "bandwidth": bandwidth,
-            "nchan": nchan,
-            "beam": beam,
-            "nant": nant,
-            "nantEff": nantEff,
-            "npol": npol,
-            "obsType": obsType,
-            "utcStart": utcStart,
-            "raj": raj,
-            "decj": decj,
-            "duration": duration,
-            "nbit": nbit,
-            "tsamp": tsamp,
-            "foldNbin": foldNbin,
-            "foldNchan": foldNchan,
-            "foldTsubint": foldTsubint,
-            "filterbankNbit": filterbankNbit,
-            "filterbankNpol": filterbankNpol,
-            "filterbankNchan": filterbankNchan,
-            "filterbankTsamp": filterbankTsamp,
-            "filterbankDm": filterbankDm,
-        }
-        return self.mutation_graphql()
-
-    def delete(self, id):
-        """Delete a Observation database object.
-
-        Parameters
-        ----------
-        id : int
-            The database ID
-
-        Returns
-        -------
-        client_response:
-            A client response object.
-        """
-        self.mutation_name = "deleteObservation"
-        self.mutation = """
-        mutation ($id: Int!) {
-            deleteObservation(id: $id) {
-                ok
-            }
-        }
-        """
-        self.variables = {
-            "id": id,
-        }
-        return self.mutation_graphql()
-
-    def process(self, args):
-        """Parse the arguments collected by the CLI."""
-        self.print_stdout = True
-        if args.subcommand == "list":
-            return self.list(
-                id=args.id,
-                pulsar_name=args.pulsar,
-                telescope_name=args.telescope_name,
-                project_id=args.project_id,
-                project_short=args.project_code,
-                main_project=args.main_project,
-                utcs=args.utcs,
-                utce=args.utce,
-                obs_type=args.obs_type,
-                unprocessed=args.unprocessed,
-                incomplete=args.incomplete,
-            )
-        elif args.subcommand == "download":
-            return self.download(
-                id=args.id,
-                pulsar_name=args.pulsar,
-                telescope_name=args.telescope_name,
-                project_id=args.project_id,
-                project_short=args.project_code,
-                main_project=args.main_project,
-                utcs=args.utcs,
-                utce=args.utce,
-                obs_type=args.obs_type,
-                unprocessed=args.unprocessed,
-                incomplete=args.incomplete,
-            )
-        else:
-            raise RuntimeError(f"{args.subcommand} command is not implemented")
-
-    @classmethod
-    def get_name(cls):
-        return "observation"
-
-    @classmethod
-    def get_description(cls):
-        return "Observation details."
-
-    @classmethod
-    def get_parsers(cls):
-        """Returns the default parser for this model"""
-        parser = GraphQLTable.get_default_parser("Observations model parser")
-        cls.configure_parsers(parser)
-        return parser
-
-    @classmethod
-    def configure_parsers(cls, parser):
-        """Add sub-parsers for each of the valid commands."""
-        # create the parser for the "list" command
-        parser.set_defaults(command=cls.get_name())
-        subs = parser.add_subparsers(dest="subcommand")
-        subs.required = True
-
-        parser_list = subs.add_parser("list", help="list existing observations")
-        parser_list.add_argument("--id", metavar="ID", type=int, help="list observations matching the id [int]")
-        parser_list.add_argument(
-            "--target_id", metavar="TGTID", type=int, help="list observations matching the target (pulsar) id [int]"
-        )
-        parser_list.add_argument(
-            "--pulsar", metavar="TGTNAME", type=str, nargs='+', help="list observations matching the target (pulsar) name [str]"
-        )
-        parser_list.add_argument(
-            "--telescope_id", metavar="TELID", type=int, help="list observations matching the telescope id [int]"
-        )
-        parser_list.add_argument(
-            "--telescope_name", metavar="TELNAME", type=str, help="list observations matching the telescope name [int]"
-        )
-        parser_list.add_argument(
-            "--instrumentconfig_id",
-            metavar="ICID",
-            type=int,
-            help="list observations matching the instrument_config id [int]",
-        )
-        parser_list.add_argument(
-            "--instrumentconfig_name",
-            metavar="ICNAME",
-            type=str,
-            help="list observations matching the instrument_config name [str]",
-        )
-        parser_list.add_argument(
-            "--project_id", metavar="PROJID", type=int, help="list observations matching the project id [id]"
-        )
-        parser_list.add_argument(
-            "--project_code", metavar="PROJCODE", type=str, help="list observations matching the project code [str]"
-        )
-        parser_list.add_argument(
-            "--main_project",
-            metavar="MAINPROJECT",
-            type=str,
-            default="MeerTIME",
-            help="list observations matching the mainproject [str]",
-        )
-        parser_list.add_argument(
-            "--utcs",
-            metavar="UTCGTE",
-            type=str,
-            help="list observations with utc_start greater than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
-        )
-        parser_list.add_argument(
-            "--utce",
-            metavar="UTCLET",
-            type=str,
-            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
-        )
-        parser_list.add_argument(
-            "--obs_type",
-            metavar="OBSTYPE",
-            type=str,
-            help="An observation type from fold, search and cal",
-        )
-        parser_list.add_argument(
-            "--unprocessed",
-            action='store_true',
-            default=None,
-            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
-        )
-        parser_list.add_argument(
-            "--incomplete",
-            action='store_true',
-            default=None,
-            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
-        )
-
-        parser_download = subs.add_parser("download", help="download a csv with can be input to meerpipe based on the following filters")
-        parser_download.add_argument("--id", metavar="ID", type=int, help="list observations matching the id [int]")
-        parser_download.add_argument(
-            "--target_id", metavar="TGTID", type=int, help="list observations matching the target (pulsar) id [int]"
-        )
-        parser_download.add_argument(
-            "--pulsar", metavar="TGTNAME", type=str, nargs='+', help="list observations matching the target (pulsar) name [str]"
-        )
-        parser_download.add_argument(
-            "--telescope_id", metavar="TELID", type=int, help="list observations matching the telescope id [int]"
-        )
-        parser_download.add_argument(
-            "--telescope_name", metavar="TELNAME", type=str, help="list observations matching the telescope name [int]"
-        )
-        parser_download.add_argument(
-            "--instrumentconfig_id",
-            metavar="ICID",
-            type=int,
-            help="list observations matching the instrument_config id [int]",
-        )
-        parser_download.add_argument(
-            "--instrumentconfig_name",
-            metavar="ICNAME",
-            type=str,
-            help="list observations matching the instrument_config name [str]",
-        )
-        parser_download.add_argument(
-            "--project_id", metavar="PROJID", type=int, help="list observations matching the project id [id]"
-        )
-        parser_download.add_argument(
-            "--project_code", metavar="PROJCODE", type=str, help="list observations matching the project code [str]"
-        )
-        parser_download.add_argument(
-            "--main_project",
-            metavar="MAINPROJECT",
-            type=str,
-            default="MeerTIME",
-            help="list observations matching the mainproject [str]"
-        )
-        parser_download.add_argument(
-            "--utcs",
-            metavar="UTCGTE",
-            type=str,
-            help="list observations with utc_start greater than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
-        )
-        parser_download.add_argument(
-            "--utce",
-            metavar="UTCLET",
-            type=str,
-            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
-        )
-        parser_download.add_argument(
-            "--obs_type",
-            metavar="OBSTYPE",
-            type=str,
-            default="fold",
-            help="An observation type from fold, search and cal",
-        )
-        parser_download.add_argument(
-            "--unprocessed",
-            action='store_true',
-            default=None,
-            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
-        )
-        parser_download.add_argument(
-            "--incomplete",
-            action='store_true',
-            default=None,
-            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
-        )
-
-
+from datetime import datetime
+
+from psrdb.graphql_table import GraphQLTable
+from psrdb.utils.other import decode_id
+
+
+def get_parsers():
+    """Returns the default parser for this model"""
+    parser = GraphQLTable.get_default_parser("The following options will allow you to interact with the Observation database object on the command line in different ways based on the sub-commands.")
+    Observation.configure_parsers(parser)
+    return parser
+
+
+class Observation(GraphQLTable):
+    """Class for interacting with the Observation database object.
+
+    Parameters
+    ----------
+    client : GraphQLClient
+        GraphQLClient class instance with the URL and Token already set.
+    """
+    def __init__(self, client, logger=None):
+        GraphQLTable.__init__(self, client, logger)
+        self.table_name = "observation"
+        self.field_names = [
+            "id",
+            "pulsar { name }",
+            "calibration { id }",
+            "calibration { location }",
+            "telescope { name }",
+            "project { code }",
+            "project { short }",
+            "utcStart",
+            "beam",
+            "band",
+            "duration",
+            "foldNchan",
+            "foldNbin",
+            "modeDuration"
+        ]
+
+    def list(
+        self,
+        id=None,
+        pulsar_name=None,
+        telescope_name=None,
+        project_id=None,
+        project_short=None,
+        main_project="All",
+        utcs=None,
+        utce=None,
+        obs_type='fold',
+        unprocessed=None,
+        incomplete=None,
+    ):
+        """Return a list of Observation information based on the `self.field_names` and filtered by the parameters.
+
+        Parameters
+        ----------
+        id : int, optional
+            Filter by the database ID, by default None
+        pulsar_name : str, optional
+            Filter by the pulsar name, by default None
+        telescope_name : str, optional
+            Filter by the telescope name, by default None
+        project_id : int, optional
+            Filter by the project id, by default None
+        project_short : str, optional
+            Filter by the project short name, by default None
+        utcs : str, optional
+            Filter by the utc start time greater than or equal to the timestamp in the format YYYY-MM-DDTHH:MM:SS+00:00, by default None
+        utce : str, optional
+            Filter by the utc start time less than or equal to the timestamp in the format YYYY-MM-DDTHH:MM:SS+00:00, by default None
+        obs_type : str, optional
+            Filter by the observation type (fold, search or cal), by default 'fold'
+        unprocessed : str, optional
+            Filter to only returned unprocessed observations (no PulsarFoldResult)
+        incomplete : str, optional
+            Filter to only return incomplete observations (most recent job run is not "Completed)
+
+        Returns
+        -------
+        list of dicts
+            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
+        client_response:
+            Else a client response object.
+        """
+        # Convert dates to correct format
+        if utcs == "":
+            utcs = None
+        elif utcs is not None:
+            d = datetime.strptime(utcs, '%Y-%m-%d-%H:%M:%S')
+            utcs = f"{d.date()}T{d.time()}+00:00"
+        if utce == "":
+            utce = None
+        elif utce is not None:
+            d = datetime.strptime(utce, '%Y-%m-%d-%H:%M:%S')
+            utce = f"{d.date()}T{d.time()}+00:00"
+        if project_short == "":
+            project_short = None
+        if pulsar_name == "":
+            pulsar_name = None
+        """Return a list of records matching the id and/or any of the arguments."""
+        filters = [
+            {"field": "id", "value": id},
+            {"field": "pulsar_Name", "value": pulsar_name},
+            {"field": "telescope_Name", "value": telescope_name},
+            {"field": "project_Id", "value": project_id},
+            {"field": "project_Short", "value": project_short},
+            {"field": "mainProject", "value": main_project},
+            {"field": "utcStartGte", "value": utcs},
+            {"field": "utcStartLte", "value": utce},
+            {"field": "obsType", "value": obs_type},
+        ]
+        if unprocessed is not None:
+            filters.append({"field": "unprocessed", "value": unprocessed})
+        if incomplete is not None:
+            filters.append({"field": "incomplete", "value": incomplete})
+        return GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
+
+    def download(
+        self,
+        id=None,
+        pulsar_name=None,
+        telescope_name=None,
+        project_id=None,
+        project_short=None,
+        main_project="meertime",
+        utcs=None,
+        utce=None,
+        obs_type='fold',
+        unprocessed=None,
+        incomplete=None,
+    ):
+        """Return a list of Observation information based on the `self.field_names` and filtered by the parameters.
+
+        Parameters
+        ----------
+        id : int, optional
+            Filter by the database ID, by default None
+        pulsar_name : str, optional
+            Filter by the pulsar name, by default None
+        telescope_name : str, optional
+            Filter by the telescope name, by default None
+        project_id : int, optional
+            Filter by the project id, by default None
+        project_short : str, optional
+            Filter by the project short name, by default None
+        utcs : str, optional
+            Filter by the utc start time greater than or equal to the timestamp in the format YYYY-MM-DDTHH:MM:SS+00:00, by default None
+        utce : str, optional
+            Filter by the utc start time less than or equal to the timestamp in the format YYYY-MM-DDTHH:MM:SS+00:00, by default None
+        obs_type : str, optional
+            Filter by the observation type (fold, search or cal), by default 'fold'
+        unprocessed : str, optional
+            Filter to only returned unprocessed observations (no PulsarFoldResult)
+        incomplete : str, optional
+            Filter to only return incomplete observations (most recent job run is not "Completed)
+
+        Returns
+        -------
+        list of dicts
+            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
+        client_response:
+            Else a client response object.
+        """
+        # Convert dates to correct format
+        if utcs == "":
+            utcs = None
+        elif utcs is not None:
+            d = datetime.strptime(utcs, '%Y-%m-%d-%H:%M:%S')
+            utcs = f"{d.date()}T{d.time()}+00:00"
+        if utce == "":
+            utce = None
+        elif utce is not None:
+            d = datetime.strptime(utce, '%Y-%m-%d-%H:%M:%S')
+            utce = f"{d.date()}T{d.time()}+00:00"
+        if project_short == "":
+            project_short = None
+        if pulsar_name == "":
+            pulsar_name = None
+        """Return a list of records matching the id and/or any of the arguments."""
+        filters = [
+            {"field": "id", "value": id},
+            {"field": "pulsar_Name", "value": pulsar_name},
+            {"field": "telescope_Name", "value": telescope_name},
+            {"field": "project_Id", "value": project_id},
+            {"field": "project_Short", "value": project_short},
+            {"field": "mainProject", "value": main_project},
+            {"field": "utcStartGte", "value": utcs},
+            {"field": "utcStartLte", "value": utce},
+            {"field": "obsType", "value": obs_type},
+        ]
+        if unprocessed is not None:
+            filters.append({"field": "unprocessed", "value": unprocessed})
+        if incomplete is not None:
+            filters.append({"field": "incomplete", "value": incomplete})
+
+        self.get_dicts = True
+        observations_dicts = GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
+
+        # Create the output name
+        output_name = "observations"
+        if main_project:
+            output_name += f"_{main_project}"
+        if pulsar_name:
+            output_name += f"_{'_'.join(pulsar_name)}"
+        if telescope_name:
+            output_name += f"_{telescope_name}"
+        if project_id:
+            output_name += f"_{project_id}"
+        if project_short:
+            output_name += f"_{project_short}"
+        if utcs:
+            output_name += f"_utcs{utcs}"
+        if utce:
+            output_name += f"_utce{utce}"
+        if obs_type:
+            output_name += f"_{obs_type}"
+        if unprocessed:
+            output_name += "_unprocessed"
+        if incomplete:
+            output_name += "_incomplete"
+        output_name += ".csv"
+
+        # Loop over the pulsar_fold_results and dump them as a file
+        with open(output_name, "w") as f:
+            f.write("Obs ID,Pulsar Jname,UTC Start,Project Short Name,Beam #,Observing Band,Duration (s),Mode Duration (s),Nchan,Nbin,Calibration Location\n")
+            for observations_dict in observations_dicts:
+                data_line = [
+                    str(decode_id(observations_dict["id"])),
+                    str(observations_dict["pulsar"]["name"]),
+                    str(datetime.strptime(observations_dict['utcStart'], '%Y-%m-%dT%H:%M:%S+00:00').strftime('%Y-%m-%d-%H:%M:%S')),
+                    str(observations_dict["project"]["short"]),
+                    str(observations_dict["beam"]),
+                    str(observations_dict["band"]),
+                    str(observations_dict["duration"]),
+                    str(observations_dict["modeDuration"]),
+                    str(observations_dict["foldNchan"]),
+                    str(observations_dict["foldNbin"]),
+                    str(observations_dict["calibration"]["location"]),
+                ]
+                f.write(f"{','.join(data_line)}\n")
+        return output_name
+
+    def create(
+        self,
+        pulsarName,
+        telescopeName,
+        projectCode,
+        calibrationId,
+        ephemerisText,
+        frequency,
+        bandwidth,
+        nchan,
+        beam,
+        nant,
+        nantEff,
+        npol,
+        obsType,
+        utcStart,
+        raj,
+        decj,
+        duration,
+        nbit,
+        tsamp,
+        foldNbin,
+        foldNchan,
+        foldTsubint,
+        filterbankNbit,
+        filterbankNpol,
+        filterbankNchan,
+        filterbankTsamp,
+        filterbankDm,
+    ):
+        """Create a new Observation database object.
+
+        Parameters
+        ----------
+        pulsarName : str
+            The pulsar name.
+        telescopeName : str
+            The telescope name.
+        projectCode : str
+            The project code.
+        calibrationId : int
+            The ID of the Calibration database object.
+        ephemerisText : str
+            The ephemeris text as a single string (includes new line characters).
+        frequency : float
+            The frequency of the observation in MHz.
+        bandwidth : float
+            The bandwidth of the observation in MHz.
+        nchan : int
+            The number of frequency channels.
+        beam : int
+            The beam number.
+        nant : int
+            The number of antennas used in the observation.
+        nantEff : int
+            The effective number of antennas used in the observation.
+        npol : int
+            The number of polarisations.
+        obsType : str
+            The type of observation (fold, search or cal).
+        utcStart : `datetime`
+            The UTC start time of the observation as a `datetime` object.
+        raj : str
+            The right ascension of the observation in HH:MM:SS.SS format.
+        decj : str
+            The declination of the observation in DD:MM:SS.SS format.
+        duration : float
+            The duration of the observation in seconds.
+        nbit : int
+            The number of bits per sample.
+        tsamp : float
+            The sampling time in microseconds.
+        foldNbin : int
+            The number of bins in the folded data (None for non fold observations).
+        foldNchan : int
+            The number of frequency channels in the folded data (None for non fold observations).
+        foldTsubint : int
+            The number of time samples in each sub-integration of the folded data (None for non fold observations).
+        filterbankNbit : int
+            The number of bits per sample in the filterbank data (None for non search observations).
+        filterbankNpol : int
+            The number of polarisations in the filterbank data (None for non search observations).
+        filterbankNchan : int
+            The number of frequency channels in the filterbank data (None for non search observations).
+        filterbankTsamp : float
+            The sampling time in microseconds in the filterbank data (None for non search observations).
+        filterbankDm : float
+            The dispersion measure in the filterbank data (None for non search observations).
+
+        Returns
+        -------
+        client_response:
+            A client response object.
+        """
+        # create a new record
+        self.mutation_name = "createObservation"
+        self.mutation = """
+        mutation (
+            $pulsarName: String!,
+            $telescopeName: String!,
+            $projectCode: String!,
+            $calibrationId: Int!,
+            $frequency: Float!,
+            $bandwidth: Float!,
+            $nchan: Int!,
+            $beam: Int!,
+            $nant: Int!,
+            $nantEff: Int!,
+            $npol: Int!,
+            $obsType: String!,
+            $utcStart: DateTime!,
+            $raj: String!,
+            $decj: String!,
+            $duration: Float!,
+            $nbit: Int!,
+            $tsamp: Float!,
+            # Fold options
+            $ephemerisText: String,
+            $foldNbin: Int,
+            $foldNchan: Int,
+            $foldTsubint: Int,
+            # Search options
+            $filterbankNbit: Int,
+            $filterbankNpol: Int,
+            $filterbankNchan: Int,
+            $filterbankTsamp: Float,
+            $filterbankDm: Float,
+        ) {
+            createObservation(input: {
+                pulsarName: $pulsarName,
+                telescopeName: $telescopeName,
+                projectCode: $projectCode,
+                calibrationId: $calibrationId,
+                frequency: $frequency,
+                bandwidth: $bandwidth,
+                nchan: $nchan,
+                beam: $beam,
+                nant: $nant,
+                nantEff: $nantEff,
+                npol: $npol,
+                obsType: $obsType,
+                utcStart: $utcStart,
+                raj: $raj,
+                decj: $decj,
+                duration: $duration,
+                nbit: $nbit,
+                tsamp: $tsamp,
+                ephemerisText: $ephemerisText,
+                foldNbin: $foldNbin,
+                foldNchan: $foldNchan,
+                foldTsubint: $foldTsubint,
+                filterbankNbit: $filterbankNbit,
+                filterbankNpol: $filterbankNpol,
+                filterbankNchan: $filterbankNchan,
+                filterbankTsamp: $filterbankTsamp,
+                filterbankDm: $filterbankDm,
+            }) {
+                observation {
+                    id
+                }
+            }
+        }
+        """
+        self.variables = {
+            "pulsarName": pulsarName,
+            "telescopeName": telescopeName,
+            "projectCode": projectCode,
+            "calibrationId": calibrationId,
+            "ephemerisText": ephemerisText,
+            "frequency": frequency,
+            "bandwidth": bandwidth,
+            "nchan": nchan,
+            "beam": beam,
+            "nant": nant,
+            "nantEff": nantEff,
+            "npol": npol,
+            "obsType": obsType,
+            "utcStart": utcStart,
+            "raj": raj,
+            "decj": decj,
+            "duration": duration,
+            "nbit": nbit,
+            "tsamp": tsamp,
+            "foldNbin": foldNbin,
+            "foldNchan": foldNchan,
+            "foldTsubint": foldTsubint,
+            "filterbankNbit": filterbankNbit,
+            "filterbankNpol": filterbankNpol,
+            "filterbankNchan": filterbankNchan,
+            "filterbankTsamp": filterbankTsamp,
+            "filterbankDm": filterbankDm,
+        }
+        return self.mutation_graphql()
+
+    def update(
+        self,
+        id,
+        pulsarName,
+        telescopeName,
+        projectCode,
+        calibrationId,
+        ephemerisText,
+        frequency,
+        bandwidth,
+        nchan,
+        beam,
+        nant,
+        nantEff,
+        npol,
+        obsType,
+        utcStart,
+        raj,
+        decj,
+        duration,
+        nbit,
+        tsamp,
+        foldNbin,
+        foldNchan,
+        foldTsubint,
+        filterbankNbit,
+        filterbankNpol,
+        filterbankNchan,
+        filterbankTsamp,
+        filterbankDm,
+    ):
+        """Update a Observation database object.
+
+        Parameters
+        ----------
+        id : int
+            The database ID
+        pulsarName : str
+            The pulsar name.
+        telescopeName : str
+            The telescope name.
+        projectCode : str
+            The project code.
+        calibrationId : int
+            The ID of the Calibration database object.
+        ephemerisText : str
+            The ephemeris text as a single string (includes new line characters).
+        frequency : float
+            The frequency of the observation in MHz.
+        bandwidth : float
+            The bandwidth of the observation in MHz.
+        nchan : int
+            The number of frequency channels.
+        beam : int
+            The beam number.
+        nant : int
+            The number of antennas used in the observation.
+        nantEff : int
+            The effective number of antennas used in the observation.
+        npol : int
+            The number of polarisations.
+        obsType : str
+            The type of observation (fold, search or cal).
+        utcStart : `datetime`
+            The UTC start time of the observation as a `datetime` object.
+        raj : str
+            The right ascension of the observation in HH:MM:SS.SS format.
+        decj : str
+            The declination of the observation in DD:MM:SS.SS format.
+        duration : float
+            The duration of the observation in seconds.
+        nbit : int
+            The number of bits per sample.
+        tsamp : float
+            The sampling time in microseconds.
+        foldNbin : int
+            The number of bins in the folded data (None for non fold observations).
+        foldNchan : int
+            The number of frequency channels in the folded data (None for non fold observations).
+        foldTsubint : int
+            The number of time samples in each sub-integration of the folded data (None for non fold observations).
+        filterbankNbit : int
+            The number of bits per sample in the filterbank data (None for non search observations).
+        filterbankNpol : int
+            The number of polarisations in the filterbank data (None for non search observations).
+        filterbankNchan : int
+            The number of frequency channels in the filterbank data (None for non search observations).
+        filterbankTsamp : float
+            The sampling time in microseconds in the filterbank data (None for non search observations).
+        filterbankDm : float
+            The dispersion measure in the filterbank data (None for non search observations).
+
+
+        Returns
+        -------
+        client_response:
+            A client response object.
+        """
+        self.mutation_name = "updateObservation"
+        self.mutation = """
+        mutation (
+            $id: Int!,
+            $pulsarName: String!,
+            $telescopeName: String!,
+            $projectCode: String!,
+            $calibrationId: Int!,
+            $frequency: Float!,
+            $bandwidth: Float!,
+            $nchan: Int!,
+            $beam: Int!,
+            $nant: Int!,
+            $nantEff: Int!,
+            $npol: Int!,
+            $obsType: String!,
+            $utcStart: DateTime!,
+            $raj: String!,
+            $decj: String!,
+            $duration: Float!,
+            $nbit: Int!,
+            $tsamp: Float!,
+            # Fold options
+            $ephemerisText: String,
+            $foldNbin: Int,
+            $foldNchan: Int,
+            $foldTsubint: Int,
+            # Search options
+            $filterbankNbit: Int,
+            $filterbankNpol: Int,
+            $filterbankNchan: Int,
+            $filterbankTsamp: Float,
+            $filterbankDm: Float,
+        ) {
+            updateObservation(input: {
+                id: $id,
+                pulsarName: $pulsarName,
+                telescopeName: $telescopeName,
+                projectCode: $projectCode,
+                calibrationId: $calibrationId,
+                frequency: $frequency,
+                bandwidth: $bandwidth,
+                nchan: $nchan,
+                beam: $beam,
+                nant: $nant,
+                nantEff: $nantEff,
+                npol: $npol,
+                obsType: $obsType,
+                utcStart: $utcStart,
+                raj: $raj,
+                decj: $decj,
+                duration: $duration,
+                nbit: $nbit,
+                tsamp: $tsamp,
+                ephemerisText: $ephemerisText,
+                foldNbin: $foldNbin,
+                foldNchan: $foldNchan,
+                foldTsubint: $foldTsubint,
+                filterbankNbit: $filterbankNbit,
+                filterbankNpol: $filterbankNpol,
+                filterbankNchan: $filterbankNchan,
+                filterbankTsamp: $filterbankTsamp,
+                filterbankDm: $filterbankDm,
+            }) {
+                observation {
+                    id
+                }
+            }
+        }
+        """
+        self.variables = {
+            "id": id,
+            "pulsarName": pulsarName,
+            "telescopeName": telescopeName,
+            "projectCode": projectCode,
+            "calibrationId": calibrationId,
+            "ephemerisText": ephemerisText,
+            "frequency": frequency,
+            "bandwidth": bandwidth,
+            "nchan": nchan,
+            "beam": beam,
+            "nant": nant,
+            "nantEff": nantEff,
+            "npol": npol,
+            "obsType": obsType,
+            "utcStart": utcStart,
+            "raj": raj,
+            "decj": decj,
+            "duration": duration,
+            "nbit": nbit,
+            "tsamp": tsamp,
+            "foldNbin": foldNbin,
+            "foldNchan": foldNchan,
+            "foldTsubint": foldTsubint,
+            "filterbankNbit": filterbankNbit,
+            "filterbankNpol": filterbankNpol,
+            "filterbankNchan": filterbankNchan,
+            "filterbankTsamp": filterbankTsamp,
+            "filterbankDm": filterbankDm,
+        }
+        return self.mutation_graphql()
+
+    def delete(self, id):
+        """Delete a Observation database object.
+
+        Parameters
+        ----------
+        id : int
+            The database ID
+
+        Returns
+        -------
+        client_response:
+            A client response object.
+        """
+        self.mutation_name = "deleteObservation"
+        self.mutation = """
+        mutation ($id: Int!) {
+            deleteObservation(id: $id) {
+                ok
+            }
+        }
+        """
+        self.variables = {
+            "id": id,
+        }
+        return self.mutation_graphql()
+
+    def process(self, args):
+        """Parse the arguments collected by the CLI."""
+        self.print_stdout = True
+        if args.subcommand == "list":
+            return self.list(
+                id=args.id,
+                pulsar_name=args.pulsar,
+                telescope_name=args.telescope_name,
+                project_id=args.project_id,
+                project_short=args.project_code,
+                main_project=args.main_project,
+                utcs=args.utcs,
+                utce=args.utce,
+                obs_type=args.obs_type,
+                unprocessed=args.unprocessed,
+                incomplete=args.incomplete,
+            )
+        elif args.subcommand == "download":
+            return self.download(
+                id=args.id,
+                pulsar_name=args.pulsar,
+                telescope_name=args.telescope_name,
+                project_id=args.project_id,
+                project_short=args.project_code,
+                main_project=args.main_project,
+                utcs=args.utcs,
+                utce=args.utce,
+                obs_type=args.obs_type,
+                unprocessed=args.unprocessed,
+                incomplete=args.incomplete,
+            )
+        else:
+            raise RuntimeError(f"{args.subcommand} command is not implemented")
+
+    @classmethod
+    def get_name(cls):
+        return "observation"
+
+    @classmethod
+    def get_description(cls):
+        return "Observation details."
+
+    @classmethod
+    def get_parsers(cls):
+        """Returns the default parser for this model"""
+        parser = GraphQLTable.get_default_parser("Observations model parser")
+        cls.configure_parsers(parser)
+        return parser
+
+    @classmethod
+    def configure_parsers(cls, parser):
+        """Add sub-parsers for each of the valid commands."""
+        # create the parser for the "list" command
+        parser.set_defaults(command=cls.get_name())
+        subs = parser.add_subparsers(dest="subcommand")
+        subs.required = True
+
+        parser_list = subs.add_parser("list", help="list existing observations")
+        parser_list.add_argument("--id", metavar="ID", type=int, help="list observations matching the id [int]")
+        parser_list.add_argument(
+            "--target_id", metavar="TGTID", type=int, help="list observations matching the target (pulsar) id [int]"
+        )
+        parser_list.add_argument(
+            "--pulsar", metavar="TGTNAME", type=str, nargs='+', help="list observations matching the target (pulsar) name [str]"
+        )
+        parser_list.add_argument(
+            "--telescope_id", metavar="TELID", type=int, help="list observations matching the telescope id [int]"
+        )
+        parser_list.add_argument(
+            "--telescope_name", metavar="TELNAME", type=str, help="list observations matching the telescope name [int]"
+        )
+        parser_list.add_argument(
+            "--instrumentconfig_id",
+            metavar="ICID",
+            type=int,
+            help="list observations matching the instrument_config id [int]",
+        )
+        parser_list.add_argument(
+            "--instrumentconfig_name",
+            metavar="ICNAME",
+            type=str,
+            help="list observations matching the instrument_config name [str]",
+        )
+        parser_list.add_argument(
+            "--project_id", metavar="PROJID", type=int, help="list observations matching the project id [id]"
+        )
+        parser_list.add_argument(
+            "--project_code", metavar="PROJCODE", type=str, help="list observations matching the project code [str]"
+        )
+        parser_list.add_argument(
+            "--main_project",
+            metavar="MAINPROJECT",
+            type=str,
+            default="MeerTIME",
+            help="list observations matching the mainproject [str]",
+        )
+        parser_list.add_argument(
+            "--utcs",
+            metavar="UTCGTE",
+            type=str,
+            help="list observations with utc_start greater than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
+        )
+        parser_list.add_argument(
+            "--utce",
+            metavar="UTCLTE",
+            type=str,
+            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
+        )
+        parser_list.add_argument(
+            "--obs_type",
+            metavar="OBSTYPE",
+            type=str,
+            help="An observation type from fold, search and cal",
+        )
+        parser_list.add_argument(
+            "--unprocessed",
+            action='store_true',
+            default=None,
+            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
+        )
+        parser_list.add_argument(
+            "--incomplete",
+            action='store_true',
+            default=None,
+            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
+        )
+
+        parser_download = subs.add_parser("download", help="download a csv with can be input to meerpipe based on the following filters")
+        parser_download.add_argument("--id", metavar="ID", type=int, help="list observations matching the id [int]")
+        parser_download.add_argument(
+            "--target_id", metavar="TGTID", type=int, help="list observations matching the target (pulsar) id [int]"
+        )
+        parser_download.add_argument(
+            "--pulsar", metavar="TGTNAME", type=str, nargs='+', help="list observations matching the target (pulsar) name [str]"
+        )
+        parser_download.add_argument(
+            "--telescope_id", metavar="TELID", type=int, help="list observations matching the telescope id [int]"
+        )
+        parser_download.add_argument(
+            "--telescope_name", metavar="TELNAME", type=str, help="list observations matching the telescope name [int]"
+        )
+        parser_download.add_argument(
+            "--instrumentconfig_id",
+            metavar="ICID",
+            type=int,
+            help="list observations matching the instrument_config id [int]",
+        )
+        parser_download.add_argument(
+            "--instrumentconfig_name",
+            metavar="ICNAME",
+            type=str,
+            help="list observations matching the instrument_config name [str]",
+        )
+        parser_download.add_argument(
+            "--project_id", metavar="PROJID", type=int, help="list observations matching the project id [id]"
+        )
+        parser_download.add_argument(
+            "--project_code", metavar="PROJCODE", type=str, help="list observations matching the project code [str]"
+        )
+        parser_download.add_argument(
+            "--main_project",
+            metavar="MAINPROJECT",
+            type=str,
+            default="MeerTIME",
+            help="list observations matching the mainproject [str]"
+        )
+        parser_download.add_argument(
+            "--utcs",
+            metavar="UTCGTE",
+            type=str,
+            help="list observations with utc_start greater than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
+        )
+        parser_download.add_argument(
+            "--utce",
+            metavar="UTCLTE",
+            type=str,
+            help="list observations with utc_start less than or equal to the timestamp [YYYY-MM-DDTHH:MM:SS+HH:MM]",
+        )
+        parser_download.add_argument(
+            "--obs_type",
+            metavar="OBSTYPE",
+            type=str,
+            default="fold",
+            help="An observation type from fold, search and cal",
+        )
+        parser_download.add_argument(
+            "--unprocessed",
+            action='store_true',
+            default=None,
+            help="Filter to only returned unprocessed observations (no PulsarFoldResult)",
+        )
+        parser_download.add_argument(
+            "--incomplete",
+            action='store_true',
+            default=None,
+            help='Filter to only return incomplete observations (most recent job run is not "Completed"',
+        )
+
+
```

### Comparing `psrdb-3.0.5/psrdb/tables/pipeline_image.py` & `psrdb-3.0.6/psrdb/tables/pipeline_image.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/tables/pipeline_run.py` & `psrdb-3.0.6/psrdb/tables/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/tables/project.py` & `psrdb-3.0.6/psrdb/tables/project.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/tables/pulsar.py` & `psrdb-3.0.6/psrdb/tables/pulsar.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/tables/pulsar_fold_result.py` & `psrdb-3.0.6/psrdb/tables/pulsar_fold_result.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,182 +1,223 @@
-from psrdb.graphql_table import GraphQLTable
-
-
-def get_parsers():
-    """Returns the default parser for this model"""
-    parser = GraphQLTable.get_default_parser("The following options will allow you to interact with the PulsarFoldResult database object on the command line in different ways based on the sub-commands.")
-    PulsarFoldResult.configure_parsers(parser)
-    return parser
-
-
-class PulsarFoldResult(GraphQLTable):
-    """Class for interacting with the PulsarFoldResult database object.
-
-    Parameters
-    ----------
-    client : GraphQLClient
-        GraphQLClient class instance with the URL and Token already set.
-    """
-    def __init__(self, client):
-        GraphQLTable.__init__(self, client)
-        self.table_name = "pulsar_fold_result"
-        self.field_names = [
-            "id",
-            "observation { utcStart }",
-            "observation { band }",
-            "observation { duration }",
-            "pipelineRun { id }",
-            "pipelineRun { dm }",
-            "pipelineRun { dmErr }",
-            "pipelineRun { dmEpoch }",
-            "pipelineRun { dmEpoch }",
-            "pipelineRun { dmChi2r }",
-            "pipelineRun { dmTres }",
-            "pipelineRun { sn }",
-            "pipelineRun { flux }",
-            "pipelineRun { rm }",
-            "pipelineRun { rmErr }",
-            "pipelineRun { percentRfiZapped }",
-        ]
-
-    def list(
-            self,
-            pulsar=None,
-            mainProject=None,
-            utcStart=None,
-            beam=None
-        ):
-        """Return a list of PulsarFoldResult information based on the `self.field_names` and filtered by the parameters.
-
-        Parameters
-        ----------
-        pulsar : str, optional
-            Filter by the pulsar name, by default None
-        mainProject : str, optional
-            Filter by the main project name, by default None
-        utcStart : str, optional
-            Filter by the utcStart, by default None
-        beam : int, optional
-            Filter by the beam number, by default None
-
-        Returns
-        -------
-        list of dicts
-            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
-        client_response:
-            Else a client response object.
-        """
-        filters = [
-            {"field": "pulsar", "value": pulsar},
-            {"field": "mainProject", "value": mainProject},
-            {"field": "utcStart", "value": utcStart},
-            {"field": "beam", "value": beam},
-        ]
-        return GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
-
-    def download(
-            self,
-            pulsar,
-            mainProject=None,
-            utcStart=None,
-            beam=None
-        ):
-        # Grab a dictionary of the pulsar_fold_results
-        filters = [
-            {"field": "pulsar", "value": pulsar},
-            {"field": "mainProject", "value": mainProject},
-            {"field": "utcStart", "value": utcStart},
-            {"field": "beam", "value": beam},
-        ]
-        self.get_dicts = True
-        pulsar_fold_result_dicts = GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
-
-        # Create the output name
-        output_name = f"pulsar_fold_result_{pulsar}"
-        if mainProject is not None and mainProject:
-            output_name += f"_{mainProject}"
-        if utcStart is not None and utcStart:
-            output_name += f"_{utcStart}"
-        if beam is not None and beam:
-            output_name += f"_beam{beam}"
-        output_name += ".csv"
-
-        # Loop over the pulsar_fold_results and dump them as a file
-        with open(output_name, "w") as f:
-            f.write("ID,UTC Start,Observing band,Duration (s),DM (pc cm^-3),DM error (pc cm^-3),DM epoch (MJD),DM chi2r,DM tres,SN,Flux (mJy),RM (rad m^-2),RM error (rad m^-2),RFI zapped (%)\n")
-            for pulsar_fold_result_dict in pulsar_fold_result_dicts:
-                data_line = [
-                    str(pulsar_fold_result_dict["id"]),
-                    str(pulsar_fold_result_dict["observation"]["utcStart"]),
-                    str(pulsar_fold_result_dict["observation"]["band"]),
-                    str(pulsar_fold_result_dict["observation"]["duration"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["dm"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["dmErr"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["dmEpoch"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["dmChi2r"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["dmTres"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["sn"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["flux"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["rm"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["rmErr"]),
-                    str(pulsar_fold_result_dict["pipelineRun"]["percentRfiZapped"]),
-                ]
-                f.write(f"{','.join(data_line)}\n")
-        return output_name
-
-
-    def process(self, args):
-        """Parse the arguments collected by the CLI."""
-        self.print_stdout = True
-        if args.subcommand == "list":
-            return self.list(
-                args.pulsar,
-                args.mainProject,
-                args.utcStart,
-                args.beam,
-            )
-        elif args.subcommand == "download":
-            return self.download(
-                args.pulsar,
-                args.mainProject,
-                args.utcStart,
-                args.beam,
-            )
-        else:
-            raise RuntimeError(f"{args.subcommand} command is not implemented")
-
-    @classmethod
-    def get_name(cls):
-        return "pulsar_fold_result"
-
-    @classmethod
-    def get_description(cls):
-        return "A pulsar pulsar_fold_result/standard"
-
-    @classmethod
-    def get_parsers(cls):
-        """Returns the default parser for this model"""
-        parser = GraphQLTable.get_default_parser("PulsarFoldResult model parser")
-        cls.configure_parsers(parser)
-        return parser
-
-    @classmethod
-    def configure_parsers(cls, parser):
-        """Add sub-parsers for each of the valid commands."""
-        # create the parser for the "list" command
-        parser.set_defaults(command=cls.get_name())
-        subs = parser.add_subparsers(dest="subcommand")
-        subs.required = True
-
-        parser_list = subs.add_parser("list", help="list existing ephemerides")
-        parser_list.add_argument("--pulsar", type=str, help="Name of the pulsar [str]")
-        parser_list.add_argument("--mainProject", type=str, help="Name of the main project you want to filter pulsar_fold_results by [str]")
-        parser_list.add_argument("--utcStart",  type=str, help="UTC start time you want the results of [str]")
-        parser_list.add_argument("--beam", type=int, help="Beam number you want to filter pulsar_fold_results by [int]")
-
-        # create the parser for the "download" command
-        parser_download = subs.add_parser("download", help="Download TOAs for a pulsar to a .tim file")
-        parser_download.add_argument("pulsar", type=str, help="Name of the pulsar [str]")
-        parser_download.add_argument("--mainProject", type=str, help="Name of the main project you want to filter pulsar_fold_results by [str]")
-        parser_download.add_argument("--utcStart",  type=str, help="UTC start time you want the results of [str]")
-        parser_download.add_argument("--beam", type=int, help="Beam number you want to filter pulsar_fold_results by [int]")
-
+from datetime import datetime
+
+from psrdb.graphql_table import GraphQLTable
+from psrdb.load_data import EXCLUDE_BADGES_CHOICES
+
+
+def get_parsers():
+    """Returns the default parser for this model"""
+    parser = GraphQLTable.get_default_parser("The following options will allow you to interact with the PulsarFoldResult database object on the command line in different ways based on the sub-commands.")
+    PulsarFoldResult.configure_parsers(parser)
+    return parser
+
+
+class PulsarFoldResult(GraphQLTable):
+    """Class for interacting with the PulsarFoldResult database object.
+
+    Parameters
+    ----------
+    client : GraphQLClient
+        GraphQLClient class instance with the URL and Token already set.
+    """
+    def __init__(self, client):
+        GraphQLTable.__init__(self, client)
+        self.table_name = "pulsar_fold_result"
+        self.field_names = [
+            "id",
+            "observation { utcStart }",
+            "observation { band }",
+            "observation { duration }",
+            "pipelineRun { id }",
+            "pipelineRun { dm }",
+            "pipelineRun { dmErr }",
+            "pipelineRun { dmEpoch }",
+            "pipelineRun { dmEpoch }",
+            "pipelineRun { dmChi2r }",
+            "pipelineRun { dmTres }",
+            "pipelineRun { sn }",
+            "pipelineRun { flux }",
+            "pipelineRun { rm }",
+            "pipelineRun { rmErr }",
+            "pipelineRun { percentRfiZapped }",
+        ]
+
+    def list(
+            self,
+            pulsar=None,
+            mainProject=None,
+            utcStart=None,
+            beam=None,
+            utcs=None,
+            utce=None,
+        ):
+        """Return a list of PulsarFoldResult information based on the `self.field_names` and filtered by the parameters.
+
+        Parameters
+        ----------
+        pulsar : str, optional
+            Filter by the pulsar name, by default None
+        mainProject : str, optional
+            Filter by the main project name, by default None
+        utcStart : str, optional
+            Filter by the utcStart, by default None
+        beam : int, optional
+            Filter by the beam number, by default None
+
+        Returns
+        -------
+        list of dicts
+            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
+        client_response:
+            Else a client response object.
+        """
+        filters = [
+            {"field": "pulsar", "value": pulsar},
+            {"field": "mainProject", "value": mainProject},
+            {"field": "utcStart", "value": utcStart},
+            {"field": "beam", "value": beam},
+        ]
+        if utcs is not None:
+            d = datetime.strptime(utcs, '%Y-%m-%d-%H:%M:%S')
+            filters.append({"field": "utcStartGte", "value": f"{d.date()}T{d.time()}+00:00"})
+        if utce is not None:
+            d = datetime.strptime(utce, '%Y-%m-%d-%H:%M:%S')
+            filters.append({"field": "utcStartLte", "value": f"{d.date()}T{d.time()}+00:00"})
+        return GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
+
+    def download(
+            self,
+            pulsar,
+            mainProject=None,
+            utcStart=None,
+            beam=None,
+            exclude_badges=None,
+            utcs=None,
+            utce=None,
+        ):
+        # Grab a dictionary of the pulsar_fold_results
+        filters = [
+            {"field": "pulsar", "value": pulsar},
+            {"field": "mainProject", "value": mainProject},
+            {"field": "utcStart", "value": utcStart},
+            {"field": "beam", "value": beam},
+        ]
+        if exclude_badges is not None:
+            filters.append({"field": "excludeBadges", "value": exclude_badges})
+        if utcs is not None:
+            d = datetime.strptime(utcs, '%Y-%m-%d-%H:%M:%S')
+            filters.append({"field": "utcStartGte", "value": f"{d.date()}T{d.time()}+00:00"})
+        if utce is not None:
+            d = datetime.strptime(utce, '%Y-%m-%d-%H:%M:%S')
+            filters.append({"field": "utcStartLte", "value": f"{d.date()}T{d.time()}+00:00"})
+        self.get_dicts = True
+        pulsar_fold_result_dicts = GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
+
+        # Create the output name
+        output_name = f"pulsar_fold_result_{pulsar}"
+        if mainProject is not None and mainProject:
+            output_name += f"_{mainProject}"
+        if utcStart is not None and utcStart:
+            output_name += f"_{utcStart}"
+        if beam is not None and beam:
+            output_name += f"_beam{beam}"
+        output_name += ".csv"
+
+        # Loop over the pulsar_fold_results and dump them as a file
+        with open(output_name, "w") as f:
+            f.write("ID,UTC Start,Observing band,Duration (s),DM (pc cm^-3),DM error (pc cm^-3),DM epoch (MJD),DM chi2r,DM tres,SN,Flux (mJy),RM (rad m^-2),RM error (rad m^-2),RFI zapped (%)\n")
+            for pulsar_fold_result_dict in pulsar_fold_result_dicts:
+                data_line = [
+                    str(pulsar_fold_result_dict["id"]),
+                    str(pulsar_fold_result_dict["observation"]["utcStart"]),
+                    str(pulsar_fold_result_dict["observation"]["band"]),
+                    str(pulsar_fold_result_dict["observation"]["duration"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["dm"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["dmErr"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["dmEpoch"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["dmChi2r"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["dmTres"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["sn"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["flux"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["rm"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["rmErr"]),
+                    str(pulsar_fold_result_dict["pipelineRun"]["percentRfiZapped"]),
+                ]
+                f.write(f"{','.join(data_line)}\n")
+        return output_name
+
+
+    def process(self, args):
+        """Parse the arguments collected by the CLI."""
+        self.print_stdout = True
+        if args.subcommand == "list":
+            return self.list(
+                args.pulsar,
+                args.mainProject,
+                args.utcStart,
+                args.beam,
+            )
+        elif args.subcommand == "download":
+            return self.download(
+                args.pulsar,
+                args.mainProject,
+                args.utcStart,
+                args.beam,
+                args.exclude_badges,
+                args.utcs,
+                args.utce,
+            )
+        else:
+            raise RuntimeError(f"{args.subcommand} command is not implemented")
+
+    @classmethod
+    def get_name(cls):
+        return "pulsar_fold_result"
+
+    @classmethod
+    def get_description(cls):
+        return "A pulsar pulsar_fold_result/standard"
+
+    @classmethod
+    def get_parsers(cls):
+        """Returns the default parser for this model"""
+        parser = GraphQLTable.get_default_parser("PulsarFoldResult model parser")
+        cls.configure_parsers(parser)
+        return parser
+
+    @classmethod
+    def configure_parsers(cls, parser):
+        """Add sub-parsers for each of the valid commands."""
+        # create the parser for the "list" command
+        parser.set_defaults(command=cls.get_name())
+        subs = parser.add_subparsers(dest="subcommand")
+        subs.required = True
+
+        parser_list = subs.add_parser("list", help="list existing ephemerides")
+        parser_list.add_argument("--pulsar", type=str, help="Name of the pulsar [str]")
+        parser_list.add_argument("--mainProject", type=str, help="Name of the main project you want to filter pulsar_fold_results by [str]")
+        parser_list.add_argument("--utcStart",  type=str, help="UTC start time you want the results of [str]")
+        parser_list.add_argument("--beam", type=int, help="Beam number you want to filter pulsar_fold_results by [int]")
+
+        # create the parser for the "download" command
+        parser_download = subs.add_parser("download", help="Download TOAs for a pulsar to a .tim file")
+        parser_download.add_argument("pulsar", type=str, help="Name of the pulsar [str]")
+        parser_download.add_argument("--mainProject", type=str, help="Name of the main project you want to filter pulsar_fold_results by [str]")
+        parser_download.add_argument("--utcStart",  type=str, help="UTC start time you want the results of [str]")
+        parser_download.add_argument("--beam", type=int, help="Beam number you want to filter pulsar_fold_results by [int]")
+        parser_download.add_argument(
+            '--exclude_badges',
+            nargs='*',
+            choices=EXCLUDE_BADGES_CHOICES,
+            help=f'List of observation badges/flags to exclude from download ToAs. The choices are: {EXCLUDE_BADGES_CHOICES}'
+        )
+        parser_download.add_argument(
+            "--utcs",
+            type=str,
+            help="Only use observations with utc_start greater than or equal to the timestamp [YYYY-MM-DD-HH:MM:SS]",
+        )
+        parser_download.add_argument(
+            "--utce",
+            type=str,
+            help="Only use observations with utc_start less than or equal to the timestamp [YYYY-MM-DD-HH:MM:SS]",
+        )
+
```

### Comparing `psrdb-3.0.5/psrdb/tables/residual.py` & `psrdb-3.0.6/psrdb/tables/residual.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-from psrdb.graphql_table import GraphQLTable
-from psrdb.utils.residual import residual_line_to_dict
-from psrdb.utils.other import decode_id, chunk_list
-
-
-def get_parsers():
-    """Returns the default parser for this model"""
-    parser = GraphQLTable.get_default_parser("The following options will allow you to interact with the Residual database object on the command line in different ways based on the sub-commands.")
-    Residual.configure_parsers(parser)
-    return parser
-
-
-class Residual(GraphQLTable):
-    """Class for interacting with the Residual database object.
-
-    Parameters
-    ----------
-    client : GraphQLClient
-        GraphQLClient class instance with the URL and Token already set.
-    """
-    def __init__(self, client):
-        GraphQLTable.__init__(self, client)
-        self.table_name = "toa"
-        self.field_names = [
-            "id",
-            "pipelineRun{ id }",
-            "ephemeris { id }",
-            "template { id }",
-            "archive",
-            "freqMhz",
-            "mjd",
-            "mjdErr",
-            "telescope",
-            "fe",
-            "be",
-            "f",
-            "bw",
-            "tobs",
-            "tmplt",
-            "gof",
-            "nbin",
-            "nch",
-            "chan",
-            "rcvr",
-            "snr",
-            "length",
-            "subint",
-        ]
-
-    def list(
-        self,
-        pulsar,
-        project_short,
-    ):
-        """Return a list of Residual information based on the `self.field_names` and filtered by the parameters.
-
-        Parameters
-        ----------
-        id : int, optional
-            Filter by the database ID, by default None
-        pulsar : str, optional
-            Filter by the pulsar name, by default None
-        project_short : str, optional
-            Filter by the project short code, by default None
-
-        Returns
-        -------
-        list of dicts
-            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
-        client_response:
-            Else a client response object.
-        """
-        filters = [
-            {"field": "id", "value": id},
-            {"field": "pulsar_Name", "value": pulsar},
-            {"field": "projectShort", "value": project_short},
-        ]
-        return GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
-
-    def create(
-        self,
-        residual_lines,
-    ):
-        """Create a new Residual database object.
-
-        Parameters
-        ----------
-        residual_lines : list of str
-            A list of strings containing the residual lines.
-
-        Returns
-        -------
-        client_response:
-            A client response object.
-        """
-        self.mutation_name = "createResidual"
-        self.mutation = """
-        mutation (
-            $residualLines: [String]!,
-        ) {
-            createResidual (input: {
-                residualLines: $residualLines,
-            }) {
-                toa {
-                    id,
-                }
-            }
-        }
-        """
-        # Loop over the lines and grab the important info to reduce upload size
-        residual_line_info = []
-        for residual_line in residual_lines:
-            residual_line = residual_line.rstrip("\n")
-            # Loop over residual lines and turn into a dict
-            residual_dict = residual_line_to_dict(residual_line)
-            # return only important info as a comma sperated string
-            residual_line_info.append(f"{decode_id(residual_dict['id'])},{residual_dict['mjd']},{residual_dict['residual']},{residual_dict['residual_error']},{residual_dict['residual_phase']}")
-        # Upload the residuals 1000 at a time
-        responses = []
-        for residual_chunk in chunk_list(residual_line_info, 1000):
-            self.variables = {
-                'residualLines': residual_chunk,
-            }
-            responses.append(self.mutation_graphql())
-        if len(responses) == 0:
-            return None
-        else:
-            return responses[-1]
-
-    def process(self, args):
-        """Parse the arguments collected by the CLI."""
-        self.print_stdout = True
-        if args.subcommand == "create":
-            with open(args.residual_path, "r") as f:
-                residual_lines = f.readlines()
-                return self.create(
-                    residual_lines,
-                )
-        elif args.subcommand == "list":
-            return self.list(args.id, args.processing, args.folding, args.ephemeris, args.template)
-        else:
-            raise RuntimeError(f"{args.subcommand} command is not implemented")
-
-    @classmethod
-    def get_name(cls):
-        return "residual"
-
-    @classmethod
-    def get_description(cls):
-        return "A pulsar residual/standard"
-
-    @classmethod
-    def get_parsers(cls):
-        """Returns the default parser for this model"""
-        parser = GraphQLTable.get_default_parser("Residual model parser")
-        cls.configure_parsers(parser)
-        return parser
-
-    @classmethod
-    def configure_parsers(cls, parser):
-        """Add sub-parsers for each of the valid commands."""
-        # create the parser for the "list" command
-        parser.set_defaults(command=cls.get_name())
-        subs = parser.add_subparsers(dest="subcommand")
-        subs.required = True
-
-        parser_list = subs.add_parser("list", help="list existing ephemerides")
-        parser_list.add_argument("--id", metavar="ID", type=int, help="list residual matching the id [int]")
-        parser_list.add_argument(
-            "--processing", metavar="PROC", type=int, help="list residual matching the processing id [int]"
-        )
-        parser_list.add_argument("--folding", metavar="FOLD", type=int, help="list residual that used the folding id [int]")
-        parser_list.add_argument(
-            "--ephemeris", metavar="EPH", type=int, help="list residual matching the timing ephemeris id [int]"
-        )
-        parser_list.add_argument(
-            "--template", metavar="TEMPL", type=int, help="list residual matching the template id [int]"
-        )
-
-        # create the parser for the "create" command
-        parser_create = subs.add_parser("create", help="Create a new Residual")
-        parser_create.add_argument(
-            "residual_path", metavar="TOA", type=str, help="Path to the residual file [str]"
+from psrdb.graphql_table import GraphQLTable
+from psrdb.utils.residual import residual_line_to_dict
+from psrdb.utils.other import decode_id, chunk_list
+
+
+def get_parsers():
+    """Returns the default parser for this model"""
+    parser = GraphQLTable.get_default_parser("The following options will allow you to interact with the Residual database object on the command line in different ways based on the sub-commands.")
+    Residual.configure_parsers(parser)
+    return parser
+
+
+class Residual(GraphQLTable):
+    """Class for interacting with the Residual database object.
+
+    Parameters
+    ----------
+    client : GraphQLClient
+        GraphQLClient class instance with the URL and Token already set.
+    """
+    def __init__(self, client):
+        GraphQLTable.__init__(self, client)
+        self.table_name = "toa"
+        self.field_names = [
+            "id",
+            "pipelineRun{ id }",
+            "ephemeris { id }",
+            "template { id }",
+            "archive",
+            "freqMhz",
+            "mjd",
+            "mjdErr",
+            "telescope",
+            "fe",
+            "be",
+            "f",
+            "bw",
+            "tobs",
+            "tmplt",
+            "gof",
+            "nbin",
+            "nch",
+            "chan",
+            "rcvr",
+            "snr",
+            "length",
+            "subint",
+        ]
+
+    def list(
+        self,
+        pulsar,
+        project_short,
+    ):
+        """Return a list of Residual information based on the `self.field_names` and filtered by the parameters.
+
+        Parameters
+        ----------
+        id : int, optional
+            Filter by the database ID, by default None
+        pulsar : str, optional
+            Filter by the pulsar name, by default None
+        project_short : str, optional
+            Filter by the project short code, by default None
+
+        Returns
+        -------
+        list of dicts
+            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
+        client_response:
+            Else a client response object.
+        """
+        filters = [
+            {"field": "id", "value": id},
+            {"field": "pulsar_Name", "value": pulsar},
+            {"field": "projectShort", "value": project_short},
+        ]
+        return GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
+
+    def create(
+        self,
+        residual_lines,
+    ):
+        """Create a new Residual database object.
+
+        Parameters
+        ----------
+        residual_lines : list of str
+            A list of strings containing the residual lines.
+
+        Returns
+        -------
+        client_response:
+            A client response object.
+        """
+        self.mutation_name = "createResidual"
+        self.mutation = """
+        mutation (
+            $residualLines: [String]!,
+        ) {
+            createResidual (input: {
+                residualLines: $residualLines,
+            }) {
+                toa {
+                    id,
+                }
+            }
+        }
+        """
+        # Loop over the lines and grab the important info to reduce upload size
+        residual_line_info = []
+        for residual_line in residual_lines:
+            residual_line = residual_line.rstrip("\n")
+            # Loop over residual lines and turn into a dict
+            residual_dict = residual_line_to_dict(residual_line)
+            # return only important info as a comma sperated string
+            residual_line_info.append(f"{decode_id(residual_dict['id'])},{residual_dict['mjd']},{residual_dict['residual']},{residual_dict['residual_error']},{residual_dict['residual_phase']}")
+        # Upload the residuals 1000 at a time
+        responses = []
+        for residual_chunk in chunk_list(residual_line_info, 1000):
+            self.variables = {
+                'residualLines': residual_chunk,
+            }
+            responses.append(self.mutation_graphql())
+        if len(responses) == 0:
+            return None
+        else:
+            return responses[-1]
+
+    def process(self, args):
+        """Parse the arguments collected by the CLI."""
+        self.print_stdout = True
+        if args.subcommand == "create":
+            with open(args.residual_path, "r") as f:
+                residual_lines = f.readlines()
+                return self.create(
+                    residual_lines,
+                )
+        elif args.subcommand == "list":
+            return self.list(args.id, args.processing, args.folding, args.ephemeris, args.template)
+        else:
+            raise RuntimeError(f"{args.subcommand} command is not implemented")
+
+    @classmethod
+    def get_name(cls):
+        return "residual"
+
+    @classmethod
+    def get_description(cls):
+        return "A pulsar residual/standard"
+
+    @classmethod
+    def get_parsers(cls):
+        """Returns the default parser for this model"""
+        parser = GraphQLTable.get_default_parser("Residual model parser")
+        cls.configure_parsers(parser)
+        return parser
+
+    @classmethod
+    def configure_parsers(cls, parser):
+        """Add sub-parsers for each of the valid commands."""
+        # create the parser for the "list" command
+        parser.set_defaults(command=cls.get_name())
+        subs = parser.add_subparsers(dest="subcommand")
+        subs.required = True
+
+        parser_list = subs.add_parser("list", help="list existing ephemerides")
+        parser_list.add_argument("--id", metavar="ID", type=int, help="list residual matching the id [int]")
+        parser_list.add_argument(
+            "--processing", metavar="PROC", type=int, help="list residual matching the processing id [int]"
+        )
+        parser_list.add_argument("--folding", metavar="FOLD", type=int, help="list residual that used the folding id [int]")
+        parser_list.add_argument(
+            "--ephemeris", metavar="EPH", type=int, help="list residual matching the timing ephemeris id [int]"
+        )
+        parser_list.add_argument(
+            "--template", metavar="TEMPL", type=int, help="list residual matching the template id [int]"
+        )
+
+        # create the parser for the "create" command
+        parser_create = subs.add_parser("create", help="Create a new Residual")
+        parser_create.add_argument(
+            "residual_path", metavar="TOA", type=str, help="Path to the residual file [str]"
         )
```

### Comparing `psrdb-3.0.5/psrdb/tables/telescope.py` & `psrdb-3.0.6/psrdb/tables/telescope.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/tables/toa.py` & `psrdb-3.0.6/psrdb/tables/toa.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,432 +1,447 @@
-from psrdb.graphql_table import GraphQLTable
-from psrdb.utils.toa import toa_dict_to_line
-from psrdb.utils.other import chunk_list
-
-
-def get_parsers():
-    """Returns the default parser for this model"""
-    parser = GraphQLTable.get_default_parser("The following options will allow you to interact with the Toa database object on the command line in different ways based on the sub-commands.")
-    Toa.configure_parsers(parser)
-    return parser
-
-
-class Toa(GraphQLTable):
-    """Class for interacting with the Toa database object.
-
-    Parameters
-    ----------
-    client : GraphQLClient
-        GraphQLClient class instance with the URL and Token already set.
-    """
-    def __init__(self, client):
-        GraphQLTable.__init__(self, client)
-        self.table_name = "toa"
-
-        self.field_names = [
-            "id",
-            "pipelineRun{ id }",
-            "ephemeris { id }",
-            "template { id }",
-            "archive",
-            "freqMhz",
-            "mjd",
-            "mjdErr",
-            "telescope",
-            "fe",
-            "be",
-            "f",
-            "bw",
-            "tobs",
-            "tmplt",
-            "gof",
-            "nbin",
-            "nch",
-            "chan",
-            "rcvr",
-            "snr",
-            "length",
-            "subint",
-        ]
-
-    def list(
-        self,
-        id=None,
-        pulsar=None,
-        pipeline_run_id=None,
-        project_short=None,
-        dm_corrected=None,
-        minimum_nsubs=None,
-        maximum_nsubs=None,
-        obs_nchan=None,
-    ):
-        """Return a list of Toa information based on the `self.field_names` and filtered by the parameters.
-
-        Parameters
-        ----------
-        id : int, optional
-            Filter by the database ID, by default None
-        pulsar : str, optional
-            Filter by the pulsar name, by default None
-        pipeline_run_id : int, optional
-            Filter by the pipeline run id, by default None
-        project_short : str
-            The project short name (e.g PTA).
-        dm_corrected : bool, optional
-            Filter by if the toa was DM corrected, by default None
-        minimum_nsubs : bool, optional
-            Filter by if the toa was generated with the minimum number of time subbands, by default None
-        maximum_nsubs : bool, optional
-            Filter by if the toa was generated with the maximum number of time subbands, by default None
-        obs_nchan : int, optional
-            Filter by the number of channels, by default None
-
-        Returns
-        -------
-        list of dicts
-            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
-        client_response:
-            Else a client response object.
-        """
-        filters = [
-            {"field": "id", "value": id},
-            {"field": "pulsar", "value": pulsar},
-            {"field": "pipelineRunId", "value": pipeline_run_id},
-            {"field": "projectShort", "value": project_short},
-            {"field": "dmCorrected", "value": dm_corrected},
-            {"field": "obsNchan", "value": obs_nchan},
-        ]
-        if minimum_nsubs:
-            filters.append({"field": "minimumNsubs", "value": minimum_nsubs})
-        if maximum_nsubs:
-            filters.append({"field": "maximumNsubs", "value": maximum_nsubs})
-        return GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
-
-    def create(
-        self,
-        pipeline_run_id,
-        project_short,
-        ephemeris,
-        template_id,
-        toa_lines,
-        dmCorrected=False,
-        minimumNsubs=False,
-        maximumNsubs=False,
-        allNsubs=False,
-        modeNsubs=False,
-        npol=1,
-        nchan=1,
-    ):
-        """Create a new Toa database object.
-
-        Parameters
-        ----------
-        pipeline_run_id : int
-            The ID of the PipelineRun database object for this Toa.
-        project_short : str
-            The project short name (e.g PTA).
-        ephemeris : str
-            The path to the ephemeris file used to create the residuals.
-        template_id : int
-            The ID of the Template database object for this Toa.
-        toa_lines : list
-            A list containing the toa lines.
-        dmCorrected : bool
-            If the toa was DM corrected.
-        minimumNsubs : bool
-            If the toa was generated with the minimum number of time subbands.
-        maximumNsubs : bool
-            If the toa was generated with the maximum number of time subbands.
-        npol : int
-            The number of Stokes polarisations.
-        nchan : int
-            The number of frequency channels.
-
-        Returns
-        -------
-        client_response:
-            A client response object.
-        """
-        self.mutation_name = "createToa"
-        self.mutation = """
-        mutation (
-            $pipelineRunId: Int!,
-            $projectShort: String!,
-            $templateId: Int!,
-            $ephemerisText: String!,
-            $toaLines: [String]!,
-            $dmCorrected: Boolean!,
-            $minimumNsubs: Boolean!,
-            $maximumNsubs: Boolean!,
-            $allNsubs: Boolean!,
-            $modeNsubs: Boolean!,
-            $obsNpol: Int!,
-            $obsNchan: Int!,
-        ) {
-            createToa (input: {
-                pipelineRunId: $pipelineRunId,
-                projectShort: $projectShort,
-                templateId: $templateId,
-                ephemerisText: $ephemerisText,
-                toaLines: $toaLines,
-                dmCorrected: $dmCorrected,
-                minimumNsubs: $minimumNsubs,
-                maximumNsubs: $maximumNsubs,
-                allNsubs: $allNsubs,
-                modeNsubs: $modeNsubs,
-                obsNpol: $obsNpol,
-                obsNchan: $obsNchan,
-            }) {
-                toa {
-                    id,
-                }
-            }
-        }
-        """
-        # Read ephemeris file
-        with open(ephemeris, "r") as f:
-            ephemeris_str = f.read()
-
-        responses = []
-        for toa_chunk in chunk_list(toa_lines, 1000):
-            # Upload the toa
-            self.variables = {
-                'pipelineRunId': pipeline_run_id,
-                'projectShort': project_short,
-                'templateId': template_id,
-                'ephemerisText': ephemeris_str,
-                'toaLines': toa_chunk,
-                'dmCorrected': dmCorrected,
-                'minimumNsubs': minimumNsubs,
-                'maximumNsubs': maximumNsubs,
-                'allNsubs': allNsubs,
-                'modeNsubs': modeNsubs,
-                "obsNpol": npol,
-                "obsNchan": nchan,
-            }
-            responses.append(self.mutation_graphql())
-        if len(responses) == 0:
-            return None
-        else:
-            return responses[-1]
-
-    def delete(
-        self,
-        id,
-    ):
-        """Delete a Toa database object.
-
-        Parameters
-        ----------
-        id : int
-            The database ID
-
-        Returns
-        -------
-        client_response:
-            A client response object.
-        """
-        self.mutation_name = "deleteToa"
-        self.mutation = """
-        mutation ($id: Int!) {
-            deleteToa(id: $id) {
-                ok
-            }
-        }
-        """
-        self.variables = {
-            "id": id,
-        }
-        return self.mutation_graphql()
-
-    def download(
-        self,
-        pulsar,
-        id=None,
-        pipeline_run_id=None,
-        project_short=None,
-        dm_corrected=None,
-        nsub_type=None,
-        obs_nchan=None,
-        npol=None,
-    ):
-        """Download a file containing ToAs based on the filters.
-
-        Parameters
-        ----------
-        pulsar : str
-            Filter by the pulsar name
-        id : int, optional
-            Filter by the database ID, by default None
-        pipeline_run_id : int, optional
-            Filter by the pipeline run id, by default None
-        project_short : str
-            The project short name (e.g PTA).
-        dm_corrected : bool, optional
-            Filter by if the toa was DM corrected, by default None
-        nsub_type : str
-            The method used to calculate the number of subintegrations. The choices are:
-                "1": a single nsub,
-                "max" the maximum number of subints possible for the observation based on the S/N ratio,
-                "mode" the length of each subintegration is equal to the most common observation duration,
-                "all": all available nsubs (no time scrunching).
-        obs_nchan : int, optional
-            Filter by the number of channels, by default None
-        npol : int
-            The number of Stokes polarisations.
-
-        Returns
-        -------
-        list of dicts
-            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
-        client_response:
-            Else a client response object.
-        """
-        filters = [
-            {"field": "id", "value": id},
-            {"field": "pulsar", "value": pulsar},
-            {"field": "pipelineRunId", "value": pipeline_run_id},
-            {"field": "projectShort", "value": project_short},
-            {"field": "dmCorrected", "value": dm_corrected},
-            {"field": "obsNchan", "value": obs_nchan},
-            {"field": "obsNpol", "value": npol},
-        ]
-        if nsub_type == "1":
-            filters.append({"field": "minimumNsubs", "value": True})
-        if nsub_type == "max":
-            filters.append({"field": "maximumNsubs", "value": True})
-        if nsub_type == "all":
-            filters.append({"field": "allNsubs", "value": True})
-        if nsub_type == "mode":
-            filters.append({"field": "modeNsubs", "value": True})
-
-        self.get_dicts = True
-        toa_dicts = GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names, paginate_num=10000)
-
-        # Create the output name
-        output_name = f"toa_{pulsar}"
-        if id is not None:
-            output_name += f"_id{id}"
-        if pipeline_run_id is not None:
-            output_name += f"_pipeline_run_id{pipeline_run_id}"
-        if project_short is not None:
-            output_name += f"_{project_short}"
-        if dm_corrected is not None and dm_corrected:
-            output_name += "_dm_corrected"
-        if nsub_type is not None:
-            output_name += f"_{nsub_type}_nsub"
-        if obs_nchan is not None:
-            output_name += f"_nchan{obs_nchan}"
-        if npol is not None:
-            output_name += f"_npol{npol}"
-        output_name += ".tim"
-
-        # Loop over the toas and dump them as a file
-        with open(output_name, "w") as f:
-            f.write("FORMAT 1\n")
-            for toa_dict in toa_dicts:
-                # Convert to toa format
-                # del toa_dict["id"]
-                del toa_dict["pipelineRun"]
-                del toa_dict["ephemeris"]
-                del toa_dict["template"]
-                toa_dict["freq_MHz"] = toa_dict["freqMhz"]
-                toa_dict["mjd_err"] = toa_dict["mjdErr"]
-                del toa_dict["freqMhz"]
-                del toa_dict["mjdErr"]
-                toa_line = toa_dict_to_line(toa_dict)
-                f.write(f"{toa_line}\n")
-        return output_name
-
-
-    def process(self, args):
-        """Parse the arguments collected by the CLI."""
-        self.print_stdout = True
-        if args.subcommand == "create":
-
-            with open(args.toa_path, "r") as f:
-                toa_lines = f.readlines()
-                self.create(
-                    args.pipeline_run_id,
-                    args.ephemeris_id,
-                    args.template_id,
-                    input_toa_line,
-                    args.dm_corrected,
-                    args.minimumNsubs,
-                    args.maximumNsubs,
-                    args.npol,
-                )
-        elif args.subcommand == "delete":
-            return self.delete(args.id)
-        elif args.subcommand == "list":
-            return self.list(args.id, args.processing, args.folding, args.ephemeris, args.template)
-        elif args.subcommand == "download":
-            return self.download(
-                args.pulsar,
-                args.id,
-                args.pipeline_run_id,
-                args.project,
-                args.dm_corrected,
-                args.nsub_type,
-                args.nchan,
-                args.npol,
-            )
-        else:
-            raise RuntimeError(f"{args.subcommand} command is not implemented")
-
-    @classmethod
-    def get_name(cls):
-        return "toa"
-
-    @classmethod
-    def get_description(cls):
-        return "A pulsar toa/standard"
-
-    @classmethod
-    def get_parsers(cls):
-        """Returns the default parser for this model"""
-        parser = GraphQLTable.get_default_parser("Toa model parser")
-        cls.configure_parsers(parser)
-        return parser
-
-    @classmethod
-    def configure_parsers(cls, parser):
-        """Add sub-parsers for each of the valid commands."""
-        # create the parser for the "list" command
-        parser.set_defaults(command=cls.get_name())
-        subs = parser.add_subparsers(dest="subcommand")
-        subs.required = True
-
-        parser_list = subs.add_parser("list", help="list existing ephemerides")
-        parser_list.add_argument("--id", metavar="ID", type=int, help="list toa matching the id [int]")
-        parser_list.add_argument(
-            "--processing", metavar="PROC", type=int, help="list toa matching the processing id [int]"
-        )
-        parser_list.add_argument("--folding", metavar="FOLD", type=int, help="list toa that used the folding id [int]")
-        parser_list.add_argument(
-            "--ephemeris", metavar="EPH", type=int, help="list toa matching the timing ephemeris id [int]"
-        )
-        parser_list.add_argument(
-            "--template", metavar="TEMPL", type=int, help="list toa matching the template id [int]"
-        )
-
-        # create the parser for the "download" command
-        parser_download = subs.add_parser("download", help="Download TOAs for a pulsar to a .tim file")
-        parser_download.add_argument("pulsar", type=str, help="Name of the pulsar [str]")
-        parser_download.add_argument("--project", type=str, help="The project short (e.g. PTA) [str]", required=True)
-        parser_download.add_argument("--id", type=int, help="id of the toa [int]")
-        parser_download.add_argument("--pipeline_run_id", type=int, help="pipeline_run_id of the toa [int]")
-        parser_download.add_argument("--dm_corrected",  action="store_true", help="Return TOAs that have had their DM corrected for each observation [bool]")
-        parser_download.add_argument(
-            '--nsub_type',
-            type=str,
-            choices=['1', 'max', 'mode', 'all'],
-            required=True,
-            help='The method used to calculate the number of subintegrations. The choices are: '
-                '"1": a single nsub, '
-                '"max" the maximum number of subints possible for the observation based on the S/N ratio, '
-                '"mode" the length of each subintegration is equal to the most common observation duration, '
-                '"all": all available nsubs (no time scrunching).'
-        )
-        parser_download.add_argument("--nchan", type=int, help="Only use TOAs with this many subchans (common values are 1,4 and 16) [int]", required=True)
-        parser_download.add_argument("--npol", type=int, help="Only use TOAs with this many stokes polarisations (4 for all and 1 for summed) [int]", required=True)
-
+from datetime import datetime
+
+from psrdb.graphql_table import GraphQLTable
+from psrdb.utils.toa import toa_dict_to_line
+from psrdb.utils.other import chunk_list
+from psrdb.load_data import EXCLUDE_BADGES_CHOICES
+
+
+def get_parsers():
+    """Returns the default parser for this model"""
+    parser = GraphQLTable.get_default_parser("The following options will allow you to interact with the Toa database object on the command line in different ways based on the sub-commands.")
+    Toa.configure_parsers(parser)
+    return parser
+
+
+class Toa(GraphQLTable):
+    """Class for interacting with the Toa database object.
+
+    Parameters
+    ----------
+    client : GraphQLClient
+        GraphQLClient class instance with the URL and Token already set.
+    """
+    def __init__(self, client):
+        GraphQLTable.__init__(self, client)
+        self.table_name = "toa"
+
+        self.field_names = [
+            "id",
+            "pipelineRun{ id }",
+            "ephemeris { id }",
+            "template { id }",
+            "archive",
+            "freqMhz",
+            "mjd",
+            "mjdErr",
+            "telescope",
+            "fe",
+            "be",
+            "f",
+            "bw",
+            "tobs",
+            "tmplt",
+            "gof",
+            "nbin",
+            "nch",
+            "chan",
+            "rcvr",
+            "snr",
+            "length",
+            "subint",
+        ]
+
+    def list(
+        self,
+        id=None,
+        pulsar=None,
+        pipeline_run_id=None,
+        project_short=None,
+        dm_corrected=None,
+        minimum_nsubs=None,
+        maximum_nsubs=None,
+        obs_nchan=None,
+    ):
+        """Return a list of Toa information based on the `self.field_names` and filtered by the parameters.
+
+        Parameters
+        ----------
+        id : int, optional
+            Filter by the database ID, by default None
+        pulsar : str, optional
+            Filter by the pulsar name, by default None
+        pipeline_run_id : int, optional
+            Filter by the pipeline run id, by default None
+        project_short : str
+            The project short name (e.g PTA).
+        dm_corrected : bool, optional
+            Filter by if the toa was DM corrected, by default None
+        minimum_nsubs : bool, optional
+            Filter by if the toa was generated with the minimum number of time subbands, by default None
+        maximum_nsubs : bool, optional
+            Filter by if the toa was generated with the maximum number of time subbands, by default None
+        obs_nchan : int, optional
+            Filter by the number of channels, by default None
+
+        Returns
+        -------
+        list of dicts
+            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
+        client_response:
+            Else a client response object.
+        """
+        filters = [
+            {"field": "id", "value": id},
+            {"field": "pulsar", "value": pulsar},
+            {"field": "pipelineRunId", "value": pipeline_run_id},
+            {"field": "projectShort", "value": project_short},
+            {"field": "dmCorrected", "value": dm_corrected},
+            {"field": "obsNchan", "value": obs_nchan},
+        ]
+        if minimum_nsubs:
+            filters.append({"field": "minimumNsubs", "value": minimum_nsubs})
+        if maximum_nsubs:
+            filters.append({"field": "maximumNsubs", "value": maximum_nsubs})
+        return GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names)
+
+    def create(
+        self,
+        pipeline_run_id,
+        project_short,
+        ephemeris,
+        template_id,
+        toa_lines,
+        dmCorrected=False,
+        nsub_type=None,
+        npol=1,
+        nchan=1,
+    ):
+        """Create a new Toa database object.
+
+        Parameters
+        ----------
+        pipeline_run_id : int
+            The ID of the PipelineRun database object for this Toa.
+        project_short : str
+            The project short name (e.g PTA).
+        ephemeris : str
+            The path to the ephemeris file used to create the residuals.
+        template_id : int
+            The ID of the Template database object for this Toa.
+        toa_lines : list
+            A list containing the toa lines.
+        dmCorrected : bool
+            If the toa was DM corrected.
+        minimumNsubs : bool
+            If the toa was generated with the minimum number of time subbands.
+        maximumNsubs : bool
+            If the toa was generated with the maximum number of time subbands.
+        npol : int
+            The number of Stokes polarisations.
+        nchan : int
+            The number of frequency channels.
+
+        Returns
+        -------
+        client_response:
+            A client response object.
+        """
+        self.mutation_name = "createToa"
+        self.mutation = """
+        mutation (
+            $pipelineRunId: Int!,
+            $projectShort: String!,
+            $templateId: Int!,
+            $ephemerisText: String!,
+            $toaLines: [String]!,
+            $dmCorrected: Boolean!,
+            $nsubType: String!,
+            $obsNpol: Int!,
+            $obsNchan: Int!,
+        ) {
+            createToa (input: {
+                pipelineRunId: $pipelineRunId,
+                projectShort: $projectShort,
+                templateId: $templateId,
+                ephemerisText: $ephemerisText,
+                toaLines: $toaLines,
+                dmCorrected: $dmCorrected,
+                nsubType: $nsubType,
+                obsNpol: $obsNpol,
+                obsNchan: $obsNchan,
+            }) {
+                toa {
+                    id,
+                }
+            }
+        }
+        """
+        # Read ephemeris file
+        with open(ephemeris, "r") as f:
+            ephemeris_str = f.read()
+
+        responses = []
+        for toa_chunk in chunk_list(toa_lines, 1000):
+            # Upload the toa
+            self.variables = {
+                'pipelineRunId': pipeline_run_id,
+                'projectShort': project_short,
+                'templateId': template_id,
+                'ephemerisText': ephemeris_str,
+                'toaLines': toa_chunk,
+                'dmCorrected': dmCorrected,
+                'nsubType': nsub_type,
+                "obsNpol": npol,
+                "obsNchan": nchan,
+            }
+            responses.append(self.mutation_graphql())
+        if len(responses) == 0:
+            return None
+        else:
+            return responses[-1]
+
+    def delete(
+        self,
+        id,
+    ):
+        """Delete a Toa database object.
+
+        Parameters
+        ----------
+        id : int
+            The database ID
+
+        Returns
+        -------
+        client_response:
+            A client response object.
+        """
+        self.mutation_name = "deleteToa"
+        self.mutation = """
+        mutation ($id: Int!) {
+            deleteToa(id: $id) {
+                ok
+            }
+        }
+        """
+        self.variables = {
+            "id": id,
+        }
+        return self.mutation_graphql()
+
+    def download(
+        self,
+        pulsar,
+        id=None,
+        pipeline_run_id=None,
+        project_short=None,
+        dm_corrected=None,
+        nsub_type=None,
+        obs_nchan=None,
+        npol=None,
+        exclude_badges=None,
+        utcs=None,
+        utce=None,
+    ):
+        """Download a file containing ToAs based on the filters.
+
+        Parameters
+        ----------
+        pulsar : str
+            Filter by the pulsar name
+        id : int, optional
+            Filter by the database ID, by default None
+        pipeline_run_id : int, optional
+            Filter by the pipeline run id, by default None
+        project_short : str
+            The project short name (e.g PTA).
+        dm_corrected : bool, optional
+            Filter by if the toa was DM corrected, by default None
+        nsub_type : str
+            The method used to calculate the number of subintegrations. The choices are:
+                "1": a single nsub,
+                "max" the maximum number of subints possible for the observation based on the S/N ratio,
+                "mode" the length of each subintegration is equal to the most common observation duration,
+                "all": all available nsubs (no time scrunching).
+        obs_nchan : int, optional
+            Filter by the number of channels, by default None
+        npol : int
+            The number of Stokes polarisations.
+
+        Returns
+        -------
+        list of dicts
+            If `self.get_dicts` is `True`, a list of dictionaries containing the results.
+        client_response:
+            Else a client response object.
+        """
+        filters = [
+            {"field": "id", "value": id},
+            {"field": "pulsar", "value": pulsar},
+            {"field": "pipelineRunId", "value": pipeline_run_id},
+            {"field": "projectShort", "value": project_short},
+            {"field": "dmCorrected", "value": dm_corrected},
+            {"field": "obsNchan", "value": obs_nchan},
+            {"field": "obsNpol", "value": npol},
+            {"field": "nsubType", "value": nsub_type},
+        ]
+        if exclude_badges is not None:
+            filters.append({"field": "excludeBadges", "value": exclude_badges})
+        if utcs is not None:
+            d = datetime.strptime(utcs, '%Y-%m-%d-%H:%M:%S')
+            filters.append({"field": "utcStartGte", "value": f"{d.date()}T{d.time()}+00:00"})
+        if utce is not None:
+            d = datetime.strptime(utce, '%Y-%m-%d-%H:%M:%S')
+            filters.append({"field": "utcStartLte", "value": f"{d.date()}T{d.time()}+00:00"})
+
+
+        self.get_dicts = True
+        toa_dicts = GraphQLTable.list_graphql(self, self.table_name, filters, [], self.field_names, paginate_num=10000)
+
+        # Create the output name
+        output_name = f"toa_{pulsar}"
+        if id is not None:
+            output_name += f"_id{id}"
+        if pipeline_run_id is not None:
+            output_name += f"_pipeline_run_id{pipeline_run_id}"
+        if project_short is not None:
+            output_name += f"_{project_short}"
+        if dm_corrected is not None and dm_corrected:
+            output_name += "_dm_corrected"
+        if nsub_type is not None:
+            output_name += f"_{nsub_type}_nsub"
+        if obs_nchan is not None:
+            output_name += f"_nchan{obs_nchan}"
+        if npol is not None:
+            output_name += f"_npol{npol}"
+        output_name += ".tim"
+
+        # Loop over the toas and dump them as a file
+        with open(output_name, "w") as f:
+            f.write("FORMAT 1\n")
+            for toa_dict in toa_dicts:
+                # Convert to toa format
+                # del toa_dict["id"]
+                del toa_dict["pipelineRun"]
+                del toa_dict["ephemeris"]
+                del toa_dict["template"]
+                toa_dict["freq_MHz"] = toa_dict["freqMhz"]
+                toa_dict["mjd_err"] = toa_dict["mjdErr"]
+                del toa_dict["freqMhz"]
+                del toa_dict["mjdErr"]
+                toa_line = toa_dict_to_line(toa_dict)
+                f.write(f"{toa_line}\n")
+        return output_name
+
+
+    def process(self, args):
+        """Parse the arguments collected by the CLI."""
+        self.print_stdout = True
+        if args.subcommand == "create":
+
+            with open(args.toa_path, "r") as f:
+                toa_lines = f.readlines()
+                self.create(
+                    args.pipeline_run_id,
+                    args.ephemeris_id,
+                    args.template_id,
+                    toa_lines,
+                    args.dm_corrected,
+                    args.minimumNsubs,
+                    args.maximumNsubs,
+                    args.npol,
+                )
+        elif args.subcommand == "delete":
+            return self.delete(args.id)
+        elif args.subcommand == "list":
+            return self.list(args.id, args.processing, args.folding, args.ephemeris, args.template)
+        elif args.subcommand == "download":
+            return self.download(
+                args.pulsar,
+                args.id,
+                args.pipeline_run_id,
+                args.project,
+                args.dm_corrected,
+                args.nsub_type,
+                args.nchan,
+                args.npol,
+                args.exclude_badges,
+                args.utcs,
+                args.utce,
+            )
+        else:
+            raise RuntimeError(f"{args.subcommand} command is not implemented")
+
+    @classmethod
+    def get_name(cls):
+        return "toa"
+
+    @classmethod
+    def get_description(cls):
+        return "A pulsar toa/standard"
+
+    @classmethod
+    def get_parsers(cls):
+        """Returns the default parser for this model"""
+        parser = GraphQLTable.get_default_parser("Toa model parser")
+        cls.configure_parsers(parser)
+        return parser
+
+    @classmethod
+    def configure_parsers(cls, parser):
+        """Add sub-parsers for each of the valid commands."""
+        # create the parser for the "list" command
+        parser.set_defaults(command=cls.get_name())
+        subs = parser.add_subparsers(dest="subcommand")
+        subs.required = True
+
+        parser_list = subs.add_parser("list", help="list existing ephemerides")
+        parser_list.add_argument("--id", metavar="ID", type=int, help="list toa matching the id [int]")
+        parser_list.add_argument(
+            "--processing", metavar="PROC", type=int, help="list toa matching the processing id [int]"
+        )
+        parser_list.add_argument("--folding", metavar="FOLD", type=int, help="list toa that used the folding id [int]")
+        parser_list.add_argument(
+            "--ephemeris", metavar="EPH", type=int, help="list toa matching the timing ephemeris id [int]"
+        )
+        parser_list.add_argument(
+            "--template", metavar="TEMPL", type=int, help="list toa matching the template id [int]"
+        )
+
+        # create the parser for the "download" command
+        parser_download = subs.add_parser("download", help="Download TOAs for a pulsar to a .tim file")
+        parser_download.add_argument("pulsar", type=str, help="Name of the pulsar [str]")
+        parser_download.add_argument("--project", type=str, help="The project short (e.g. PTA) [str]", required=True)
+        parser_download.add_argument("--id", type=int, help="id of the toa [int]")
+        parser_download.add_argument("--pipeline_run_id", type=int, help="pipeline_run_id of the toa [int]")
+        parser_download.add_argument("--dm_corrected",  action="store_true", help="Return TOAs that have had their DM corrected for each observation [bool]")
+        parser_download.add_argument(
+            '--nsub_type',
+            type=str,
+            choices=['1', 'max', 'mode', 'all'],
+            required=True,
+            help='The method used to calculate the number of subintegrations. The choices are: '
+                '"1": a single nsub, '
+                '"max" the maximum number of subints possible for the observation based on the S/N ratio, '
+                '"mode" the length of each subintegration is equal to the most common observation duration, '
+                '"all": all available nsubs (no time scrunching).'
+        )
+        parser_download.add_argument("--nchan", type=int, help="Only use TOAs with this many subchans (common values are 1,4 and 16) [int]", required=True)
+        parser_download.add_argument("--npol", type=int, help="Only use TOAs with this many stokes polarisations (4 for all and 1 for summed) [int]", required=True)
+        parser_download.add_argument(
+            '--exclude_badges',
+            nargs='*',
+            choices=EXCLUDE_BADGES_CHOICES,
+            help=f'List of observation badges/flags to exclude from download ToAs. The choices are: {EXCLUDE_BADGES_CHOICES}'
+        )
+        parser_download.add_argument(
+            "--utcs",
+            type=str,
+            help="Only use observations with utc_start greater than or equal to the timestamp [YYYY-MM-DD-HH:MM:SS]",
+        )
+        parser_download.add_argument(
+            "--utce",
+            type=str,
+            help="Only use observations with utc_start less than or equal to the timestamp [YYYY-MM-DD-HH:MM:SS]",
+        )
+
```

### Comparing `psrdb-3.0.5/psrdb/utils/ephemeris.py` & `psrdb-3.0.6/psrdb/utils/ephemeris.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/utils/header.py` & `psrdb-3.0.6/psrdb/utils/header.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/utils/other.py` & `psrdb-3.0.6/psrdb/utils/other.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-import os
-import re
-import json
-import logging
-from base64 import b64decode, b64encode
-
-
-def setup_logging(
-        console=True,
-        logfile=False,
-        filedir=None,
-        filename='psrdb.log',
-        level=logging.INFO,
-    ):
-    """
-    Setup log handler for the logger object
-
-    Parameters
-    ----------
-    console : `boolean`
-        Output logging to the command line
-    logfile : `boolean`
-        Output logging to the log file
-    filedir : `str`
-        Directory to output logger file to
-    filename : `str`
-        Name of the output logger file
-
-    Returns
-    -------
-    logger : logger object
-        The modified logger object
-    """
-    # create formatter
-    formatter = logging.Formatter('%(asctime)s - %(name)s - %(lineno)-4d - %(levelname)-9s :: %(message)s')
-    # Create a logger and set the logging level
-    logger = logging.getLogger()
-    logger.setLevel(level)
-
-    # Create a console handler and set the logging level if console is True
-    if console:
-        console_handler = logging.StreamHandler()
-        console_handler.setLevel(level)
-        console_handler.setFormatter(formatter)
-        logger.addHandler(console_handler)
-        logger.info("Console logger enabled")
-
-    # Create a file handler and set the logging level if logfile is True
-    if logfile:
-        if not filedir:
-            raise ValueError("Filedir must be specified when enabling logfile output.")
-        if not os.path.exists(filedir):
-            os.makedirs(filedir)
-        file_handler = logging.FileHandler(os.path.join(filedir, filename))
-        file_handler.setLevel(level)
-        file_handler.setFormatter(formatter)
-        logger.addHandler(file_handler)
-        logger.info(f"File logging enabled into file: {os.path.join(filedir, filename)}")
-
-        #Check if file already exists, if so, add a demarcator to differentiate among runs
-        if os.path.exists(os.path.join(filedir, filename)):
-            with open(os.path.join(filedir, filename), 'a') as f:
-                f.write(20*"#")
-                f.write("\n")
-
-    return logger
-
-
-def to_snake_case(text):
-    snake_case = re.sub(r'(?<!^)(?=[A-Z])', '_', text).lower()
-    return snake_case
-
-
-def to_camel_case(text):
-    words = re.split(r'[_\s]+', text)
-    return words[0].lower() + ''.join(word.title() for word in words[1:])
-
-
-def get_graphql_id(response, table, logger):
-    """
-    Parses the graphql response to return the id of the newly created object
-    """
-    content = json.loads(response.content)
-    logger.debug(content.keys())
-
-    if "errors" in content.keys():
-        logger.error(f"Error in GraphQL response: {content['errors']}")
-        raise ValueError(f"Error in GraphQL response: {content['errors']}")
-    else:
-        data = content["data"]
-        # Convert from snake_case to CamelCase
-        mutation_name = to_camel_case(f"create_{table}")
-        table_name = to_camel_case(table)
-        models_made = data[mutation_name][table_name]
-        # Turn into list if multiple objects were created
-        if type(models_made) != list:
-            models_made = [models_made]
-        for model in models_made:
-            try:
-                graphql_id = model["id"]
-            except KeyError:
-                raise KeyError(f"No key ['{mutation_name}']['{table_name}']['id'] in {data}")
-            try:
-                return int(graphql_id)
-            except ValueError:
-                return decode_id(graphql_id)
-
-
-def get_rest_api_id(response, logger):
-    content = json.loads(response.content)
-    logger.debug(content.keys())
-
-    if content["errors"] is None:
-        try:
-            return int(content["id"])
-        except KeyError:
-            return None
-    else:
-        logger.error(f"Error in GraphQL response: {content['errors']}")
-        return None
-
-
-def decode_id(encoded):
-    decoded = b64decode(encoded).decode("ascii")
-    return decoded.split(":")[1]
-
-
-def chunk_list(lst, chunk_size):
-    for i in range(0, len(lst), chunk_size):
+import os
+import re
+import json
+import logging
+from base64 import b64decode, b64encode
+
+
+def setup_logging(
+        console=True,
+        logfile=False,
+        filedir=None,
+        filename='psrdb.log',
+        level=logging.INFO,
+    ):
+    """
+    Setup log handler for the logger object
+
+    Parameters
+    ----------
+    console : `boolean`
+        Output logging to the command line
+    logfile : `boolean`
+        Output logging to the log file
+    filedir : `str`
+        Directory to output logger file to
+    filename : `str`
+        Name of the output logger file
+
+    Returns
+    -------
+    logger : logger object
+        The modified logger object
+    """
+    # create formatter
+    formatter = logging.Formatter('%(asctime)s - %(name)s - %(lineno)-4d - %(levelname)-9s :: %(message)s')
+    # Create a logger and set the logging level
+    logger = logging.getLogger()
+    logger.setLevel(level)
+
+    # Create a console handler and set the logging level if console is True
+    if console:
+        console_handler = logging.StreamHandler()
+        console_handler.setLevel(level)
+        console_handler.setFormatter(formatter)
+        logger.addHandler(console_handler)
+        logger.info("Console logger enabled")
+
+    # Create a file handler and set the logging level if logfile is True
+    if logfile:
+        if not filedir:
+            raise ValueError("Filedir must be specified when enabling logfile output.")
+        if not os.path.exists(filedir):
+            os.makedirs(filedir)
+        file_handler = logging.FileHandler(os.path.join(filedir, filename))
+        file_handler.setLevel(level)
+        file_handler.setFormatter(formatter)
+        logger.addHandler(file_handler)
+        logger.info(f"File logging enabled into file: {os.path.join(filedir, filename)}")
+
+        #Check if file already exists, if so, add a demarcator to differentiate among runs
+        if os.path.exists(os.path.join(filedir, filename)):
+            with open(os.path.join(filedir, filename), 'a') as f:
+                f.write(20*"#")
+                f.write("\n")
+
+    return logger
+
+
+def to_snake_case(text):
+    snake_case = re.sub(r'(?<!^)(?=[A-Z])', '_', text).lower()
+    return snake_case
+
+
+def to_camel_case(text):
+    words = re.split(r'[_\s]+', text)
+    return words[0].lower() + ''.join(word.title() for word in words[1:])
+
+
+def get_graphql_id(response, table, logger):
+    """
+    Parses the graphql response to return the id of the newly created object
+    """
+    content = json.loads(response.content)
+    logger.debug(content.keys())
+
+    if "errors" in content.keys():
+        logger.error(f"Error in GraphQL response: {content['errors']}")
+        raise ValueError(f"Error in GraphQL response: {content['errors']}")
+    else:
+        data = content["data"]
+        # Convert from snake_case to CamelCase
+        mutation_name = to_camel_case(f"create_{table}")
+        table_name = to_camel_case(table)
+        models_made = data[mutation_name][table_name]
+        # Turn into list if multiple objects were created
+        if type(models_made) != list:
+            models_made = [models_made]
+        for model in models_made:
+            try:
+                graphql_id = model["id"]
+            except KeyError:
+                raise KeyError(f"No key ['{mutation_name}']['{table_name}']['id'] in {data}")
+            try:
+                return int(graphql_id)
+            except ValueError:
+                return decode_id(graphql_id)
+
+
+def get_rest_api_id(response, logger):
+    content = json.loads(response.content)
+    logger.debug(content.keys())
+
+    if content["errors"] is None:
+        try:
+            return int(content["id"])
+        except KeyError:
+            return None
+    else:
+        logger.error(f"Error in GraphQL response: {content['errors']}")
+        return None
+
+
+def decode_id(encoded):
+    decoded = b64decode(encoded).decode("ascii")
+    return decoded.split(":")[1]
+
+
+def chunk_list(lst, chunk_size):
+    for i in range(0, len(lst), chunk_size):
         yield lst[i:i + chunk_size]
```

### Comparing `psrdb-3.0.5/psrdb/utils/residual.py` & `psrdb-3.0.6/psrdb/utils/residual.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/psrdb/utils/toa.py` & `psrdb-3.0.6/psrdb/utils/toa.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from decimal import Decimal, getcontext
-
-def format_float(value, threshold=1e3, decimal_places=2):
-    if abs(value) >= threshold:
-        e_format = "{:.{}e}".format(value, decimal_places)
-        return e_format.replace("0e", "e").replace("0e", "e").replace(".e", "e")  # remove trailing zeros
-    else:
-        return f"{value}"
-
-
-def toa_line_to_dict(toa_line):
-    """
-    Parse a single line from a .toa file.
-
-    Args:
-        toa_line (str): A line from a .toa file.
-
-    Returns:
-        dict: A dictionary containing the parsed values.
-    """
-    toa_dict = {}
-    toa_args = toa_line.split(" -")
-    archive, freq_MHz, mjd, mjd_err, telescope = toa_args[0].split()
-    toa_dict["archive"] = archive
-    toa_dict["freq_MHz"] = float(freq_MHz)
-    # MJDs are stored as Decimals as standard floats don't have enough precision
-    getcontext().prec = 12
-    toa_dict["mjd"] = Decimal(mjd)
-    toa_dict["mjd_err"] = float(mjd_err)
-    toa_dict["telescope"] = telescope
-
-    for toa_arg in toa_args[1:]:
-        arg, value = toa_arg.split()
-        toa_dict[arg] = value
-
-    return toa_dict
-
-
-def toa_dict_to_line(toa_dict):
-    """
-    Convert a dictionary to a line in a .toa file.
-
-    Args:
-        toa_dict (dict): A dictionary containing the parsed values.
-
-    Returns:
-        str: A line from a .toa file.
-    """
-    toa_line = ""
-    telescope = toa_dict['telescope']
-    if telescope == "meerkat":
-        telescope = " meerkat "
-    toa_line += f"{toa_dict['archive']} {toa_dict['freq_MHz']:.6f} {toa_dict['mjd']} {toa_dict['mjd_err']:>7.3f} {telescope}"  # noqa: E501
-    for key, value in toa_dict.items():
-        if key not in ["archive", "freq_MHz", "mjd", "mjd_err", "telescope"]:
-            if isinstance(value, float) and key == "gof":
-                toa_line += f" -{key} {format_float(value, threshold=1e3, decimal_places=2)}"
-            else:
-                toa_line += f" -{key} {value}"
+from decimal import Decimal, getcontext
+
+def format_float(value, threshold=1e3, decimal_places=2):
+    if abs(value) >= threshold:
+        e_format = "{:.{}e}".format(value, decimal_places)
+        return e_format.replace("0e", "e").replace("0e", "e").replace(".e", "e")  # remove trailing zeros
+    else:
+        return f"{value}"
+
+
+def toa_line_to_dict(toa_line):
+    """
+    Parse a single line from a .toa file.
+
+    Args:
+        toa_line (str): A line from a .toa file.
+
+    Returns:
+        dict: A dictionary containing the parsed values.
+    """
+    toa_dict = {}
+    toa_args = toa_line.split(" -")
+    archive, freq_MHz, mjd, mjd_err, telescope = toa_args[0].split()
+    toa_dict["archive"] = archive
+    toa_dict["freq_MHz"] = float(freq_MHz)
+    # MJDs are stored as Decimals as standard floats don't have enough precision
+    getcontext().prec = 12
+    toa_dict["mjd"] = Decimal(mjd)
+    toa_dict["mjd_err"] = float(mjd_err)
+    toa_dict["telescope"] = telescope
+
+    for toa_arg in toa_args[1:]:
+        arg, value = toa_arg.split()
+        toa_dict[arg] = value
+
+    return toa_dict
+
+
+def toa_dict_to_line(toa_dict):
+    """
+    Convert a dictionary to a line in a .toa file.
+
+    Args:
+        toa_dict (dict): A dictionary containing the parsed values.
+
+    Returns:
+        str: A line from a .toa file.
+    """
+    toa_line = ""
+    telescope = toa_dict['telescope']
+    if telescope == "meerkat":
+        telescope = " meerkat "
+    toa_line += f"{toa_dict['archive']} {toa_dict['freq_MHz']:.6f} {toa_dict['mjd']} {toa_dict['mjd_err']:>7.3f} {telescope}"  # noqa: E501
+    for key, value in toa_dict.items():
+        if key not in ["archive", "freq_MHz", "mjd", "mjd_err", "telescope"]:
+            if isinstance(value, float) and key == "gof":
+                toa_line += f" -{key} {format_float(value, threshold=1e3, decimal_places=2)}"
+            else:
+                toa_line += f" -{key} {value}"
     return toa_line
```

### Comparing `psrdb-3.0.5/psrdb/utils/upload.py` & `psrdb-3.0.6/psrdb/utils/upload.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.5/pyproject.toml` & `psrdb-3.0.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-[tool.poetry]
-name = "psrdb"
-version = "3.0.5"
-description = "CLI for pulsars.org.au"
-authors = ["GWDC"]
-license = "MIT"
-packages = [{include = "psrdb"}]
-include = ["psrdb/data/molonglo_phasing.txt"]
-
-[tool.poetry.scripts]
-psrdb = "psrdb.scripts.psrdb:main"
-generate_meerkat_json = "psrdb.scripts.generate_meerkat_json:main"
-generate_molonglo_json = "psrdb.scripts.generate_molonglo_json:main"
-ingest_obs = "psrdb.scripts.ingest_obs:main"
-remove_fluxcals = "psrdb.scripts.remove_fluxcals:main"
-
-[tool.poetry.dependencies]
-python = "^3.9"
-requests = "^2.25.1"
-python-decouple = "^3.8"
-pulsar-paragraph = "^1.0.1"
-
-[tool.poetry.group.docs.dependencies]
-numpydoc = "^1.5.0"
-sphinx = "^7.2.4"
-myst-parser = "^2.0.0"
-sphinx-rtd-theme = "^1.3.0"
-sphinx-argparse = "^0.4.0"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
-isort = "^5.12.0"
-black = "^23.3.0"
-flake8 = "^6.0.0"
-urllib3 = "<2"
-responses = "^0.23.1"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "psrdb"
+version = "3.0.6"
+description = "CLI for pulsars.org.au"
+authors = ["GWDC"]
+license = "MIT"
+packages = [{include = "psrdb"}]
+include = ["psrdb/data/molonglo_phasing.txt"]
+
+[tool.poetry.scripts]
+psrdb = "psrdb.scripts.psrdb:main"
+generate_meerkat_json = "psrdb.scripts.generate_meerkat_json:main"
+generate_molonglo_json = "psrdb.scripts.generate_molonglo_json:main"
+ingest_obs = "psrdb.scripts.ingest_obs:main"
+remove_fluxcals = "psrdb.scripts.remove_fluxcals:main"
+
+[tool.poetry.dependencies]
+python = "^3.9"
+requests = "^2.25.1"
+python-decouple = "^3.8"
+pulsar-paragraph = "^1.0.1"
+
+[tool.poetry.group.docs.dependencies]
+numpydoc = "^1.5.0"
+sphinx = "^7.2.4"
+myst-parser = "^2.0.0"
+sphinx-rtd-theme = "^1.3.0"
+sphinx-argparse = "^0.4.0"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+isort = "^5.12.0"
+black = "^23.3.0"
+flake8 = "^6.0.0"
+urllib3 = "<2"
+responses = "^0.23.1"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `psrdb-3.0.5/PKG-INFO` & `psrdb-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrdb
-Version: 3.0.5
+Version: 3.0.6
 Summary: CLI for pulsars.org.au
 License: MIT
 Author: GWDC
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

