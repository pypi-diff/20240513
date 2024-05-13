# Comparing `tmp/teradatamodelops-7.0.6rc2.tar.gz` & `tmp/teradatamodelops-7.0.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teradatamodelops-7.0.6rc2.tar", last modified: Tue Apr 16 10:47:35 2024, max compression
+gzip compressed data, was "teradatamodelops-7.0.7b1.tar", last modified: Mon May 13 09:25:54 2024, max compression
```

## Comparing `teradatamodelops-7.0.6rc2.tar` & `teradatamodelops-7.0.7b1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.380822 teradatamodelops-7.0.6rc2/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9081 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    13324 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/LICENSE.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)       70 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/MANIFEST.in
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23651 2024-04-16 10:47:35.380359 teradatamodelops-7.0.6rc2/PKG-INFO
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2202 2024-04-16 10:43:57.000000 teradatamodelops-7.0.6rc2/README.md
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.288562 teradatamodelops-7.0.6rc2/aoa/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1205 2024-04-16 10:45:01.000000 teradatamodelops-7.0.6rc2/aoa/__init__.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.310488 teradatamodelops-7.0.6rc2/aoa/api/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/api/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1641 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/api_iterator.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4591 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/base_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3711 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/dataset_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1699 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/dataset_connection_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2513 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/dataset_template_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3280 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/deployment_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      774 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/iterator_base_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     5008 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/job_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3530 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/job_event_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      972 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/message_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4542 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/model_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2838 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/project_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6473 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/trained_model_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6324 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/trained_model_artefacts_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4817 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/trained_model_event_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      926 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/user_attributes_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    18419 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api_client.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.323010 teradatamodelops-7.0.6rc2/aoa/cli/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/cli/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4394 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/cli/base_model.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     7171 2024-04-16 10:38:58.000000 teradatamodelops-7.0.6rc2/aoa/cli/evaluate_model.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.328826 teradatamodelops-7.0.6rc2/aoa/cli/metadata_files/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      143 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/cli/metadata_files/.gitignore
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      179 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/cli/metadata_files/readme.md
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     5068 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/cli/repo_manager.py
--rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)     2017 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/cli/run_model.R
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4178 2024-04-16 10:38:58.000000 teradatamodelops-7.0.6rc2/aoa/cli/score_model.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4895 2024-04-16 10:38:58.000000 teradatamodelops-7.0.6rc2/aoa/cli/train_model.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.330588 teradatamodelops-7.0.6rc2/aoa/context/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/context/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3837 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/context/model_context.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.334311 teradatamodelops-7.0.6rc2/aoa/crypto/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    29683 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/crypto/TJEncryptPassword.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/crypto/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6611 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/crypto/crypto.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.337813 teradatamodelops-7.0.6rc2/aoa/stats/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/stats/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    16762 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/stats/stats.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    22482 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/stats/stats_util.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3647 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/stats/store.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.342792 teradatamodelops-7.0.6rc2/aoa/util/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      123 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/util/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      685 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/util/artifacts.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1610 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/util/byom.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6344 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/util/connections.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9042 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/util/sto.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.344855 teradatamodelops-7.0.6rc2/scripts/
--rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)      245 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/scripts/aoa
--rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)    53532 2024-04-16 10:34:40.000000 teradatamodelops-7.0.6rc2/scripts/tmo
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      442 2024-04-16 10:47:35.386241 teradatamodelops-7.0.6rc2/setup.cfg
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      986 2024-04-16 08:05:35.000000 teradatamodelops-7.0.6rc2/setup.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.379242 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23651 2024-04-16 10:47:34.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/PKG-INFO
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1322 2024-04-16 10:47:35.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/SOURCES.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        1 2024-04-16 10:47:34.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/dependency_links.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      210 2024-04-16 10:47:34.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/requires.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        4 2024-04-16 10:47:34.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/top_level.txt
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:54.142463 teradatamodelops-7.0.7b1/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9081 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    13324 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/LICENSE.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)       70 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/MANIFEST.in
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23791 2024-05-13 09:25:54.141926 teradatamodelops-7.0.7b1/PKG-INFO
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2210 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/README.md
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:53.745901 teradatamodelops-7.0.7b1/aoa/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1204 2024-05-02 12:24:20.000000 teradatamodelops-7.0.7b1/aoa/__init__.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:53.885249 teradatamodelops-7.0.7b1/aoa/api/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/api/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1641 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/api_iterator.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4591 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/base_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3711 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/dataset_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1699 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/dataset_connection_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2513 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/dataset_template_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3280 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/deployment_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      774 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/iterator_base_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     5008 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/job_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3530 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/job_event_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      972 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/message_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4542 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/model_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2838 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/project_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6473 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/trained_model_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6324 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/trained_model_artefacts_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4817 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/trained_model_event_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      926 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api/user_attributes_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    18419 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/api_client.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:53.942927 teradatamodelops-7.0.7b1/aoa/cli/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/cli/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4394 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/cli/base_model.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     7171 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/cli/evaluate_model.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:53.959360 teradatamodelops-7.0.7b1/aoa/cli/metadata_files/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      143 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/cli/metadata_files/.gitignore
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      179 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/cli/metadata_files/readme.md
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     5068 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/cli/repo_manager.py
+-rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)     2017 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/cli/run_model.R
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4178 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/cli/score_model.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4895 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/cli/train_model.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:53.969786 teradatamodelops-7.0.7b1/aoa/context/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/context/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3837 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/context/model_context.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:53.989094 teradatamodelops-7.0.7b1/aoa/crypto/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    29683 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/crypto/TJEncryptPassword.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/crypto/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6611 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/crypto/crypto.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:54.061202 teradatamodelops-7.0.7b1/aoa/stats/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/stats/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    16757 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/stats/stats.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    22482 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/stats/stats_util.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3647 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/stats/store.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:54.101541 teradatamodelops-7.0.7b1/aoa/util/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      123 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/util/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      685 2023-03-02 09:03:18.000000 teradatamodelops-7.0.7b1/aoa/util/artifacts.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1610 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/util/byom.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6344 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/util/connections.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9042 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/aoa/util/sto.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:54.121158 teradatamodelops-7.0.7b1/scripts/
+-rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)      245 2024-04-16 17:36:07.000000 teradatamodelops-7.0.7b1/scripts/aoa
+-rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)    53794 2024-05-13 09:14:50.000000 teradatamodelops-7.0.7b1/scripts/tmo
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      441 2024-05-13 09:25:54.144677 teradatamodelops-7.0.7b1/setup.cfg
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      986 2024-04-16 08:05:35.000000 teradatamodelops-7.0.7b1/setup.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-05-13 09:25:54.141030 teradatamodelops-7.0.7b1/teradatamodelops.egg-info/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23791 2024-05-13 09:25:53.000000 teradatamodelops-7.0.7b1/teradatamodelops.egg-info/PKG-INFO
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1322 2024-05-13 09:25:53.000000 teradatamodelops-7.0.7b1/teradatamodelops.egg-info/SOURCES.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        1 2024-05-13 09:25:53.000000 teradatamodelops-7.0.7b1/teradatamodelops.egg-info/dependency_links.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      210 2024-05-13 09:25:53.000000 teradatamodelops-7.0.7b1/teradatamodelops.egg-info/requires.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        4 2024-05-13 09:25:53.000000 teradatamodelops-7.0.7b1/teradatamodelops.egg-info/top_level.txt
```

### Comparing `teradatamodelops-7.0.6rc2/LICENSE-3RD-PARTY.txt` & `teradatamodelops-7.0.7b1/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/LICENSE.txt` & `teradatamodelops-7.0.7b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/PKG-INFO` & `teradatamodelops-7.0.7b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teradatamodelops
-Version: 7.0.6rc2
+Version: 7.0.7b1
 Summary: Python client for Teradata ModelOps (TMO)
 Home-page: 
 Author: Teradata
 Author-email: teradata.corporation@teradatacorporation.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -429,14 +429,19 @@
 ```
 
 
 ## Release Notes
 
 ### current
 
+- Explicitly ask for `logmech` when defining a local Vantage connection
+- Fixed `tmo connection create-byom-table` logging error
+
+### 7.0.6
+
 - Fixed compatibility issue with `teradataml>=20.0.0.0`
 - Minor formatting updates
 - Added user attributes API
 - Updated programmatic BYOM import examples
 
 ### 7.0.5
```

### Comparing `teradatamodelops-7.0.6rc2/README.md` & `teradatamodelops-7.0.7b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 pip install dist/*.whl
 ```
 
 ## Code Style
 
 ```bash
 pip install -r dev_requirements.txt
-python -m black aoa/* scripts/* examples/*.ipynb -t py38 -t py39 
+python -m black aoa/* tests/* scripts/* examples/*.ipynb -t py38 -t py39 
 ```
 
 ## Testing
 
 ```bash
 pip install -r dev_requirements.txt
 python -m pytest
```

### Comparing `teradatamodelops-7.0.6rc2/aoa/__init__.py` & `teradatamodelops-7.0.7b1/aoa/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "7.0.6rc2"
+__version__ = "7.0.7b1"
 
 # import client
 from aoa.api_client import AoaClient
 
 # import APIs into api package
 from aoa.api.dataset_api import DatasetApi
 from aoa.api.dataset_template_api import DatasetTemplateApi
```

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/api_iterator.py` & `teradatamodelops-7.0.7b1/aoa/api/api_iterator.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/base_api.py` & `teradatamodelops-7.0.7b1/aoa/api/base_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/dataset_api.py` & `teradatamodelops-7.0.7b1/aoa/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/dataset_connection_api.py` & `teradatamodelops-7.0.7b1/aoa/api/dataset_connection_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/dataset_template_api.py` & `teradatamodelops-7.0.7b1/aoa/api/dataset_template_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/deployment_api.py` & `teradatamodelops-7.0.7b1/aoa/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/iterator_base_api.py` & `teradatamodelops-7.0.7b1/aoa/api/iterator_base_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/job_api.py` & `teradatamodelops-7.0.7b1/aoa/api/job_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/job_event_api.py` & `teradatamodelops-7.0.7b1/aoa/api/job_event_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/message_api.py` & `teradatamodelops-7.0.7b1/aoa/api/message_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/model_api.py` & `teradatamodelops-7.0.7b1/aoa/api/model_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/project_api.py` & `teradatamodelops-7.0.7b1/aoa/api/project_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/trained_model_api.py` & `teradatamodelops-7.0.7b1/aoa/api/trained_model_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/trained_model_artefacts_api.py` & `teradatamodelops-7.0.7b1/aoa/api/trained_model_artefacts_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/trained_model_event_api.py` & `teradatamodelops-7.0.7b1/aoa/api/trained_model_event_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api/user_attributes_api.py` & `teradatamodelops-7.0.7b1/aoa/api/user_attributes_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/api_client.py` & `teradatamodelops-7.0.7b1/aoa/api_client.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/cli/base_model.py` & `teradatamodelops-7.0.7b1/aoa/cli/base_model.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/cli/evaluate_model.py` & `teradatamodelops-7.0.7b1/aoa/cli/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/cli/repo_manager.py` & `teradatamodelops-7.0.7b1/aoa/cli/repo_manager.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/cli/run_model.R` & `teradatamodelops-7.0.7b1/aoa/cli/run_model.R`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/cli/score_model.py` & `teradatamodelops-7.0.7b1/aoa/cli/score_model.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/cli/train_model.py` & `teradatamodelops-7.0.7b1/aoa/cli/train_model.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/context/model_context.py` & `teradatamodelops-7.0.7b1/aoa/context/model_context.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/crypto/TJEncryptPassword.py` & `teradatamodelops-7.0.7b1/aoa/crypto/TJEncryptPassword.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/crypto/crypto.py` & `teradatamodelops-7.0.7b1/aoa/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/stats/stats.py` & `teradatamodelops-7.0.7b1/aoa/stats/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import logging
 import math
 import numbers
 
-from typing import List, Dict, Set
+from typing import List, Dict
 from teradataml.analytics.valib import *
 from teradataml import DataFrame
 from aoa.context.model_context import ModelContext
 from aoa.stats.stats_util import (
     _capture_stats,
     _NpEncoder,
     _parse_scoring_stats,
```

### Comparing `teradatamodelops-7.0.6rc2/aoa/stats/stats_util.py` & `teradatamodelops-7.0.7b1/aoa/stats/stats_util.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/stats/store.py` & `teradatamodelops-7.0.7b1/aoa/stats/store.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/util/artifacts.py` & `teradatamodelops-7.0.7b1/aoa/util/artifacts.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/util/byom.py` & `teradatamodelops-7.0.7b1/aoa/util/byom.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/util/connections.py` & `teradatamodelops-7.0.7b1/aoa/util/connections.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/aoa/util/sto.py` & `teradatamodelops-7.0.7b1/aoa/util/sto.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/scripts/tmo` & `teradatamodelops-7.0.7b1/scripts/tmo`

 * *Files 1% similar despite different names*

```diff
@@ -567,14 +567,15 @@
         name = args.name
         username = args.username
         password = args.password
         host = args.host
         database = args.database
         val_db = args.val_db
         byom_db = args.byom_db
+        logmech = args.logmech
 
     elif not (args.username or args.password or args.name or args.host):
         name = input_string(name="name", tooltip="Type the connection name")
         username = input_string(name="username", tooltip="Type the connection username")
         password = input_string(
             name="password",
             tooltip="Type the connection password (will not show)",
@@ -588,14 +589,17 @@
             name="VAL database ", required=True, tooltip="The VAL installation to use"
         )
         database = input_string(
             name="database",
             required=False,
             tooltip="Type the default database (optional)",
         )
+        logmech = input_string(
+            name="logmech", tooltip="The Logmech to use (TD2, LDAP or TDNEGO)"
+        )
 
     else:
         logging.error("Invalid arguments...")
         args.parent_parser.print_help()
         exit(1)
 
     import uuid
@@ -610,15 +614,15 @@
     connections.append(
         {
             "id": connection_id,
             "name": name,
             "username": username,
             "password": encrypted_password,
             "host": host,
-            "logmech": "TDNEGO",
+            "logmech": logmech,
             "database": database,
             "val_db": val_db,
             "byom_db": byom_db,
         }
     )
     connections_dict["connections"] = connections
 
@@ -903,15 +907,15 @@
         try:
             aoa_create_context()
             logging.debug(ct_query)
             execute_sql(ct_query)
         except Exception as ex:
             raise Exception("Could not create BYOM table: {}".format(ex)) from ex
 
-        print("BYOM table {} created successfully".format(args.metadata_table))
+        print("BYOM table {} created successfully".format(args.name))
     else:
         print(
             "Execution not requested, just showing DDL. To execute this DDL, add -e to the command."
         )
 
 
 def compute_stats(args, **kwargs):
@@ -1350,14 +1354,17 @@
         )
         subparser_add_connections.add_argument(
             "--byom-db",
             type=str,
             default="mldb",
             help="Configure BYOM installation db (default is mldb)",
         )
+        subparser_add_connections.add_argument(
+            "-l", "--logmech", type=str, help="Logmech to use"
+        )
         subparser_add_connections.set_defaults(
             func=add_connections, parent_parser=subparser_add_connections
         )
         subparser_remove_connections = subparser_connections.add_parser(
             "remove", help="Remove a local connection", parents=[common_parser]
         )
         subparser_remove_connections.add_argument(
```

### Comparing `teradatamodelops-7.0.6rc2/setup.py` & `teradatamodelops-7.0.7b1/setup.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/PKG-INFO` & `teradatamodelops-7.0.7b1/teradatamodelops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teradatamodelops
-Version: 7.0.6rc2
+Version: 7.0.7b1
 Summary: Python client for Teradata ModelOps (TMO)
 Home-page: 
 Author: Teradata
 Author-email: teradata.corporation@teradatacorporation.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -429,14 +429,19 @@
 ```
 
 
 ## Release Notes
 
 ### current
 
+- Explicitly ask for `logmech` when defining a local Vantage connection
+- Fixed `tmo connection create-byom-table` logging error
+
+### 7.0.6
+
 - Fixed compatibility issue with `teradataml>=20.0.0.0`
 - Minor formatting updates
 - Added user attributes API
 - Updated programmatic BYOM import examples
 
 ### 7.0.5
```

### Comparing `teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/SOURCES.txt` & `teradatamodelops-7.0.7b1/teradatamodelops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

