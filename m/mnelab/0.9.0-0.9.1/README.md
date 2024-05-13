# Comparing `tmp/mnelab-0.9.0.tar.gz` & `tmp/mnelab-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnelab-0.9.0.tar", last modified: Fri Jan 19 09:31:25 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mnelab-0.9.0.tar` & `mnelab-0.9.1.tar`

### file list

```diff
@@ -1,100 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.764134 mnelab-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    23632 2024-01-19 09:31:18.000000 mnelab-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-01-19 09:31:18.000000 mnelab-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-19 09:31:18.000000 mnelab-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-19 09:31:18.000000 mnelab-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-01-19 09:31:25.764134 mnelab-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-01-19 09:31:18.000000 mnelab-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.752133 mnelab-0.9.0/mnelab/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.760134 mnelab-0.9.0/mnelab/dialogs/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/append.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/channel_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/drop_bad_epochs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/epoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/erds.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/error_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/find_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/interpolate_bads.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/mat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/montage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/npy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/pick_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/plot_evoked.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/rename_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/run_ica.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/xdf_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/xdf_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/dialogs/xdf_streams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.760134 mnelab-0.9.0/mnelab/icons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.760134 mnelab-0.9.0/mnelab/icons/dark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.760134 mnelab-0.9.0/mnelab/icons/dark/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/chan-props.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/epoch-data.svg
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/filter-data.svg
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/find-events.svg
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/open-file.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/plot-data.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/plot-locations.svg
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/plot-psd.svg
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/run-ica.svg
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/actions/xdf-metadata.svg
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/dark/index.theme
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.760134 mnelab-0.9.0/mnelab/icons/light/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.764134 mnelab-0.9.0/mnelab/icons/light/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/chan-props.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/epoch-data.svg
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/filter-data.svg
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/find-events.svg
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/open-file.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/plot-data.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/plot-locations.svg
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/plot-psd.svg
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/run-ica.svg
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/actions/xdf-metadata.svg
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/light/index.theme
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/mnelab-logo-macos.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/icons/mnelab-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.764134 mnelab-0.9.0/mnelab/images/
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/images/mnelab_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.764134 mnelab-0.9.0/mnelab/io/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/io/mat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/io/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/io/xdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    53785 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.764134 mnelab-0.9.0/mnelab/test/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/test/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/test/test_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.764134 mnelab-0.9.0/mnelab/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/utils/syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.764134 mnelab-0.9.0/mnelab/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab/widgets/infowidget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 09:31:25.764134 mnelab-0.9.0/mnelab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-01-19 09:31:25.000000 mnelab-0.9.0/mnelab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-01-19 09:31:25.000000 mnelab-0.9.0/mnelab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 09:31:25.000000 mnelab-0.9.0/mnelab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-19 09:31:25.000000 mnelab-0.9.0/mnelab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-19 09:31:25.000000 mnelab-0.9.0/mnelab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-19 09:31:25.000000 mnelab-0.9.0/mnelab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)   942653 2024-01-19 09:31:18.000000 mnelab-0.9.0/mnelab.png
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-01-19 09:31:18.000000 mnelab-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 09:31:25.764134 mnelab-0.9.0/setup.cfg
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mnelab-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    24172 2020-02-02 00:00:00.000000 mnelab-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 mnelab-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0   942653 2020-02-02 00:00:00.000000 mnelab-0.9.1/mnelab.png
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 mnelab-0.9.1/readthedocs.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mnelab-0.9.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 mnelab-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 mnelab-0.9.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/make.bat
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/requirements.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/about.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/conf.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/index.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/_static/custom.css
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/_static/favicon.png
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/_templates/page.html
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/erds_maps.md
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/erp.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/index.md
+-rw-r--r--   0        0        0    44448 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erds_maps/append_data.png
+-rw-r--r--   0        0        0    26827 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erds_maps/create_epochs.png
+-rw-r--r--   0        0        0    64365 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erds_maps/data_sets_loaded.png
+-rw-r--r--   0        0        0    63141 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erds_maps/pick_channels.png
+-rw-r--r--   0        0        0    66951 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erds_maps/plot_erds_maps.png
+-rw-r--r--   0        0        0    99289 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erds_maps/result_feet.png
+-rw-r--r--   0        0        0    70252 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erds_maps/result_hand.png
+-rw-r--r--   0        0        0    39269 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/create_epochs.png
+-rw-r--r--   0        0        0    81884 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/crop_data.png
+-rw-r--r--   0        0        0    55725 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/drop_bad_epochs.png
+-rw-r--r--   0        0        0   105244 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/evoked_comparison.png
+-rw-r--r--   0        0        0   152305 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/evoked_event_1.png
+-rw-r--r--   0        0        0   163005 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/evoked_event_3.png
+-rw-r--r--   0        0        0    54769 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/filter_data.png
+-rw-r--r--   0        0        0   153770 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/joint_plot.png
+-rw-r--r--   0        0        0    39472 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/pick_channels.png
+-rw-r--r--   0        0        0    73438 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/plot_evoked.png
+-rw-r--r--   0        0        0    70408 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/plot_evoked_comparison.png
+-rw-r--r--   0        0        0    47593 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/plot_evoked_topomaps.png
+-rw-r--r--   0        0        0    76198 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/plot_joint.png
+-rw-r--r--   0        0        0    52614 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/sensor_locations.png
+-rw-r--r--   0        0        0    59502 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/examples/images/erp/topomaps_event_1.png
+-rw-r--r--   0        0        0    19872 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/tutorial/empty_window.png
+-rw-r--r--   0        0        0    61705 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/tutorial/file_loaded.png
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/tutorial/index.md
+-rw-r--r--   0        0        0    40052 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/tutorial/menu_disabled.png
+-rw-r--r--   0        0        0    71829 2020-02-02 00:00:00.000000 mnelab-0.9.1/docs/source/tutorial/plot_menu.png
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/__main__.py
+-rw-r--r--   0        0        0    54817 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/mainwindow.py
+-rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/model.py
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/settings.py
+-rw-r--r--   0        0        0    11746 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/viz.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/__init__.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/annotations.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/append.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/calc.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/channel_properties.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/crop.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/drop_bad_epochs.py
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/epoch.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/erds.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/error_message.py
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/events.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/filter.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/find_events.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/history.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/interpolate_bads.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/mat.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/montage.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/npy.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/pick_channels.py
+-rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/plot_evoked.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/reference.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/rename_channels.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/run_ica.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/utils.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/xdf_chunks.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/xdf_metadata.py
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/dialogs/xdf_streams.py
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/mnelab-logo-macos.svg
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/mnelab-logo.svg
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/index.theme
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/chan-props.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/epoch-data.svg
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/filter-data.svg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/find-events.svg
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/open-file.svg
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/plot-data.svg
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/plot-locations.svg
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/plot-psd.svg
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/run-ica.svg
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/settings.svg
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/dark/actions/xdf-metadata.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/index.theme
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/chan-props.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/epoch-data.svg
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/filter-data.svg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/find-events.svg
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/open-file.svg
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/plot-data.svg
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/plot-locations.svg
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/plot-psd.svg
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/run-ica.svg
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/settings.svg
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/icons/light/actions/xdf-metadata.svg
+-rw-r--r--   0        0        0    13709 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/images/mnelab_logo.png
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/io/__init__.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/io/mat.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/io/readers.py
+-rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/io/writers.py
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/io/xdf.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/utils/__init__.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/utils/dependencies.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/utils/syntax.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/utils/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/widgets/__init__.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 mnelab-0.9.1/src/mnelab/widgets/infowidget.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mnelab-0.9.1/tests/test_actions.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 mnelab-0.9.1/tests/test_readers.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mnelab-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mnelab-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 mnelab-0.9.1/README.md
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 mnelab-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 mnelab-0.9.1/PKG-INFO
```

### Comparing `mnelab-0.9.0/CHANGELOG.md` & `mnelab-0.9.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## [0.9.1] - 2024-05-13
+### Added
+- Add option to select browser backend in settings ([#415](https://github.com/cbrnr/mnelab/pull/415) by [Clemens Brunner](https://github.com/cbrnr))
+
+### Fixed
+- Prepare support for plotting raw data with MNE-Qt-Browser ([#403](https://github.com/cbrnr/mnelab/pull/403) by [Martin Schulz](https://github.com/marsipu) and [Clemens Brunner](https://github.com/cbrnr))
+- Fix drag and drop for PySide ≥ 6.7.0 ([#422](https://github.com/cbrnr/mnelab/pull/422) by [Clemens Brunner](https://github.com/cbrnr))
+
 ## [0.9.0] - 2024-01-19
 ### Added
 - Add automatic light/dark theme switching on Windows ([#398](https://github.com/cbrnr/mnelab/pull/398) by [Clemens Brunner](https://github.com/cbrnr))
 - Add support for importing .npy files ([#213](https://github.com/cbrnr/mnelab/pull/213) by [jgcaffari1](https://github.com/jgcaffari1) and [Clemens Brunner](https://github.com/cbrnr))
 - Add ability to import selected XDF marker streams (previously, all marker streams were automatically imported) ([#395](https://github.com/cbrnr/mnelab/pull/395) by [Clemens Brunner](https://github.com/cbrnr))
 
 ### Removed
```

### Comparing `mnelab-0.9.0/CONTRIBUTING.md` & `mnelab-0.9.1/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,68 @@
 ## Contributing to MNELAB
-If you want to implement a new feature, fix an existing bug, or help improve MNELAB in any other way (such as adding or improving documentation), please consider submitting a [pull request](https://github.com/cbrnr/mnelab/pulls) on GitHub. It might be a good idea to open an [issue](https://github.com/cbrnr/mnelab/issues) beforehand to discuss your planned contributions with the developers.
+
+If you want to implement a new feature, fix an existing bug, or help improve MNELAB in any other way (such as adding or improving documentation), please consider submitting a [pull request](https://github.com/cbrnr/mnelab/pulls). It might be a good idea to open an [issue](https://github.com/cbrnr/mnelab/issues) first to discuss your planned contributions with the developers.
 
 Before you start working on your contribution, please make sure to follow the guidelines described in this document.
 
 
 ### Setting up the development environment
+
 You will need to have a working Python installation (make sure to use one of the supported Python versions). Installation methods vary across platforms, but if you don't have any specific preferences, the [official installers](https://www.python.org/) are a great option on Windows and macOS.
 
-In addition to Python, you will also need a working [Git](https://git-scm.com/) installation. Again, installation methods are different depending on which platform you are using. If you are on Windows, you can install [Git for Windows](https://gitforwindows.org/). If you are on macOS, you can install the XCode command line tools with `xcode-select --install`.
+In addition to Python, you will also need a working [Git](https://git-scm.com/) installation. Again, installation methods are different depending on which platform you are using. If you are on Windows, you can install [Git for Windows](https://gitforwindows.org/). If you are on macOS, you can install the XCode command line tools with `xcode-select --install`, which contain Git.
+
 
 ### Forking and cloning MNELAB
-On the [GitHub website](https://github.com/cbrnr/mnelab), click on the "Fork" button in the top right corner to create your own fork of MNELAB (you need to be logged in with your GitHub account). Next, from the main page of your fork, click on the green "Clone or download" button. Copy the URL to the clipboard – you will need this URL to create your local MNELAB repository.
 
-Open a terminal and change into the folder where you would like your MNELAB project to live. Then, type `git clone <URL>` (replace `<URL>` with the repository URL you copied to the clipboard earlier). Your fork of MNELAB is now available in the `mnelab` folder.
+On the [repository website](https://github.com/cbrnr/mnelab), click on the "Fork" button in the top right corner to create your own fork of MNELAB (you need to be logged in with your GitHub account). Next, from the main page of your fork, click on the green "Clone or download" button. Copy the URL to the clipboard – you will need this URL to create your local MNELAB repository.
+
+Open a terminal and change into the folder where you would like your MNELAB fork to live. Then, type `git clone <URL>` (replace `<URL>` with the repository URL you copied to the clipboard earlier). Your fork of MNELAB is now available in the `mnelab` folder.
+
 
 ### Installing required Python packages
+
 In a terminal, change to the `mnelab` folder containing your MNELAB fork. You can install the package and all dependencies with the following command:
 
 ```
 pip install -e ".[full]"
 ```
 
-You might want to [create a virtual environment](https://docs.python.org/3/library/venv.html#creating-virtual-environments) instead of installing everything into your main environment.
+You might want to [create a virtual environment](https://docs.python.org/3/library/venv.html#creating-virtual-environments) instead of installing everything into your global environment.
+
 
 ### Creating a new branch
+
 Before you start working with the MNELAB codebase, you should create a new branch. In a terminal, type `git switch -c <BRANCH_NAME>` (replacing `<BRANCH_NAME>` with a suitable name for your branch). You are now ready to work on your contribution.
 
+
 ### Making a pull request
+
 Once you have committed all of your changes, you can push them to your remote fork by typing `git push`. The GitHub page of your fork will now show a prompt to create a new pull request. Think of a good title and describe your contribution. If you have a corresponding issue, make sure to reference this issue in your description (it will be automatically closed after your pull request is merged).
 
+
+### Modifying icons
+
+MNELAB bundles its icons in the `icons` folder, which contains two themes ("light" and "dark"). If you want to modify an existing icon or add a new one, make sure to apply your changes to both the "light" and "dark" themes. All icons are SVGs and taken from the [Material Symbols](https://fonts.google.com/icons) icon set.
+
+If you want to add a new icon, download it from the Material Symbols website, rename it (use a suitable name reflecting its intended action), and place it in the `icons/light/actions` folder. Next, edit the SVG file in a text editor and add the `fill="black"` attribute to the `<svg>` tag. Finally, copy the SVG file to the `icons/dark/actions` folder and change the `fill` attribute to `fill="white"`.
+
+
 ### Adding a changelog entry
-Once you have an open pull request, add an entry to the top of `CHANGELOG.md` in the most suitable section: "Added" lists new features, "Fixed" lists bug fixes, and "Changed" lists changes to existing functionality. Finally, make sure to mention your pull request and your name.
+
+Once you have an open pull request, add an entry to the top of `CHANGELOG.md` in the most suitable section: "Added" lists new features, "Fixed" lists bug fixes, and "Changed" lists changes to existing functionality. Finally, make sure to mention the pull request and your name.
+
 
 ### Coding style
-MNELAB uses [Black](https://black.readthedocs.io/en/stable/?badge=stable#) code style (using [Ruff](https://docs.astral.sh/ruff/formatter/) for formatting) wherever possible (with the noteable exception that we use a maximum line length of 92 characters as opposed to the default 88 characters). Because [PySide6](https://doc.qt.io/qtforpython-6/index.html) is based on the C++-based Qt library, most of its names use camel case instead of snake case. In your own code, please use snake case whereever possible.
+
+MNELAB uses [Ruff](https://docs.astral.sh/ruff/formatter/) for formatting (with the noteable customization that we use a maximum line length of 92 characters as opposed to the default 88 characters). Because [PySide6](https://doc.qt.io/qtforpython-6/index.html) is based on the C++-based Qt library, most of its names use camel case instead of snake case. In your own code, please use snake case whereever possible.
+
 
 ## Making a PyPI release
+
 Follow these steps to make a new [PyPI](https://pypi.org/project/mnelab/) release (requires write permissions for GitHub and PyPI project sites):
 
 - Remove the `.dev0` suffix from the `__version__` string in `mnelab/__init__.py` (and adapt the version to be released if necessary)
 - Update the section in `CHANGELOG.md` corresponding to the new release with the version and current date
 - Commit these changes and push
 - Create a new release on GitHub and use the version as the tag name (make sure to prepend the version with a `v`, e.g. `v0.7.0`)
 - A GitHub Action takes care of building and uploading wheels to PyPI
```

### Comparing `mnelab-0.9.0/LICENSE` & `mnelab-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/PKG-INFO` & `mnelab-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,52 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mnelab
-Version: 0.9.0
+Version: 0.9.1
 Summary: A graphical user interface for MNE
-Author-email: Clemens Brunner <clemens.brunner@gmail.com>
-License: BSD 3-Clause
 Project-URL: homepage, https://github.com/cbrnr/mnelab
 Project-URL: documentation, https://mnelab.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/cbrnr/mnelab
 Project-URL: changelog, https://github.com/cbrnr/mnelab/blob/main/CHANGELOG.md
-Keywords: EEG,MEG,MNE,GUI,electrophysiology
+Author-email: Clemens Brunner <clemens.brunner@gmail.com>
+License: BSD 3-Clause
+License-File: LICENSE
+Keywords: EEG,GUI,MEG,MNE,electrophysiology
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: mne>=1.6.0
-Requires-Dist: PySide6>=6.6.0
-Requires-Dist: numpy>=1.25.0
-Requires-Dist: scipy>=1.10.0
 Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: mne>=1.7.0
+Requires-Dist: numpy>=1.25.0
+Requires-Dist: pyobjc-framework-cocoa>=10.0; platform_system == 'Darwin'
+Requires-Dist: pyside6<6.7.0,>=6.6.2
 Requires-Dist: pyxdf>=1.16.4
-Requires-Dist: pyobjc-framework-Cocoa>=10.0; platform_system == "Darwin"
-Provides-Extra: full
-Requires-Dist: scikit-learn>=1.3.0; extra == "full"
-Requires-Dist: python-picard>=0.7.0; extra == "full"
-Requires-Dist: pyEDFlib>=0.1.35; extra == "full"
-Requires-Dist: pybv>=0.7.4; extra == "full"
+Requires-Dist: scipy>=1.10.0
 Provides-Extra: dev
-Requires-Dist: mnelab[full]; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: setuptools; extra == "dev"
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: mne-qt-browser>=0.6.2; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: pybv>=0.7.4; extra == 'dev'
+Requires-Dist: pyedflib>=0.1.35; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-qt; extra == 'dev'
+Requires-Dist: python-picard>=0.7.0; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: scikit-learn>=1.3.0; extra == 'dev'
+Provides-Extra: full
+Requires-Dist: mne-qt-browser>=0.6.2; extra == 'full'
+Requires-Dist: pybv>=0.7.4; extra == 'full'
+Requires-Dist: pyedflib>=0.1.35; extra == 'full'
+Requires-Dist: python-picard>=0.7.0; extra == 'full'
+Requires-Dist: scikit-learn>=1.3.0; extra == 'full'
+Description-Content-Type: text/markdown
 
 ![Python](https://img.shields.io/pypi/pyversions/mnelab.svg?logo=python&logoColor=white)
 [![PyPI](https://img.shields.io/pypi/v/mnelab)](https://pypi.org/project/mnelab/)
 [![Docs](https://readthedocs.org/projects/mnelab/badge/?version=latest)](https://mnelab.readthedocs.io/)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04650/status.svg)](https://doi.org/10.21105/joss.04650)
 [![License](https://img.shields.io/github/license/cbrnr/mnelab)](LICENSE)
 
@@ -94,15 +102,15 @@
 python -m mnelab
 ```
 
 ### Dependencies
 
 MNELAB requires Python ≥ 3.9 and the following packages:
 - [mne](https://mne.tools/stable/index.html) ≥ 1.6.0
-- [PySide6](https://www.qt.io/qt-for-python) ≥ 6.6.0
+- [PySide6](https://www.qt.io/qt-for-python) ≥ 6.6.2
 - [numpy](http://www.numpy.org/) ≥ 1.25.0
 - [scipy](https://scipy.org/) ≥ 1.10.0
 - [matplotlib](https://matplotlib.org/) ≥ 3.8.0
 - [pyxdf](https://github.com/xdf-modules/xdf-Python) ≥ 1.16.4
 - [pyobjc-framework-Cocoa](https://pyobjc.readthedocs.io/en/latest/) ≥ 10.0 (macOS only)
 
 Optional dependencies provide additional features:
```

### Comparing `mnelab-0.9.0/README.md` & `mnelab-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 python -m mnelab
 ```
 
 ### Dependencies
 
 MNELAB requires Python ≥ 3.9 and the following packages:
 - [mne](https://mne.tools/stable/index.html) ≥ 1.6.0
-- [PySide6](https://www.qt.io/qt-for-python) ≥ 6.6.0
+- [PySide6](https://www.qt.io/qt-for-python) ≥ 6.6.2
 - [numpy](http://www.numpy.org/) ≥ 1.25.0
 - [scipy](https://scipy.org/) ≥ 1.10.0
 - [matplotlib](https://matplotlib.org/) ≥ 3.8.0
 - [pyxdf](https://github.com/xdf-modules/xdf-Python) ≥ 1.16.4
 - [pyobjc-framework-Cocoa](https://pyobjc.readthedocs.io/en/latest/) ≥ 10.0 (macOS only)
 
 Optional dependencies provide additional features:
```

### Comparing `mnelab-0.9.0/mnelab/__init__.py` & `mnelab-0.9.1/src/mnelab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import QApplication
 
 from mnelab.mainwindow import MainWindow
 from mnelab.model import Model
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 
 def main():
     mp.set_start_method("spawn", force=True)  # required for Linux
     app_name = "MNELAB"
     if sys.platform.startswith("darwin"):
         # set bundle name on macOS (app name shown in the menu bar)
```

### Comparing `mnelab-0.9.0/mnelab/dialogs/__init__.py` & `mnelab-0.9.1/src/mnelab/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/annotations.py` & `mnelab-0.9.1/src/mnelab/dialogs/annotations.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/append.py` & `mnelab-0.9.1/src/mnelab/dialogs/append.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/calc.py` & `mnelab-0.9.1/src/mnelab/dialogs/calc.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/channel_properties.py` & `mnelab-0.9.1/src/mnelab/dialogs/channel_properties.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/crop.py` & `mnelab-0.9.1/src/mnelab/dialogs/crop.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/drop_bad_epochs.py` & `mnelab-0.9.1/src/mnelab/dialogs/drop_bad_epochs.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/epoch.py` & `mnelab-0.9.1/src/mnelab/dialogs/epoch.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/erds.py` & `mnelab-0.9.1/src/mnelab/dialogs/erds.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/events.py` & `mnelab-0.9.1/src/mnelab/dialogs/events.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/filter.py` & `mnelab-0.9.1/src/mnelab/dialogs/filter.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/find_events.py` & `mnelab-0.9.1/src/mnelab/dialogs/find_events.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/history.py` & `mnelab-0.9.1/src/mnelab/dialogs/history.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/interpolate_bads.py` & `mnelab-0.9.1/src/mnelab/dialogs/interpolate_bads.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/mat.py` & `mnelab-0.9.1/src/mnelab/dialogs/mat.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/montage.py` & `mnelab-0.9.1/src/mnelab/dialogs/montage.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/npy.py` & `mnelab-0.9.1/src/mnelab/dialogs/npy.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/pick_channels.py` & `mnelab-0.9.1/src/mnelab/dialogs/pick_channels.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/plot_evoked.py` & `mnelab-0.9.1/src/mnelab/dialogs/plot_evoked.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/reference.py` & `mnelab-0.9.1/src/mnelab/dialogs/reference.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/rename_channels.py` & `mnelab-0.9.1/src/mnelab/dialogs/rename_channels.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/run_ica.py` & `mnelab-0.9.1/src/mnelab/dialogs/run_ica.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/utils.py` & `mnelab-0.9.1/src/mnelab/dialogs/utils.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/xdf_chunks.py` & `mnelab-0.9.1/src/mnelab/dialogs/xdf_chunks.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/xdf_metadata.py` & `mnelab-0.9.1/src/mnelab/dialogs/xdf_metadata.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/dialogs/xdf_streams.py` & `mnelab-0.9.1/src/mnelab/dialogs/xdf_streams.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/icons/mnelab-logo-macos.svg` & `mnelab-0.9.1/src/mnelab/icons/mnelab-logo-macos.svg`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/icons/mnelab-logo.svg` & `mnelab-0.9.1/src/mnelab/icons/mnelab-logo.svg`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/images/mnelab_logo.png` & `mnelab-0.9.1/src/mnelab/images/mnelab_logo.png`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/io/mat.py` & `mnelab-0.9.1/src/mnelab/io/mat.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/io/readers.py` & `mnelab-0.9.1/src/mnelab/io/readers.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/io/writers.py` & `mnelab-0.9.1/src/mnelab/io/writers.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/io/xdf.py` & `mnelab-0.9.1/src/mnelab/io/xdf.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/mainwindow.py` & `mnelab-0.9.1/src/mnelab/mainwindow.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pathlib import Path
 from sys import version_info
 
 import mne
 import numpy as np
 from mne import channel_type
 from PySide6.QtCore import QEvent, QMetaObject, QModelIndex, QObject, Qt, QUrl, Slot
-from PySide6.QtGui import QAction, QDesktopServices, QDropEvent, QIcon, QKeySequence
+from PySide6.QtGui import QAction, QDesktopServices, QIcon, QKeySequence
 from PySide6.QtWidgets import (
     QApplication,
     QFileDialog,
     QFrame,
     QLabel,
     QListWidget,
     QMainWindow,
@@ -67,28 +67,43 @@
 
         # restore settings
         settings = read_settings()
         self.recent = settings["recent"]  # list of recent files
         self.resize(settings["size"])
         self.move(settings["pos"])
 
+        self.installEventFilter(self)
+
         # remove None entries from self.recent
         self.recent = [recent for recent in self.recent if recent is not None]
 
+        # plot backend
+        self.plot_backends = ["Matplotlib"]
+        if have["mne-qt-browser"]:
+            self.plot_backends.append("Qt")
+        plot_backend = settings["plot_backend"]
+        if plot_backend not in self.plot_backends:
+            plot_backend = "Matplotlib"
+        mne.viz.set_browser_backend(plot_backend)
+        self.model.history.append(f'mne.viz.set_browser_backend("{plot_backend}")')
+        self.model.history.append("")
+
         # trigger theme setting
-        QIcon.setThemeSearchPaths([str(Path(__file__).parent / "icons")])
-        self.event(QEvent(QEvent.PaletteChange))
+        QIcon.setThemeSearchPaths(
+            [f"{Path(__file__).parent}/icons"] + QIcon.themeSearchPaths()
+        )
+        QIcon.setFallbackThemeName("light")
+        QApplication.sendEvent(self, QEvent(QEvent.PaletteChange))
 
         self.actions = {}  # contains all actions
 
         # initialize menus
         file_menu = self.menuBar().addMenu("&File")
-        icon = QIcon.fromTheme("open-file")
         self.actions["open_file"] = file_menu.addAction(
-            icon, "&Open...", self.open_data, QKeySequence.Open
+            QIcon.fromTheme("open-file"), "&Open...", self.open_data, QKeySequence.Open
         )
         self.recent_menu = file_menu.addMenu("Open recent")
         self.recent_menu.aboutToShow.connect(self._update_recent_menu)
         self.recent_menu.triggered.connect(self._load_recent)
         if not self.recent:
             self.recent_menu.setEnabled(False)
         self.actions["close_file"] = file_menu.addAction(
@@ -137,26 +152,28 @@
             ),
         )
         self.actions["export_ica"] = file_menu.addAction(
             "Export ICA...",
             lambda: self.export_file(model.export_ica, "Export ICA", "*.fif *.fif.gz"),
         )
         file_menu.addSeparator()
-        icon = QIcon.fromTheme("xdf-metadata")
         self.actions["xdf_metadata"] = file_menu.addAction(
+            QIcon.fromTheme("xdf-metadata"),
             "Show XDF metadata",
             self.xdf_metadata,
         )
         self.actions["xdf_chunks"] = file_menu.addAction(
             "Inspect XDF chunks...", self.xdf_chunks
         )
         file_menu.addSeparator()
         self.actions["settings"] = file_menu.addAction(
+            QIcon.fromTheme("settings"),
             "Settings...",
-            SettingsDialog(self).exec,
+            QKeySequence(Qt.CTRL | Qt.Key_Comma),
+            self.settings,
         )
         file_menu.addSeparator()
         self.actions["quit"] = file_menu.addAction("&Quit", self.close, QKeySequence.Quit)
 
         edit_menu = self.menuBar().addMenu("&Edit")
         self.actions["pick_chans"] = edit_menu.addAction(
             "P&ick channels...", self.pick_channels
@@ -181,32 +198,32 @@
         edit_menu.addSeparator()
         self.actions["change_ref"] = edit_menu.addAction(
             "Change &reference...",
             self.change_reference,
         )
         edit_menu.addSeparator()
         self.actions["annotations"] = edit_menu.addAction(
-            "Edit &Annotations...",
+            "Edit &annotations...",
             self.edit_annotations,
         )
         self.actions["events"] = edit_menu.addAction(
-            "Edit &Events...",
+            "Edit &events...",
             self.edit_events,
         )
 
         edit_menu.addSeparator()
         self.actions["crop"] = edit_menu.addAction("&Crop data...", self.crop)
         self.actions["append_data"] = edit_menu.addAction(
             "Appen&d data...", self.append_data
         )
 
         plot_menu = self.menuBar().addMenu("&Plot")
         self.actions["plot_data"] = plot_menu.addAction(
             QIcon.fromTheme("plot-data"),
-            "Plot &Data",
+            "Plot &data",
             self.plot_data,
         )
         self.actions["plot_psd"] = plot_menu.addAction(
             QIcon.fromTheme("plot-psd"),
             "Plot &PSD",
             self.plot_psd,
         )
@@ -245,21 +262,19 @@
         )
         self.actions["plot_ica_sources"] = plot_menu.addAction(
             "Plot ICA &sources",
             self.plot_ica_sources,
         )
 
         tools_menu = self.menuBar().addMenu("&Tools")
-        icon = QIcon.fromTheme("filter-data")
         self.actions["filter"] = tools_menu.addAction(
-            icon, "&Filter data...", self.filter_data
+            QIcon.fromTheme("filter-data"), "&Filter data...", self.filter_data
         )
-        icon = QIcon.fromTheme("find-events")
         self.actions["find_events"] = tools_menu.addAction(
-            icon, "Find &events...", self.find_events
+            QIcon.fromTheme("find-events"), "Find &events...", self.find_events
         )
         self.actions["events_from_annotations"] = tools_menu.addAction(
             "Create events from annotations", self.events_from_annotations
         )
         self.actions["annotations_from_events"] = tools_menu.addAction(
             "Create annotations from events", self.annotations_from_events
         )
@@ -270,25 +285,25 @@
         )
         self.actions["convert_bl"] = tools_menu.addAction(
             "Convert to &haemoglobin",
             self.convert_bl,
         )
         tools_menu.addSeparator()
 
-        icon = QIcon.fromTheme("run-ica")
-        self.actions["run_ica"] = tools_menu.addAction(icon, "Run &ICA...", self.run_ica)
+        self.actions["run_ica"] = tools_menu.addAction(
+            QIcon.fromTheme("run-ica"), "Run &ICA...", self.run_ica
+        )
         self.actions["apply_ica"] = tools_menu.addAction("Apply &ICA", self.apply_ica)
         tools_menu.addSeparator()
         self.actions["interpolate_bads"] = tools_menu.addAction(
             "Interpolate bad channels...", self.interpolate_bads
         )
         tools_menu.addSeparator()
-        icon = QIcon.fromTheme("epoch-data")
         self.actions["epoch_data"] = tools_menu.addAction(
-            icon, "Create epochs...", self.epoch_data
+            QIcon.fromTheme("epoch-data"), "Create epochs...", self.epoch_data
         )
         self.actions["drop_bad_epochs"] = tools_menu.addAction(
             "Drop bad epochs...",
             self.drop_bad_epochs,
         )
 
         view_menu = self.menuBar().addMenu("&View")
@@ -337,14 +352,16 @@
         self.toolbar.addAction(self.actions["plot_psd"])
         self.toolbar.addAction(self.actions["plot_locations"])
         self.toolbar.addSeparator()
         self.toolbar.addAction(self.actions["filter"])
         self.toolbar.addAction(self.actions["find_events"])
         self.toolbar.addAction(self.actions["epoch_data"])
         self.toolbar.addAction(self.actions["run_ica"])
+        self.toolbar.addSeparator()
+        self.toolbar.addAction(self.actions["settings"])
         self.toolbar.setMovable(False)
         self.setUnifiedTitleAndToolBarOnMac(True)
         if settings["toolbar"]:
             self.toolbar.show()
             self.actions["toolbar"].setChecked(True)
         else:
             self.toolbar.hide()
@@ -364,15 +381,17 @@
         self.sidebar.clicked.connect(self._update_data)
 
         splitter = QSplitter()
         splitter.addWidget(self.sidebar)
 
         self.infowidget = QStackedWidget()
         self.infowidget.addWidget(InfoWidget())
-        emptywidget = EmptyWidget(itemgetter("open_file", "history")(self.actions))
+        emptywidget = EmptyWidget(
+            itemgetter("open_file", "history", "settings")(self.actions)
+        )
         self.infowidget.addWidget(emptywidget)
         splitter.addWidget(self.infowidget)
         width = splitter.size().width()
         splitter.setSizes((int(width * 0.3), int(width * 0.7)))
         self.setCentralWidget(splitter)
 
         self.status_label = QLabel()
@@ -814,24 +833,23 @@
             show=False,
         )
         if events is not None:
             hist = f"data.plot(events=events, n_channels={nchan})"
         else:
             hist = f"data.plot(n_channels={nchan})"
         self.model.history.append(hist)
-        win = fig.canvas.manager.window
-        win.setWindowTitle(self.model.current["name"])
-        win.statusBar().hide()  # not necessary since matplotlib 3.3
-        win.installEventFilter(self)  # detect if the figure is closed
-
-        # prevent closing the window with the escape key
-        try:
-            fig._mne_params["close_key"] = None
-        except AttributeError:  # does not exist in older MNE versions
-            pass
+        if mne.viz.get_browser_backend() == "matplotlib":
+            win = fig.canvas.manager.window
+            win.setWindowTitle(self.model.current["name"])
+            win.statusBar().hide()  # not necessary since matplotlib 3.3
+            fig.canvas.mpl_connect("close_event", self._plot_closed)
+            fig.mne.close_key = None
+        else:
+            fig.gotClosed.connect(self._plot_closed)
+            fig.mne.keyboard_shortcuts.pop("escape")
 
         fig.show()
 
     def plot_psd(self):
         """Plot power spectral density (PSD)."""
         kwds = {}
         if self.model.current["dtype"] == "raw":
@@ -1242,14 +1260,22 @@
         QMessageBox.aboutQt(self, "About Qt")
 
     def show_documentation(self):
         url = QUrl("https://mnelab.readthedocs.io/")
         if not QDesktopServices.openUrl(url):
             QMessageBox.warning(self, "Open Url", "Could not open url")
 
+    def settings(self):
+        old_backend = read_settings("plot_backend")
+        SettingsDialog(self, self.plot_backends).exec()
+        new_backend = read_settings("plot_backend")
+        if old_backend != new_backend:
+            mne.viz.set_browser_backend(new_backend)
+            self.model.history.append(f'mne.viz.set_browser_backend("{new_backend}")')
+
     def auto_duplicate(self):
         """Automatically duplicate current data set.
 
         If the current data set is stored in a file (i.e. was loaded directly from a file),
         a new data set is automatically created. If the current data set is not stored in a
         file (i.e. was created by operations in MNELAB), a dialog box asks the user if the
         current data set should be overwritten or duplicated.
@@ -1350,55 +1376,56 @@
     def _toggle_statusbar(self):
         if self.statusBar().isHidden():
             self.statusBar().show()
         else:
             self.statusBar().hide()
         write_settings(statusbar=not self.statusBar().isHidden())
 
-    @Slot(QDropEvent)
     def dragEnterEvent(self, event):
         if event.mimeData().hasUrls():
             event.acceptProposedAction()
 
-    @Slot(QDropEvent)
+    def dragMoveEvent(self, event):
+        event.acceptProposedAction()
+
+    def dragLeaveEvent(self, event):
+        event.accept()
+
     def dropEvent(self, event):
         mime = event.mimeData()
         if mime.hasUrls():
             urls = mime.urls()
             for url in urls:
                 try:
                     self.open_data(url.toLocalFile())
                 except FileNotFoundError as e:
                     QMessageBox.critical(self, "File not found", str(e))
+        event.acceptProposedAction()
 
     @Slot(QEvent)
     def closeEvent(self, event):
         """Close application.
 
         Parameters
         ----------
         event : QEvent
             Close event.
         """
         write_settings(size=self.size(), pos=self.pos())
         if self.model.history:
             print("\n# Command History\n")
             print("\n".join(self.model.history))
-        QApplication.quit()
+        event.accept()
 
-    def eventFilter(self, source, event):
-        # currently the only source is the raw plot window
-        if event.type() == QEvent.Close:
-            self.data_changed()
-            bads = self.model.current["data"].info["bads"]
-            if self.bads != bads:
-                self.model.history.append(f'data.info["bads"] = {bads}')
-        return QObject.eventFilter(self, source, event)
+    def _plot_closed(self, event=None):
+        self.data_changed()
+        bads = self.model.current["data"].info["bads"]
+        if self.bads != bads:
+            self.model.history.append(f'data.info["bads"] = {bads}')
 
-    def event(self, ev):
-        """Catch system events."""
-        if ev.type() == QEvent.PaletteChange:  # detect theme switches
+    def eventFilter(self, source, event):
+        if event.type() == QEvent.PaletteChange:
             if (style := QApplication.styleHints().colorScheme()) != Qt.ColorScheme.Unknown:
                 QIcon.setThemeName(style.name.lower())
             else:
                 QIcon.setThemeName("light")  # fallback
-        return super().event(ev)
+        return QObject.eventFilter(self, source, event)
```

### Comparing `mnelab-0.9.0/mnelab/model.py` & `mnelab-0.9.1/src/mnelab/model.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/settings.py` & `mnelab-0.9.1/src/mnelab/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # © MNELAB developers
 #
 # License: BSD (3-clause)
 
 from PySide6.QtCore import QPoint, QSettings, QSize, Slot
+from PySide6.QtGui import Qt
 from PySide6.QtWidgets import (
+    QComboBox,
     QDialog,
     QDialogButtonBox,
-    QDoubleSpinBox,
     QGridLayout,
     QHBoxLayout,
     QLabel,
     QPushButton,
+    QSpinBox,
 )
 
 _DEFAULTS = {
     "max_recent": 6,
     "recent": [],
     "toolbar": True,
     "statusbar": True,
     "size": QSize(700, 500),
     "pos": QPoint(100, 100),
+    "plot_backend": "Matplotlib",
 }
 
 
 def _get_value(key):
     # The third argument to QSettings().value is a typecast which is applied to the
     # retrieved value. Since booleans are stored as "true" and "false" (at least on Win10),
     # we need that typecast. However, lists would get replaced with an empty list for some
@@ -56,53 +59,64 @@
 def write_settings(**kwargs):
     """Write application settings."""
     for key, value in kwargs.items():
         QSettings().setValue(key, value)
 
 
 class SettingsDialog(QDialog):
-    def __init__(self, parent):
+    def __init__(self, parent, backends):
         super().__init__(parent)
         self.setWindowTitle("MNELAB settings")
 
         grid = QGridLayout(self)
 
-        grid.addWidget(QLabel("Maximum recent files:"), 0, 0)
-        self.max_recent = QDoubleSpinBox()
+        backend = read_settings("plot_backend")
+        if backend not in backends:
+            backend = _DEFAULTS["plot_backend"]
+        grid.addWidget(QLabel("Plot backend:"), 0, 0)
+        self.plot_backend = QComboBox()
+        self.plot_backend.addItems(backends)
+        self.plot_backend.setCurrentIndex(backends.index(backend))
+        grid.addWidget(self.plot_backend, 0, 1)
+
+        grid.addWidget(QLabel("Maximum recent files:"), 1, 0)
+        self.max_recent = QSpinBox()
         self.max_recent.setRange(5, 25)
         self.max_recent.setValue(_get_value("max_recent"))
-        self.max_recent.setDecimals(0)
-        grid.addWidget(self.max_recent, 0, 1)
+        self.max_recent.setAlignment(Qt.AlignRight)
+        grid.addWidget(self.max_recent, 1, 1)
 
         self.reset_to_defaults = QPushButton("Reset to defaults")
         self.reset_to_defaults.clicked.connect(self.reset_settings)
-        grid.addWidget(self.reset_to_defaults, 1, 0)
+        grid.addWidget(self.reset_to_defaults, 2, 0)
 
         self.reset_to_defaults = QPushButton("Reset window")
         self.reset_to_defaults.clicked.connect(self.reset_window)
-        grid.addWidget(self.reset_to_defaults, 2, 0)
+        grid.addWidget(self.reset_to_defaults, 3, 0)
 
         hbox = QHBoxLayout()
         self.buttonbox = QDialogButtonBox(
             QDialogButtonBox.Apply | QDialogButtonBox.Ok | QDialogButtonBox.Cancel
         )
         hbox.addWidget(self.buttonbox)
-        grid.addLayout(hbox, 3, 0, 1, 2)
+        grid.addLayout(hbox, 4, 0, 1, 2)
         self.buttonbox.button(QDialogButtonBox.Apply).clicked.connect(self.apply_settings)
         self.buttonbox.accepted.connect(self.accept)
         self.buttonbox.accepted.connect(self.apply_settings)
         self.buttonbox.rejected.connect(self.reject)
 
     @Slot()
     def apply_settings(self):
         QSettings().setValue("max_recent", int(self.max_recent.text()))
         self.parent().recent = self.parent().recent[: _get_value("max_recent")]
         QSettings().setValue("recent", self.parent().recent)
+        QSettings().setValue("plot_backend", self.plot_backend.currentText())
 
     @Slot()
     def reset_settings(self):
         self.max_recent.setValue(_DEFAULTS["max_recent"])
+        self.plot_backend.setValue(_DEFAULTS["plot_backend"])
 
     @Slot()
     def reset_window(self):
         self.parent().resize(_DEFAULTS["size"])
         self.parent().move(_DEFAULTS["pos"])
```

### Comparing `mnelab-0.9.0/mnelab/utils/syntax.py` & `mnelab-0.9.1/src/mnelab/utils/syntax.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/utils/utils.py` & `mnelab-0.9.1/src/mnelab/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/viz.py` & `mnelab-0.9.1/src/mnelab/viz.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab/widgets/infowidget.py` & `mnelab-0.9.1/src/mnelab/widgets/infowidget.py`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/mnelab.png` & `mnelab-0.9.1/mnelab.png`

 * *Files identical despite different names*

### Comparing `mnelab-0.9.0/pyproject.toml` & `mnelab-0.9.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 [build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "mnelab"
 description = "A graphical user interface for MNE"
 license = {text = "BSD 3-Clause"}
 authors = [
     {name = "Clemens Brunner", email = "clemens.brunner@gmail.com"},
 ]
+readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "License :: OSI Approved :: BSD License",
+    "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 keywords = ["EEG", "MEG", "MNE", "GUI", "electrophysiology"]
 dependencies = [
-    "mne >= 1.6.0",
-    "PySide6 >= 6.6.0",
+    "mne >= 1.7.0",
+    "PySide6 >= 6.6.2, < 6.7.0",
     "numpy >= 1.25.0",
     "scipy >= 1.10.0",
     "matplotlib >= 3.8.0",
     "pyxdf >= 1.16.4",
     "pyobjc-framework-Cocoa >= 10.0; platform_system=='Darwin'",
 ]
-dynamic = ["version", "readme"]
+dynamic = ["version"]
 
 [project.optional-dependencies]
 full = [
     "scikit-learn >= 1.3.0",  # fastica
     "python-picard >= 0.7.0",  # picard
     "pyEDFlib >= 0.1.35",  # edf
     "pybv >= 0.7.4",  # brainvision
+    "mne-qt-browser >= 0.6.2",  # alternative browser backend
 ]
 dev = [
     "mnelab[full]",
+    "build",
     "pre-commit",
     "pytest",
+    "pytest-qt",
     "ruff",
-    "setuptools",
 ]
 
 [project.gui-scripts]
 mnelab = "mnelab:main"
 
 [project.urls]
 homepage = "https://github.com/cbrnr/mnelab"
 documentation = "https://mnelab.readthedocs.io/en/latest/"
 repository = "https://github.com/cbrnr/mnelab"
 changelog = "https://github.com/cbrnr/mnelab/blob/main/CHANGELOG.md"
 
+[tool.hatch.version]
+path = "src/mnelab/__init__.py"
+
 [tool.ruff]
-select = ["E", "F", "I", "W", "UP"]
 line-length = 92
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint]
+select = ["E", "F", "I", "W", "UP"]
+
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "mainwindow.py" = ["F405"]
-
-[tool.setuptools.dynamic]
-version = {attr = "mnelab.__version__"}
-readme = {file = "README.md", content-type = "text/markdown"}
```

