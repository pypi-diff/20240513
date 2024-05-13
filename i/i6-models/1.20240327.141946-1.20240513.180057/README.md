# Comparing `tmp/i6_models-1.20240327.141946.tar.gz` & `tmp/i6_models-1.20240513.180057.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/i6_models-1.20240327.141946.tar", last modified: Wed Mar 27 13:22:31 2024, max compression
+gzip compressed data, was "i6_models-1.20240513.180057.tar", last modified: Mon May 13 19:07:24 2024, max compression
```

## Comparing `i6_models-1.20240327.141946.tar` & `i6_models-1.20240513.180057.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-27 13:22:30.000000 i6_models-1.20240327.141946/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/__setup__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/assemblies/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/assemblies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/assemblies/conformer/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/assemblies/conformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/assemblies/conformer/conformer_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/assemblies/e_branchformer/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/assemblies/e_branchformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/assemblies/e_branchformer/e_branchformer_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/parts/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/blstm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/parts/conformer/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/conformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/conformer/convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/conformer/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/conformer/mhsa.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/conformer/norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/parts/e_branchformer/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/e_branchformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/e_branchformer/cgmlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/e_branchformer/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/parts/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/frontend/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/frontend/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/frontend/generic_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/parts/frontend/vgg_act.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/primitives/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/primitives/specaugment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models/util/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/i6_models/util/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/i6_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-27 13:22:30.000000 i6_models-1.20240327.141946/i6_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-27 13:22:30.000000 i6_models-1.20240327.141946/i6_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:22:30.000000 i6_models-1.20240327.141946/i6_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 13:22:30.000000 i6_models-1.20240327.141946/i6_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:22:31.000000 i6_models-1.20240327.141946/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/tests/test_blstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/tests/test_conformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/tests/test_e_branchformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34506 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/tests/test_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/tests/test_frontend_vgg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-03-27 13:22:18.000000 i6_models-1.20240327.141946/tests/test_generic_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.654066 i6_models-1.20240513.180057/
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-13 19:07:24.654066 i6_models-1.20240513.180057/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 19:07:24.000000 i6_models-1.20240513.180057/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.646066 i6_models-1.20240513.180057/i6_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/__setup__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.646066 i6_models-1.20240513.180057/i6_models/assemblies/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/assemblies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.650066 i6_models-1.20240513.180057/i6_models/assemblies/conformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/assemblies/conformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/assemblies/conformer/conformer_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.650066 i6_models-1.20240513.180057/i6_models/assemblies/e_branchformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/assemblies/e_branchformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/assemblies/e_branchformer/e_branchformer_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.650066 i6_models-1.20240513.180057/i6_models/parts/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/blstm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.650066 i6_models-1.20240513.180057/i6_models/parts/conformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/conformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/conformer/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/conformer/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/conformer/mhsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/conformer/norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.650066 i6_models-1.20240513.180057/i6_models/parts/e_branchformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/e_branchformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/e_branchformer/cgmlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/e_branchformer/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.650066 i6_models-1.20240513.180057/i6_models/parts/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/frontend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/frontend/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/frontend/generic_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/parts/frontend/vgg_act.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.650066 i6_models-1.20240513.180057/i6_models/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/primitives/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/primitives/specaugment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.650066 i6_models-1.20240513.180057/i6_models/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/i6_models/util/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.654066 i6_models-1.20240513.180057/i6_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-13 19:07:24.000000 i6_models-1.20240513.180057/i6_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-13 19:07:24.000000 i6_models-1.20240513.180057/i6_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:07:24.000000 i6_models-1.20240513.180057/i6_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 19:07:24.000000 i6_models-1.20240513.180057/i6_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:07:24.654066 i6_models-1.20240513.180057/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:24.654066 i6_models-1.20240513.180057/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/tests/test_blstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/tests/test_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/tests/test_e_branchformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34506 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/tests/test_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/tests/test_frontend_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-13 19:07:15.000000 i6_models-1.20240513.180057/tests/test_generic_frontend.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `i6_models-1.20240327.141946/.gitignore` & `i6_models-1.20240513.180057/.gitignore`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/CONTRIBUTING.md` & `i6_models-1.20240513.180057/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/LICENSE` & `i6_models-1.20240513.180057/LICENSE`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/PKG-INFO` & `i6_models-1.20240513.180057/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i6_models
-Version: 1.20240327.141946
+Version: 1.20240513.180057
 Summary: A collection of PyTorch NN models and parts.
 Home-page: https://github.com/rwth-i6/i6_models/
 Author: Christoph Lüscher, Nick Rossenbach, Benedikt Hilmes, Jingjing Xu, Mohammad Zeineldeen, Albert Zeyer, Peter Vieting, Simon Berger, Eugen Beck, Ping Zheng, Wilfried Michel
 Author-email: luescher@cs.rwth-aachen.de, rossenbach@cs.rwth-aachen.de, hilmes@cs.rwth-aachen.de, jxu@cs.rwth-aachen.de, zeineldeen@cs.rwth-aachen.de, zeyer@cs.rwth-aachen.de, vieting@cs.rwth-aachen.de, sberger@cs.rwth-aachen.de, ebeck@apptek.com, p.zheng@apptek.com, wmichel@apptek.com
 License: Mozilla Public License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `i6_models-1.20240327.141946/i6_models/__setup__.py` & `i6_models-1.20240513.180057/i6_models/__setup__.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/assemblies/conformer/conformer_v1.py` & `i6_models-1.20240513.180057/i6_models/assemblies/conformer/conformer_v1.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/assemblies/e_branchformer/e_branchformer_v1.py` & `i6_models-1.20240513.180057/i6_models/assemblies/e_branchformer/e_branchformer_v1.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/config.py` & `i6_models-1.20240513.180057/i6_models/config.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/blstm.py` & `i6_models-1.20240513.180057/i6_models/parts/blstm.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/conformer/convolution.py` & `i6_models-1.20240513.180057/i6_models/parts/conformer/convolution.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/conformer/feedforward.py` & `i6_models-1.20240513.180057/i6_models/parts/conformer/feedforward.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/conformer/mhsa.py` & `i6_models-1.20240513.180057/i6_models/parts/conformer/mhsa.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/conformer/norm.py` & `i6_models-1.20240513.180057/i6_models/parts/conformer/norm.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/e_branchformer/cgmlp.py` & `i6_models-1.20240513.180057/i6_models/parts/e_branchformer/cgmlp.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/e_branchformer/merge.py` & `i6_models-1.20240513.180057/i6_models/parts/e_branchformer/merge.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/frontend/common.py` & `i6_models-1.20240513.180057/i6_models/parts/frontend/common.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/frontend/generic_frontend.py` & `i6_models-1.20240513.180057/i6_models/parts/frontend/generic_frontend.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/parts/frontend/vgg_act.py` & `i6_models-1.20240513.180057/i6_models/parts/frontend/vgg_act.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/primitives/feature_extraction.py` & `i6_models-1.20240513.180057/i6_models/primitives/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/primitives/specaugment.py` & `i6_models-1.20240513.180057/i6_models/primitives/specaugment.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models/util/compat.py` & `i6_models-1.20240513.180057/i6_models/util/compat.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/i6_models.egg-info/PKG-INFO` & `i6_models-1.20240513.180057/i6_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: i6-models
-Version: 1.20240327.141946
+Name: i6_models
+Version: 1.20240513.180057
 Summary: A collection of PyTorch NN models and parts.
 Home-page: https://github.com/rwth-i6/i6_models/
 Author: Christoph Lüscher, Nick Rossenbach, Benedikt Hilmes, Jingjing Xu, Mohammad Zeineldeen, Albert Zeyer, Peter Vieting, Simon Berger, Eugen Beck, Ping Zheng, Wilfried Michel
 Author-email: luescher@cs.rwth-aachen.de, rossenbach@cs.rwth-aachen.de, hilmes@cs.rwth-aachen.de, jxu@cs.rwth-aachen.de, zeineldeen@cs.rwth-aachen.de, zeyer@cs.rwth-aachen.de, vieting@cs.rwth-aachen.de, sberger@cs.rwth-aachen.de, ebeck@apptek.com, p.zheng@apptek.com, wmichel@apptek.com
 License: Mozilla Public License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `i6_models-1.20240327.141946/i6_models.egg-info/SOURCES.txt` & `i6_models-1.20240513.180057/i6_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/setup.py` & `i6_models-1.20240513.180057/setup.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/tests/test_blstm.py` & `i6_models-1.20240513.180057/tests/test_blstm.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/tests/test_config.py` & `i6_models-1.20240513.180057/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/tests/test_conformer.py` & `i6_models-1.20240513.180057/tests/test_conformer.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/tests/test_e_branchformer.py` & `i6_models-1.20240513.180057/tests/test_e_branchformer.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/tests/test_feature_extraction.py` & `i6_models-1.20240513.180057/tests/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/tests/test_frontend_vgg.py` & `i6_models-1.20240513.180057/tests/test_frontend_vgg.py`

 * *Files identical despite different names*

### Comparing `i6_models-1.20240327.141946/tests/test_generic_frontend.py` & `i6_models-1.20240513.180057/tests/test_generic_frontend.py`

 * *Files identical despite different names*

