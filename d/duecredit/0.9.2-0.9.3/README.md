# Comparing `tmp/duecredit-0.9.2.tar.gz` & `tmp/duecredit-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duecredit-0.9.2.tar", last modified: Wed Feb  1 14:27:42 2023, max compression
+gzip compressed data, was "duecredit-0.9.3.tar", last modified: Sun Nov 12 15:56:53 2023, max compression
```

## Comparing `duecredit-0.9.2.tar` & `duecredit-0.9.3.tar`

### file list

```diff
@@ -1,80 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.215103 duecredit-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-01 14:27:05.000000 duecredit-0.9.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-02-01 14:27:05.000000 duecredit-0.9.2/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-02-01 14:27:33.000000 duecredit-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-02-01 14:27:05.000000 duecredit-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-02-01 14:27:05.000000 duecredit-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-01 14:27:05.000000 duecredit-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-02-01 14:27:42.215103 duecredit-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-02-01 14:27:05.000000 duecredit-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.211103 duecredit-0.9.2/duecredit/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.211103 duecredit-0.9.2/duecredit/cmdline/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/cmdline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/cmdline/cmd_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/cmdline/cmd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/cmdline/common_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/cmdline/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/cmdline/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/dueswitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/entries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.215103 duecredit-0.9.2/duecredit/injections/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/injector.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_biosig.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_dipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_mne.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_nibabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_nipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_nipype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_psychopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_skimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/injections/mod_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14582 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.215103 duecredit-0.9.2/duecredit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.207103 duecredit-0.9.2/duecredit/tests/envs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.215103 duecredit-0.9.2/duecredit/tests/envs/nolxml/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/envs/nolxml/lxml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.215103 duecredit-0.9.2/duecredit/tests/mod/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/mod/imported.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/mod/submod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_dueswitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_import_doi
--rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_injections.py
--rw-r--r--   0 runner    (1001) docker     (123)    21379 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-01 14:27:42.000000 duecredit-0.9.2/duecredit/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-02-01 14:27:05.000000 duecredit-0.9.2/duecredit/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.211103 duecredit-0.9.2/duecredit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-02-01 14:27:42.000000 duecredit-0.9.2/duecredit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-02-01 14:27:42.000000 duecredit-0.9.2/duecredit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 14:27:42.000000 duecredit-0.9.2/duecredit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-01 14:27:42.000000 duecredit-0.9.2/duecredit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-01 14:27:42.000000 duecredit-0.9.2/duecredit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-01 14:27:42.000000 duecredit-0.9.2/duecredit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:27:42.215103 duecredit-0.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-01 14:27:05.000000 duecredit-0.9.2/examples/example_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-01 14:27:05.000000 duecredit-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-01 14:27:42.215103 duecredit-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4827 2023-02-01 14:27:05.000000 duecredit-0.9.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-01 14:27:05.000000 duecredit-0.9.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.148357 duecredit-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-12 15:56:24.000000 duecredit-0.9.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)    17709 2023-11-12 15:56:42.000000 duecredit-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2023-11-12 15:56:24.000000 duecredit-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2023-11-12 15:56:24.000000 duecredit-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-11-12 15:56:24.000000 duecredit-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2023-11-12 15:56:53.148357 duecredit-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14721 2023-11-12 15:56:24.000000 duecredit-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.144357 duecredit-0.9.3/duecredit/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.144357 duecredit-0.9.3/duecredit/cmdline/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/cmdline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/cmdline/cmd_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/cmdline/cmd_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/cmdline/common_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/cmdline/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7702 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/cmdline/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17526 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/dueswitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/entries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.148357 duecredit-0.9.3/duecredit/injections/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16890 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/injector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_biosig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_dipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_mne.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_nibabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_nipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_nipype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_psychopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_skimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/injections/mod_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14364 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7978 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.148357 duecredit-0.9.3/duecredit/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.140357 duecredit-0.9.3/duecredit/tests/envs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.148357 duecredit-0.9.3/duecredit/tests/envs/nolxml/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/envs/nolxml/lxml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.148357 duecredit-0.9.3/duecredit/tests/mod/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/mod/imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/mod/submod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10374 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_dueswitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_import_doi
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_injections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-12 15:56:53.000000 duecredit-0.9.3/duecredit/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2023-11-12 15:56:24.000000 duecredit-0.9.3/duecredit/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.144357 duecredit-0.9.3/duecredit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2023-11-12 15:56:53.000000 duecredit-0.9.3/duecredit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-11-12 15:56:53.000000 duecredit-0.9.3/duecredit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 15:56:53.000000 duecredit-0.9.3/duecredit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-12 15:56:53.000000 duecredit-0.9.3/duecredit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-12 15:56:53.000000 duecredit-0.9.3/duecredit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-12 15:56:53.000000 duecredit-0.9.3/duecredit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 15:56:53.148357 duecredit-0.9.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2023-11-12 15:56:24.000000 duecredit-0.9.3/examples/example_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2023-11-12 15:56:24.000000 duecredit-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2023-11-12 15:56:53.148357 duecredit-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4838 2023-11-12 15:56:24.000000 duecredit-0.9.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2023-11-12 15:56:24.000000 duecredit-0.9.3/tox.ini
```

### Comparing `duecredit-0.9.2/CHANGELOG.md` & `duecredit-0.9.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+# 0.9.3 (Sun Nov 12 2023)
+
+#### 🐛 Bug Fix
+
+- ENH: codespell [#185](https://github.com/duecredit/duecredit/pull/185) ([@yarikoptic](https://github.com/yarikoptic))
+
+#### 🏠 Internal
+
+- RF: remove remaining usage of SIX, and thus move away fully from Python 2 [#186](https://github.com/duecredit/duecredit/pull/186) ([@a-detiste](https://github.com/a-detiste) [@yarikoptic](https://github.com/yarikoptic))
+- Ignore "vor" which is now detected as typo [#186](https://github.com/duecredit/duecredit/pull/186) ([@yarikoptic](https://github.com/yarikoptic))
+
+#### 🧪 Tests
+
+- Use teardown_method instead of nose-y teardown [#190](https://github.com/duecredit/duecredit/pull/190) ([@yarikoptic](https://github.com/yarikoptic))
+- Move from Travis to github workflow, disable coveralls [#187](https://github.com/duecredit/duecredit/pull/187) ([@yarikoptic](https://github.com/yarikoptic))
+
+#### Authors: 2
+
+- Alexandre Detiste ([@a-detiste](https://github.com/a-detiste))
+- Yaroslav Halchenko ([@yarikoptic](https://github.com/yarikoptic))
+
+---
+
 # 0.9.2 (Wed Feb 01 2023)
 
 #### 🐛 Bug Fix
 
 - Tell LGTM to ignore unused imports in stub.py [#179](https://github.com/duecredit/duecredit/pull/179) ([@jwodder](https://github.com/jwodder))
 
 #### 🏠 Internal
```

### Comparing `duecredit-0.9.2/CONTRIBUTING.md` & `duecredit-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/LICENSE` & `duecredit-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/PKG-INFO` & `duecredit-0.9.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: duecredit
-Version: 0.9.2
-Summary: Publications (and donations) tracer
-Home-page: https://github.com/duecredit/duecredit
-Author: Yaroslav Halchenko, Matteo Visconti di Oleggio Castello
-Author-email: yoh@onerussian.com
-License: 2-clause BSD License
-Keywords: citation tracing
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Environment :: Other Environment
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Legal Industry
-Classifier: Intended Audience :: Other Audience
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Documentation
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
 # duecredit
 
 
 [![Build Status](https://travis-ci.org/duecredit/duecredit.svg?branch=master)](https://travis-ci.org/duecredit/duecredit)
 [![Coverage Status](https://coveralls.io/repos/duecredit/duecredit/badge.svg)](https://coveralls.io/r/duecredit/duecredit)
 [![DOI](https://zenodo.org/badge/DOI/110.5281/zenodo.3376260.svg)](https://doi.org/10.5281/zenodo.3376260)
 [![PyPI version fury.io](https://badge.fury.io/py/duecredit.svg)](https://pypi.python.org/pypi/duecredit/)
```

### Comparing `duecredit-0.9.2/README.md` & `duecredit-0.9.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+Metadata-Version: 2.1
+Name: duecredit
+Version: 0.9.3
+Summary: Publications (and donations) tracer
+Home-page: https://github.com/duecredit/duecredit
+Author: Yaroslav Halchenko, Matteo Visconti di Oleggio Castello
+Author-email: yoh@onerussian.com
+License: 2-clause BSD License
+Keywords: citation tracing
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Environment :: Other Environment
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Legal Industry
+Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: citeproc-py>=0.4
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: vcrpy; extra == "tests"
+Requires-Dist: contextlib2; extra == "tests"
+
 # duecredit
 
 
 [![Build Status](https://travis-ci.org/duecredit/duecredit.svg?branch=master)](https://travis-ci.org/duecredit/duecredit)
 [![Coverage Status](https://coveralls.io/repos/duecredit/duecredit/badge.svg)](https://coveralls.io/r/duecredit/duecredit)
 [![DOI](https://zenodo.org/badge/DOI/110.5281/zenodo.3376260.svg)](https://doi.org/10.5281/zenodo.3376260)
 [![PyPI version fury.io](https://badge.fury.io/py/duecredit.svg)](https://pypi.python.org/pypi/duecredit/)
```

### Comparing `duecredit-0.9.2/duecredit/__init__.py` & `duecredit-0.9.3/duecredit/__init__.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/__main__.py` & `duecredit-0.9.3/duecredit/__main__.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/cmdline/cmd_summary.py` & `duecredit-0.9.3/duecredit/cmdline/cmd_summary.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/cmdline/cmd_test.py` & `duecredit-0.9.3/duecredit/cmdline/cmd_test.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/cmdline/common_args.py` & `duecredit-0.9.3/duecredit/cmdline/common_args.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/cmdline/helpers.py` & `duecredit-0.9.3/duecredit/cmdline/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     opt_kwargs = opt_tmpl[2].copy()
     opt_kwargs.update(kwargs)
     if names is None:
         parser.add_argument(*opt_tmpl[1], **opt_kwargs)
     else:
         parser.add_argument(*names, **opt_kwargs)
 
-class RegexpType(object):
+class RegexpType:
     """Factory for creating regular expression types for argparse
 
     DEPRECATED AFAIK -- now things are in the config file...
     but we might provide a mode where we operate solely from cmdline
     """
     def __call__(self, string):
         if string:
```

### Comparing `duecredit-0.9.2/duecredit/cmdline/main.py` & `duecredit-0.9.3/duecredit/cmdline/main.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/collector.py` & `duecredit-0.9.3/duecredit/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 """Citation and citations Collector classes"""
 
 import os
 import sys
 from functools import wraps
 
-from six import iteritems, itervalues
-
 from .config import DUECREDIT_FILE
 from .entries import DueCreditEntry
 from .stub import InactiveDueCreditCollector
 from .io import TextOutput, PickleOutput
 from .utils import never_fail, borrowdoc
 from .versions import external_versions
 from collections import namedtuple
 
 import logging
 lgr = logging.getLogger('duecredit.collector')
 
 CitationKey = namedtuple('CitationKey', ['path', 'entry_key'])
 
-class Citation(object):
+class Citation:
     """Encapsulates citations and information on their use"""
 
     def __init__(self, entry, description=None, path=None, version=None,
                  cite_module=False, tags=['implementation']):
         """Cite a reference
 
         Parameters
@@ -170,15 +168,15 @@
     def get_key(path, entry_key):
         return CitationKey(path, entry_key)
 
     def set_entry(self, newentry):
         self._entry = newentry
 
 
-class DueCreditCollector(object):
+class DueCreditCollector:
     """Collect the references
 
     The mighty beast which will might become later a proxy on the way to
     talk to a real collector
 
     Parameters
     ----------
@@ -270,37 +268,37 @@
                     package = modname.split('.', 1)[0]
                 else:
                     package = modname
 
                 # package_loaded = sys.modules.get(package)
                 # if package_loaded:
                 #     # find the citation for that module
-                #     for citation in itervalues(self.citations):
+                #     for citation in self.citations.values():
                 #         if citation.package == package \
                 #                 and not citation.version:
                 version = external_versions[package]
             citation.version = version
 
         return citation
 
     def _citations_fromentrykey(self):
         """Return a dictionary with the current citations indexed by the entry key"""
         citations_key = dict()
-        for (path, entry_key), citation in iteritems(self.citations):
+        for (path, entry_key), citation in self.citations.items():
             if entry_key not in citations_key:
                 citations_key[entry_key] = citation
 
         return citations_key
 
 
     @staticmethod
     def _args_match_conditions(conditions, *fargs, **fkwargs):
         """Helper to identify when to trigger citation given parameters to the function call
         """
-        for (argpos, kwarg), values in iteritems(conditions):
+        for (argpos, kwarg), values in conditions.items():
             # main logic -- assess default and if get to the next one if
             # given argument is not present
             if not ((len(fargs) > argpos) or (kwarg in fkwargs)):
                 if not ('DC_DEFAULT' in values):
                     # if value was specified but not provided and not default
                     # conditions are not satisfied
                     return False
@@ -365,15 +363,15 @@
         ...     if method == 'purge': return "crap"
         ...     elif method == 'drug': return "swallow"
         >>> relief("doesn't matter")
         'crap'
 
         Conditional based on the state of the object
 
-        >>> class Citeable(object):
+        >>> class Citeable:
         ...     def __init__(self, param=None):
         ...         self.param = param
         ...     @due.dcite('XXX00', description="The same good old relief",
         ...                conditions={(0, 'self.param'): {'magic'}})
         ...     def __call__(self, data):
         ...         return sum(data)
         >>> Citeable('magic')([1, 2])
@@ -437,15 +435,15 @@
     def __str__(self):
         return self.__class__.__name__ + \
             ' {0:d} entries, {1:d} citations'.format(
                 len(self._entries), len(self.citations))
 
 
 # TODO: redo heavily -- got very messy
-class CollectorSummary(object):
+class CollectorSummary:
     """A helper which would take care about exporting citations upon its Death
     """
     def __init__(self, collector, outputs="stdout,pickle", fn=DUECREDIT_FILE):
         self._due = collector
         self.fn = fn
         # for now decide on output "format" right here
         self._outputs = [
@@ -466,9 +464,9 @@
             raise NotImplementedError()
 
     def dump(self):
         for output in self._outputs:
             output.dump()
 
 
-# TODO:  provide HTML, MD, RST etc formattings
+# TODO:  provide HTML, MD, RST etc output formats
```

### Comparing `duecredit-0.9.2/duecredit/config.py` & `duecredit-0.9.3/duecredit/config.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/dueswitch.py` & `duecredit-0.9.3/duecredit/dueswitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             return _get_inactive_due()
     else:
         due_ = DueCreditCollector()
 
     return due_
 
 
-class DueSwitch(object):
+class DueSwitch:
     """Adapter between two types of collectors -- Inactive and Active
 
     Once activated though, cannot be fully deactivated since it would inject
     duecredit decorators and register an event atexit.
     """
     def __init__(self, inactive, active, activate=False):
         self.__active = None
@@ -124,8 +124,8 @@
                 self.__prepare_exit_and_injections()
             except Exception as e:
                 lgr.error("Failed to prepare injections etc: %s" % str(e))
             finally:
                 self.__activations_done = True
 
 
-due = DueSwitch(_get_inactive_due(), _get_active_due(), _get_duecredit_enable())
+due = DueSwitch(_get_inactive_due(), _get_active_due(), _get_duecredit_enable())
```

### Comparing `duecredit-0.9.2/duecredit/entries.py` & `duecredit-0.9.3/duecredit/entries.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 #
 #   See COPYING file distributed along with the duecredit package for the
 #   copyright and license terms.   Originates from datalad package distributed
 #   under MIT license
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 import re
-from six import PY2
 
 import logging
 lgr = logging.getLogger('duecredit.entries')
 
 
-class DueCreditEntry(object):
+class DueCreditEntry:
     def __init__(self, rawentry, key=None):
         self._rawentry = rawentry
         self._key = key or rawentry.lower()
 
     def __eq__(self, other):
         return (
             (self._rawentry == other._rawentry) and
@@ -30,18 +29,15 @@
 
     @property
     def key(self):
         return self.get_key()
 
     @property
     def rawentry(self):
-        if PY2:
-            return unicode(self._rawentry)
-        else:
-            return self._rawentry
+        return self._rawentry
 
     def _process_rawentry(self):
         pass
 
     def __repr__(self):
         args = [repr(self._rawentry),
                 "key={0}".format(repr(self._key))]
```

### Comparing `duecredit-0.9.2/duecredit/injections/__init__.py` & `duecredit-0.9.3/duecredit/injections/__init__.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/injector.py` & `duecredit-0.9.3/duecredit/injections/injector.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from glob import glob
 import sys
 from functools import wraps
 
 import logging
 from ..log import lgr
 
-from six import iteritems
 import builtins as __builtin__
 
 
 __all__ = ['DueCreditInjector', 'find_object']
 
 # TODO: move elsewhere
 def _short_str(obj, l=30):
@@ -59,15 +58,15 @@
 # We will keep a very original __import__ to mitigate cases of buggy python
 # behavior, see e.g.
 # https://github.com/duecredit/duecredit/issues/40
 # But we will also keep the __import__ as of 'activate' call state so we could
 # stay friendly to anyone else who might decorate __import__ as well
 _very_orig_import = __builtin__.__import__
 
-class DueCreditInjector(object):
+class DueCreditInjector:
     """Takes care about "injecting" duecredit references into 3rd party modules upon their import
 
     First entries to be "injected" need to be add'ed to the instance.
     To not incur significant duecredit startup penalty, those entries are added
     for a corresponding package only whenever corresponding top-level module gets
     imported.
     """
@@ -193,15 +192,15 @@
         except KeyError:
             lgr.warning("Failed to access module %s among sys.modules" % mod_name)
             return
 
         # go through the known entries and register them within the collector, and
         # decorate corresponding methods
         # There could be multiple records per module
-        for obj_path, obj_entry_records in iteritems(self._entry_records[mod_name]):
+        for obj_path, obj_entry_records in self._entry_records[mod_name].items():
             parent, obj_name = None, None
             if obj_path:
                 # so we point to an object within the mod
                 try:
                     parent, obj_name, obj = find_object(mod, obj_path)
                 except (KeyError, AttributeError) as e:
                     lgr.warning("Could not find %s in module %s: %s" % (obj_path, mod, e))
```

### Comparing `duecredit-0.9.2/duecredit/injections/mod_biosig.py` & `duecredit-0.9.3/duecredit/injections/mod_biosig.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_dipy.py` & `duecredit-0.9.3/duecredit/injections/mod_dipy.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_matplotlib.py` & `duecredit-0.9.3/duecredit/injections/mod_matplotlib.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_mdp.py` & `duecredit-0.9.3/duecredit/injections/mod_mdp.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_mne.py` & `duecredit-0.9.3/duecredit/injections/mod_mne.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_nibabel.py` & `duecredit-0.9.3/duecredit/injections/mod_nibabel.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_nipy.py` & `duecredit-0.9.3/duecredit/injections/mod_nipy.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_nipype.py` & `duecredit-0.9.3/duecredit/injections/mod_nipype.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_numpy.py` & `duecredit-0.9.3/duecredit/injections/mod_numpy.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_pandas.py` & `duecredit-0.9.3/duecredit/injections/mod_pandas.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_psychopy.py` & `duecredit-0.9.3/duecredit/injections/mod_psychopy.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_scipy.py` & `duecredit-0.9.3/duecredit/injections/mod_scipy.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_skimage.py` & `duecredit-0.9.3/duecredit/injections/mod_skimage.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/injections/mod_sklearn.py` & `duecredit-0.9.3/duecredit/injections/mod_sklearn.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/io.py` & `duecredit-0.9.3/duecredit/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import locale
 import time
 from collections import defaultdict
 import copy
 from os.path import dirname, exists
 import pickle
 import tempfile
-from six import PY2, itervalues, iteritems
 import warnings
 import platform
 from time import sleep
 
 from .config import CACHE_DIR, DUECREDIT_FILE
 from .entries import BibTeX, Doi, Text, Url
 from .log import lgr
@@ -45,16 +44,14 @@
 def import_doi(doi, sleep=0.5, retries=10):
     import requests
     cached = get_doi_cache_file(doi)
 
     if exists(cached):
         with open(cached) as f:
             doi = f.read()
-            if PY2:
-                return doi.decode('utf-8')
             return doi
 
     # else -- fetch it
     headers = {'Accept': 'application/x-bibtex; charset=utf-8'}
     url = 'https://doi.org/' + doi
     while retries > 0:
         lgr.debug("Submitting GET to %s with headers %s", url, headers)
@@ -74,31 +71,28 @@
                          #'BibTeX response was: %(bibtex)s'
                          % locals())
     if not exists(cached):
         cache_dir = dirname(cached)
         if not exists(cache_dir):
             os.makedirs(cache_dir)
         with open(cached, 'w') as f:
-            if PY2:
-                f.write(bibtex.encode('utf-8'))
-            else:
-                f.write(bibtex)
+            f.write(bibtex)
     return bibtex
 
 
 def _is_contained(toppath, subpath):
     if ':' not in toppath:
         return ((toppath == subpath) or
                 (subpath.startswith(toppath + '.')) or
                 (subpath.startswith(toppath + ':')))
     else:
         return subpath.startswith(toppath + '.')
 
 
-class Output(object):
+class Output:
     """A generic class for setting up citations that then will be outputted
     differently (e.g., Bibtex, Text, etc.)"""
     def __init__(self, fd, collector):
         self.fd = fd
         self.collector = collector
 
     def _get_collated_citations(self, tags=None, all_=None):
@@ -111,24 +105,24 @@
             all_ = os.environ.get('DUECREDIT_REPORT_ALL', '').lower() in {'1', 'true', 'yes', 'on'}
         tags = set(tags)
 
         citations = self.collector.citations
         if tags != {'*'}:
             # Filter out citations based on tags
             citations = dict((k, c)
-                             for k, c in iteritems(citations)
+                             for k, c in citations.items()
                              if tags.intersection(c.tags))
 
         packages = defaultdict(list)
         modules = defaultdict(list)
         objects = defaultdict(list)
 
         # store the citations according to their path and divide them into
         # the right level
-        for (path, entry_key), citation in iteritems(citations):
+        for (path, entry_key), citation in citations.items():
             if ':' in path:
                 objects[path].append(citation)
             elif '.' in path:
                 modules[path].append(citation)
             else:
                 packages[path].append(citation)
 
@@ -347,15 +341,15 @@
 
     biblio_out = bibliography.bibliography()
     assert(len(biblio_out) == 1)
     biblio_out = ''.join(biblio_out[0])
     return biblio_out # if biblio_out else str(bibtex_entry)
 
 # TODO: harmonize order of arguments
-class PickleOutput(object):
+class PickleOutput:
     def __init__(self, collector, fn=DUECREDIT_FILE):
         self.collector = collector
         self.fn = fn
 
     def dump(self):
         with open(self.fn, 'wb') as f:
             pickle.dump(self.collector, f)
```

### Comparing `duecredit-0.9.2/duecredit/log.py` & `duecredit-0.9.3/duecredit/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     base = basename(s)
     if base.endswith('.py'):
         base = base[:-3]
     if base in set(['base', '__init__']):
         base = basename(dirname(s)) + '.' + base
     return base
 
-class TraceBack(object):
+class TraceBack:
     """Customized traceback to be included in debug messages
     """
 
     def __init__(self, collide=False):
         """Initialize TraceBack metric
 
         Parameters
@@ -134,15 +134,15 @@
         record.msg = record.msg.replace("\n", "\n| ")
         if self._tb:
             record.msg = self._tb() + "  " + record.msg
 
         return logging.Formatter.format(self, record)
 
 
-class LoggerHelper(object):
+class LoggerHelper:
     """Helper to establish and control a Logger"""
 
     def __init__(self, name='duecredit'):
         self.name = name
         self.lgr = logging.getLogger(name)
 
     def _get_environ(self, var, default=None):
```

### Comparing `duecredit-0.9.2/duecredit/parsers.py` & `duecredit-0.9.3/duecredit/parsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import re
-
 def extract_references_from_rst(rst):
     # for now will be very simple, just trying to separate
     # then up until the end or another section starting
     pass
 
 def test_extract_references_from_rst():
     # some obscure examples of how people specify references
```

### Comparing `duecredit-0.9.2/duecredit/stub.py` & `duecredit-0.9.3/duecredit/stub.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 Copyright:  2015-2021  DueCredit developers
 License:    BSD-2
 """
 
 __version__ = '0.0.9'
 
 
-class InactiveDueCreditCollector(object):
+class InactiveDueCreditCollector:
     """Just a stub at the Collector which would not do anything"""
     def _donothing(self, *args, **kwargs):
         """Perform no good and no bad"""
         pass
 
     def dcite(self, *args, **kwargs):
         """If I could cite I would"""
```

### Comparing `duecredit-0.9.2/duecredit/tests/mod/imported.py` & `duecredit-0.9.3/duecredit/tests/mod/imported.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 def testfunc1(arg1, kwarg1=None):
     """custom docstring"""
     return "testfunc1: %s, %s" % (arg1, kwarg1)
 
 
-class TestClass1(object):
+class TestClass1:
     """wrong custom docstring"""
     def testmeth1(self, arg1, kwarg1=None):
         """custom docstring"""
         return "TestClass1.testmeth1: %s, %s" % (arg1, kwarg1)
 
 
-class TestClass12(object):
+class TestClass12:
     """wrong custom docstring"""
-    class Embed(object):
+    class Embed:
         """wrong custom docstring"""
         def testmeth1(self, arg1, kwarg1=None):
             """custom docstring"""
             return "TestClass12.Embed.testmeth1: %s, %s" % (arg1, kwarg1)
```

### Comparing `duecredit-0.9.2/duecredit/tests/test__main__.py` & `duecredit-0.9.3/duecredit/tests/test__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #   copyright and license terms.
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 
 import sys
 import pytest
 
-from six.moves import StringIO
+from io import StringIO
 
 from .. import __main__, __version__
 from .. import due
 
 
 def test_main_help(monkeypatch):
     # Patch stdout
```

### Comparing `duecredit-0.9.2/duecredit/tests/test_api.py` & `duecredit-0.9.3/duecredit/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     # dcite  for decorator cite
     # cite specific functionality if/when it gets called up
     @due.dcite('XXX00', description="Provides an answer for meaningless existence")
     def purpose_of_life():
         return None
 
-    class Child(object):
+    class Child:
         # Conception process is usually way too easy to be referenced
         def __init__(self):
             pass
 
         # including functionality within/by the methods
         @due.dcite('XXX00')
         def birth(self, gender):
@@ -125,15 +125,18 @@
 
     monkeypatch.setitem(os.environ, 'PYTHONPATH', "%s:%s" % (badlxml_path, os.environ.get('PYTHONPATH', '')))
     ret, out, err = run_python_command('import lxml')
     assert ret == 1
     assert 'ImportError' in err
 
     ret, out, err = run_python_command('import duecredit')
-    assert err == ''
+    if "CoverageWarning" not in err:
+        # TODO: deal with that warning 
+        # "--include is ignored because --source is set"
+        assert err == ''
     assert out == ''
     assert ret == 0
 
 
 @pytest.mark.parametrize(
     "env", [{},
             {'DUECREDIT_ENABLE': 'yes'},
```

### Comparing `duecredit-0.9.2/duecredit/tests/test_cmdline.py` & `duecredit-0.9.3/duecredit/tests/test_cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 #
 #   See COPYING file distributed along with the duecredit package for the
 #   copyright and license terms.
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 
 import sys
+from io import StringIO
 
-from six.moves import StringIO
 import pytest
 
 from .. import __version__
 from ..cmdline import main
 
 
 def test_import():
```

### Comparing `duecredit-0.9.2/duecredit/tests/test_collector.py` & `duecredit-0.9.3/duecredit/tests/test_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         @due.dcite("XXX0", path='method')
         def method(arg1, kwarg2="blah"):
             """docstring"""
             assert arg1 == "magical"
             assert kwarg2 == 1
             return "load"
 
-        class SomeClass(object):
+        class SomeClass:
             @due.dcite("XXX0", path='someclass:method')
             def method(self, arg1, kwarg2="blah"):
                 """docstring"""
                 assert arg1 == "magical"
                 assert kwarg2 == 1
                 return "load"
 
@@ -145,15 +145,15 @@
             citation = due.citations[("someclass:method", "XXX0")]
             assert citation.path == "someclass:method"
             assert citation.count == 1
 
             # And we explicitly stated that module need to be cited
             assert citation.cite_module
 
-        class SomeClass2(object):
+        class SomeClass2:
             # Used to test for classes that are not instantiated
             @due.dcite("XXX0", path="some.module.without.method")
             def method2(self, arg1, kwarg2="blah"):
                 assert arg1 == "magical"
                 return "load"
 
         # and a method pointing to the module
@@ -245,15 +245,15 @@
 
 
 def test_dcite_match_conditions_method():
 
     due = DueCreditCollector()
     due.add(BibTeX(_sample_bibtex))
 
-    class Citeable(object):
+    class Citeable:
         def __init__(self, param=None):
             self.param = param
 
         @due.dcite("XXX0", path='obj.callable',
                    conditions={(2, "kwarg2"): {"blah", "DC_DEFAULT"},
                                (0, 'self.param'): {"paramvalue"}  # must be matched
                                })
```

### Comparing `duecredit-0.9.2/duecredit/tests/test_dueswitch.py` & `duecredit-0.9.3/duecredit/tests/test_dueswitch.py`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/tests/test_entries.py` & `duecredit-0.9.3/duecredit/tests/test_entries.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 import random
 import re
 import pickle
 import os
 import pytest
 
-from six.moves import StringIO
-from six import text_type
+from io import StringIO
 
 import duecredit.io
 from ..collector import DueCreditCollector, Citation
 from .test_collector import _sample_bibtex, _sample_doi, _sample_bibtex2
 from ..entries import BibTeX, Doi, Text, Url
 
 
@@ -31,8 +30,8 @@
 
     assert Doi("123/1", 'key') == Doi("123/1", 'key')
     assert Url("http://123/1", 'key') == Url("http://123/1", 'key')
 
 
 def test_sugaring_api():
     assert Url("http://1.com").url == "http://1.com"
-    assert Doi("1.com").doi == "1.com"
+    assert Doi("1.com").doi == "1.com"
```

### Comparing `duecredit-0.9.2/duecredit/tests/test_import_doi` & `duecredit-0.9.3/duecredit/tests/test_import_doi`

 * *Files identical despite different names*

### Comparing `duecredit-0.9.2/duecredit/tests/test_injections.py` & `duecredit-0.9.3/duecredit/tests/test_injections.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,15 @@
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 
 import gc
 import sys
 import pytest
 
-from six import viewvalues, PY2
-
-if PY2:
-    import __builtin__
-else:
-    import builtins as __builtin__
+import builtins as __builtin__
 _orig__import__ = __builtin__.__import__
 
 from duecredit.collector import DueCreditCollector
 from duecredit.entries import Doi
 import duecredit.tests.mod as mod
 
 from ..injections.injector import DueCreditInjector, find_object, get_modules_for_injection
@@ -32,23 +27,23 @@
 except ImportError:
     _have_mvpa2 = False
 
 from logging import getLogger
 lgr = getLogger('duecredit.tests.injector')
 
 
-class TestActiveInjector(object):
-    def setup(self):
+class TestActiveInjector:
+    def setup_method(self):
         lgr.log(5, "Setting up for a TestActiveInjector test")
         self._cleanup_modules()
         self.due = DueCreditCollector()
         self.injector = DueCreditInjector(collector=self.due)
         self.injector.activate(retrospect=False)  # numpy might be already loaded...
 
-    def teardown(self):
+    def teardown_method(self):
         lgr.log(5, "Tearing down after a TestActiveInjector test")
         # gc might not pick up inj after some tests complete
         # so we will always deactivate explicitly
         self.injector.deactivate()
         assert __builtin__.__import__ is _orig__import__
         self._cleanup_modules()
 
@@ -84,15 +79,15 @@
         # TODO: awkwardly 'ret' is not found in the scope while running pytest
         # under python3.4, although present in locals()... WTF?
         assert locals_['ret'] == "%s: None, somevalue" % func
         assert len(self.due._entries) == 1
         assert len(self.due.citations) == 1
 
         # TODO: there must be a cleaner way to get first value
-        citation = list(viewvalues(self.due.citations))[0]
+        citation = list(self.due.citations.values())[0]
         # TODO: ATM we don't allow versioning of the submodules -- we should
         # assert_equal(citation.version, '0.5')
         # ATM it will be the duecredit's version
         assert citation.version == __version__
 
         assert(citation.tags == ['implementation', 'very custom'])
 
@@ -131,15 +126,15 @@
         # TODO: awkwardly 'ret' is not found in the scope while running pytest
         # under python3.4, although present in locals()... WTF?
         assert locals_['ret'] == "%s: None, somevalue" % func
         assert len(self.due._entries) == 2
         assert len(self.due.citations) == 2
 
         # TODO: there must be a cleaner way to get first value
-        citation = list(viewvalues(self.due.citations))[0]
+        citation = list(self.due.citations.values())[0]
         # TODO: ATM we don't allow versioning of the submodules -- we should
         # assert_equal(citation.version, '0.5')
         # ATM it will be the duecredit's version
         assert citation.version, __version__
 
         assert (citation.tags == ['implementation', 'very custom'])
```

### Comparing `duecredit-0.9.2/duecredit/tests/test_io.py` & `duecredit-0.9.3/duecredit/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,40 +8,41 @@
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 
 import random
 import re
 import pickle
 import os
 import pytest
-
-from six.moves import StringIO
-from six import text_type
+from io import StringIO
 
 import duecredit.io
 from ..collector import DueCreditCollector, Citation
 from .test_collector import _sample_bibtex, _sample_doi, _sample_bibtex2
 from ..entries import BibTeX, Doi, Text, Url
 from ..io import TextOutput, PickleOutput, import_doi, \
     get_text_rendering, format_bibtex, _is_contained, Output, BibTeXOutput
 
 try:
-    import vcr
+	# TODO: for some reason test below started to complain that we are trying
+	# to overwrite the cassette.
+	# 
+    # import vcr
 
-    @vcr.use_cassette()
+    # @vcr.use_cassette()
     def test_import_doi():
         doi_good = '10.1038/nrd842'
         kw = dict(sleep=0.00001, retries=2)
-        assert isinstance(import_doi(doi_good, **kw), text_type)
+        assert isinstance(import_doi(doi_good, **kw), str)
 
         doi_bad = 'fasljfdldaksj'
         with pytest.raises(ValueError):
             import_doi(doi_bad, **kw)
 
         doi_zenodo = '10.5281/zenodo.50186'
-        assert isinstance(import_doi(doi_zenodo, **kw), text_type)
+        assert isinstance(import_doi(doi_zenodo, **kw), str)
 
 except ImportError:
     # no vcr, and that is in 2015!
     pass
 
 
 def test_pickleoutput(tmpdir):
```

### Comparing `duecredit-0.9.2/duecredit/tests/test_versions.py` & `duecredit-0.9.3/duecredit/tests/test_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 #
 #   See COPYING file distributed along with the duecredit package for the
 #   copyright and license terms.
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 
 from os import linesep
+
 import pytest
 
 from ..version import __version__
 from ..versions import ExternalVersions, StrictVersion
 
-from six import PY3
-
-if PY3:
-    # just to ease testing
-    def cmp(a, b):
-        return (a > b) - (a < b)
+# just to ease testing
+def cmp(a, b):
+    return (a > b) - (a < b)
 
 
 def test_external_versions_basic():
     ev = ExternalVersions()
     assert ev._versions == {}
     assert ev['duecredit'] == __version__
     # and it could be compared
```

### Comparing `duecredit-0.9.2/duecredit/utils.py` & `duecredit-0.9.3/duecredit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 
 import glob
 import os
 import logging
 import sys
 import platform
+import shutil
+import stat
 import tempfile
+import time
 
-from six import binary_type
 from os.path import exists, join as opj, isabs, expandvars, expanduser, abspath
 
 from os.path import realpath
 from functools import wraps
 
 #
 # Some useful variables
@@ -137,15 +139,15 @@
             rmtree(f, *args, **kwargs)
         else:
             for i in range(10):
                 try:
                     os.unlink(f)
                 except OSError as e:
                     if i < 9:
-                        sleep(0.1)
+                        time.sleep(0.1)
                         continue
                     else:
                         raise
                 break
     else:
         lgr.info("Keeping temp file: %s" % f)
```

### Comparing `duecredit-0.9.2/duecredit/versions.py` & `duecredit-0.9.3/duecredit/versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 #   copyright and license terms.
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 """Module to help maintain a registry of versions for external modules etc
 """
 import sys
 from os import linesep
-from six import string_types
 
 from distutils.version import StrictVersion, LooseVersion
 
 try:
     from importlib.metadata import version as metadata_version
 except ImportError:
     from importlib_metadata import version as metadata_version
@@ -30,15 +29,15 @@
 
     def __cmp__(self, other):
         if other is self:
             return 0
         raise TypeError("UNKNOWN version is not comparable")
 
 
-class ExternalVersions(object):
+class ExternalVersions:
     """Helper to figure out/use versions of the external modules.
 
     It maintains a dictionary of `distuil.version.StrictVersion`s to make
     comparisons easy.  If version string doesn't conform the StrictVersion
     LooseVersion will be used.  If version can't be deduced for the module,
     'None' is assigned
     """
@@ -81,15 +80,15 @@
                 return LooseVersion(version)
         else:
             return klass.UNKNOWN
 
     def __getitem__(self, module):
         # when ran straight in its source code -- fails to discover nipy's version.. TODO
         #if module == 'nipy':
-        if not isinstance(module, string_types):
+        if not isinstance(module, str):
             modname = module.__name__
         else:
             modname = module
             module = None
 
         if modname not in self._versions:
             if module is None:
```

### Comparing `duecredit-0.9.2/duecredit.egg-info/PKG-INFO` & `duecredit-0.9.3/duecredit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duecredit
-Version: 0.9.2
+Version: 0.9.3
 Summary: Publications (and donations) tracer
 Home-page: https://github.com/duecredit/duecredit
 Author: Yaroslav Halchenko, Matteo Visconti di Oleggio Castello
 Author-email: yoh@onerussian.com
 License: 2-clause BSD License
 Keywords: citation tracing
 Classifier: Development Status :: 4 - Beta
@@ -22,16 +22,23 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: citeproc-py>=0.4
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: vcrpy; extra == "tests"
+Requires-Dist: contextlib2; extra == "tests"
 
 # duecredit
 
 
 [![Build Status](https://travis-ci.org/duecredit/duecredit.svg?branch=master)](https://travis-ci.org/duecredit/duecredit)
 [![Coverage Status](https://coveralls.io/repos/duecredit/duecredit/badge.svg)](https://coveralls.io/r/duecredit/duecredit)
 [![DOI](https://zenodo.org/badge/DOI/110.5281/zenodo.3376260.svg)](https://doi.org/10.5281/zenodo.3376260)
```

### Comparing `duecredit-0.9.2/duecredit.egg-info/SOURCES.txt` & `duecredit-0.9.3/duecredit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .coveragerc
-.travis.yml
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
```

### Comparing `duecredit-0.9.2/setup.py` & `duecredit-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,20 +85,20 @@
     name=PACKAGE,
     version=__version__,
     packages=find_packages(),
     python_requires=">=3.6",
     install_requires=[
         'requests',
         'citeproc-py>=0.4',
-        'six',
         'importlib-metadata; python_version<"3.8"',
     ],
     extras_require={
         'tests': [
             'pytest',
+            'pytest-cov',
             'vcrpy', 'contextlib2'
         ]
     },
     include_package_data=True,
     entry_points={
         'console_scripts': [
              'duecredit=duecredit.cmdline.main:main',
```

