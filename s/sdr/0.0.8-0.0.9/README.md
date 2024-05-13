# Comparing `tmp/sdr-0.0.8.tar.gz` & `tmp/sdr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sdr/sdr/dist/.tmp-c6_3vypg/sdr-0.0.8.tar", last modified: Mon Sep  4 17:52:48 2023, max compression
+gzip compressed data, was "/home/runner/work/sdr/sdr/dist/.tmp-2_6kzbyz/sdr-0.0.9.tar", last modified: Sun Nov 12 21:10:09 2023, max compression
```

## Comparing `sdr-0.0.8.tar` & `sdr-0.0.9.tar`

### file list

```diff
@@ -1,193 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     1010 2023-09-04 17:52:23.000000 sdr-0.0.8/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     4875 2023-09-04 17:52:23.000000 sdr-0.0.8/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1465 2023-09-04 17:52:23.000000 sdr-0.0.8/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2232 2023-09-04 17:52:23.000000 sdr-0.0.8/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     5798 2023-09-04 17:52:23.000000 sdr-0.0.8/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      136 2023-09-04 17:52:23.000000 sdr-0.0.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (999)     1313 2023-09-04 17:52:23.000000 sdr-0.0.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (999)     1084 2023-09-04 17:52:23.000000 sdr-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     6156 2023-09-04 17:52:48.000000 sdr-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4363 2023-09-04 17:52:23.000000 sdr-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (999)       42 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)      634 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (999)     1336 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/_static/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (999)      421 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/_templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (999)      318 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/conversions.rst
--rw-r--r--   0 runner    (1001) docker     (999)       67 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/data-manipulation.rst
--rw-r--r--   0 runner    (1001) docker     (999)      169 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/detection.rst
--rw-r--r--   0 runner    (1001) docker     (999)      442 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/dsp.rst
--rw-r--r--   0 runner    (1001) docker     (999)      257 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/link-budgets.rst
--rw-r--r--   0 runner    (1001) docker     (999)      276 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/measurement.rst
--rw-r--r--   0 runner    (1001) docker     (999)      544 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/modulation.rst
--rw-r--r--   0 runner    (1001) docker     (999)      526 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/plotting.rst
--rw-r--r--   0 runner    (1001) docker     (999)       62 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/probability.rst
--rw-r--r--   0 runner    (1001) docker     (999)       56 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/sequences.rst
--rw-r--r--   0 runner    (1001) docker     (999)      193 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/simulation.rst
--rw-r--r--   0 runner    (1001) docker     (999)       62 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/api/synchronization.rst
--rw-r--r--   0 runner    (1001) docker     (999)    15737 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/docs/development/
--rw-r--r--   0 runner    (1001) docker     (999)     1204 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/development/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1755 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/development/installation.rst
--rw-r--r--   0 runner    (1001) docker     (999)      958 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/development/linter.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1238 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/development/unit-tests.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (999)   439036 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/examples/farrow-resampler.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)   408867 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/examples/fir-filters.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)   925481 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/examples/iir-filters.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)   772080 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/examples/peak-to-average-power.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)   582290 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/examples/phase-locked-loop.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)   917023 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/examples/psk.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)   926152 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/examples/pulse-shapes.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)     3891 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      760 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/docs/release-notes/
--rw-r--r--   0 runner    (1001) docker     (999)     6460 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/release-notes/v0.0.md
--rw-r--r--   0 runner    (1001) docker     (999)      723 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/release-notes/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (999)      131 2023-09-04 17:52:23.000000 sdr-0.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)     3808 2023-09-04 17:52:23.000000 sdr-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      103 2023-09-04 17:52:23.000000 sdr-0.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-04 17:52:48.000000 sdr-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr/
--rw-r--r--   0 runner    (1001) docker     (999)      831 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    10317 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (999)     5843 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_data.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr/_detection/
--rw-r--r--   0 runner    (1001) docker     (999)      128 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    11006 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_detection/_correlator.py
--rw-r--r--   0 runner    (1001) docker     (999)    12056 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_detection/_energy.py
--rw-r--r--   0 runner    (1001) docker     (999)     3300 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_detection/_theory.py
--rw-r--r--   0 runner    (1001) docker     (999)     5959 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_farrow.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr/_filter/
--rw-r--r--   0 runner    (1001) docker     (999)      112 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    10865 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_filter/_fir.py
--rw-r--r--   0 runner    (1001) docker     (999)    11327 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_filter/_iir.py
--rw-r--r--   0 runner    (1001) docker     (999)    33219 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_filter/_polyphase.py
--rw-r--r--   0 runner    (1001) docker     (999)     1662 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr/_link_budget/
--rw-r--r--   0 runner    (1001) docker     (999)      126 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_link_budget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2755 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_link_budget/_antenna.py
--rw-r--r--   0 runner    (1001) docker     (999)     6103 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_link_budget/_capacity.py
--rw-r--r--   0 runner    (1001) docker     (999)     2545 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_link_budget/_path_loss.py
--rw-r--r--   0 runner    (1001) docker     (999)     4885 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_loop_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr/_measurement/
--rw-r--r--   0 runner    (1001) docker     (999)      174 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      571 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_measurement/_energy.py
--rw-r--r--   0 runner    (1001) docker     (999)     5492 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_measurement/_errors.py
--rw-r--r--   0 runner    (1001) docker     (999)     5242 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_measurement/_modulation.py
--rw-r--r--   0 runner    (1001) docker     (999)     2132 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_measurement/_power.py
--rw-r--r--   0 runner    (1001) docker     (999)     2137 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_measurement/_voltage.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr/_modulation/
--rw-r--r--   0 runner    (1001) docker     (999)      208 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_modulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    11266 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_modulation/_linear.py
--rw-r--r--   0 runner    (1001) docker     (999)     5031 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_modulation/_msk.py
--rw-r--r--   0 runner    (1001) docker     (999)    31888 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_modulation/_psk.py
--rw-r--r--   0 runner    (1001) docker     (999)    16557 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_modulation/_pulse_shapes.py
--rw-r--r--   0 runner    (1001) docker     (999)     3294 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_modulation/_symbol_encoding.py
--rw-r--r--   0 runner    (1001) docker     (999)     1599 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_modulation/_symbol_mapping.py
--rw-r--r--   0 runner    (1001) docker     (999)     7024 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_nco.py
--rw-r--r--   0 runner    (1001) docker     (999)     9037 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_pll.py
--rw-r--r--   0 runner    (1001) docker     (999)     1428 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_probability.py
--rw-r--r--   0 runner    (1001) docker     (999)     6550 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_sequence.py
--rw-r--r--   0 runner    (1001) docker     (999)    14785 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr/_simulation/
--rw-r--r--   0 runner    (1001) docker     (999)      124 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4760 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_simulation/_channel_model.py
--rw-r--r--   0 runner    (1001) docker     (999)    11867 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/_simulation/_impairment.py
--rw-r--r--   0 runner    (1001) docker     (999)      160 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr/plot/
--rw-r--r--   0 runner    (1001) docker     (999)      280 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3051 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/plot/_detection.py
--rw-r--r--   0 runner    (1001) docker     (999)    26010 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/plot/_filter.py
--rw-r--r--   0 runner    (1001) docker     (999)    14674 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/plot/_modulation.py
--rw-r--r--   0 runner    (1001) docker     (999)      852 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/plot/_rc_params.py
--rw-r--r--   0 runner    (1001) docker     (999)     7287 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/plot/_spectral_estimation.py
--rw-r--r--   0 runner    (1001) docker     (999)     9796 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/plot/_time_domain.py
--rw-r--r--   0 runner    (1001) docker     (999)     1476 2023-09-04 17:52:23.000000 sdr-0.0.8/src/sdr/plot/_units.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     6156 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4691 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       56 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-09-04 17:52:48.000000 sdr-0.0.8/src/sdr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/conversions/
--rw-r--r--   0 runner    (1001) docker     (999)     1960 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/conversions/test_ebn0_to_esn0.py
--rw-r--r--   0 runner    (1001) docker     (999)     2029 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/conversions/test_ebn0_to_snr.py
--rw-r--r--   0 runner    (1001) docker     (999)     1960 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/conversions/test_esn0_to_ebn0.py
--rw-r--r--   0 runner    (1001) docker     (999)     1697 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/conversions/test_esn0_to_snr.py
--rw-r--r--   0 runner    (1001) docker     (999)     2035 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/conversions/test_snr_to_ebn0.py
--rw-r--r--   0 runner    (1001) docker     (999)     1703 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/conversions/test_snr_to_esn0.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/data_manipulation/
--rw-r--r--   0 runner    (1001) docker     (999)     1362 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/data_manipulation/test_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (999)     2405 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/data_manipulation/test_pack.py
--rw-r--r--   0 runner    (1001) docker     (999)     2615 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/data_manipulation/test_unpack.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/detection/
--rw-r--r--   0 runner    (1001) docker     (999)     3202 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/detection/test_albersheim.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/dsp/
--rw-r--r--   0 runner    (1001) docker     (999)    14015 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_decimator.py
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_downsample.py
--rw-r--r--   0 runner    (1001) docker     (999)     2262 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_farrow.py
--rw-r--r--   0 runner    (1001) docker     (999)     1888 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_fir.py
--rw-r--r--   0 runner    (1001) docker     (999)     1394 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_iir.py
--rw-r--r--   0 runner    (1001) docker     (999)    22490 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (999)     1337 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_mix.py
--rw-r--r--   0 runner    (1001) docker     (999)    18112 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_multirate_taps.py
--rw-r--r--   0 runner    (1001) docker     (999)      341 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_to_complex_bb.py
--rw-r--r--   0 runner    (1001) docker     (999)      335 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_to_real_pb.py
--rw-r--r--   0 runner    (1001) docker     (999)     1120 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/dsp/test_upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/link_budgets/
--rw-r--r--   0 runner    (1001) docker     (999)      264 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/link_budgets/test_awgn_capacity.py
--rw-r--r--   0 runner    (1001) docker     (999)      533 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/link_budgets/test_bec_capacity.py
--rw-r--r--   0 runner    (1001) docker     (999)      633 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/link_budgets/test_bsc_capacity.py
--rw-r--r--   0 runner    (1001) docker     (999)     4392 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/link_budgets/test_fspl.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/measurements/
--rw-r--r--   0 runner    (1001) docker     (999)      939 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/measurements/test_crest_factor.py
--rw-r--r--   0 runner    (1001) docker     (999)      431 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/measurements/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (999)      711 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/measurements/test_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (999)     6219 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/measurements/test_evm.py
--rw-r--r--   0 runner    (1001) docker     (999)      891 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/measurements/test_papr.py
--rw-r--r--   0 runner    (1001) docker     (999)      487 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/measurements/test_power.py
--rw-r--r--   0 runner    (1001) docker     (999)      490 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/measurements/test_voltage.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/modulation/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/modulation/psk/
--rw-r--r--   0 runner    (1001) docker     (999)     6123 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/psk/test_ber.py
--rw-r--r--   0 runner    (1001) docker     (999)     3189 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/psk/test_ber_diff.py
--rw-r--r--   0 runner    (1001) docker     (999)     3637 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/psk/test_decide_symbols.py
--rw-r--r--   0 runner    (1001) docker     (999)     1522 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/psk/test_demodulate.py
--rw-r--r--   0 runner    (1001) docker     (999)    13791 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/psk/test_map_symbols.py
--rw-r--r--   0 runner    (1001) docker     (999)     1826 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/psk/test_modulate.py
--rw-r--r--   0 runner    (1001) docker     (999)     6271 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/psk/test_ser.py
--rw-r--r--   0 runner    (1001) docker     (999)     3313 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/psk/test_ser_diff.py
--rw-r--r--   0 runner    (1001) docker     (999)      852 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/test_binary_code.py
--rw-r--r--   0 runner    (1001) docker     (999)      861 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/test_diff_decode.py
--rw-r--r--   0 runner    (1001) docker     (999)      861 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/test_diff_encode.py
--rw-r--r--   0 runner    (1001) docker     (999)     4834 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (999)      844 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/test_gray_code.py
--rw-r--r--   0 runner    (1001) docker     (999)      842 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/test_half_sine.py
--rw-r--r--   0 runner    (1001) docker     (999)    14497 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/test_raised_cosine.py
--rw-r--r--   0 runner    (1001) docker     (999)      758 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/test_rectangular.py
--rw-r--r--   0 runner    (1001) docker     (999)    14473 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/modulation/test_root_raised_cosine.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/probability/
--rw-r--r--   0 runner    (1001) docker     (999)     2380 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/probability/test_normal.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/sequences/
--rw-r--r--   0 runner    (1001) docker     (999)     2247 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/sequences/test_barker.py
--rw-r--r--   0 runner    (1001) docker     (999)    12009 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/sequences/test_zadoff_chu.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/simulation/
--rw-r--r--   0 runner    (1001) docker     (999)     2411 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/simulation/test_awgn.py
--rw-r--r--   0 runner    (1001) docker     (999)      622 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/simulation/test_bec.py
--rw-r--r--   0 runner    (1001) docker     (999)      623 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/simulation/test_bsc.py
--rw-r--r--   0 runner    (1001) docker     (999)     1386 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/simulation/test_dmc.py
--rw-r--r--   0 runner    (1001) docker     (999)      486 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/simulation/test_iq_imbalance.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:52:48.000000 sdr-0.0.8/tests/synchronization/
--rw-r--r--   0 runner    (1001) docker     (999)      779 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/synchronization/test_dds.py
--rw-r--r--   0 runner    (1001) docker     (999)     1349 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/synchronization/test_loop_filter.py
--rw-r--r--   0 runner    (1001) docker     (999)      725 2023-09-04 17:52:23.000000 sdr-0.0.8/tests/synchronization/test_nco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-11-12 21:09:53.000000 sdr-0.0.9/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2023-11-12 21:09:53.000000 sdr-0.0.9/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-11-12 21:09:53.000000 sdr-0.0.9/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-11-12 21:09:53.000000 sdr-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2023-11-12 21:09:53.000000 sdr-0.0.9/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-12 21:09:53.000000 sdr-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-11-12 21:09:53.000000 sdr-0.0.9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-11-12 21:09:53.000000 sdr-0.0.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-12 21:09:53.000000 sdr-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2023-11-12 21:10:09.000000 sdr-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2023-11-12 21:09:53.000000 sdr-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/_static/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/_templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/conversions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/data-manipulation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/detection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/dsp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/link-budgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/measurement.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/modulation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/probability.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/sequences.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/api/synchronization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15847 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/development/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/development/formatting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/development/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/development/unit-tests.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   439036 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/examples/farrow-resampler.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   408867 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/examples/fir-filters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   925481 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/examples/iir-filters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   772080 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/examples/peak-to-average-power.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   582290 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/examples/phase-locked-loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   917023 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/examples/psk.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   926152 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/examples/pulse-shapes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/docs/release-notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/release-notes/v0.0.md
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/release-notes/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2023-11-12 21:09:53.000000 sdr-0.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2023-11-12 21:09:53.000000 sdr-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-12 21:09:53.000000 sdr-0.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-12 21:10:09.000000 sdr-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10942 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_detection/_correlator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12008 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_detection/_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_detection/_theory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_farrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13240 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_filter/_fir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13630 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_filter/_iir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49333 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_filter/_polyphase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/_link_budget/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_link_budget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_link_budget/_antenna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_link_budget/_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_link_budget/_path_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/_measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_measurement/_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_measurement/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_measurement/_modulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_measurement/_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_measurement/_voltage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/_modulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_modulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11511 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_modulation/_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_modulation/_msk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31918 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_modulation/_psk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16668 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_modulation/_pulse_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_modulation/_symbol_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_modulation/_symbol_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14668 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_simulation/_channel_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_simulation/_impairment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/_synchronization/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_synchronization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_synchronization/_loop_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_synchronization/_nco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/_synchronization/_pll.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/plot/_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25954 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/plot/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/plot/_modulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/plot/_rc_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/plot/_spectral_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/plot/_time_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-11-12 21:09:53.000000 sdr-0.0.9/src/sdr/plot/_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-12 21:10:09.000000 sdr-0.0.9/src/sdr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/test_ebn0_to_esn0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/test_ebn0_to_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/test_esn0_to_ebn0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/test_esn0_to_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/test_percent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/test_ppb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/test_ppm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/test_snr_to_ebn0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/conversions/test_snr_to_esn0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/data_manipulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/data_manipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/data_manipulation/test_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/data_manipulation/test_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/data_manipulation/test_unpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/detection/test_albersheim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/dsp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_decimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_differentiator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_farrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_fir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_iir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22780 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18112 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_multirate_taps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_to_complex_bb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_to_real_pb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/dsp/test_upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/link_budgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/link_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/link_budgets/test_awgn_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/link_budgets/test_bec_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/link_budgets/test_bsc_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/link_budgets/test_fspl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/measurements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/measurements/test_crest_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/measurements/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/measurements/test_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/measurements/test_evm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/measurements/test_papr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/measurements/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/measurements/test_voltage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/modulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/modulation/cpm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/cpm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/modulation/msk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/msk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/modulation/psk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/psk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/psk/test_ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/psk/test_ber_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/psk/test_decide_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/psk/test_demodulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/psk/test_map_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/psk/test_modulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/psk/test_ser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/psk/test_ser_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/test_binary_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/test_diff_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/test_diff_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/test_gray_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/test_half_sine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14497 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/test_raised_cosine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/test_rectangular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14473 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/modulation/test_root_raised_cosine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/probability/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/probability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/probability/test_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/sequences/test_barker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/sequences/test_zadoff_chu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/simulation/test_awgn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/simulation/test_bec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/simulation/test_bsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/simulation/test_dmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/simulation/test_iq_imbalance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 21:10:09.000000 sdr-0.0.9/tests/synchronization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/synchronization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/synchronization/test_loop_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2023-11-12 21:09:53.000000 sdr-0.0.9/tests/synchronization/test_nco.py
```

### Comparing `sdr-0.0.8/.github/workflows/build.yaml` & `sdr-0.0.9/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/.github/workflows/docs.yaml` & `sdr-0.0.9/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/.github/workflows/lint.yaml` & `sdr-0.0.9/.github/workflows/lint.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   pull_request:
     branches:
       - main
       - 'release/*'
 
 jobs:
   run-linter:
-    name: Lint
+    name: Ruff Lint
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [3.7, 3.8, 3.9, '3.10', 3.11]
     steps:
       - uses: actions/checkout@v3
 
@@ -30,22 +30,19 @@
 
       - name: Install the dev requirements
         run: python3 -m pip install -r requirements-dev.txt
 
       - name: Install the `sdr` package
         run: python3 -m pip install .
 
-      - name: Lint code with pylint
-        run: python3 -m pylint src/sdr/
-
-      # - name: Lint tests with pylint
-      #   run: python3 -m pylint tests/
+      - name: Lint with ruff
+        run: python3 -m ruff check --output-format=github .
 
   run-formatter:
-    name: Format
+    name: Ruff Format
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python 3.10
         uses: actions/setup-python@v4
         with:
@@ -56,9 +53,9 @@
 
       - name: Install the dev requirements
         run: python3 -m pip install -r requirements-dev.txt
 
       - name: Install the `sdr` package
         run: python3 -m pip install .
 
-      - name: Format with black
-        run: python3 -m black . --check
+      - name: Format with ruff
+        run: python3 -m ruff format --check .
```

### Comparing `sdr-0.0.8/.github/workflows/release.yaml` & `sdr-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/.github/workflows/test.yaml` & `sdr-0.0.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/LICENSE` & `sdr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/PKG-INFO` & `sdr-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdr
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for software-defined radio
 Author-email: Matt Hostetter <matthostetter@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mhostetter/sdr
 Project-URL: Source, https://github.com/mhostetter/sdr
 Project-URL: Issues, https://github.com/mhostetter/sdr/issues
 Project-URL: Documentation, https://mhostetter.github.io/sdr/latest/
@@ -57,15 +57,15 @@
 The `sdr` library is a Python 3 package for software-defined radio (SDR).
 
 The goal of `sdr` is to provide tools to design, analyze, build, and test digital communication systems
 in Python. The library relies on and is designed to be interoperable with NumPy, SciPy, and Matplotlib.
 Performance is also very important. So, where possible, Numba is used to accelerate computationally-intensive
 functions.
 
-Additionally, the library aims to replicate relevant functionality from Matlab's Communications and
+Additionally, the library aims to replicate relevant functionality from MATLAB's Communications and
 DSP Toolboxes.
 
 We are progressively adding functionality to the library. If there is something you'd like to see included
 in `sdr`, please open an issue on GitHub.
 
 > Enjoying the library? Give us a :star: on [GitHub](https://github.com/mhostetter/sdr)!
 
@@ -83,27 +83,26 @@
 
 ## Features
 
 View all available classes and functions in the [API Reference](https://mhostetter.github.io/sdr/latest/api/dsp/).
 
 - **Digital signal processing**: Finite impulse response (FIR) filters, infinite impulse response (IIR) filters,
   polyphase interpolator, polyphase decimator, polyphase resampler, Farrow arbitrary resampler,
-  complex mixing, real/complex conversion.
+  FIR differentiator, IIR integrator, complex mixing, real/complex conversion.
 - **Sequences**: Barker, Zadoff-Chu.
 - **Modulation**: Phase-shift keying (PSK), $\pi/M$ PSK, offset QPSK, rectangular pulse shape, half-sine pulse shape,
   raised cosine pulse shape, root raised cosine pulse shape, Gaussian pulse shape, binary and Gray symbol mapping,
   differential encoding.
-- **Synchronization**: Numerically-controlled oscillators (NCO), direct digital synthesizers (DDS), loop filters,
-  closed-loop PLL analysis.
+- **Synchronization**: Numerically-controlled oscillators (NCO), loop filters, closed-loop PLL analysis.
 - **Measurement**: Energy, power, voltage, bit/symbol error rate, error vector magnitude (EVM).
 - **Conversions**: Between linear units and decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$.
 - **Simulation**: Binary symmetric channel (BSC), binary erasure channel (BEC), discrete memoryless channel (DMC),
   additive white Gaussian noise (AWGN), frequency offset, sample rate offset, IQ imbalance.
 - **Link budgets**: Channel capacities, free-space path loss, antenna gains.
-- **Data manipulation**: Packing and unpacking binary data, hexdumping binary data.
+- **Data manipulation**: Packing and unpacking binary data, hexdump of binary data.
 - **Plotting**: Time-domain, raster, periodogram, spectrogram, constellation, symbol map, eye diagram,
   bit error rate (BER), symbol error rate (SER), impulse response, step response, magnitude response, phase response,
   phase delay, group delay, and zeros/poles.
 
 ## Examples
 
 There are detailed examples published at <https://mhostetter.github.io/sdr/latest/examples/pulse-shapes/>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdr Version: 0.0.8 Summary: A Python package for
+Metadata-Version: 2.1 Name: sdr Version: 0.0.9 Summary: A Python package for
 software-defined radio Author-email: Matt Hostetter
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/mhostetter/
 sdr Project-URL: Source, https://github.com/mhostetter/sdr Project-URL: Issues,
 https://github.com/mhostetter/sdr/issues Project-URL: Documentation, https://
 mhostetter.github.io/sdr/latest/ Project-URL: Discuss, https://github.com/
 mhostetter/sdr/discussions Project-URL: Twitter, https://twitter.com/sdr_py
 Keywords: software-defined radio,sdr,digital communications,wireless
@@ -35,39 +35,39 @@
                           _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_F_J_M_L_7_9_Z_U_K_]
 The `sdr` library is a Python 3 package for software-defined radio (SDR). The
 goal of `sdr` is to provide tools to design, analyze, build, and test digital
 communication systems in Python. The library relies on and is designed to be
 interoperable with NumPy, SciPy, and Matplotlib. Performance is also very
 important. So, where possible, Numba is used to accelerate computationally-
 intensive functions. Additionally, the library aims to replicate relevant
-functionality from Matlab's Communications and DSP Toolboxes. We are
+functionality from MATLAB's Communications and DSP Toolboxes. We are
 progressively adding functionality to the library. If there is something you'd
 like to see included in `sdr`, please open an issue on GitHub. > Enjoying the
 library? Give us a :star: on [GitHub](https://github.com/mhostetter/sdr)! ##
 Documentation The documentation for `sdr` is located at
 mhostetter.github.io/sdr/latest/>. ## Installation The latest version of `sdr`
 can be installed from [PyPI](https://pypi.org/project/sdr/) using `pip`.
 ```console python3 -m pip install sdr ``` ## Features View all available
 classes and functions in the [API Reference](https://mhostetter.github.io/sdr/
 latest/api/dsp/). - **Digital signal processing**: Finite impulse response
 (FIR) filters, infinite impulse response (IIR) filters, polyphase interpolator,
-polyphase decimator, polyphase resampler, Farrow arbitrary resampler, complex
-mixing, real/complex conversion. - **Sequences**: Barker, Zadoff-Chu. -
-**Modulation**: Phase-shift keying (PSK), $\pi/M$ PSK, offset QPSK, rectangular
-pulse shape, half-sine pulse shape, raised cosine pulse shape, root raised
-cosine pulse shape, Gaussian pulse shape, binary and Gray symbol mapping,
-differential encoding. - **Synchronization**: Numerically-controlled
-oscillators (NCO), direct digital synthesizers (DDS), loop filters, closed-loop
-PLL analysis. - **Measurement**: Energy, power, voltage, bit/symbol error rate,
-error vector magnitude (EVM). - **Conversions**: Between linear units and
-decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$. - **Simulation**: Binary
-symmetric channel (BSC), binary erasure channel (BEC), discrete memoryless
-channel (DMC), additive white Gaussian noise (AWGN), frequency offset, sample
-rate offset, IQ imbalance. - **Link budgets**: Channel capacities, free-space
-path loss, antenna gains. - **Data manipulation**: Packing and unpacking binary
-data, hexdumping binary data. - **Plotting**: Time-domain, raster, periodogram,
-spectrogram, constellation, symbol map, eye diagram, bit error rate (BER),
-symbol error rate (SER), impulse response, step response, magnitude response,
-phase response, phase delay, group delay, and zeros/poles. ## Examples There
-are detailed examples published at
+polyphase decimator, polyphase resampler, Farrow arbitrary resampler, FIR
+differentiator, IIR integrator, complex mixing, real/complex conversion. -
+**Sequences**: Barker, Zadoff-Chu. - **Modulation**: Phase-shift keying (PSK),
+$\pi/M$ PSK, offset QPSK, rectangular pulse shape, half-sine pulse shape,
+raised cosine pulse shape, root raised cosine pulse shape, Gaussian pulse
+shape, binary and Gray symbol mapping, differential encoding. -
+**Synchronization**: Numerically-controlled oscillators (NCO), loop filters,
+closed-loop PLL analysis. - **Measurement**: Energy, power, voltage, bit/symbol
+error rate, error vector magnitude (EVM). - **Conversions**: Between linear
+units and decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$. - **Simulation**:
+Binary symmetric channel (BSC), binary erasure channel (BEC), discrete
+memoryless channel (DMC), additive white Gaussian noise (AWGN), frequency
+offset, sample rate offset, IQ imbalance. - **Link budgets**: Channel
+capacities, free-space path loss, antenna gains. - **Data manipulation**:
+Packing and unpacking binary data, hexdump of binary data. - **Plotting**:
+Time-domain, raster, periodogram, spectrogram, constellation, symbol map, eye
+diagram, bit error rate (BER), symbol error rate (SER), impulse response, step
+response, magnitude response, phase response, phase delay, group delay, and
+zeros/poles. ## Examples There are detailed examples published at
 mhostetter.github.io/sdr/latest/examples/pulse-shapes/>. The Jupyter notebooks
 behind the examples are available for experimentation in `docs/examples/`.
```

### Comparing `sdr-0.0.8/README.md` & `sdr-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 The `sdr` library is a Python 3 package for software-defined radio (SDR).
 
 The goal of `sdr` is to provide tools to design, analyze, build, and test digital communication systems
 in Python. The library relies on and is designed to be interoperable with NumPy, SciPy, and Matplotlib.
 Performance is also very important. So, where possible, Numba is used to accelerate computationally-intensive
 functions.
 
-Additionally, the library aims to replicate relevant functionality from Matlab's Communications and
+Additionally, the library aims to replicate relevant functionality from MATLAB's Communications and
 DSP Toolboxes.
 
 We are progressively adding functionality to the library. If there is something you'd like to see included
 in `sdr`, please open an issue on GitHub.
 
 > Enjoying the library? Give us a :star: on [GitHub](https://github.com/mhostetter/sdr)!
 
@@ -46,27 +46,26 @@
 
 ## Features
 
 View all available classes and functions in the [API Reference](https://mhostetter.github.io/sdr/latest/api/dsp/).
 
 - **Digital signal processing**: Finite impulse response (FIR) filters, infinite impulse response (IIR) filters,
   polyphase interpolator, polyphase decimator, polyphase resampler, Farrow arbitrary resampler,
-  complex mixing, real/complex conversion.
+  FIR differentiator, IIR integrator, complex mixing, real/complex conversion.
 - **Sequences**: Barker, Zadoff-Chu.
 - **Modulation**: Phase-shift keying (PSK), $\pi/M$ PSK, offset QPSK, rectangular pulse shape, half-sine pulse shape,
   raised cosine pulse shape, root raised cosine pulse shape, Gaussian pulse shape, binary and Gray symbol mapping,
   differential encoding.
-- **Synchronization**: Numerically-controlled oscillators (NCO), direct digital synthesizers (DDS), loop filters,
-  closed-loop PLL analysis.
+- **Synchronization**: Numerically-controlled oscillators (NCO), loop filters, closed-loop PLL analysis.
 - **Measurement**: Energy, power, voltage, bit/symbol error rate, error vector magnitude (EVM).
 - **Conversions**: Between linear units and decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$.
 - **Simulation**: Binary symmetric channel (BSC), binary erasure channel (BEC), discrete memoryless channel (DMC),
   additive white Gaussian noise (AWGN), frequency offset, sample rate offset, IQ imbalance.
 - **Link budgets**: Channel capacities, free-space path loss, antenna gains.
-- **Data manipulation**: Packing and unpacking binary data, hexdumping binary data.
+- **Data manipulation**: Packing and unpacking binary data, hexdump of binary data.
 - **Plotting**: Time-domain, raster, periodogram, spectrogram, constellation, symbol map, eye diagram,
   bit error rate (BER), symbol error rate (SER), impulse response, step response, magnitude response, phase response,
   phase delay, group delay, and zeros/poles.
 
 ## Examples
 
 There are detailed examples published at <https://mhostetter.github.io/sdr/latest/examples/pulse-shapes/>.
```

#### html2text {}

```diff
@@ -11,39 +11,39 @@
                           _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_F_J_M_L_7_9_Z_U_K_]
 The `sdr` library is a Python 3 package for software-defined radio (SDR). The
 goal of `sdr` is to provide tools to design, analyze, build, and test digital
 communication systems in Python. The library relies on and is designed to be
 interoperable with NumPy, SciPy, and Matplotlib. Performance is also very
 important. So, where possible, Numba is used to accelerate computationally-
 intensive functions. Additionally, the library aims to replicate relevant
-functionality from Matlab's Communications and DSP Toolboxes. We are
+functionality from MATLAB's Communications and DSP Toolboxes. We are
 progressively adding functionality to the library. If there is something you'd
 like to see included in `sdr`, please open an issue on GitHub. > Enjoying the
 library? Give us a :star: on [GitHub](https://github.com/mhostetter/sdr)! ##
 Documentation The documentation for `sdr` is located at
 mhostetter.github.io/sdr/latest/>. ## Installation The latest version of `sdr`
 can be installed from [PyPI](https://pypi.org/project/sdr/) using `pip`.
 ```console python3 -m pip install sdr ``` ## Features View all available
 classes and functions in the [API Reference](https://mhostetter.github.io/sdr/
 latest/api/dsp/). - **Digital signal processing**: Finite impulse response
 (FIR) filters, infinite impulse response (IIR) filters, polyphase interpolator,
-polyphase decimator, polyphase resampler, Farrow arbitrary resampler, complex
-mixing, real/complex conversion. - **Sequences**: Barker, Zadoff-Chu. -
-**Modulation**: Phase-shift keying (PSK), $\pi/M$ PSK, offset QPSK, rectangular
-pulse shape, half-sine pulse shape, raised cosine pulse shape, root raised
-cosine pulse shape, Gaussian pulse shape, binary and Gray symbol mapping,
-differential encoding. - **Synchronization**: Numerically-controlled
-oscillators (NCO), direct digital synthesizers (DDS), loop filters, closed-loop
-PLL analysis. - **Measurement**: Energy, power, voltage, bit/symbol error rate,
-error vector magnitude (EVM). - **Conversions**: Between linear units and
-decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$. - **Simulation**: Binary
-symmetric channel (BSC), binary erasure channel (BEC), discrete memoryless
-channel (DMC), additive white Gaussian noise (AWGN), frequency offset, sample
-rate offset, IQ imbalance. - **Link budgets**: Channel capacities, free-space
-path loss, antenna gains. - **Data manipulation**: Packing and unpacking binary
-data, hexdumping binary data. - **Plotting**: Time-domain, raster, periodogram,
-spectrogram, constellation, symbol map, eye diagram, bit error rate (BER),
-symbol error rate (SER), impulse response, step response, magnitude response,
-phase response, phase delay, group delay, and zeros/poles. ## Examples There
-are detailed examples published at
+polyphase decimator, polyphase resampler, Farrow arbitrary resampler, FIR
+differentiator, IIR integrator, complex mixing, real/complex conversion. -
+**Sequences**: Barker, Zadoff-Chu. - **Modulation**: Phase-shift keying (PSK),
+$\pi/M$ PSK, offset QPSK, rectangular pulse shape, half-sine pulse shape,
+raised cosine pulse shape, root raised cosine pulse shape, Gaussian pulse
+shape, binary and Gray symbol mapping, differential encoding. -
+**Synchronization**: Numerically-controlled oscillators (NCO), loop filters,
+closed-loop PLL analysis. - **Measurement**: Energy, power, voltage, bit/symbol
+error rate, error vector magnitude (EVM). - **Conversions**: Between linear
+units and decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$. - **Simulation**:
+Binary symmetric channel (BSC), binary erasure channel (BEC), discrete
+memoryless channel (DMC), additive white Gaussian noise (AWGN), frequency
+offset, sample rate offset, IQ imbalance. - **Link budgets**: Channel
+capacities, free-space path loss, antenna gains. - **Data manipulation**:
+Packing and unpacking binary data, hexdump of binary data. - **Plotting**:
+Time-domain, raster, periodogram, spectrogram, constellation, symbol map, eye
+diagram, bit error rate (BER), symbol error rate (SER), impulse response, step
+response, magnitude response, phase response, phase delay, group delay, and
+zeros/poles. ## Examples There are detailed examples published at
 mhostetter.github.io/sdr/latest/examples/pulse-shapes/>. The Jupyter notebooks
 behind the examples are available for experimentation in `docs/examples/`.
```

### Comparing `sdr-0.0.8/docs/Makefile` & `sdr-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/_static/extra.css` & `sdr-0.0.9/docs/_static/extra.css`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/api/modulation.rst` & `sdr-0.0.9/docs/api/modulation.rst`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/api/plotting.rst` & `sdr-0.0.9/docs/api/plotting.rst`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/conf.py` & `sdr-0.0.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,15 @@
 html_use_index = True
 html_domain_indices = True
 
 nitpicky = True
 nitpick_ignore = [
     ("py:class", "numpy.typing.ArrayLike"),  # Wish this would work
     ("py:class", "numpy.typing.DTypeLike"),  # Wish this would work
+    ("py:class", "numpy.typing.NDArray"),  # Wish this would work
 ]
 
 
 # -- Extension configuration -------------------------------------------------
 
 # Create hyperlinks to other documentation
 intersphinx_mapping = {
@@ -211,14 +212,15 @@
 autodoc_typehints = "signature"
 autodoc_typehints_description_target = "documented"
 autodoc_typehints_format = "short"
 
 autodoc_type_aliases = {
     "npt.ArrayLike": "~numpy.typing.ArrayLike",
     "npt.DTypeLike": "~numpy.typing.DTypeLike",
+    "npt.NDArray": "~numpy.typing.NDArray",
 }
 
 ipython_execlines = [
     "import math",
     "import matplotlib.pyplot as plt",
     "import numpy as np",
     "import sdr",
```

### Comparing `sdr-0.0.8/docs/development/documentation.rst` & `sdr-0.0.9/docs/development/documentation.rst`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/development/installation.rst` & `sdr-0.0.9/docs/development/installation.rst`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/development/linter.rst` & `sdr-0.0.9/docs/development/formatting.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,77 @@
-Linter
-======
+Formatting
+==========
 
-The :obj:`sdr` library uses `pylint <https://pylint.org/>`_ for static analysis and code
+The :obj:`sdr` library uses `Ruff <https://docs.astral.sh/ruff/>`_ for static analysis, linting, and code
 formatting.
 
 Install
 -------
 
-First, `pylint` needs to be installed on your system. Easily install it by installing the development dependencies.
+First, `ruff` needs to be installed on your system. Easily install it by installing the development dependencies.
 
 .. code-block:: console
 
    $ python3 -m pip install -r requirements-dev.txt
 
 Configuration
 -------------
 
-Various nuisance `pylint` warnings are added to an ignore list in `pyproject.toml`.
+The `ruff` configuration is provided in `pyproject.toml`.
 
 .. literalinclude:: ../../pyproject.toml
    :caption: pyproject.toml
-   :start-at: [tool.pylint]
-   :end-before: [tool.black]
+   :start-at: [tool.ruff]
+   :end-before: [tool.pytest.ini_options]
    :language: toml
 
-Run from the command line
--------------------------
+Run the linter
+--------------
 
-Run the linter manually from the command line.
+Run the Ruff linter manually from the command line.
 
 .. code-block:: console
 
-   $ python3 -m pylint src/sdr/
+   $ python3 -m ruff check .
+
+Run the formatter
+-----------------
+
+Run the Ruff formatter manually from the command line.
+
+.. code-block:: console
+
+   $ python3 -m ruff format --check .
+
+Pre-commit
+----------
+
+A `pre-commit` configuration file with various hooks is provided in `.pre-commit-config.yaml`.
+
+.. literalinclude:: ../../.pre-commit-config.yaml
+   :caption: .pre-commit-config.yaml
+   :language: yaml
+
+Enable `pre-commit` by installing the pre-commit hooks.
+
+.. code-block:: console
+
+   $ pre-commit install
+
+Run `pre-commit` on all files.
+
+.. code-block:: console
+
+   $ pre-commit run --all-files
+
+Disable `pre-commit` by uninstalling the pre-commit hooks.
+
+.. code-block:: console
+
+   $ pre-commit uninstall
 
 Run from VS Code
 ----------------
 
+Install the `Ruff extension <https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff>`_ for VS Code.
 Included is a VS Code configuration file `.vscode/settings.json`.
-This instructs VS Code about how to invoke `pylint`.
-VS Code will run the linter as you view and edit files.
+VS Code will run the linter and formatter as you view and edit files.
```

### Comparing `sdr-0.0.8/docs/development/unit-tests.rst` & `sdr-0.0.9/docs/development/unit-tests.rst`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/examples/farrow-resampler.ipynb` & `sdr-0.0.9/docs/examples/farrow-resampler.ipynb`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/examples/fir-filters.ipynb` & `sdr-0.0.9/docs/examples/fir-filters.ipynb`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/examples/iir-filters.ipynb` & `sdr-0.0.9/docs/examples/iir-filters.ipynb`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/examples/peak-to-average-power.ipynb` & `sdr-0.0.9/docs/examples/peak-to-average-power.ipynb`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/examples/phase-locked-loop.ipynb` & `sdr-0.0.9/docs/examples/phase-locked-loop.ipynb`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/examples/psk.ipynb` & `sdr-0.0.9/docs/examples/psk.ipynb`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/examples/pulse-shapes.ipynb` & `sdr-0.0.9/docs/examples/pulse-shapes.ipynb`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/index.rst` & `sdr-0.0.9/docs/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 The :obj:`sdr` library is a Python 3 package for software-defined radio (SDR).
 
 The goal of :obj:`sdr` is to provide tools to design, analyze, build, and test digital communication systems
 in Python. The library relies on and is designed to be interoperable with `NumPy`_, `SciPy`_, and `Matplotlib`_.
 Performance is also very important. So, where possible, `Numba`_ is used to accelerate computationally-intensive
 functions.
 
-Additionally, the library aims to replicate relevant functionality from Matlab's `Communications`_ and
+Additionally, the library aims to replicate relevant functionality from MATLAB's `Communications`_ and
 `DSP`_ Toolboxes.
 
 We are progressively adding functionality to the library. If there is something you'd like to see included
 in :obj:`sdr`, please open an issue on `GitHub`_.
 
 .. _NumPy: https://numpy.org/
 .. _SciPy: https://www.scipy.org/
@@ -37,27 +37,26 @@
 Features
 --------
 
 View all available classes and functions in the `API Reference <https://mhostetter.github.io/sdr/latest/api/dsp/>`_.
 
 - **Digital signal processing**: Finite impulse response (FIR) filters, infinite impulse response (IIR) filters,
   polyphase interpolator, polyphase decimator, polyphase resampler, Farrow arbitrary resampler,
-  complex mixing, real/complex conversion.
+  FIR differentiator, IIR integrator, complex mixing, real/complex conversion.
 - **Sequences**: Barker, Zadoff-Chu.
 - **Modulation**: Phase-shift keying (PSK), $\pi/M$ PSK, offset QPSK, rectangular pulse shape, half-sine pulse shape,
   raised cosine pulse shape, root raised cosine pulse shape, Gaussian pulse shape, binary and Gray symbol mapping,
   differential encoding.
-- **Synchronization**: Numerically-controlled oscillators (NCO), direct digital synthesizers (DDS), loop filters,
-  closed-loop PLL analysis.
+- **Synchronization**: Numerically-controlled oscillators (NCO), loop filters, closed-loop PLL analysis.
 - **Measurement**: Energy, power, voltage, bit/symbol error rate, error vector magnitude (EVM).
 - **Conversions**: Between linear units and decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$.
 - **Simulation**: Binary symmetric channel (BSC), binary erasure channel (BEC), discrete memoryless channel (DMC),
   additive white Gaussian noise (AWGN), frequency offset, sample rate offset, IQ imbalance.
 - **Link budgets**: Channel capacities, free-space path loss, antenna gains.
-- **Data manipulation**: Packing and unpacking binary data, hexdumping binary data.
+- **Data manipulation**: Packing and unpacking binary data, hexdump of binary data.
 - **Plotting**: Time-domain, raster, periodogram, spectrogram, constellation, symbol map, eye diagram,
   bit error rate (BER), symbol error rate (SER), impulse response, step response, magnitude response, phase response,
   phase delay, group delay, and zeros/poles.
 
 .. toctree::
    :caption: Examples
    :hidden:
@@ -71,15 +70,15 @@
    examples/phase-locked-loop.ipynb
 
 .. toctree::
    :caption: Development
    :hidden:
 
    development/installation.rst
-   development/linter.rst
+   development/formatting.rst
    development/unit-tests.rst
    development/documentation.rst
 
 .. toctree::
    :caption: API Reference
    :hidden:
    :maxdepth: 4
```

### Comparing `sdr-0.0.8/docs/make.bat` & `sdr-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/docs/release-notes/v0.0.md` & `sdr-0.0.9/docs/release-notes/v0.0.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,35 @@
 ---
 tocdepth: 2
 ---
 
 # v0.0
 
+## v0.0.9
+
+*Released November 12, 2023*
+
+### Changes
+
+- Added polyphase rational resampling in `sdr.Resampler`.
+- Added discrete-time FIR differentiating filters in `sdr.Differentiator`.
+- Added discrete-time IIR integrating filters in `sdr.Integrator`.
+- Added `sdr.percent()`, `sdr.ppm()`, and `sdr.ppb()`.
+- Moved `sdr.DDS` functionality into `sdr.NCO`. Removed `sdr.DDS`.
+- Added ability to seed the channel models.
+- Added option to compute measurements along a specified axis.
+- Added option to return measurements in decibels.
+- Replaced `pylint` with `ruff`.
+- Replaced `black` with `ruff`.
+- Improved type annotations.
+
+### Contributors
+
+- Matt Hostetter ([@mhostetter](https://github.com/mhostetter))
+
 ## v0.0.8
 
 *Released September 4, 2023*
 
 ### Changes
 
 - Added minimum-shift keying (MSK) in `sdr.MSK`.
```

### Comparing `sdr-0.0.8/docs/release-notes/versioning.rst` & `sdr-0.0.9/docs/release-notes/versioning.rst`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/pyproject.toml` & `sdr-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -48,26 +48,14 @@
     "scipy",
     "matplotlib",
     # "numba >= 0.55, < 0.58",  # v0.55 is needed for support of NumPy 1.21
     "typing_extensions >= 4.0.0", # v4.0.0 is needed for use of Self (Python 3.11+) and Literal (Python 3.8+)
 ]
 dynamic = ["version"]
 
-# [project.optional-dependencies]
-# dev = [
-#     "pylint >= 2.14",
-#     "black >= 22.8.0",
-#     "pytest",
-#     "pytest-cov[toml]",
-#     "pytest-xdist",
-#     "pytest-benchmark >= 4.0.0",
-#     "requests",
-#     "pdfminer.six"
-# ]
-
 [project.urls]
 Homepage = "https://github.com/mhostetter/sdr"
 Source = "https://github.com/mhostetter/sdr"
 Issues = "https://github.com/mhostetter/sdr/issues"
 Documentation = "https://mhostetter.github.io/sdr/latest/"
 Discuss = "https://github.com/mhostetter/sdr/discussions"
 # Changelog = "https://mhostetter.github.io/sdr/latest/release-notes/versioning/"
@@ -82,48 +70,33 @@
 [tool.setuptools.package-data]
 "sdr" = ["py.typed"]
 # "sdr._databases" = ["*.db"]
 
 [tool.distutils.bdist_wheel]
 universal = false
 
-[tool.pylint]
-ignore-paths = ["src/sdr/_version.py"]
-disable = [
-    "comparison-with-callable",     # pylint doesn't understand metaclass properties
-    "fixme",
-    "global-statement",
-    "invalid-name",
-    "missing-function-docstring",
-    "protected-access",
-    "too-many-ancestors",
-    "too-many-arguments",
-    "too-many-branches",
-    "too-many-instance-attributes",
-    "too-many-lines",
-    "too-many-locals",
-    "too-many-public-methods",
-    "unneeded-not",
-]
-min-similarity-lines = 100
-max-line-length = 120
-
-[tool.black]
+[tool.ruff]
+src = ["src"]
+extend-include = ["*.ipynb"]
+extend-exclude = ["build", "dist", "docs", "src/sdr/_version.py"]
 line-length = 120
-exclude = '''
-/(
-      build
-)/
-    | src/sdr/_version.py
-'''
-# NOTE: You must use single-quoted strings in TOML for regular expressions. It's the equivalent of r-strings in Python.
-# For some reason, this exclude line doesn't work when on a single line.
 
-[tool.isort]
-profile = "black"
+[tool.ruff.lint]
+select = [
+    "E",  # pycodestyle
+    "F",  # Pyflakes
+    "UP", # pyupgrade
+    "B",  # flake8-bugbear
+    # "SIM",# flake8-simplify
+    "I", # isort
+]
+ignore = ["E501", "E713", "E714"]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["F401", "F403"]
 
 [tool.pytest.ini_options]
 minversion = "6.2"
 addopts = "-s --showlocals"
 testpaths = ["tests"]
 
 [tool.coverage.report]
```

### Comparing `sdr-0.0.8/src/sdr/__init__.py` & `sdr-0.0.9/src/sdr/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 except ModuleNotFoundError:  # pragma: no cover
     import warnings
 
     __version__ = "0.0.0"
     __version_tuple__ = (0, 0, 0)
     warnings.warn(
         "An error occurred during package install where setuptools_scm failed to create a _version.py file. "
-        "Defaulting version to 0.0.0."
+        "Defaulting version to 0.0.0.",
+        stacklevel=3,
     )
 
 from . import plot
 from ._conversion import *
 from ._data import *
 from ._detection import *
 from ._farrow import *
 from ._filter import *
 from ._link_budget import *
-from ._loop_filter import *
 from ._measurement import *
 from ._modulation import *
-from ._nco import *
-from ._pll import *
 from ._probability import *
 from ._sequence import *
 from ._signal import *
 from ._simulation import *
+from ._synchronization import *
```

### Comparing `sdr-0.0.8/src/sdr/_conversion.py` & `sdr-0.0.9/src/sdr/_conversion.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # Decibels
 ##############################################################################
 
 
 @export
 def db(
     x: npt.ArrayLike,
-    type: Literal["value", "power", "voltage"] = "value",  # pylint: disable=redefined-builtin
-) -> np.ndarray:
+    type: Literal["value", "power", "voltage"] = "value",
+) -> npt.NDArray[np.float_]:
     r"""
     Converts from linear units to decibels.
 
     Arguments:
         x: The input value or signal.
         type: The type of input value or signal.
 
@@ -75,16 +75,16 @@
 
     raise ValueError(f"Argument 'type' must be 'value', 'power', or 'voltage', not {type!r}.")
 
 
 @export
 def linear(
     x: npt.ArrayLike,
-    type: Literal["value", "power", "voltage"] = "value",  # pylint: disable=redefined-builtin
-) -> np.ndarray:
+    type: Literal["value", "power", "voltage"] = "value",
+) -> npt.NDArray[np.float_]:
     r"""
     Converts from decibels to linear units.
 
     Arguments:
         x: The input value or signal in dB.
         type: The type of output value or signal.
 
@@ -133,20 +133,118 @@
     if type == "voltage":
         return 10 ** (x / 20)
 
     raise ValueError(f"Argument 'type' must be 'value', 'power', or 'voltage', not {type!r}.")
 
 
 ##############################################################################
+# Ratios
+##############################################################################
+
+
+@export
+def percent(x: npt.ArrayLike) -> npt.NDArray[np.float_]:
+    r"""
+    Converts from a ratio to a percentage.
+
+    Arguments:
+        x: The input ratio.
+
+    Returns:
+        The percentage.
+
+    Examples:
+        Convert 0.5 to 50%.
+
+        .. ipython:: python
+
+            sdr.percent(0.5)
+
+        Convert 0.25 to 25%.
+
+        .. ipython:: python
+
+            sdr.percent(0.25)
+
+    Group:
+        conversions-ratios
+    """
+    x = np.asarray(x)
+    return 100 * x
+
+
+@export
+def ppm(x: npt.ArrayLike) -> npt.NDArray[np.float_]:
+    r"""
+    Converts from a ratio to parts per million (ppm).
+
+    Arguments:
+        x: The input ratio.
+
+    Returns:
+        The parts per million (ppm).
+
+    Examples:
+        Convert 0.005 to 5000 ppm.
+
+        .. ipython:: python
+
+            sdr.ppm(0.005)
+
+        Convert 0.000025 to 25 ppm.
+
+        .. ipython:: python
+
+            sdr.ppm(0.000025)
+
+    Group:
+        conversions-ratios
+    """
+    x = np.asarray(x)
+    return 1e6 * x
+
+
+@export
+def ppb(x: npt.ArrayLike) -> npt.NDArray[np.float_]:
+    r"""
+    Converts from a ratio to parts per billion (ppb).
+
+    Arguments:
+        x: The input ratio.
+
+    Returns:
+        The parts per billion (ppb).
+
+    Examples:
+        Convert 0.000005 to 5000 ppb.
+
+        .. ipython:: python
+
+            sdr.ppb(0.000005)
+
+        Convert 0.000000025 to 25 ppb.
+
+        .. ipython:: python
+
+            sdr.ppb(0.000000025)
+
+    Group:
+        conversions-ratios
+    """
+    x = np.asarray(x)
+    return 1e9 * x
+
+
+##############################################################################
 # From Eb/N0
 ##############################################################################
 
 
 @export
-def ebn0_to_esn0(ebn0: npt.ArrayLike, bps: int, rate: int = 1) -> np.ndarray:
+def ebn0_to_esn0(ebn0: npt.ArrayLike, bps: int, rate: int = 1) -> npt.NDArray[np.float_]:
     r"""
     Converts from $E_b/N_0$ to $E_s/N_0$.
 
     $$
     \frac{E_s}{N_0} = \frac{E_b}{N_0} \frac{k}{n} \log_2 M
     $$
 
@@ -178,15 +276,15 @@
     ebn0 = np.asarray(ebn0)  # Energy per information bit
     ecn0 = ebn0 + db(rate)  # Energy per coded bit
     esn0 = ecn0 + db(bps)  # Energy per symbol
     return esn0
 
 
 @export
-def ebn0_to_snr(ebn0: npt.ArrayLike, bps: int, rate: int = 1, sps: int = 1) -> np.ndarray:
+def ebn0_to_snr(ebn0: npt.ArrayLike, bps: int, rate: int = 1, sps: int = 1) -> npt.NDArray[np.float_]:
     r"""
     Converts from $E_b/N_0$ to $S/N$.
 
     $$
     \frac{S}{N} = \frac{E_b}{N_0} \frac{k}{n} \log_2 M \frac{f_{sym}}{f_s}
     $$
 
@@ -223,15 +321,15 @@
 
 ##############################################################################
 # From Es/N0
 ##############################################################################
 
 
 @export
-def esn0_to_ebn0(esn0: npt.ArrayLike, bps: int, rate: int = 1) -> np.ndarray:
+def esn0_to_ebn0(esn0: npt.ArrayLike, bps: int, rate: int = 1) -> npt.NDArray[np.float_]:
     r"""
     Converts from $E_s/N_0$ to $E_b/N_0$.
 
     $$
     \frac{E_b}{N_0} = \frac{E_s}{N_0} \frac{n}{k} \frac{1}{\log_2 M}
     $$
 
@@ -263,15 +361,15 @@
     esn0 = np.asarray(esn0)
     ecn0 = esn0 - db(bps)  # Energy per coded bit
     ebn0 = ecn0 - db(rate)  # Energy per information bit
     return ebn0
 
 
 @export
-def esn0_to_snr(esn0: npt.ArrayLike, sps: int = 1) -> np.ndarray:
+def esn0_to_snr(esn0: npt.ArrayLike, sps: int = 1) -> npt.NDArray[np.float_]:
     r"""
     Converts from $E_s/N_0$ to $S/N$.
 
     $$
     \frac{S}{N} = \frac{E_s}{N_0} \frac{f_{sym}}{f_s}
     $$
 
@@ -306,15 +404,15 @@
 
 ##############################################################################
 # From SNR
 ##############################################################################
 
 
 @export
-def snr_to_ebn0(snr: npt.ArrayLike, bps: int, rate: int = 1, sps: int = 1) -> np.ndarray:
+def snr_to_ebn0(snr: npt.ArrayLike, bps: int, rate: int = 1, sps: int = 1) -> npt.NDArray[np.float_]:
     r"""
     Converts from $S/N$ to $E_b/N_0$.
 
     $$
     \frac{E_b}{N_0} = \frac{S}{N} \frac{f_s}{f_{sym}} \frac{n}{k} \frac{1}{\log_2 M}
     $$
 
@@ -347,15 +445,15 @@
     snr = np.asarray(snr)  # SNR per sample
     esn0 = snr_to_esn0(snr, sps=sps)  # Energy per symbol
     ebn0 = esn0_to_ebn0(esn0, bps, rate=rate)  # Energy per information bit
     return ebn0
 
 
 @export
-def snr_to_esn0(snr: npt.ArrayLike, sps: int = 1) -> np.ndarray:
+def snr_to_esn0(snr: npt.ArrayLike, sps: int = 1) -> npt.NDArray[np.float_]:
     r"""
     Converts from $S/N$ to $E_s/N_0$.
 
     $$
     \frac{E_s}{N_0} = \frac{S}{N} \frac{f_s}{f_{sym}}
     $$
```

### Comparing `sdr-0.0.8/src/sdr/_data.py` & `sdr-0.0.9/src/sdr/_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import numpy.typing as npt
 
 from ._helper import export
 
 
 @export
-def pack(x: npt.ArrayLike, bpe: int, dtype: npt.DTypeLike | None = None) -> np.ndarray:
+def pack(x: npt.ArrayLike, bpe: int, dtype: npt.DTypeLike | None = None) -> npt.NDArray[np.int_]:
     """
     Packs a binary array into an array with multiple bits per element.
 
     The data is assumed to have the most significant bit first. If there are not enough bits in the
     input array to fill the last element of the output array, the remaining bits are filled with
     zeros.
 
@@ -62,15 +62,15 @@
         single_bits = 2 ** np.arange(bpe - 1, -1, -1, dtype=dtype)
         y = np.sum(X * single_bits, axis=-1)
 
     return y.astype(dtype)
 
 
 @export
-def unpack(x: npt.ArrayLike, bpe: int, dtype: npt.DTypeLike | None = None) -> np.ndarray:
+def unpack(x: npt.ArrayLike, bpe: int, dtype: npt.DTypeLike | None = None) -> npt.NDArray[np.int_]:
     """
     Unpacks an array with multiple bits per element into a binary array.
 
     The data is assumed to have the most significant bit first.
 
     Arguments:
         x: The input array with `bpe` bits per element.
```

### Comparing `sdr-0.0.8/src/sdr/_detection/_correlator.py` & `sdr-0.0.9/src/sdr/_detection/_correlator.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,16 +82,16 @@
 
     #     self._fir = FIR(np.ones(N_nc), streaming=streaming)
 
     @staticmethod
     def roc(
         enr: float,
         p_fa: npt.ArrayLike | None = None,
-        complex: bool = True,  # pylint: disable=redefined-builtin
-    ) -> tuple[np.ndarray, np.ndarray]:
+        complex: bool = True,
+    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.float_]]:
         r"""
         Computes the receiver operating characteristic (ROC) curve.
 
         Arguments:
             enr: The received energy-to-noise ratio $\mathcal{E}/\sigma^2$ in dB.
             p_fa: The probability of false alarm $P_{FA}$. If `None`, the ROC curve is computed for
                 `p_fa = np.logspace(-10, 0, 101)`.
@@ -125,16 +125,16 @@
 
         return p_fa, p_d
 
     @staticmethod
     def p_d(
         enr: npt.ArrayLike,
         p_fa: npt.ArrayLike,
-        complex: bool = True,  # pylint: disable=redefined-builtin
-    ) -> np.ndarray:
+        complex: bool = True,
+    ) -> npt.NDArray[np.float_]:
         r"""
         Computes the probability of detection $P_D$.
 
         Arguments:
             enr: The received energy-to-noise ratio $\mathcal{E}/\sigma^2$ in dB.
             p_fa: The probability of false alarm $P_{FA}$.
             complex: Indicates whether the signal is complex.
@@ -184,16 +184,16 @@
         return p_d
 
     @staticmethod
     def p_fa(
         threshold: npt.ArrayLike,
         energy: npt.ArrayLike,
         sigma2: npt.ArrayLike,
-        complex: bool = True,  # pylint: disable=redefined-builtin
-    ) -> np.ndarray:
+        complex: bool = True,
+    ) -> npt.NDArray[np.float_]:
         r"""
         Computes the probability of false alarm $P_{FA}$.
 
         Arguments:
             threshold: The threshold $\gamma'$.
             energy: The received energy $\mathcal{E} = \sum_{i=0}^{N-1} \left| s[n] \right|^2$.
             sigma2: The noise variance $\sigma^2$.
@@ -227,16 +227,16 @@
         return p_fa
 
     @staticmethod
     def threshold(
         p_fa: npt.ArrayLike,
         energy: npt.ArrayLike,
         sigma2: npt.ArrayLike,
-        complex: bool = True,  # pylint: disable=redefined-builtin
-    ) -> np.ndarray:
+        complex: bool = True,
+    ) -> npt.NDArray[np.float_]:
         r"""
         Computes the threshold $\gamma'$.
 
         Arguments:
             p_fa: The probability of false alarm $P_{FA}$.
             energy: The received energy $\mathcal{E} = \sum_{i=0}^{N-1} \left| s[n] \right|^2$.
             sigma2: The noise variance $\sigma^2$.
@@ -266,15 +266,15 @@
         if not complex:
             gamma_prime = np.sqrt(energy * sigma2) * Qinv(p_fa)
         else:
             gamma_prime = np.sqrt(energy * sigma2 / 2) * Qinv(p_fa)
 
         return gamma_prime
 
-    # def test_statistic(self, x: npt.ArrayLike) -> np.ndarray:
+    # def test_statistic(self, x: npt.ArrayLike) -> npt.NDArray[np.float_]:
     #     """
     #     Computes the test statistic $T(x)$.
 
     #     Arguments:
     #         x: The received signal $x[n]$.
 
     #     Returns:
@@ -283,15 +283,15 @@
     #     x = np.asarray(x)
 
     #     if self.streaming:
     #         return self._fir(np.abs(x) ** 2)
 
     #     return self._fir(np.abs(x) ** 2, mode="same")
 
-    # def detect(self, x: npt.ArrayLike, sigma2: float) -> np.ndarray:
+    # def detect(self, x: npt.ArrayLike, sigma2: float) -> npt.NDArray[np.float_]:
     #     r"""
     #     Detects the presence of a signal.
 
     #     Arguments:
     #         x: The received signal $x[n]$.
     #         sigma2: The noise variance $\sigma^2$.
```

### Comparing `sdr-0.0.8/src/sdr/_detection/_energy.py` & `sdr-0.0.9/src/sdr/_detection/_energy.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,16 +78,16 @@
     #     self._fir = FIR(np.ones(N_nc), streaming=streaming)
 
     @staticmethod
     def roc(
         snr: float,
         N_nc: float,
         p_fa: npt.ArrayLike | None = None,
-        complex: bool = True,  # pylint: disable=redefined-builtin
-    ) -> tuple[np.ndarray, np.ndarray]:
+        complex: bool = True,
+    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.float_]]:
         r"""
         Computes the receiver operating characteristic (ROC) curve.
 
         Arguments:
             snr: The received signal-to-noise ratio $\sigma_s^2 / \sigma^2$ in dB.
             N_nc: The number of samples $N_{NC}$ to non-coherently integrate.
             p_fa: The probability of false alarm $P_{FA}$. If `None`, the ROC curve is computed for
@@ -138,16 +138,16 @@
         return p_fa, p_d
 
     @staticmethod
     def p_d(
         snr: npt.ArrayLike,
         N_nc: npt.ArrayLike,
         p_fa: npt.ArrayLike,
-        complex: bool = True,  # pylint: disable=redefined-builtin
-    ) -> np.ndarray:
+        complex: bool = True,
+    ) -> npt.NDArray[np.float_]:
         r"""
         Computes the probability of detection $P_D$.
 
         Arguments:
             snr: The received signal-to-noise ratio $\sigma_s^2 / \sigma^2$ in dB.
             N_nc: The number of samples $N_{NC}$ to non-coherently integrate.
             p_fa: The probability of false alarm $P_{FA}$.
@@ -202,16 +202,16 @@
         return p_d
 
     @staticmethod
     def p_fa(
         threshold: npt.ArrayLike,
         N_nc: npt.ArrayLike,
         sigma2: npt.ArrayLike,
-        complex: bool = True,  # pylint: disable=redefined-builtin
-    ) -> np.ndarray:
+        complex: bool = True,
+    ) -> npt.NDArray[np.float_]:
         r"""
         Computes the probability of false alarm $P_{FA}$.
 
         Arguments:
             threshold: The threshold $\gamma'$.
             N_nc: The number of samples $N_{NC}$ to non-coherently integrate.
             sigma2: The noise variance $\sigma^2$.
@@ -247,16 +247,16 @@
         return p_fa
 
     @staticmethod
     def threshold(
         N_nc: npt.ArrayLike,
         p_fa: npt.ArrayLike,
         sigma2: npt.ArrayLike,
-        complex: bool = True,  # pylint: disable=redefined-builtin
-    ) -> np.ndarray:
+        complex: bool = True,
+    ) -> npt.NDArray[np.float_]:
         r"""
         Computes the threshold $\gamma'$.
 
         Arguments:
             N_nc: The number of samples $N_{NC}$ to non-coherently integrate.
             p_fa: The probability of false alarm $P_{FA}$.
             sigma2: The noise variance $\sigma^2$.
@@ -285,17 +285,17 @@
         if not complex:
             nu = N_nc  # Degrees of freedom
             gamma_prime = sigma2 * scipy.stats.chi2.isf(p_fa, nu)
         else:
             nu = 2 * N_nc  # Degrees of freedom
             gamma_prime = sigma2 / 2 * scipy.stats.chi2.isf(p_fa, nu)
 
-        return gamma_prime
+        return gamma_prime  # type: ignore
 
-    # def test_statistic(self, x: npt.ArrayLike) -> np.ndarray:
+    # def test_statistic(self, x: npt.ArrayLike) -> npt.NDArray[np.float_]:
     #     """
     #     Computes the test statistic $T(x)$.
 
     #     Arguments:
     #         x: The received signal $x[n]$.
 
     #     Returns:
@@ -304,15 +304,15 @@
     #     x = np.asarray(x)
 
     #     if self.streaming:
     #         return self._fir(np.abs(x) ** 2)
 
     #     return self._fir(np.abs(x) ** 2, mode="same")
 
-    # def detect(self, x: npt.ArrayLike, sigma2: float) -> np.ndarray:
+    # def detect(self, x: npt.ArrayLike, sigma2: float) -> npt.NDArray[np.float_]:
     #     r"""
     #     Detects the presence of a signal.
 
     #     Arguments:
     #         x: The received signal $x[n]$.
     #         sigma2: The noise variance $\sigma^2$.
```

### Comparing `sdr-0.0.8/src/sdr/_detection/_theory.py` & `sdr-0.0.9/src/sdr/_detection/_theory.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import numpy.typing as npt
 
 from .._helper import export
 
 
 @export
-def albersheim(p_d: npt.ArrayLike, p_fa: npt.ArrayLike, N_nc: npt.ArrayLike = 1) -> np.ndarray:
+def albersheim(p_d: npt.ArrayLike, p_fa: npt.ArrayLike, N_nc: npt.ArrayLike = 1) -> npt.NDArray[np.float_]:
     r"""
     Estimates the minimum required single-sample SNR, given $N_{NC}$ non-coherent combinations, to achieve
     a probability of detection $P_D$ and probability of false alarm $P_{FA}$. This function implements
     Albersheim's equation.
 
     Arguments:
         p_d: The desired probability of detection $P_D$ in $(0, 1)$.
@@ -62,15 +62,15 @@
             plt.xlabel("Probability of false alarm, $P_{FA}$"); \
             plt.ylabel("Minimum required SNR (dB)"); \
             plt.title(f"Estimated minimum required SNR across non-coherent combinations for $P_D = 0.9$\nusing Albersheim's approximation"); \
             plt.tight_layout()
 
     Group:
         detection-theory
-    """  # pylint: disable=line-too-long
+    """
     p_d = np.asarray(p_d)
     if not np.all(np.logical_and(0 < p_d, p_d < 1)):
         raise ValueError("Argument 'p_d' must have values in (0, 1).")
 
     p_fa = np.asarray(p_fa)
     if not np.all(np.logical_and(0 < p_fa, p_fa < 1)):
         raise ValueError("Argument 'p_fa' must have values in (0, 1).")
```

### Comparing `sdr-0.0.8/src/sdr/_farrow.py` & `sdr-0.0.9/src/sdr/_farrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
     References:
         - https://wirelesspi.com/fractional-delay-filters-using-the-farrow-structure/
 
     Examples:
         See the :ref:`farrow-arbitrary-resampler` example.
 
     Group:
-        resampling
+        dsp-arbitrary-resampling
     """
 
     def __init__(self, streaming: bool = False):
         """
         Creates a new Farrow arbitrary resampler.
 
         Arguments:
             streaming: Indicates whether to use streaming mode. In streaming mode, previous inputs are
                 preserved between calls to :meth:`~FarrowResampler.__call__()`.
 
         Examples:
             See the :ref:`farrow-arbitrary-resampler` example.
         """
         self._streaming = streaming
-        self._x_prev: np.ndarray  # FIR filter state. Will be updated in reset().
+        self._x_prev: npt.NDArray  # FIR filter state. Will be updated in reset().
         self._mu_next: float  # The next fractional sample delay value
 
         # Construct the four FIR filter taps
         self._taps = np.array(
             [
                 [-1 / 6, 1 / 2, -1 / 2, 1 / 6],
                 [0, 1 / 2, -1, 1 / 2],
@@ -71,15 +71,15 @@
             if not state.size == self._taps.shape[1] - 1:
                 raise ValueError(f"Argument 'state' must have {self._taps.shape[1]} elements, not {state.size}.")
             self._x_prev = state
 
         # Initial fractional sample delay accounts for filter delay
         self._mu_next = self._taps.shape[1] // 2
 
-    def __call__(self, x: npt.ArrayLike, rate: float) -> np.ndarray:
+    def __call__(self, x: npt.NDArray, rate: float) -> npt.NDArray:
         r"""
         Resamples the input signal $x[n]$ by the given arbitrary rate $r$.
 
         Arguments:
             x: The input signal $x[n] = x(n T_s)$.
             rate: The resampling rate $r$.
 
@@ -136,15 +136,15 @@
 
         # Interpolate the output samples using the Horner method
         y = mu * (mu * (mu * y0[idxs] + y1[idxs]) + y2[idxs]) + y3[idxs]
 
         return y
 
     @property
-    def taps(self) -> np.ndarray:
+    def taps(self) -> npt.NDArray:
         """
         The Farrow filter taps.
 
         Examples:
             See the :ref:`farrow-arbitrary-resampler` example.
         """
         return self._taps
```

### Comparing `sdr-0.0.8/src/sdr/_filter/_fir.py` & `sdr-0.0.9/src/sdr/_filter/_fir.py`

 * *Files 21% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 
         Examples:
             See the :ref:`fir-filters` example.
         """
         self._taps = np.asarray(h)
         self._streaming = streaming
 
-        self._state: np.ndarray  # The filter state. Will be updated in reset().
+        self._state: npt.NDArray  # The filter state. Will be updated in reset().
         self.reset()
 
     ##############################################################################
     # Special methods
     ##############################################################################
 
-    def __call__(self, x: npt.ArrayLike, mode: Literal["full", "valid", "same"] = "full") -> np.ndarray:
+    def __call__(self, x: npt.ArrayLike, mode: Literal["full", "valid", "same"] = "full") -> npt.NDArray:
         r"""
         Filters the input signal $x[n]$ with the FIR filter.
 
         Arguments:
             x: The input signal $x[n]$ with length $L$.
             mode: The non-streaming convolution mode.
 
@@ -147,15 +147,15 @@
             See the :ref:`fir-filters` example.
 
         Group:
             Streaming mode only
         """
         self._state = np.zeros(self.taps.size - 1, dtype=self.taps.dtype)
 
-    def flush(self) -> np.ndarray:
+    def flush(self) -> npt.NDArray:
         """
         Flushes the filter state by passing zeros through the filter. Only useful when using streaming mode.
 
         Returns:
             The remaining filtered signal $y[n]$.
 
         Examples:
@@ -180,15 +180,15 @@
 
         Group:
             Streaming mode only
         """
         return self._streaming
 
     @property
-    def state(self) -> np.ndarray:
+    def state(self) -> npt.NDArray:
         """
         The filter state consisting of the previous $N$ inputs.
 
         Examples:
             See the :ref:`fir-filters` example.
 
         Group:
@@ -196,15 +196,15 @@
         """
         return self._state
 
     ##############################################################################
     # Methods
     ##############################################################################
 
-    def impulse_response(self, N: int | None = None) -> np.ndarray:
+    def impulse_response(self, N: int | None = None) -> npt.NDArray:
         r"""
         Returns the impulse response $h[n]$ of the FIR filter. The impulse response $h[n]$ is the
         filter output when the input is an impulse $\delta[n]$.
 
         Arguments:
             N: The number of samples to return. The default is the filter length.
 
@@ -227,15 +227,15 @@
         d = np.zeros(N - self.taps.size + 1, dtype=float)
         d[0] = 1
 
         h = scipy.signal.convolve(d, self.taps, mode="full")
 
         return h
 
-    def step_response(self, N: int | None = None) -> np.ndarray:
+    def step_response(self, N: int | None = None) -> npt.NDArray:
         """
         Returns the step response $s[n]$ of the FIR filter. The step response $s[n]$ is the
         filter output when the input is a unit step $u[n]$.
 
         Arguments:
             N: The number of samples to return. The default is the filter length.
 
@@ -257,15 +257,15 @@
         # Unit step function
         u = np.ones(N - self.taps.size + 1, dtype=float)
 
         s = scipy.signal.convolve(u, self.taps, mode="full")
 
         return s
 
-    def frequency_response(self, sample_rate: float = 1.0, N: int = 1024) -> tuple[np.ndarray, np.ndarray]:
+    def frequency_response(self, sample_rate: float = 1.0, N: int = 1024) -> tuple[npt.NDArray, npt.NDArray]:
         r"""
         Returns the frequency response $H(\omega)$ of the FIR filter.
 
         Arguments:
             sample_rate: The sample rate $f_s$ of the filter in samples/s.
             N: The number of samples in the frequency response.
 
@@ -285,15 +285,15 @@
         w = np.fft.fftshift(w)
         H = np.fft.fftshift(H)
 
         return w, H
 
     def frequency_response_log(
         self, sample_rate: float = 1.0, N: int = 1024, decades: int = 4
-    ) -> tuple[np.ndarray, np.ndarray]:
+    ) -> tuple[npt.NDArray, npt.NDArray]:
         r"""
         Returns the frequency response $H(\omega)$ of the FIR filter on a logarithmic frequency axis.
 
         Arguments:
             sample_rate: The sample rate $f_s$ of the filter in samples/s.
             N: The number of samples in the frequency response.
             decades: The number of frequency decades to plot.
@@ -314,15 +314,15 @@
         return w, H
 
     ##############################################################################
     # Properties
     ##############################################################################
 
     @property
-    def taps(self) -> np.ndarray:
+    def taps(self) -> npt.NDArray:
         """
         The feedforward taps $h_i$ for $i = 0,...,N$.
 
         Examples:
             See the :ref:`fir-filters` example.
         """
         return self._taps
@@ -342,7 +342,90 @@
         r"""
         The delay of the FIR filter $d = \lfloor \frac{N + 1}{2} \rfloor$ in samples.
 
         Examples:
             See the :ref:`fir-filters` example.
         """
         return self.taps.size // 2
+
+
+@export
+class Differentiator(FIR):
+    r"""
+    Implements a differentiator FIR filter.
+
+    Notes:
+        A discrete-time differentiator is a FIR filter with the transfer function
+
+        $$H(z) = 1 - z^{-1} .$$
+
+        .. code-block:: text
+            :caption: FIR Differentiator Block Diagram
+
+            x[n] --+---------------@--> y[n]
+                   |               ^
+                   |   +------+    | -1
+                   +-->| z^-1 |----+
+                       +------+
+
+    Examples:
+        Create a differentiator FIR filter.
+
+        .. ipython:: python
+
+            fir = sdr.Differentiator()
+
+        Differentiate a Gaussian pulse.
+
+        .. ipython:: python
+
+            x = sdr.gaussian(0.3, 5, 10); \
+            y = fir(x)
+
+            @savefig sdr_Differentiator_1.png
+            plt.figure(figsize=(8, 4)); \
+            sdr.plot.time_domain(x, label="Input"); \
+            sdr.plot.time_domain(y, offset=-fir.delay, label="Derivative"); \
+            plt.title("Discrete-time differentiation of a Gaussian pulse"); \
+            plt.tight_layout();
+
+        Differentiate a raised cosine pulse.
+
+        .. ipython:: python
+
+            x = sdr.root_raised_cosine(0.1, 8, 10); \
+            y = fir(x)
+
+            @savefig sdr_Differentiator_2.png
+            plt.figure(figsize=(8, 4)); \
+            sdr.plot.time_domain(x, label="Input"); \
+            sdr.plot.time_domain(y, offset=-fir.delay, label="Derivative"); \
+            plt.title("Discrete-time differentiation of a raised cosine pulse"); \
+            plt.tight_layout();
+
+        Plot the frequency response.
+
+        .. ipython:: python
+
+            @savefig sdr_Differentiator_3.png
+            plt.figure(figsize=(8, 4)); \
+            sdr.plot.magnitude_response(fir);
+
+    Group:
+        dsp-filtering-applications
+    """
+
+    def __init__(self, streaming: bool = False):
+        """
+        Creates a differentiator FIR filter.
+
+        Arguments:
+            streaming: Indicates whether to use streaming mode. In streaming mode, previous inputs are
+                preserved between calls to :meth:`~sdr.Differentiator.__call__()`.
+
+        Examples:
+            See the :ref:`fir-filters` example.
+        """
+        h = np.array([1, -1], dtype=float)
+        super().__init__(h, streaming=streaming)
+
+    # TODO: Use np.diff() if it is faster
```

### Comparing `sdr-0.0.8/src/sdr/_filter/_iir.py` & `sdr-0.0.9/src/sdr/_filter/_iir.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         Examples:
             See the :ref:`iir-filters` example.
         """
         self._b_taps = np.asarray(b)
         self._a_taps = np.asarray(a)
         self._streaming = streaming
 
-        self._state: np.ndarray  # The filter state. Will be updated in reset().
+        self._state: npt.NDArray  # The filter state. Will be updated in reset().
         self.reset()
 
         # Compute the zeros and poles of the transfer function
         self._zeros, self._poles, self._gain = scipy.signal.tf2zpk(self.b_taps, self.a_taps)
 
     ##############################################################################
     # Alternate constructors
@@ -82,15 +82,15 @@
 
         return cls(b, a, streaming=streaming)
 
     ##############################################################################
     # Special methods
     ##############################################################################
 
-    def __call__(self, x: npt.ArrayLike) -> np.ndarray:
+    def __call__(self, x: npt.ArrayLike) -> npt.NDArray:
         r"""
         Filters the input signal $x[n]$ with the IIR filter.
 
         Arguments:
             x: The input signal $x[n]$ with length $L$.
 
         Returns:
@@ -177,15 +177,15 @@
 
         Group:
             Streaming mode only
         """
         return self._streaming
 
     @property
-    def state(self) -> np.ndarray:
+    def state(self) -> npt.NDArray:
         """
         The filter state.
 
         Examples:
             See the :ref:`iir-filters` example.
 
         Group:
@@ -193,15 +193,15 @@
         """
         return self._state
 
     ##############################################################################
     # Methods
     ##############################################################################
 
-    def impulse_response(self, N: int = 100) -> np.ndarray:
+    def impulse_response(self, N: int = 100) -> npt.NDArray:
         r"""
         Returns the impulse response $h[n]$ of the IIR filter. The impulse response $h[n]$ is the
         filter output when the input is an impulse $\delta[n]$.
 
         Arguments:
             N: The number of samples to return.
 
@@ -220,15 +220,15 @@
 
         zi = self._state
         h = self(d)
         self._state = zi  # Restore the filter state
 
         return h
 
-    def step_response(self, N: int = 100) -> np.ndarray:
+    def step_response(self, N: int = 100) -> npt.NDArray:
         """
         Returns the step response $s[n]$ of the IIR filter. The step response $s[n]$ is the
         filter output when the input is a unit step $u[n]$.
 
         Arguments:
             N: The number of samples to return.
 
@@ -246,15 +246,15 @@
 
         state = self._state
         s = self(u)
         self._state = state  # Restore the filter state
 
         return s
 
-    def frequency_response(self, sample_rate: float = 1.0, N: int = 1024) -> tuple[np.ndarray, np.ndarray]:
+    def frequency_response(self, sample_rate: float = 1.0, N: int = 1024) -> tuple[npt.NDArray, npt.NDArray]:
         r"""
         Returns the frequency response $H(\omega)$ of the IIR filter.
 
         Arguments:
             sample_rate: The sample rate $f_s$ of the filter in samples/s.
             N: The number of samples in the frequency response.
 
@@ -264,25 +264,25 @@
 
         See Also:
             sdr.plot.magnitude_response, sdr.plot.phase_response
 
         Examples:
             See the :ref:`iir-filters` example.
         """
-        w, H = scipy.signal.freqz(self.b_taps, self.a_taps, worN=N, whole=True, fs=sample_rate)
+        w, H = scipy.signal.freqz(self.b_taps, self.a_taps, worN=N, whole=True, fs=sample_rate)  # type: ignore
 
         w[w >= 0.5 * sample_rate] -= sample_rate  # Wrap frequencies from [0, 1) to [-0.5, 0.5)
         w = np.fft.fftshift(w)
         H = np.fft.fftshift(H)
 
         return w, H
 
     def frequency_response_log(
         self, sample_rate: float = 1.0, N: int = 1024, decades: int = 4
-    ) -> tuple[np.ndarray, np.ndarray]:
+    ) -> tuple[npt.NDArray, npt.NDArray]:
         r"""
         Returns the frequency response $H(\omega)$ of the IIR filter on a logarithmic frequency axis.
 
         Arguments:
             sample_rate: The sample rate $f_s$ of the filter in samples/s.
             N: The number of samples in the frequency response.
             decades: The number of frequency decades to plot.
@@ -294,34 +294,34 @@
         See Also:
             sdr.plot.magnitude_response, sdr.plot.phase_response
 
         Examples:
             See the :ref:`iir-filters` example.
         """
         w = np.logspace(np.log10(sample_rate / 2 / 10**decades), np.log10(sample_rate / 2), N)
-        w, H = scipy.signal.freqz(self.b_taps, self.a_taps, worN=w, whole=False, fs=sample_rate)
+        w, H = scipy.signal.freqz(self.b_taps, self.a_taps, worN=w, whole=False, fs=sample_rate)  # type: ignore
 
         return w, H
 
     ##############################################################################
     # Properties
     ##############################################################################
 
     @property
-    def b_taps(self) -> np.ndarray:
+    def b_taps(self) -> npt.NDArray:
         """
         The feedforward taps $b_i$ for $i = 0,...,M$.
 
         Examples:
             See the :ref:`iir-filters` example.
         """
         return self._b_taps
 
     @property
-    def a_taps(self) -> np.ndarray:
+    def a_taps(self) -> npt.NDArray:
         """
         The feedback taps $a_j$ for $j = 0,...,N$.
 
         Examples:
             See the :ref:`iir-filters` example.
         """
         return self._a_taps
@@ -333,25 +333,25 @@
 
         Examples:
             See the :ref:`iir-filters` example.
         """
         return self._a_taps.size - 1
 
     @property
-    def zeros(self) -> np.ndarray:
+    def zeros(self) -> npt.NDArray:
         """
         The zeros of the IIR filter.
 
         Examples:
             See the :ref:`iir-filters` example.
         """
         return self._zeros
 
     @property
-    def poles(self) -> np.ndarray:
+    def poles(self) -> npt.NDArray:
         """
         The poles of the IIR filter.
 
         Examples:
             See the :ref:`iir-filters` example.
         """
         return self._poles
@@ -361,7 +361,89 @@
         """
         The gain of the IIR filter.
 
         Examples:
             See the :ref:`iir-filters` example.
         """
         return self._gain
+
+
+@export
+class Integrator(IIR):
+    r"""
+    Implements an integrator IIR filter.
+
+    Notes:
+        A discrete-time integrator is an IIR filter with the transfer function
+
+        $$H(z) = \frac{1}{1 - z^{-1}} .$$
+
+        .. code-block:: text
+            :caption: IIR Integrator Block Diagram
+
+            x[n] -->@---------------+--> y[n]
+                    ^               |
+                 -1 |   +------+    |
+                    +---| z^-1 |<---+
+                        +------+
+
+    Examples:
+        Create an integrating IIR filter.
+
+        .. ipython:: python
+
+            iir = sdr.Integrator()
+
+        Integrate a Gaussian pulse.
+
+        .. ipython:: python
+
+            x = sdr.gaussian(0.3, 5, 10); \
+            y = iir(x)
+
+            @savefig sdr_Integrator_1.png
+            plt.figure(figsize=(8, 4)); \
+            sdr.plot.time_domain(x, label="Input"); \
+            sdr.plot.time_domain(y, label="Integral"); \
+            plt.title("Discrete-time integration of a Gaussian pulse"); \
+            plt.tight_layout();
+
+        Integrate a raised cosine pulse.
+
+        .. ipython:: python
+
+            x = sdr.root_raised_cosine(0.1, 8, 10); \
+            y = iir(x)
+
+            @savefig sdr_Integrator_2.png
+            plt.figure(figsize=(8, 4)); \
+            sdr.plot.time_domain(x, label="Input"); \
+            sdr.plot.time_domain(y, label="Integral"); \
+            plt.title("Discrete-time integration of a raised cosine pulse"); \
+            plt.tight_layout();
+
+        Plot the frequency response.
+
+        .. ipython:: python
+
+            @savefig sdr_Integrator_3.png
+            plt.figure(figsize=(8, 4)); \
+            sdr.plot.magnitude_response(iir);
+
+    Group:
+        dsp-filtering-applications
+    """
+
+    def __init__(self, streaming: bool = False):
+        """
+        Creates an integrating IIR filter.
+
+        Arguments:
+            streaming: Indicates whether to use streaming mode. In streaming mode, previous inputs and outputs are
+                preserved between calls to :meth:`~Integrator.__call__()`.
+
+        Examples:
+            See the :ref:`iir-filters` example.
+        """
+        super().__init__([1], [1, -1], streaming=streaming)
+
+    # TODO: Use np.cumsum() if it is faster
```

### Comparing `sdr-0.0.8/src/sdr/_filter/_polyphase.py` & `sdr-0.0.9/src/sdr/_filter/_polyphase.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
 from .._helper import export
 from ._fir import FIR
 
 
 @export
 def multirate_taps(
-    P: int,
-    Q: int = 1,
+    up: int,
+    down: int = 1,
     half_length: int = 12,
     A_stop: float = 80,
-) -> np.ndarray:
+) -> npt.NDArray[np.float_]:
     r"""
     Computes the multirate FIR filter that achieves rational resampling by $P/Q$.
 
     Note:
-        This filter can be used with :class:`sdr.Interpolator` or :class:`sdr.Decimator`.
+        This filter can be used with :class:`sdr.Interpolator`, :class:`sdr.Decimator`, or :class:`sdr.Resampler`.
 
     Arguments:
-        P: The interpolation rate $P$.
-        Q: The decimation rate $Q$.
+        up: The interpolation rate $P$.
+        down: The decimation rate $Q$.
         half_length: The half-length of the polyphase filters.
         A_stop: The stopband attenuation $A_{\text{stop}}$ in dB.
 
     Returns:
         The multirate FIR filter $h[n]$.
 
     References:
@@ -54,38 +54,40 @@
             @savefig sdr_multirate_fir_2.png
             plt.figure(figsize=(8, 4)); \
             sdr.plot.magnitude_response(h);
 
     Group:
         dsp-multirate-filtering
     """
-    if not isinstance(P, int):
-        raise TypeError(f"Argument 'P' must be an integer, not {P}.")
-    if not P >= 1:
-        raise ValueError(f"Argument 'P' must be at least 1, not {P}.")
-
-    if not isinstance(Q, int):
-        raise TypeError(f"Argument 'Q' must be an integer, not {Q}.")
-    if not Q >= 1:
-        raise ValueError(f"Argument 'Q' must be at least 1, not {Q}.")
+    if not isinstance(up, int):
+        raise TypeError(f"Argument 'up' must be an integer, not {up}.")
+    if not up >= 1:
+        raise ValueError(f"Argument 'up' must be at least 1, not {up}.")
+    P = up
+
+    if not isinstance(down, int):
+        raise TypeError(f"Argument 'down' must be an integer, not {down}.")
+    if not down >= 1:
+        raise ValueError(f"Argument 'down' must be at least 1, not {down}.")
+    Q = down
 
     B = P if P > 1 else Q  # The number of polyphase branches
     R = max(P, Q)  # Inverse of the filter's fractional bandwidth
 
     # Compute the filter order, which is length - 1
     N = 2 * half_length * B
 
     # Compute ideal lowpass filter
     n = np.arange(N + 1)
     h = P / R * np.sinc((n - N // 2) / R)
 
     # Compute Kaiser window
     # beta = scipy.signal.windows.kaiser_beta(A_stop)
     if A_stop >= 50:
-        beta = 0.1102 * (A_stop - 8.71)  # TODO: Matlab uses 8.71 and SciPy uses 8.7
+        beta = 0.1102 * (A_stop - 8.71)  # TODO: MATLAB uses 8.71 and SciPy uses 8.7
     elif A_stop > 21:
         beta = 0.5842 * (A_stop - 21) ** 0.4 + 0.07886 * (A_stop - 21)
     else:
         beta = 0
     w = scipy.signal.windows.kaiser(N + 1, beta)
 
     # Compute windowed filter
@@ -100,23 +102,55 @@
     # If the above condition is not true, the first and last elements are non-zero. The filter length
     # is 2 * half_length * B + 1 and each polyphase branch has length 2 * half_length + 1. The final
     # column in the polyphase matrix will be padded with zeros.
 
     return h
 
 
+def _multirate_taps_linear(rate: int) -> npt.NDArray[np.float_]:
+    r"""
+    The multirate filter is designed to linearly interpolate between samples. The filter coefficients are a
+    length-$2r$ linear ramp $\frac{1}{r} [0, ..., r-1, r, r-1, ..., 1]$. The first output sample aligns with the
+    first input sample.
+    """
+    h = np.zeros(2 * rate, dtype=float)
+    h[:rate] = np.arange(0, rate) / rate
+    h[rate:] = np.arange(rate, 0, -1) / rate
+    return h
+
+
+def _multirate_taps_linear_matlab(rate: int) -> npt.NDArray[np.float_]:
+    r"""
+    The multirate filter is designed to linearly interpolate between samples. The filter coefficients are a
+    length-$2r$ linear ramp $\frac{1}{r} [1, ..., r-1, r, r-1, ..., 0]$. This is method MATLAB uses. The first
+    output sample is advanced from the first input sample.
+    """
+    h = np.zeros(2 * rate, dtype=float)
+    h[:rate] = np.arange(1, rate + 1) / rate
+    h[rate:] = np.arange(rate - 1, -1, -1) / rate
+    return h
+
+
+def _multirate_taps_zoh(rate: int) -> npt.NDArray[np.float_]:
+    """
+    The multirate filter is designed to be a zero-order hold. The filter coefficients are a length-$r$ array of ones.
+    """
+    h = np.ones(rate, dtype=float)
+    return h
+
+
 @export
-def polyphase_matrix(P: int, Q: int, taps: npt.ArrayLike) -> np.ndarray:
+def polyphase_matrix(up: int, down: int, taps: npt.ArrayLike) -> npt.NDArray:
     """
     Converts the multirate FIR filter taps $h_i$ into the polyphase matrix $H_{i, j}$ that achieves
     rational resampling by $P/Q$.
 
     Arguments:
-        P: The interpolation rate $P$.
-        Q: The decimation rate $Q$.
+        up: The interpolation rate $P$.
+        down: The decimation rate $Q$.
         taps: The multirate FIR filter taps $h_i$.
 
     Returns:
         The polyphase matrix $H_{i, j}$.
 
     Notes:
         The multirate FIR filter taps $h_i$ are arranged down the columns of the polyphase matrix
@@ -145,23 +179,25 @@
             h = np.arange(0, 20)
             sdr.polyphase_matrix(3, 4, h)
             sdr.polyphase_matrix(1, 6, h)
 
     Group:
         dsp-multirate-filtering
     """
-    if not isinstance(P, int):
-        raise TypeError(f"Argument 'P' must be an integer, not {P}.")
-    if not P >= 1:
-        raise ValueError(f"Argument 'P' must be at least 1, not {P}.")
-
-    if not isinstance(Q, int):
-        raise TypeError(f"Argument 'Q' must be an integer, not {Q}.")
-    if not Q >= 1:
-        raise ValueError(f"Argument 'Q' must be at least 1, not {Q}.")
+    if not isinstance(up, int):
+        raise TypeError(f"Argument 'up' must be an integer, not {up}.")
+    if not up >= 1:
+        raise ValueError(f"Argument 'up' must be at least 1, not {up}.")
+    P = up
+
+    if not isinstance(down, int):
+        raise TypeError(f"Argument 'down' must be an integer, not {down}.")
+    if not down >= 1:
+        raise ValueError(f"Argument 'down' must be at least 1, not {down}.")
+    Q = down
 
     taps = np.asarray(taps)
 
     B = P if P > 1 else Q  # The number of polyphase branches
     N = math.ceil(taps.size / B) * B  # Filter length
 
     # Append zeros to the end of the taps so that the filter length is a multiple of B
@@ -169,18 +205,53 @@
 
     # Reshape the taps down the columns of H
     H = taps_pad.reshape(-1, B).T
 
     return H
 
 
+def _polyphase_interpolate(
+    x: npt.NDArray,
+    state: npt.NDArray,
+    H: npt.NDArray,
+    mode: Literal["rate", "full"],
+    streaming: bool,
+) -> tuple[npt.NDArray, npt.NDArray]:
+    B, M = H.shape  # Number of polyphase branches, polyphase filter length
+    dtype = np.result_type(x, H)
+
+    if streaming:
+        x_pad = np.concatenate((state, x))  # Prepend previous inputs from last __call__() call
+        Y = np.zeros((B, x.size), dtype=dtype)
+        for i in range(B):
+            Y[i] = scipy.signal.convolve(x_pad, H[i], mode="valid")
+        state = x_pad[-(M - 1) :]
+    else:
+        if mode == "full":
+            Y = np.zeros((B, x.size + M - 1), dtype=dtype)
+            for i in range(B):
+                Y[i] = scipy.signal.convolve(x, H[i], mode="full")
+        elif mode == "rate":
+            Y = np.zeros((B, x.size), dtype=dtype)
+            for i in range(B):
+                corr = scipy.signal.convolve(x, H[i], mode="full")
+                Y[i] = corr[M // 2 : M // 2 + x.size]
+        else:
+            raise ValueError(f"Argument 'mode' must be 'rate' or 'full', not {mode!r}.")
+
+    # Commutate the outputs of the polyphase filters
+    y = Y.T.flatten()
+
+    return y, state
+
+
 @export
 class Interpolator(FIR):
     r"""
-    Implements a polyphase finite impulse response (FIR) interpolating filter.
+    Implements a polyphase interpolating FIR filter.
 
     Notes:
         The polyphase interpolating filter is equivalent to first upsampling the input signal $x[n]$ by $r$
         (by inserting $r-1$ zeros between each sample) and then filtering the upsampled signal with the
         prototype FIR filter with feedforward coefficients $h_{i}$.
 
         Instead, the polyphase interpolating filter first decomposes the prototype FIR filter into $r$ polyphase
@@ -243,14 +314,15 @@
             y2 = fir(x[10:20]); \
             y3 = fir(x[20:30]); \
             y4 = fir(x[30:40]); \
             y5 = fir.flush()
 
             @savefig sdr_Interpolator_2.png
             plt.figure(figsize=(8, 4)); \
+            sdr.plot.time_domain(x, marker="o", label="Input"); \
             sdr.plot.time_domain(y1, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 0, marker=".", label="Interpolated $y_1[n]$"); \
             sdr.plot.time_domain(y2, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 10, marker=".", label="Interpolated $y_2[n]$"); \
             sdr.plot.time_domain(y3, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 20, marker=".", label="Interpolated $y_3[n]$"); \
             sdr.plot.time_domain(y4, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 30, marker=".", label="Interpolated $y_4[n]$"); \
             sdr.plot.time_domain(y5, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 40, marker=".", label="Interpolated $y_5[n]$"); \
             plt.title("Streaming interpolation by 7 with the Kaiser window method"); \
             plt.tight_layout();
@@ -265,15 +337,15 @@
             @savefig sdr_Interpolator_3.png
             plt.figure(figsize=(8, 4)); \
             sdr.plot.time_domain(x, marker="o", label="Input"); \
             sdr.plot.time_domain(y, sample_rate=fir.rate, marker=".", label="Interpolated"); \
             plt.title("Interpolation by 7 with the linear method"); \
             plt.tight_layout();
 
-        Create a polyphase filter that interpolates by 7 using the zero-order hold method. It is recommended to
+        Create a polyphase filter that interpolates by 7 using the zero-order hold method. It is recommended to use
         the `"full"` convolution mode. This way the first upsampled symbol has $r$ samples.
 
         .. ipython:: python
 
             fir = sdr.Interpolator(7, "zoh"); fir
             y = fir(x, mode="full")
 
@@ -282,73 +354,80 @@
             sdr.plot.time_domain(x, marker="o", label="Input"); \
             sdr.plot.time_domain(y, sample_rate=fir.rate, offset=-fir.delay/fir.rate, marker=".", label="Interpolated"); \
             plt.title("Interpolation by 7 with the zero-order hold method"); \
             plt.tight_layout();
 
     Group:
         dsp-multirate-filtering
-    """  # pylint: disable=line-too-long
+    """
 
     def __init__(
         self,
         rate: int,
-        taps: Literal["kaiser", "linear", "zoh"] | npt.ArrayLike = "kaiser",
+        taps: Literal["kaiser", "linear", "linear-matlab", "zoh"] | npt.ArrayLike = "kaiser",
         streaming: bool = False,
     ):
         r"""
         Creates a polyphase FIR interpolating filter.
 
         Arguments:
             rate: The interpolation rate $r$.
             taps: The multirate filter design specification.
 
                 - `"kaiser"`: The multirate filter is designed using :func:`~sdr.multirate_taps()`
                   with arguments `rate` and 1.
                 - `"linear"`: The multirate filter is designed to linearly interpolate between samples.
                   The filter coefficients are a length-$2r$ linear ramp $\frac{1}{r} [0, ..., r-1, r, r-1, ..., 1]$.
+                  The first output sample aligns with the first input sample.
+                - `"linear-matlab"`: The multirate filter is designed to linearly interpolate between samples.
+                  The filter coefficients are a length-$2r$ linear ramp $\frac{1}{r} [1, ..., r-1, r, r-1, ..., 0]$.
+                  This is method MATLAB uses. The first output sample is advanced from the first input sample.
                 - `"zoh"`: The multirate filter is designed to be a zero-order hold.
                   The filter coefficients are a length-$r$ array of ones.
                 - `npt.ArrayLike`: The multirate filter feedforward coefficients $h_i$.
 
             streaming: Indicates whether to use streaming mode. In streaming mode, previous inputs are
                 preserved between calls to :meth:`~Interpolator.__call__()`.
         """
         if not isinstance(rate, int):
             raise TypeError("Argument 'rate' must be an integer.")
         if not rate >= 1:
             raise ValueError(f"Argument 'rate' must be at least 1, not {rate}.")
         self._rate = rate
-        self._method: Literal["kaiser", "linear", "zoh", "custom"]
+        self._method: Literal["kaiser", "linear", "linear-matlab", "zoh", "custom"]
 
         if not isinstance(taps, str):
             self._method = "custom"
             taps = np.asarray(taps)
         elif taps == "kaiser":
             self._method = "kaiser"
             taps = multirate_taps(rate, 1)
         elif taps == "linear":
             self._method = "linear"
-            taps = np.zeros(2 * rate, dtype=float)
-            taps[:rate] = np.arange(0, rate) / rate
-            taps[rate:] = np.arange(rate, 0, -1) / rate
+            taps = _multirate_taps_linear(rate)
+        elif taps == "linear-matlab":
+            self._method = "linear-matlab"
+            taps = _multirate_taps_linear_matlab(rate)
         elif taps == "zoh":
             self._method = "zoh"
-            taps = np.ones(rate, dtype=float)
+            taps = _multirate_taps_zoh(rate)
         else:
-            raise ValueError(f"Argument 'taps' must be 'kaiser', 'linear', 'zoh', or an array-like, not {taps}.")
+            raise ValueError(
+                f"Argument 'taps' must be 'kaiser', 'linear', 'linear-matlab', 'zoh', or an array-like, not {taps}."
+            )
 
         self._polyphase_taps = polyphase_matrix(rate, 1, taps)
 
         super().__init__(taps, streaming=streaming)
 
     ##############################################################################
     # Special methods
     ##############################################################################
 
-    def __call__(self, x: npt.ArrayLike, mode: Literal["rate", "full"] = "rate") -> np.ndarray:
+    def __call__(self, x: npt.ArrayLike, mode: Literal["rate", "full"] = "rate") -> npt.NDArray:
         r"""
         Interpolates and filters the input signal $x[n]$ with the polyphase FIR filter.
 
         Arguments:
             x: The input signal $x[n]$ with sample rate $f_s$ and length $L$.
             mode: The non-streaming convolution mode.
 
@@ -407,59 +486,35 @@
                 y3 = fir(np.zeros(fir.polyphase_taps.shape[1])); \
                 y = np.concatenate((y1, y2, y3))
 
                 @savefig sdr_Interpolator_call_3.png
                 plt.figure(figsize=(8, 4)); \
                 sdr.plot.time_domain(x, marker="o", label="$x[n]$"); \
                 sdr.plot.time_domain(y, sample_rate=fir.rate, offset=-fir.delay/fir.rate, marker=".", label="$y[n]$");
-        """  # pylint: disable=line-too-long
+        """
         x = np.atleast_1d(x)
         if not x.ndim == 1:
             raise ValueError(f"Argument 'x' must be a 1-D, not {x.ndim}-D.")
 
-        dtype = np.result_type(x, self.polyphase_taps)
-        H = self.polyphase_taps
-        B, M = self.polyphase_taps.shape  # Number of polyphase branches, polyphase filter length
-
-        if self.streaming:
-            x_pad = np.concatenate((self._state, x))  # Prepend previous inputs from last __call__() call
-            Y = np.zeros((B, x.size), dtype=dtype)
-            for i in range(B):
-                Y[i] = scipy.signal.convolve(x_pad, H[i], mode="valid")
-            self._state = x_pad[-(M - 1) :]
-        else:
-            if mode == "full":
-                Y = np.zeros((B, x.size + M - 1), dtype=dtype)
-                for i in range(B):
-                    Y[i] = scipy.signal.convolve(x, H[i], mode="full")
-            elif mode == "rate":
-                Y = np.zeros((B, x.size), dtype=dtype)
-                for i in range(B):
-                    corr = scipy.signal.convolve(x, H[i], mode="full")
-                    Y[i] = corr[M // 2 : M // 2 + x.size]
-            else:
-                raise ValueError(f"Argument 'mode' must be 'rate' or 'full', not {mode!r}.")
-
-        # Commutate the outputs of the polyphase filters
-        y = Y.T.flatten()
+        y, self._state = _polyphase_interpolate(x, self._state, self.polyphase_taps, mode, self.streaming)
 
         return y
 
     def __repr__(self) -> str:
         """
         Returns a code-styled string representation of the object.
 
         Examples:
             .. ipython:: python
 
                 fir = sdr.Interpolator(7)
                 fir
         """
         if self.method == "custom":
-            h_str = np.array2string(self.taps, max_line_width=1e6, separator=", ", suppress_small=True)
+            h_str = np.array2string(self.taps, max_line_width=int(1e6), separator=", ", suppress_small=True)
         else:
             h_str = repr(self.method)
         return f"sdr.{type(self).__name__}({self.rate}, {h_str}, streaming={self.streaming})"
 
     def __str__(self) -> str:
         """
         Returns a human-readable string representation of the object.
@@ -494,22 +549,22 @@
     def rate(self) -> int:
         """
         The interpolation rate $r$.
         """
         return self._rate
 
     @property
-    def method(self) -> Literal["kaiser", "linear", "zoh", "custom"]:
+    def method(self) -> Literal["kaiser", "linear", "linear-matlab", "zoh", "custom"]:
         """
         The method used to design the multirate filter.
         """
         return self._method
 
     @property
-    def taps(self) -> np.ndarray:
+    def taps(self) -> npt.NDArray:
         """
         The prototype feedforward taps $h_i$.
 
         Notes:
             The prototype feedforward taps $h_i$ are the feedforward taps of the FIR filter before
             polyphase decomposition. The polyphase feedforward taps $h_{i, j}$ are the feedforward taps
             of the FIR filter after polyphase decomposition.
@@ -524,15 +579,15 @@
                 fir = sdr.Interpolator(3, np.arange(10))
                 fir.taps
                 fir.polyphase_taps
         """
         return self._taps
 
     @property
-    def polyphase_taps(self) -> np.ndarray:
+    def polyphase_taps(self) -> npt.NDArray:
         """
         The polyphase feedforward taps $h_{i, j}$.
 
         Notes:
             The prototype feedforward taps $h_i$ are the feedforward taps of the FIR filter before
             polyphase decomposition. The polyphase feedforward taps $h_{i, j}$ are the feedforward taps
             of the FIR filter after polyphase decomposition.
@@ -546,19 +601,72 @@
 
                 fir = sdr.Interpolator(3, np.arange(10))
                 fir.taps
                 fir.polyphase_taps
         """
         return self._polyphase_taps
 
+    @property
+    def delay(self) -> int:
+        """
+        The delay of FIR filter in samples. The delay indicates the output sample index that corresponds to the
+        first input sample.
+        """
+        return super().delay
+
+
+def _polyphase_decimate(
+    x: npt.NDArray,
+    state: npt.NDArray,
+    H: npt.NDArray,
+    mode: Literal["rate", "full"],
+    streaming: bool,
+) -> tuple[npt.NDArray, npt.NDArray]:
+    B, M = H.shape  # Number of polyphase branches, polyphase filter length
+    dtype = np.result_type(x, H)
+
+    if streaming:
+        x_pad = np.concatenate((state, x))  # Prepend previous inputs from last __call__() call
+        X_cols = x_pad.size // B
+        X_pad = x_pad[0 : X_cols * B].reshape(X_cols, B).T  # Commutate across polyphase filters
+        X_pad = np.flipud(X_pad)  # Commutate from bottom to top
+        Y = np.zeros((B, X_cols - M + 1), dtype=dtype)
+        for i in range(B):
+            Y[i] = scipy.signal.convolve(X_pad[i], H[i], mode="valid")
+        state = x_pad[-(B * M - 1) :]
+    else:
+        # Prepend zeros to so the first sample is alone in the first commutated column
+        x_pad = np.insert(x, 0, np.zeros(B - 1))
+        # Append zeros to input signal to distribute evenly across the B branches
+        x_pad = np.append(x_pad, np.zeros(B - (x_pad.size % B), dtype=dtype))
+        X_cols = x_pad.size // B
+        X_pad = x_pad.reshape(X_cols, B).T  # Commutate across polyphase filters
+        X_pad = np.flipud(X_pad)  # Commutate from bottom to top
+        if mode == "full":
+            Y = np.zeros((B, X_cols + M - 1), dtype=dtype)
+            for i in range(B):
+                Y[i] = scipy.signal.convolve(X_pad[i], H[i], mode="full")
+        elif mode == "rate":
+            Y = np.zeros((B, X_cols), dtype=dtype)
+            for i in range(B):
+                corr = scipy.signal.convolve(X_pad[i], H[i], mode="full")
+                Y[i] = corr[M // 2 : M // 2 + X_cols]
+        else:
+            raise ValueError(f"Argument 'mode' must be 'rate' or 'full', not {mode!r}.")
+
+    # Sum the outputs of the polyphase filters
+    y = np.sum(Y, axis=0)
+
+    return y, state
+
 
 @export
 class Decimator(FIR):
     r"""
-    Implements a polyphase finite impulse response (FIR) decimating filter.
+    Implements a polyphase decimating FIR filter.
 
     Notes:
         The polyphase decimating filter is equivalent to first filtering the input signal $x[n]$ with the
         prototype FIR filter with feedforward coefficients $h_{i}$ and then decimating the filtered signal
         by $r$ (by discarding $r-1$ samples between each sample).
 
         Instead, the polyphase decimating filter first decomposes the prototype FIR filter into $r$ polyphase
@@ -601,16 +709,16 @@
         .. ipython:: python
 
             fir = sdr.Decimator(7); fir
             y = fir(x)
 
             @savefig sdr_Decimator_1.png
             plt.figure(figsize=(8, 4)); \
-            sdr.plot.time_domain(x, marker="o", label="Input"); \
-            sdr.plot.time_domain(y, sample_rate=1/fir.rate, marker=".", label="Decimated"); \
+            sdr.plot.time_domain(x, marker=".", label="Input"); \
+            sdr.plot.time_domain(y, sample_rate=1/fir.rate, marker="o", label="Decimated"); \
             plt.title("Decimation by 7 with the Kaiser window method"); \
             plt.tight_layout();
 
         Create a streaming polyphase filter that decimates by 7 using the Kaiser window method. This filter
         preserves state between calls.
 
         .. ipython:: python
@@ -621,25 +729,26 @@
             y2 = fir(x[70:140]); \
             y3 = fir(x[140:210]); \
             y4 = fir(x[210:280]); \
             y5 = fir.flush()
 
             @savefig sdr_Decimator_2.png
             plt.figure(figsize=(8, 4)); \
-            sdr.plot.time_domain(y1, sample_rate=1/fir.rate, offset=-fir.delay + 0, marker=".", label="Decimated $y_1[n]$"); \
-            sdr.plot.time_domain(y2, sample_rate=1/fir.rate, offset=-fir.delay + 70, marker=".", label="Decimated $y_2[n]$"); \
-            sdr.plot.time_domain(y3, sample_rate=1/fir.rate, offset=-fir.delay + 140, marker=".", label="Decimated $y_3[n]$"); \
-            sdr.plot.time_domain(y4, sample_rate=1/fir.rate, offset=-fir.delay + 210, marker=".", label="Decimated $y_4[n]$"); \
-            sdr.plot.time_domain(y5, sample_rate=1/fir.rate, offset=-fir.delay + 280, marker=".", label="Decimated $y_5[n]$"); \
+            sdr.plot.time_domain(x, marker=".", label="Input"); \
+            sdr.plot.time_domain(y1, sample_rate=1/fir.rate, offset=-fir.delay*fir.rate + 0, marker="o", label="Decimated $y_1[n]$"); \
+            sdr.plot.time_domain(y2, sample_rate=1/fir.rate, offset=-fir.delay*fir.rate + 70, marker="o", label="Decimated $y_2[n]$"); \
+            sdr.plot.time_domain(y3, sample_rate=1/fir.rate, offset=-fir.delay*fir.rate + 140, marker="o", label="Decimated $y_3[n]$"); \
+            sdr.plot.time_domain(y4, sample_rate=1/fir.rate, offset=-fir.delay*fir.rate + 210, marker="o", label="Decimated $y_4[n]$"); \
+            sdr.plot.time_domain(y5, sample_rate=1/fir.rate, offset=-fir.delay*fir.rate + 280, marker="o", label="Decimated $y_5[n]$"); \
             plt.title("Streaming decimation by 7 with the Kaiser window method"); \
             plt.tight_layout();
 
     Group:
         dsp-multirate-filtering
-    """  # pylint: disable=line-too-long
+    """
 
     def __init__(
         self,
         rate: int,
         taps: Literal["kaiser"] | npt.ArrayLike = "kaiser",
         streaming: bool = False,
     ):
@@ -679,15 +788,15 @@
 
         super().__init__(taps, streaming=streaming)
 
     ##############################################################################
     # Special methods
     ##############################################################################
 
-    def __call__(self, x: npt.ArrayLike, mode: Literal["rate", "full"] = "rate") -> np.ndarray:
+    def __call__(self, x: npt.ArrayLike, mode: Literal["rate", "full"] = "rate") -> npt.NDArray:
         """
         Filters and decimates the input signal $x[n]$ with the polyphase FIR filter.
 
         Arguments:
             x: The input signal $x[n]$ with sample rate $f_s$ and length $L$.
             mode: The non-streaming convolution mode.
 
@@ -705,64 +814,30 @@
             The filtered signal $y[n]$ with sample rate $f_s / r$. The output length is dictated by
             the `mode` argument.
         """
         x = np.atleast_1d(x)
         if not x.ndim == 1:
             raise ValueError(f"Argument 'x' must be a 1-D, not {x.ndim}-D.")
 
-        dtype = np.result_type(x, self.polyphase_taps)
-        H = self.polyphase_taps
-        B, M = self.polyphase_taps.shape  # Number of polyphase branches, polyphase filter length
-
-        if self.streaming:
-            x_pad = np.concatenate((self._state, x))  # Prepend previous inputs from last __call__() call
-            X_cols = x_pad.size // B
-            X_pad = x_pad[0 : X_cols * B].reshape(X_cols, B).T  # Commutate across polyphase filters
-            X_pad = np.flipud(X_pad)  # Commutate from bottom to top
-            Y = np.zeros((B, X_cols - M + 1), dtype=dtype)
-            for i in range(B):
-                Y[i] = scipy.signal.convolve(X_pad[i], H[i], mode="valid")
-            self._state = x_pad[-(B * M - 1) :]
-        else:
-            # Prepend zeros to so the first sample is alone in the first commutated column
-            x_pad = np.insert(x, 0, np.zeros(B - 1))
-            # Append zeros to input signal to distribute evenly across the B branches
-            x_pad = np.append(x_pad, np.zeros(B - (x_pad.size % B), dtype=dtype))
-            X_cols = x_pad.size // B
-            X_pad = x_pad.reshape(X_cols, B).T  # Commutate across polyphase filters
-            X_pad = np.flipud(X_pad)  # Commutate from bottom to top
-            if mode == "full":
-                Y = np.zeros((B, X_cols + M - 1), dtype=dtype)
-                for i in range(B):
-                    Y[i] = scipy.signal.convolve(X_pad[i], H[i], mode="full")
-            elif mode == "rate":
-                Y = np.zeros((B, X_cols), dtype=dtype)
-                for i in range(B):
-                    corr = scipy.signal.convolve(X_pad[i], H[i], mode="full")
-                    Y[i] = corr[M // 2 : M // 2 + X_cols]
-            else:
-                raise ValueError(f"Argument 'mode' must be 'rate' or 'full', not {mode!r}.")
-
-        # Sum the outputs of the polyphase filters
-        y = np.sum(Y, axis=0)
+        y, self._state = _polyphase_decimate(x, self._state, self.polyphase_taps, mode, self.streaming)
 
         return y
 
     def __repr__(self) -> str:
         """
         Returns a code-styled string representation of the object.
 
         Examples:
             .. ipython:: python
 
                 fir = sdr.Decimator(7)
                 fir
         """
         if self.method == "custom":
-            h_str = np.array2string(self.taps, max_line_width=1e6, separator=", ", suppress_small=True)
+            h_str = np.array2string(self.taps, max_line_width=int(1e6), separator=", ", suppress_small=True)
         else:
             h_str = repr(self.method)
         return f"sdr.{type(self).__name__}({self.rate}, {h_str}, streaming={self.streaming})"
 
     def __str__(self) -> str:
         """
         Returns a human-readable string representation of the object.
@@ -804,15 +879,15 @@
     def method(self) -> Literal["kaiser", "custom"]:
         """
         The method used to design the multirate filter.
         """
         return self._method
 
     @property
-    def taps(self) -> np.ndarray:
+    def taps(self) -> npt.NDArray:
         """
         The prototype feedforward taps $h_i$.
 
         Notes:
             The prototype feedforward taps $h_i$ are the feedforward taps of the FIR filter before
             polyphase decomposition. The polyphase feedforward taps $h_{i, j}$ are the feedforward taps
             of the FIR filter after polyphase decomposition.
@@ -827,15 +902,15 @@
                 fir = sdr.Decimator(3, np.arange(10))
                 fir.taps
                 fir.polyphase_taps
         """
         return self._taps
 
     @property
-    def polyphase_taps(self) -> np.ndarray:
+    def polyphase_taps(self) -> npt.NDArray:
         """
         The polyphase feedforward taps $h_{i, j}$.
 
         Notes:
             The prototype feedforward taps $h_i$ are the feedforward taps of the FIR filter before
             polyphase decomposition. The polyphase feedforward taps $h_{i, j}$ are the feedforward taps
             of the FIR filter after polyphase decomposition.
@@ -848,7 +923,346 @@
             .. ipython:: python
 
                 fir = sdr.Decimator(3, np.arange(10))
                 fir.taps
                 fir.polyphase_taps
         """
         return self._polyphase_taps
+
+    @property
+    def delay(self) -> int:
+        """
+        The delay of FIR filter in samples. The delay indicates the output sample index that corresponds to the
+        first input sample.
+        """
+        assert super().delay % self.rate == 0, f"This should always be true. {super().delay} % {self.rate} != 0"
+        return super().delay // self.rate
+
+
+@export
+class Resampler(FIR):
+    r"""
+    Implements a polyphase rational resampling FIR filter.
+
+    Notes:
+        The polyphase rational resampling filter is equivalent to first upsampling the input signal $x[n]$ by $P$
+        (by inserting $P-1$ zeros between each sample), filtering the upsampled signal with the prototype FIR filter
+        with feedforward coefficients $h_{i}$, and then decimating the filtered signal by $Q$ (by discarding $Q-1$
+        samples between each sample).
+
+        Instead, the polyphase rational resampling filter first decomposes the prototype FIR filter into $P$ polyphase
+        filters with feedforward coefficients $h_{i, j}$. The polyphase filters are then applied to the
+        input signal $x[n]$ in parallel. The output of the polyphase filters are then commutated by $Q$ to produce
+        the output signal $y[n]$. This prevents the need to multiply with zeros in the upsampled input,
+        as is needed in the first case.
+
+        .. code-block:: text
+           :caption: Polyphase 2/3 Resampling FIR Filter Block Diagram
+
+                                  +------------------------+
+                              +-->| h[0], h[2], h[4], h[6] |--> ..., ____, y[0]
+                              |   +------------------------+
+            ..., x[1], x[0] --+
+                              |   +------------------------+
+                              +-->| h[1], h[3], h[5], 0    |--> ..., y[1], ____
+                                  +------------------------+
+
+            Input Hold                                          Output Commutator by 3
+                                                                (top-to-bottom)
+
+            x[n] = Input signal with sample rate fs
+            y[n] = Output signal with sample rate fs * P / Q
+            h[n] = Prototype FIR filter
+
+        The polyphase feedforward taps $h_{i, j}$ are related to the prototype feedforward taps $h_i$ by
+
+        $$h_{i, j} = h_{i + j P} .$$
+
+        If the interpolation rate $P$ is 1, then the polyphase rational resampling filter is equivalent to the
+        polyphase decimating filter. See :class:`~sdr.Decimator`.
+
+    Examples:
+        Create an input signal to resample.
+
+        .. ipython:: python
+
+            x = np.cos(np.pi / 4 * np.arange(40))
+
+        Create a polyphase filter that resamples by 7/3 using the Kaiser window method.
+
+        .. ipython:: python
+
+            fir = sdr.Resampler(7, 3); fir
+            y = fir(x)
+
+            @savefig sdr_Resampler_1.png
+            plt.figure(figsize=(8, 4)); \
+            sdr.plot.time_domain(x, marker="o", label="Input"); \
+            sdr.plot.time_domain(y, sample_rate=fir.rate, marker=".", label="Resampled"); \
+            plt.title("Resampling by 7/3 with the Kaiser window method"); \
+            plt.tight_layout();
+
+        Create a streaming polyphase filter that resamples by 7/3 using the Kaiser window method. This filter
+        preserves state between calls.
+
+        .. ipython:: python
+
+            fir = sdr.Resampler(7, 3, streaming=True); fir
+
+            y1 = fir(x[0:10]); \
+            y2 = fir(x[10:20]); \
+            y3 = fir(x[20:30]); \
+            y4 = fir(x[30:40]); \
+            y5 = fir.flush()
+
+            @savefig sdr_Resampler_2.png
+            plt.figure(figsize=(8, 4)); \
+            sdr.plot.time_domain(x, marker="o", label="Input"); \
+            sdr.plot.time_domain(y1, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 0, marker=".", label="Resampled $y_1[n]$"); \
+            sdr.plot.time_domain(y2, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 10, marker=".", label="Resampled $y_2[n]$"); \
+            sdr.plot.time_domain(y3, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 20, marker=".", label="Resampled $y_3[n]$"); \
+            sdr.plot.time_domain(y4, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 30, marker=".", label="Resampled $y_4[n]$"); \
+            sdr.plot.time_domain(y5, sample_rate=fir.rate, offset=-fir.delay/fir.rate + 40, marker=".", label="Resampled $y_5[n]$"); \
+            plt.title("Streaming resampling by 7/3 with the Kaiser window method"); \
+            plt.tight_layout();
+
+        Create a polyphase filter that resamples by 5/7 using linear method.
+
+        .. ipython:: python
+
+            fir = sdr.Resampler(5, 7); fir
+            y = fir(x)
+
+            @savefig sdr_Resampler_3.png
+            plt.figure(figsize=(8, 4)); \
+            sdr.plot.time_domain(x, marker=".", label="Input"); \
+            sdr.plot.time_domain(y, sample_rate=fir.rate, marker="o", label="Resampled"); \
+            plt.title("Resampling by 5/7 with the Kaiser window method"); \
+            plt.tight_layout();
+
+    Group:
+        dsp-multirate-filtering
+    """
+
+    def __init__(
+        self,
+        up: int,
+        down: int,
+        taps: Literal["kaiser", "linear", "linear-matlab", "zoh"] | npt.ArrayLike = "kaiser",
+        streaming: bool = False,
+    ):
+        r"""
+        Creates a polyphase FIR rational resampling filter.
+
+        Arguments:
+            up: The interpolation rate $P$.
+            down: The decimation rate $Q$.
+            taps: The multirate filter design specification.
+
+                - `"kaiser"`: The multirate filter is designed using :func:`~sdr.multirate_taps()`
+                  with arguments `up` and `down`.
+                - `"linear"`: The multirate filter is designed to linearly interpolate between samples.
+                  The filter coefficients are a length-$2P$ linear ramp $\frac{1}{P} [0, ..., P-1, P, P-1, ..., 1]$.
+                  The first output sample aligns with the first input sample.
+                - `"linear-matlab"`: The multirate filter is designed to linearly interpolate between samples.
+                  The filter coefficients are a length-$2P$ linear ramp $\frac{1}{P} [1, ..., P-1, P, P-1, ..., 0]$.
+                  This is method MATLAB uses. The first output sample is advanced from the first input sample.
+                - `"zoh"`: The multirate filter is designed to be a zero-order hold.
+                  The filter coefficients are a length-$P$ array of ones.
+                - `npt.ArrayLike`: The multirate filter feedforward coefficients $h_i$.
+
+            streaming: Indicates whether to use streaming mode. In streaming mode, previous inputs are
+                preserved between calls to :meth:`~Resampler.__call__()`.
+        """
+        if not isinstance(up, int):
+            raise TypeError(f"Argument 'up' must be an integer, not {type(up)}.")
+        if not up >= 1:
+            raise ValueError(f"Argument 'up' must be at least 1, not {up}.")
+
+        if not isinstance(down, int):
+            raise TypeError(f"Argument 'down' must be an integer, not {type(down)}.")
+        if not down >= 1:
+            raise ValueError(f"Argument 'down' must be at least 1, not {down}.")
+
+        self._up = up
+        self._down = down
+        self._rate = up / down
+        self._method: Literal["kaiser", "linear", "linear-matlab", "zoh", "custom"]
+
+        if not isinstance(taps, str):
+            self._method = "custom"
+            taps = np.asarray(taps)
+        elif taps == "kaiser":
+            self._method = "kaiser"
+            taps = multirate_taps(up, down)
+        elif taps == "linear":
+            if not up > 1:
+                raise ValueError(f"Argument 'up' must be greater than 1 to use the 'linear' method, not {up}.")
+            self._method = "linear"
+            taps = _multirate_taps_linear(up)
+        elif taps == "linear-matlab":
+            if not up > 1:
+                raise ValueError(f"Argument 'up' must be greater than 1 to use the 'linear-matlab' method, not {up}.")
+            self._method = "linear-matlab"
+            taps = _multirate_taps_linear_matlab(up)
+        elif taps == "zoh":
+            if not up > 1:
+                raise ValueError(f"Argument 'up' must be greater than 1 to use the 'zoh' method, not {up}.")
+            self._method = "zoh"
+            taps = _multirate_taps_zoh(up)
+        else:
+            raise ValueError(
+                f"Argument 'taps' must be 'kaiser', 'linear', 'linear-matlab', 'zoh', or an array-like, not {taps}."
+            )
+
+        self._polyphase_taps = polyphase_matrix(up, down, taps)
+
+        super().__init__(taps, streaming=streaming)
+
+    ##############################################################################
+    # Special methods
+    ##############################################################################
+
+    def __call__(self, x: npt.ArrayLike, mode: Literal["rate", "full"] = "rate") -> np.ndarray:
+        r"""
+        Resamples and filters the input signal $x[n]$ with the polyphase FIR filter.
+        """
+        x = np.atleast_1d(x)
+        if not x.ndim == 1:
+            raise ValueError(f"Argument 'x' must be a 1-D, not {x.ndim}-D.")
+
+        if self.up == 1:
+            y, self._state = _polyphase_decimate(x, self._state, self.polyphase_taps, mode, self.streaming)
+        else:
+            y, self._state = _polyphase_interpolate(x, self._state, self.polyphase_taps, mode, self.streaming)
+            y = y[:: self.down]  # Downsample the interpolated output
+
+        return y
+
+    def __repr__(self) -> str:
+        """
+        Returns a code-styled string representation of the object.
+
+        Examples:
+            .. ipython:: python
+
+                fir = sdr.Resampler(4, 3)
+                fir
+        """
+        if self.method == "custom":
+            h_str = np.array2string(self.taps, max_line_width=int(1e6), separator=", ", suppress_small=True)
+        else:
+            h_str = repr(self.method)
+        return f"sdr.{type(self).__name__}({self.up}, {self.down}, {h_str}, streaming={self.streaming})"
+
+    def __str__(self) -> str:
+        """
+        Returns a human-readable string representation of the object.
+
+        Examples:
+            .. ipython:: python
+
+                fir = sdr.Resampler(4, 3)
+                print(fir)
+        """
+        string = f"sdr.{type(self).__name__}:"
+        string += f"\n  order: {self.order}"
+        string += f"\n  rate: {self.up} / {self.down}"
+        string += f"\n  method: {self._method!r}"
+        string += f"\n  polyphase_taps: {self.polyphase_taps.shape} shape"
+        string += f"\n  delay: {self.delay}"
+        string += f"\n  streaming: {self.streaming}"
+        return string
+
+    ##############################################################################
+    # Streaming mode
+    ##############################################################################
+
+    def reset(self):
+        self._state = np.zeros(self.polyphase_taps.shape[1] - 1)
+
+    ##############################################################################
+    # Properties
+    ##############################################################################
+
+    @property
+    def up(self) -> int:
+        """
+        The interpolation rate $P$.
+        """
+        return self._up
+
+    @property
+    def down(self) -> int:
+        """
+        The decimation rate $Q$.
+        """
+        return self._down
+
+    @property
+    def rate(self) -> float:
+        """
+        The resampling rate $P/Q$.
+        """
+        return self._rate
+
+    @property
+    def method(self) -> Literal["kaiser", "linear", "linear-matlab", "zoh", "custom"]:
+        """
+        The method used to design the multirate filter.
+        """
+        return self._method
+
+    @property
+    def taps(self) -> npt.NDArray:
+        """
+        The prototype feedforward taps $h_i$.
+
+        Notes:
+            The prototype feedforward taps $h_i$ are the feedforward taps of the FIR filter before
+            polyphase decomposition. The polyphase feedforward taps $h_{i, j}$ are the feedforward taps
+            of the FIR filter after polyphase decomposition.
+
+            The polyphase feedforward taps $h_{i, j}$ are related to the prototype feedforward taps $h_i$ by
+
+            $$h_{i, j} = h_{i + j P} .$$
+
+        Examples:
+            .. ipython:: python
+
+                fir = sdr.Resampler(4, 3, np.arange(10))
+                fir.taps
+                fir.polyphase_taps
+        """
+        return self._taps
+
+    @property
+    def polyphase_taps(self) -> npt.NDArray:
+        """
+        The polyphase feedforward taps $h_{i, j}$.
+
+        Notes:
+            The prototype feedforward taps $h_i$ are the feedforward taps of the FIR filter before
+            polyphase decomposition. The polyphase feedforward taps $h_{i, j}$ are the feedforward taps
+            of the FIR filter after polyphase decomposition.
+
+            The polyphase feedforward taps $h_{i, j}$ are related to the prototype feedforward taps $h_i$ by
+
+            $$h_{i, j} = h_{i + j P} .$$
+
+        Examples:
+            .. ipython:: python
+
+                fir = sdr.Resampler(4, 3, np.arange(10))
+                fir.taps
+                fir.polyphase_taps
+        """
+        return self._polyphase_taps
+
+    @property
+    def delay(self) -> int:
+        """
+        The delay of FIR filter in samples. The delay indicates the output sample index that corresponds to the
+        first input sample.
+        """
+        assert super().delay % self.down == 0, f"This should always be true. {super().delay} % {self.down} != 0"
+        return super().delay // self.down
```

### Comparing `sdr-0.0.8/src/sdr/_helper.py` & `sdr-0.0.9/src/sdr/_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         # as sdr.obj and not sdr._private_module.obj.
         idx = obj.__module__.find("._")
         obj.__module__ = obj.__module__[:idx]
 
     # Append this object to the private module's "all" list
     public_members = getattr(module, "__all__", [])
     public_members.append(obj.__name__)
-    setattr(module, "__all__", public_members)
+    module.__all__ = public_members
 
     return obj
 
 
 def extend_docstring(method, replace=None, docstring=""):
     """
     A decorator to extend the docstring of `method` with the provided docstring. The decorator also finds
```

### Comparing `sdr-0.0.8/src/sdr/_link_budget/_antenna.py` & `sdr-0.0.9/src/sdr/_link_budget/_antenna.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import scipy.constants
 
 from .._conversion import db
 from .._helper import export
 
 
 @export
-def wavelength(freq: float) -> float:
+def wavelength(freq: npt.ArrayLike) -> npt.NDArray[np.float_]:
     r"""
-    Calculates the wavelength $\lambda$ of a electromagnetic wave with frequency $f$.
+    Calculates the wavelength $\lambda$ of an electromagnetic wave with frequency $f$.
 
     $$\lambda = \frac{c}{f}$$
 
     Arguments:
         freq: The frequency $f$ in Hz of the signal.
 
     Returns:
@@ -36,18 +36,18 @@
     """
     freq = np.asarray(freq)
     return scipy.constants.speed_of_light / freq
 
 
 @export
 def parabolic_antenna(
-    freq: float,
-    diameter: float,
-    efficiency: float = 0.55,
-) -> tuple[npt.ArrayLike, npt.ArrayLike]:
+    freq: npt.ArrayLike,
+    diameter: npt.ArrayLike,
+    efficiency: npt.ArrayLike = 0.55,
+) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.float_]]:
     r"""
     Calculates the gain $G$ and beamwidth $\theta$ of a parabolic reflector.
 
     Arguments:
         freq: The frequency $f$ in Hz of the signal.
         diameter: The diameter $d$ in meters of the parabolic reflector.
         efficiency: The efficiency $0 \le \eta \le 1$ of the parabolic reflector.
@@ -76,22 +76,24 @@
 
             sdr.parabolic_antenna(1e9, 2)
 
     Group:
         link-budget-antennas
     """
     freq = np.asarray(freq)
+    if not np.all(freq > 0):
+        raise ValueError("Argument 'freq' must be positive, not {freq}.")
 
     diameter = np.asarray(diameter)
     if not np.all(diameter > 0):
-        raise ValueError("Argument 'diameter' must be positive.")
+        raise ValueError("Argument 'diameter' must be positive, not {diameter}.")
 
     efficiency = np.asarray(efficiency)
     if not np.all((0 <= efficiency) & (efficiency <= 1)):
-        raise ValueError("Argument 'efficiency' must be between 0 and 1.")
+        raise ValueError("Argument 'efficiency' must be between 0 and 1, not {efficiency}.")
 
     lambda_ = wavelength(freq)  # Wavelength in meters
     G = (np.pi * diameter / lambda_) ** 2 * efficiency  # Gain in linear units
     G = db(G)  # Gain in dBi
 
     theta = np.arcsin(3.83 * lambda_ / (np.pi * diameter))  # Beamwidth in radians
     theta = np.rad2deg(theta)  # Beamwidth in degrees
```

### Comparing `sdr-0.0.8/src/sdr/_link_budget/_capacity.py` & `sdr-0.0.9/src/sdr/_link_budget/_capacity.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 import numpy.typing as npt
 import scipy.stats
 
 from .._conversion import linear
 from .._helper import export
 
 
-def Hb(x: npt.ArrayLike) -> np.ndarray:
+def Hb(x: npt.ArrayLike) -> npt.NDArray[np.float_]:
     """
     Computes the binary entropy function $H_b(x)$.
     """
     x = np.asarray(x)
 
-    return scipy.stats.entropy([x, 1 - x], base=2)
+    return scipy.stats.entropy([x, 1 - x], base=2)  # type: ignore
 
 
 @export
-def bsc_capacity(p: npt.ArrayLike) -> np.ndarray:
+def bsc_capacity(p: npt.ArrayLike) -> npt.NDArray[np.float_]:
     r"""
     Calculates the capacity of a binary symmetric channel (BSC).
 
     Arguments:
         p: The transition probability $p$ of the BSC channel.
 
     Returns:
@@ -63,15 +63,15 @@
     if not (np.all(0 <= p) and np.all(p <= 1)):
         raise ValueError(f"Argument 'p' must be between 0 and 1, not {p}.")
 
     return 1 - Hb(p)
 
 
 @export
-def bec_capacity(p: npt.ArrayLike) -> np.ndarray:
+def bec_capacity(p: npt.ArrayLike) -> npt.NDArray[np.float_]:
     r"""
     Calculates the capacity of a binary erasure channel (BEC).
 
     Arguments:
         p: The erasure probability $p$ of the BEC channel.
 
     Returns:
@@ -105,19 +105,19 @@
     Group:
         link-budget-channel-capacity
     """
     p = np.asarray(p)
     if not (np.all(0 <= p) and np.all(p <= 1)):
         raise ValueError(f"Argument 'p' must be between 0 and 1, not {p}.")
 
-    return 1 - p
+    return 1 - p  # type: ignore
 
 
 @export
-def awgn_capacity(snr: npt.ArrayLike, bandwidth: float | None = None) -> np.ndarray:
+def awgn_capacity(snr: npt.ArrayLike, bandwidth: float | None = None) -> npt.NDArray[np.float_]:
     r"""
     Calculates the capacity of an additive white Gaussian noise (AWGN) channel.
 
     Arguments:
         snr: The signal-to-noise ratio $S / N$ in dB of the channel.
         bandwidth: The bandwidth $B$ of the channel in Hz. If specified, the capacity is calculated in bits/s.
             If `None`, the capacity is calculated in bits/2D.
```

### Comparing `sdr-0.0.8/src/sdr/_link_budget/_path_loss.py` & `sdr-0.0.9/src/sdr/_link_budget/_path_loss.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import numpy.typing as npt
 import scipy.constants
 
 from .._helper import export
 
 
 @export
-def fspl(d: npt.ArrayLike, f: npt.ArrayLike) -> np.ndarray:
+def fspl(distance: npt.ArrayLike, freq: npt.ArrayLike) -> npt.NDArray[np.float_]:
     r"""
     Calculates the free-space path loss (FSPL) in dB.
 
     $$\text{FSPL} = 10 \log_{10} \left( \frac{4 \pi d f}{c} \right)^2$$
 
     Arguments:
-        d: The distance $d$ in meters between the transmitter and receiver.
-        f: The frequency $f$ in Hz of the signal.
+        distance: The distance $d$ in meters between the transmitter and receiver.
+        freq: The frequency $f$ in Hz of the signal.
 
     Returns:
         The free-space path loss (FSPL) in dB.
 
     Note:
         The free-space path loss equation is only valid in the far field. For $d < \lambda / 4 \pi$, the FSPL
         equation has a negative result, implying a path gain. This is not possible. So these path losses
@@ -64,20 +64,25 @@
             plt.ylabel('Free-space path loss (dB)'); \
             plt.grid(True); \
             plt.tight_layout()
 
     Group:
         link-budget-path-losses
     """
-    d = np.asarray(d)
-    f = np.asarray(f)
+    distance = np.asarray(distance)
+    if not np.all(distance >= 0):
+        raise ValueError(f"Argument 'distance' must be non-negative, not {distance}.")
+
+    freq = np.asarray(freq)
+    if not np.all(freq > 0):
+        raise ValueError(f"Argument 'freq' must be positive, not {freq}.")
 
     # The free-space path loss equation is only valid in the far field. For very small distances, the FSPL
     # equation could have a negative result, implying a path gain. This is not possible. So for distances less
     # than lambda / (4 * pi), the path loss is set to 0 dB.
-    lambda_ = scipy.constants.speed_of_light / f
-    d = np.maximum(d, lambda_ / (4 * np.pi))
+    lambda_ = scipy.constants.speed_of_light / freq
+    distance = np.maximum(distance, lambda_ / (4 * np.pi))
 
     # The free-space path loss equation
-    loss = 20 * np.log10(4 * np.pi * d * f / scipy.constants.speed_of_light)
+    loss = 20 * np.log10(4 * np.pi * distance * freq / scipy.constants.speed_of_light)
 
-    return loss
+    return loss  # type: ignore
```

### Comparing `sdr-0.0.8/src/sdr/_loop_filter.py` & `sdr-0.0.9/src/sdr/_synchronization/_loop_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 A module for discrete-time loop filters.
 """
 from __future__ import annotations
 
-import numpy as np
 import numpy.typing as npt
 
-from ._filter import IIR
-from ._helper import export
+from .._filter import IIR
+from .._helper import export
 
 
 @export
 class LoopFilter:
     r"""
     Implements a 2nd order, proportional-plus-integrator (PPI) loop filter.
 
@@ -96,15 +95,15 @@
         Resets the loop filter.
 
         Examples:
             See the :ref:`phase-locked-loop` example.
         """
         self.iir.reset()
 
-    def __call__(self, x: npt.ArrayLike) -> np.ndarray:
+    def __call__(self, x: npt.NDArray) -> npt.NDArray:
         """
         Filters the input signal $x[n]$.
 
         Arguments:
             x: The input signal $x[n]$.
 
         Returns:
```

### Comparing `sdr-0.0.8/src/sdr/_measurement/_errors.py` & `sdr-0.0.9/src/sdr/_measurement/_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             The number of counts at the specified SNR.
 
         Examples:
             See the class :ref:`error-rate-example` section.
         """
         return self._counts.get(snr, 0)
 
-    def error_rate(self, snr: float | None) -> float:
+    def error_rate(self, snr: float) -> float:
         """
         Returns the error rate at the specified signal-to-noise ratio (SNR).
 
         Arguments:
             snr: The signal-to-noise ratio (SNR) in dB. This can be $E_b/N_0$, $E_s/N_0$, $S/N$, $C/N_0$,
                 or other SNR quantities. However, users are cautioned to be consistent for a given class instance.
 
@@ -145,15 +145,15 @@
             The error rate at the specified SNR.
 
         Examples:
             See the class :ref:`error-rate-example` section.
         """
         return self.errors(snr) / self.counts(snr)
 
-    def error_rates(self) -> tuple[np.ndarray, np.ndarray]:
+    def error_rates(self) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.float_]]:
         r"""
         Returns all signal-to-noise ratios (SNRs) in ascending order and their corresponding error rates.
 
         Returns:
             - The signal-to-noise ratios (SNRs). The specific SNR quantity (e.g., $E_b/N_0$, $E_s/N_0$, $S/N$,
               $C/N_0$) is whatever was consistently provided to :meth:`add`.
             - The bit or symbol error rates.
```

### Comparing `sdr-0.0.8/src/sdr/_measurement/_modulation.py` & `sdr-0.0.9/src/sdr/_measurement/_modulation.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/src/sdr/_measurement/_power.py` & `sdr-0.0.9/src/sdr/_measurement/_voltage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,83 @@
 """
-A module containing various power measurement functions.
+A module containing various voltage measurement functions.
 """
 from __future__ import annotations
 
 import numpy as np
 import numpy.typing as npt
 
 from .._conversion import db as to_db
 from .._helper import export
 
 
 @export
-def peak_power(x: npt.ArrayLike, db: bool = False) -> float:
+def peak_voltage(x: npt.NDArray, db: bool = False) -> float:
     r"""
-    Measures the peak power of a time-domain signal $x[n]$.
+    Measures the peak voltage of a time-domain signal $x[n]$.
 
-    $$P_{\text{peak}} = \max \left| x[n] \right|^2$$
+    $$V_{\text{peak}} = \max \left| x[n] \right|$$
 
     Arguments:
         x: The time-domain signal $x[n]$ to measure.
-        db: Indicates whether to return the result in dB.
+        db: Indicates whether to return the result in decibels (dB).
 
     Returns:
-        The peak power. If `db=False`, $P_{\text{peak}}$ is returned.
-        If `db=True`, $10 \log_{10} P_{\text{peak}}$ is returned.
+        The peak voltage. If `db=False`, $V_{\text{peak}}$ is returned.
+        If `db=True`, $20 \log_{10} V_{\text{peak}}$ is returned.
 
     Group:
-        measurement-power
+        measurement-voltage
     """
-    x = np.asarray(x)
-    P_peak = np.max(np.abs(x) ** 2)
+    V_peak = np.max(np.abs(x))
     if db:
-        P_peak = to_db(P_peak, type="power")
-    return P_peak
+        V_peak = to_db(V_peak, type="voltage")
+    return V_peak
 
 
 @export
-def average_power(x: npt.ArrayLike, db: bool = False) -> float:
+def rms_voltage(x: npt.NDArray, db: bool = False) -> float:
     r"""
-    Measures the average power of a time-domain signal $x[n]$.
+    Measures the root-mean-square (RMS) voltage of a time-domain signal $x[n]$.
 
-    $$P_{\text{avg}} = \frac{E}{N} = \frac{1}{N} \sum_{n=0}^{N-1} \left| x[n] \right|^2$$
+    $$V_{\text{rms}} = \sqrt{\frac{1}{N} \sum_{n=0}^{N-1} \left| x[n] \right|^2}$$
 
     Arguments:
         x: The time-domain signal $x[n]$ to measure.
-        db: Indicates whether to return the result in dB.
+        db: Indicates whether to return the result in decibels (dB).
 
     Returns:
-        The average power. If `db=False`, $P_{\text{avg}}$ is returned.
-        If `db=True`, $10 \log_{10} P_{\text{avg}}$ is returned.
+        The root-mean-square voltage. If `db=False`, $V_{\text{rms}}$ is returned.
+        If `db=True`, $20 \log_{10} V_{\text{rms}}$ is returned.
 
     Group:
-        measurement-power
+        measurement-voltage
     """
-    x = np.asarray(x)
-    P_avg = np.mean(np.abs(x) ** 2)
+    V_rms = np.sqrt(np.mean(np.abs(x) ** 2))
     if db:
-        P_avg = to_db(P_avg, type="power")
-    return P_avg
+        V_rms = to_db(V_rms, type="voltage")
+    return V_rms
 
 
 @export
-def papr(x: npt.ArrayLike) -> float:
+def crest_factor(x: npt.NDArray) -> float:
     r"""
-    Measures the peak-to-average power ratio (PAPR) of a time-domain signal $x[n]$.
+    Measures the crest factor of a time-domain signal $x[n]$.
 
-    $$\text{PAPR} = 10 \log_{10} \frac{P_{\text{peak}}}{P_{\text{avg}}}$$
+    $$\text{CF} = \frac{V_{\text{peak}}}{V_{\text{rms}}}$$
 
     Arguments:
         x: The time-domain signal $x[n]$ to measure.
 
     Returns:
-        The PAPR of $x[n]$ in dB.
+        The crest factor of $x[n]$.
 
     See Also:
-        sdr.peak_power, sdr.average_power
+        sdr.peak_voltage, sdr.rms_voltage
 
     References:
         - https://en.wikipedia.org/wiki/Crest_factor
 
     Group:
-        measurement-power
+        measurement-voltage
     """
-    x = np.asarray(x)
-    return to_db(peak_power(x) / average_power(x))
+    return peak_voltage(x) / rms_voltage(x)
```

### Comparing `sdr-0.0.8/src/sdr/_modulation/_linear.py` & `sdr-0.0.9/src/sdr/_modulation/_linear.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,96 +116,95 @@
         string = f"sdr.{type(self).__name__}:"
         string += f"\n  order: {self.order}"
         string += f"\n  symbol_map: {self.symbol_map.shape} shape"
         string += f"\n    {self.symbol_map.tolist()}"
         string += f"\n  phase_offset: {self.phase_offset}"
         return string
 
-    def map_symbols(self, s: npt.ArrayLike) -> np.ndarray:
+    def map_symbols(self, s: npt.ArrayLike) -> npt.NDArray[np.complex_]:
         r"""
         Converts the decimal symbols $s[k]$ to complex symbols $a[k]$.
 
         Arguments:
             s: The decimal symbols $s[k]$ to map, $0$ to $M-1$.
 
         Returns:
             The complex symbols $a[k]$.
         """
+        s = np.asarray(s)  # Decimal symbols
         return self._map_symbols(s)
 
-    def _map_symbols(self, s: npt.ArrayLike) -> np.ndarray:
-        s = np.asarray(s)  # Decimal symbols
+    def _map_symbols(self, s: npt.NDArray[np.int_]) -> npt.NDArray[np.complex_]:
         a = self.symbol_map[s]  # Complex symbols
         return a
 
-    def decide_symbols(self, a_hat: npt.ArrayLike) -> np.ndarray:
+    def decide_symbols(self, a_hat: npt.ArrayLike) -> npt.NDArray[np.int_]:
         r"""
         Converts the received complex symbols $\hat{a}[k]$ into decimal symbol decisions $\hat{s}[k]$
         using maximum-likelihood estimation (MLE).
 
         Arguments:
             a_hat: The received complex symbols $\hat{a}[k]$.
 
         Returns:
             The decimal symbol decisions $\hat{s}[k]$, $0$ to $M-1$.
         """
+        a_hat = np.asarray(a_hat)  # Complex symbols
         return self._decide_symbols(a_hat)
 
-    def _decide_symbols(self, a_hat: npt.ArrayLike) -> np.ndarray:
+    def _decide_symbols(self, a_hat: npt.NDArray[np.complex_]) -> npt.NDArray[np.int_]:
         error_vectors = np.subtract.outer(a_hat, self.symbol_map)
         s_hat = np.argmin(np.abs(error_vectors), axis=-1)
         return s_hat
 
-    def modulate(self, s: npt.ArrayLike) -> np.ndarray:
+    def modulate(self, s: npt.ArrayLike) -> npt.NDArray[np.complex_]:
         r"""
         Modulates the decimal symbols $s[k]$ into pulse-shaped complex samples $x[n]$.
 
         Arguments:
             s: The decimal symbols $s[k]$ to modulate, $0$ to $M-1$.
 
         Returns:
             The pulse-shaped complex samples $x[n]$ with :obj:`sps` samples per symbol
             and length `sps * s.size + pulse_shape.size - 1`.
         """
+        s = np.asarray(s)  # Decimal symbols
         return self._modulate(s)
 
-    def _modulate(self, s: npt.ArrayLike) -> np.ndarray:
+    def _modulate(self, s: npt.NDArray[np.int_]) -> npt.NDArray[np.complex_]:
         a = self._map_symbols(s)  # Complex symbols
         x = self._tx_pulse_shape(a)  # Complex samples
         return x
 
-    def _tx_pulse_shape(self, a: npt.ArrayLike) -> np.ndarray:
-        a = np.asarray(a)  # Complex symbols
+    def _tx_pulse_shape(self, a: npt.NDArray[np.complex_]) -> npt.NDArray[np.complex_]:
         x = self._tx_filter(a, mode="full")  # Complex samples
         return x
 
-    def demodulate(self, x_hat: npt.ArrayLike) -> tuple[np.ndarray, np.ndarray]:
+    def demodulate(self, x_hat: npt.ArrayLike) -> tuple[npt.NDArray[np.int_], npt.NDArray[np.complex_]]:
         r"""
         Demodulates the pulse-shaped complex samples $\hat{x}[n]$ into decimal symbol decisions $\hat{s}[k]$
         using matched filtering and maximum-likelihood estimation.
 
         Arguments:
             x_hat: The received pulse-shaped complex samples $\hat{x}[n]$ to demodulate, with :obj:`sps`
                 samples per symbol and length `sps * s_hat.size + pulse_shape.size - 1`.
 
         Returns:
             - The decimal symbol decisions $\hat{s}[k]$, $0$ to $M-1$.
             - The matched filter outputs $\hat{a}[k]$.
         """
+        x_hat = np.asarray(x_hat)  # Complex samples
         return self._demodulate(x_hat)
 
-    def _demodulate(self, x_hat: npt.ArrayLike) -> tuple[np.ndarray, np.ndarray]:
-        x_hat = np.asarray(x_hat)  # Complex samples
+    def _demodulate(self, x_hat: npt.NDArray[np.complex_]) -> tuple[npt.NDArray[np.int_], npt.NDArray[np.complex_]]:
         a_hat = self._rx_matched_filter(x_hat)  # Complex symbols
         s_hat = self._decide_symbols(a_hat)  # Decimal symbols
         return s_hat, a_hat
 
-    def _rx_matched_filter(self, x_hat: npt.ArrayLike) -> np.ndarray:
-        x_hat = np.asarray(x_hat)  # Complex samples
-
+    def _rx_matched_filter(self, x_hat: npt.NDArray[np.complex_]) -> npt.NDArray[np.complex_]:
         if self.pulse_shape.size % self.sps == 0:
             x_hat = np.insert(x_hat, 0, 0)
 
         a_hat = self._rx_filter(x_hat, mode="full")  # Complex symbols
 
         span = self.pulse_shape.size // self.sps
         if span == 1:
@@ -217,15 +216,15 @@
 
         # Select the symbol decisions from the output of the decimating filter
         a_hat = a_hat[offset : offset + N_symbols]
 
         return a_hat
 
     @abc.abstractmethod
-    def ber(self, ebn0: npt.ArrayLike | None = None) -> np.ndarray:
+    def ber(self, ebn0: npt.ArrayLike) -> npt.NDArray[np.float_]:
         r"""
         Computes the bit error rate (BER) at the provided $E_b/N_0$ values.
 
         Arguments:
             ebn0: Bit energy $E_b$ to noise PSD $N_0$ ratio in dB.
 
         Returns:
@@ -233,15 +232,15 @@
 
         See Also:
             sdr.esn0_to_ebn0, sdr.snr_to_ebn0
         """
         raise NotImplementedError("Bit error rate calculation for arbitrary linear modulations is not supported.")
 
     @abc.abstractmethod
-    def ser(self, esn0: npt.ArrayLike) -> np.ndarray:
+    def ser(self, esn0: npt.ArrayLike) -> npt.NDArray[np.float_]:
         r"""
         Computes the symbol error rate (SER) at the provided $E_s/N_0$ values.
 
         Arguments:
             esn0: Symbol energy $E_s$ to noise PSD $N_0$ ratio in dB.
 
         Returns:
@@ -270,30 +269,30 @@
     def phase_offset(self) -> float:
         r"""
         The phase offset $\phi$ in degrees.
         """
         return self._phase_offset
 
     @property
-    def symbol_map(self) -> np.ndarray:
+    def symbol_map(self) -> npt.NDArray[np.complex_]:
         r"""
         The symbol map $\{0, \dots, M-1\} \mapsto \mathbb{C}$. This maps decimal symbols from $0$ to $M-1$
         to complex symbols.
         """
         return self._symbol_map
 
     @property
     def sps(self) -> int:
         r"""
         The number of samples per symbol $f_s / f_{sym}$.
         """
         return self._sps
 
     @property
-    def pulse_shape(self) -> np.ndarray:
+    def pulse_shape(self) -> npt.NDArray[np.float_]:
         r"""
         The pulse shape $h[n]$ of the modulated signal.
         """
         return self._pulse_shape
 
     @property
     def tx_filter(self) -> Interpolator:
```

### Comparing `sdr-0.0.8/src/sdr/_modulation/_msk.py` & `sdr-0.0.9/src/sdr/_modulation/_msk.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/src/sdr/_modulation/_psk.py` & `sdr-0.0.9/src/sdr/_modulation/_psk.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         string += f"\n  order: {self.order}"
         string += f"\n  symbol_map: {self.symbol_map.shape} shape"
         string += f"\n    {self.symbol_map.tolist()}"
         string += f"\n  symbol_labels: {self._symbol_labels_str!r}"
         string += f"\n  phase_offset: {self.phase_offset}"
         return string
 
-    def ber(self, ebn0: npt.ArrayLike | None = None, diff_encoded: bool = False) -> np.ndarray:
+    def ber(self, ebn0: npt.ArrayLike, diff_encoded: bool = False) -> npt.NDArray[np.float_]:
         r"""
         Computes the bit error rate (BER) at the provided $E_b/N_0$ values.
 
         Arguments:
             ebn0: Bit energy $E_b$ to noise PSD $N_0$ ratio in dB.
             diff_encoded: Indicates whether the input symbols were differentially encoded.
 
@@ -272,15 +272,15 @@
                 # Equation 8.37 from Simon and Alouini
                 Pbe = 2 * Q(np.sqrt(2 * ebn0_linear)) - 2 * Q(np.sqrt(2 * ebn0_linear)) ** 2
             else:
                 raise ValueError("Differential encoding is not supported for M-PSK with M > 4.")
 
         return Pbe
 
-    def ser(self, esn0: npt.ArrayLike | None = None, diff_encoded: bool = False) -> np.ndarray:
+    def ser(self, esn0: npt.ArrayLike, diff_encoded: bool = False) -> npt.NDArray[np.float_]:
         r"""
         Computes the symbol error rate (SER) at the provided $E_s/N_0$ values.
 
         Arguments:
             esn0: Symbol energy $E_s$ to noise PSD $N_0$ ratio in dB.
             diff_encoded: Indicates whether the input symbols were differentially encoded.
 
@@ -430,15 +430,15 @@
                 psk.symbol_map
 
                 @savefig sdr_psk_symbol_map_2.png
                 plt.figure(figsize=(8, 4)); \
                 sdr.plot.symbol_map(psk.symbol_map, annotate="bin");
         """,
     )
-    def symbol_map(self) -> np.ndarray:
+    def symbol_map(self) -> npt.NDArray[np.complex_]:
         return super().symbol_map
 
 
 @export
 class PiMPSK(PSK):
     r"""
     Implements $\pi/M$ phase-shift keying ($\pi/M$ PSK) modulation and demodulation.
@@ -575,26 +575,24 @@
             order,
             phase_offset=phase_offset,
             symbol_labels=symbol_labels,
             sps=sps,
             pulse_shape=pulse_shape,
         )
 
-    def _map_symbols(self, s: npt.ArrayLike) -> np.ndarray:
+    def _map_symbols(self, s: npt.NDArray[np.int_]) -> npt.NDArray[np.complex_]:
         s = super()._map_symbols(s)
 
         # Rotate odd symbols by pi/M
         s_rotated = s.copy()
         s_rotated[1::2] *= np.exp(1j * np.pi / self.order)
 
         return s_rotated
 
-    def _decide_symbols(self, a_hat: npt.ArrayLike) -> np.ndarray:
-        a_hat = np.asarray(a_hat)
-
+    def _decide_symbols(self, a_hat: npt.NDArray[np.complex_]) -> npt.NDArray[np.int_]:
         # Rotate odd symbols by -pi/M
         a_hat_derotated = a_hat.copy()
         a_hat_derotated[1::2] *= np.exp(-1j * np.pi / self.order)
 
         return super()._decide_symbols(a_hat_derotated)
 
 
@@ -762,30 +760,29 @@
         string = f"sdr.{type(self).__name__}:"
         string += f"\n  symbol_map: {self.symbol_map.shape} shape"
         string += f"\n    {self.symbol_map.tolist()}"
         string += f"\n  symbol_labels: {self._symbol_labels_str!r}"
         string += f"\n  phase_offset: {self.phase_offset}"
         return string
 
-    def _map_symbols(self, s: npt.ArrayLike) -> np.ndarray:
+    def _map_symbols(self, s: npt.NDArray[np.int_]) -> npt.NDArray[np.complex_]:
         a = super()._map_symbols(s)
 
         a_I = np.repeat(a.real, 2)
         a_Q = np.repeat(a.imag, 2)
 
         # Shift Q symbols by 1/2 symbol
         a_I = np.append(a_I, 0)
         a_Q = np.insert(a_Q, 0, 0)
 
         a = a_I + 1j * a_Q
 
         return a
 
-    def _tx_pulse_shape(self, a: npt.ArrayLike) -> np.ndarray:
-        a = np.asarray(a)  # Complex symbols
+    def _tx_pulse_shape(self, a: npt.NDArray[np.complex_]) -> npt.NDArray[np.complex_]:
         a_I, a_Q = a.real, a.imag
 
         # Shift Q symbols by -1/2 symbol and grab 1 sample per symbol
         a_I = a_I[:-1:2]
         a_Q = a_Q[1::2]
 
         x_I = self._tx_filter(a_I, mode="full")  # Complex samples
@@ -795,28 +792,27 @@
         x_I = np.append(x_I, np.zeros(self.sps // 2))
         x_Q = np.insert(x_Q, 0, np.zeros(self.sps // 2))
 
         x = x_I + 1j * x_Q
 
         return x
 
-    def _decide_symbols(self, a_hat: npt.ArrayLike) -> np.ndarray:
+    def _decide_symbols(self, a_hat: npt.NDArray[np.complex_]) -> npt.NDArray[np.int_]:
         a_hat = np.asarray(a_hat)
         a_hat_I, a_hat_Q = a_hat.real, a_hat.imag
 
         # Shift Q symbols by -1/2 symbol and grab 1 sample per symbol
         a_hat_I = a_hat_I[:-1:2]
         a_hat_Q = a_hat_Q[1::2]
 
         a_hat = a_hat_I + 1j * a_hat_Q
 
         return super()._decide_symbols(a_hat)
 
-    def _rx_matched_filter(self, x_hat: npt.ArrayLike) -> np.ndarray:
-        x_hat = np.asarray(x_hat)
+    def _rx_matched_filter(self, x_hat: npt.NDArray[np.complex_]) -> npt.NDArray[np.complex_]:
         x_hat_I, x_hat_Q = x_hat.real, x_hat.imag
 
         # Shift Q samples by -1/2 symbol
         x_hat_I = x_hat_I[: -self.sps // 2]
         x_hat_Q = x_hat_Q[self.sps // 2 :]
 
         a_hat_I = super()._rx_matched_filter(x_hat_I)  # Complex samples
```

### Comparing `sdr-0.0.8/src/sdr/_modulation/_pulse_shapes.py` & `sdr-0.0.9/src/sdr/_modulation/_pulse_shapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 A module containing various discrete-time pulse shapes.
 """
 from __future__ import annotations
 
 import numpy as np
+import numpy.typing as npt
 from typing_extensions import Literal
 
 from .._helper import export
 
 
 @export
 def rectangular(
     sps: int,
     span: int = 1,
     norm: Literal["power", "energy", "passband"] = "energy",
-) -> np.ndarray:
+) -> npt.NDArray[np.float_]:
     r"""
     Returns a rectangular pulse shape.
 
     Arguments:
         sps: The number of samples per symbol.
         span: The length of the filter in symbols. The length of the filter is `span * sps` samples,
             but only the center `sps` samples are non-zero. The only reason for `span` to be larger than 1 is to
@@ -71,15 +72,15 @@
 
 
 @export
 def half_sine(
     sps: int,
     span: int = 1,
     norm: Literal["power", "energy", "passband"] = "energy",
-) -> np.ndarray:
+) -> npt.NDArray[np.float_]:
     r"""
     Returns a half-sine pulse shape.
 
     Arguments:
         sps: The number of samples per symbol.
         span: The length of the filter in symbols. The length of the filter is `span * sps` samples,
             but only the center `sps` samples are non-zero. The only reason for `span` to be larger than 1 is to
@@ -133,15 +134,15 @@
 
 @export
 def gaussian(
     time_bandwidth: float,
     span: int,
     sps: int,
     norm: Literal["power", "energy", "passband"] = "passband",
-) -> np.ndarray:
+) -> npt.NDArray[np.float_]:
     r"""
     Returns a Gaussian pulse shape.
 
     Arguments:
         time_bandwidth: The time-bandwidth product $B T_{sym}$ of the filter, where $B$ is the one-sided
             3-dB bandwidth in Hz and $T_{sym}$ is the symbol time in seconds. The time-bandwidth product
             can also be thought of as the fractional bandwidth $B / f_{sym}$. Smaller values produce
@@ -228,15 +229,15 @@
 
 @export
 def raised_cosine(
     alpha: float,
     span: int,
     sps: int,
     norm: Literal["power", "energy", "passband"] = "energy",
-) -> np.ndarray:
+) -> npt.NDArray[np.float_]:
     r"""
     Returns a raised cosine (RC) pulse shape.
 
     Arguments:
         alpha: The excess bandwidth $0 \le \alpha \le 1$ of the filter.
         span: The length of the filter in symbols. The length of the filter is `span * sps + 1` samples.
             The filter order `span * sps` must be even.
@@ -341,15 +342,15 @@
 
 @export
 def root_raised_cosine(
     alpha: float,
     span: int,
     sps: int,
     norm: Literal["power", "energy", "passband"] = "energy",
-) -> np.ndarray:
+) -> npt.NDArray[np.float_]:
     r"""
     Returns a square root raised cosine (SRRC) pulse shape.
 
     Arguments:
         alpha: The excess bandwidth $0 \le \alpha \le 1$ of the filter.
         span: The length of the filter in symbols. The length of the filter is `span * sps + 1` samples.
             The filter order `span * sps` must be even.
@@ -450,15 +451,15 @@
     h /= 1 / np.sqrt(Ts)
 
     h = _normalize(h, norm)
 
     return h
 
 
-def _normalize(h: np.ndarray, norm: Literal["power", "energy", "passband"]) -> np.ndarray:
+def _normalize(h: npt.NDArray[np.float_], norm: Literal["power", "energy", "passband"]) -> npt.NDArray[np.float_]:
     if norm == "power":
         h /= np.sqrt(np.max(np.abs(h) ** 2))
     elif norm == "energy":
         h /= np.sqrt(np.sum(np.abs(h) ** 2))
     elif norm == "passband":
         h /= np.sum(h)
     else:
```

### Comparing `sdr-0.0.8/src/sdr/_modulation/_symbol_encoding.py` & `sdr-0.0.9/src/sdr/_modulation/_symbol_encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import numpy.typing as npt
 
 from .._helper import export
 
 
 @export
-def diff_encode(x: npt.ArrayLike, y_prev: int = 0) -> np.ndarray:
+def diff_encode(x: npt.ArrayLike, y_prev: int = 0) -> npt.NDArray[np.int_]:
     """
     Differentially encodes the input data $x[k]$.
 
     Args:
         x: The input uncoded data $x[k]$.
         y_prev: The previous value of the output encoded data $y[k-1]$.
 
@@ -61,15 +61,15 @@
     for n in range(1, len(x)):
         y[n] = x[n] ^ y[n - 1]
 
     return y
 
 
 @export
-def diff_decode(y: npt.ArrayLike, y_prev: int = 0) -> np.ndarray:
+def diff_decode(y: npt.ArrayLike, y_prev: int = 0) -> npt.NDArray[np.int_]:
     """
     Differentially decodes the input data $y[k]$.
 
     Arguments:
         y: The input encoded data $y[k]$.
         y_prev: The previous value of the encoded data $y[k-1]$.
```

### Comparing `sdr-0.0.8/src/sdr/_modulation/_symbol_mapping.py` & `sdr-0.0.9/src/sdr/_modulation/_symbol_mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 A module containing functions for various symbol mapping schemes.
 """
 from __future__ import annotations
 
 import numpy as np
+import numpy.typing as npt
 
 from .._helper import export
 
 
 @export
-def binary_code(n: int) -> np.ndarray:
+def binary_code(n: int) -> npt.NDArray[np.int_]:
     """
     Generates a binary code of length $2^n$.
 
     Arguments:
         n: The length of the binary code.
 
     Returns:
@@ -33,15 +34,15 @@
     if not n >= 1:
         raise ValueError(f"Argument 'n' must be greater than or equal to 1, not {n}.")
 
     return np.arange(2**n)
 
 
 @export
-def gray_code(n: int) -> np.ndarray:
+def gray_code(n: int) -> npt.NDArray[np.int_]:
     """
     Generates a Gray code of length $2^n$.
 
     Arguments:
         n: The length of the Gray code.
 
     Returns:
```

### Comparing `sdr-0.0.8/src/sdr/_pll.py` & `sdr-0.0.9/src/sdr/_synchronization/_pll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 A module for closed-loop phase-locked loops (PLLs) analysis.
 """
 from __future__ import annotations
 
 import numpy as np
 
-from ._conversion import linear
-from ._filter import IIR
-from ._helper import export
+from .._conversion import linear
+from .._filter import IIR
+from .._helper import export
 from ._loop_filter import LoopFilter
 
 
 @export
 class ClosedLoopPLL:
     r"""
     A class that defines the performance of a closed-loop PLL.
@@ -19,26 +19,28 @@
     Note:
         This class is meant for performance analysis only.
 
     Notes:
         .. code-block:: text
             :caption: Closed-Loop PLL Block Diagram
 
-                         bb[n]
+                        bb[n]    phase_err[n]
                     +---+    +-----+    +----+
             x[n] -->| X |--->| PED |--->| LF |---+
                     +---+    +-----+    +----+   |
-                      ^                          |
-                      |  +---------+   +-----+   |
-               lo[n]  +--| e^(-j.) |<--| NCO |<--+
-                         +---------+   +-----+
+                      ^                          | phase_est[n]
+                      |      +-----+             |
+               lo[n]  +------| NCO |<------------+
+                             +-----+
 
             x[n] = Input signal
-            lo[n] = Local oscillator signal
             bb[n] = Baseband signal
+            phase_err[n] = Phase error signal
+            phase_est[n] = Phase estimate signal
+            lo[n] = Local oscillator signal
             PED = Phase error detector
             LF = Loop filter
             NCO = Numerically-controlled oscillator
 
         The transfer function of the 2nd order, proportional-plus-integrator loop filter is
 
         $$H_{LF}(z) = K_1 + K_2 \frac{ 1 }{ 1 - z^{-1}} = \frac{(K_1 + K_2) - K_1 z^{-1}}{1 - z^{-1}} .$$
```

### Comparing `sdr-0.0.8/src/sdr/_probability.py` & `sdr-0.0.9/src/sdr/_probability.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy.typing as npt
 import scipy.special
 
 from ._helper import export
 
 
 @export
-def Q(x: npt.ArrayLike) -> np.ndarray:
+def Q(x: npt.ArrayLike) -> npt.NDArray[np.float_]:
     r"""
     Computes the complementary cumulative distribution function $Q(x)$
     of the standard normal distribution $\mathcal{N}(0, 1)$.
 
     Arguments:
         x: The real-valued input $x$.
 
@@ -31,20 +31,20 @@
             sdr.Q(1)
             sdr.Qinv(0.158655)
 
     Group:
         probability
     """
     x = np.asarray(x)
-    p = scipy.special.erfc(x / np.sqrt(2)) / 2  # pylint: disable=no-member
+    p = scipy.special.erfc(x / np.sqrt(2)) / 2
     return p
 
 
 @export
-def Qinv(p: npt.ArrayLike) -> np.ndarray:
+def Qinv(p: npt.ArrayLike) -> npt.NDArray[np.float_]:
     r"""
     Computes the inverse complementary cumulative distribution function $Q^{-1}(p)$
     of the standard normal distribution $\mathcal{N}(0, 1)$.
 
     Arguments:
         p: The probability $p$ of exceeding the returned value $x$.
 
@@ -60,9 +60,9 @@
             sdr.Qinv(0.158655)
             sdr.Q(1)
 
     Group:
         probability
     """
     p = np.asarray(p)
-    x = np.sqrt(2) * scipy.special.erfcinv(2 * p)  # pylint: disable=no-member
+    x = np.sqrt(2) * scipy.special.erfcinv(2 * p)
     return x
```

### Comparing `sdr-0.0.8/src/sdr/_sequence.py` & `sdr-0.0.9/src/sdr/_sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 """
 A module containing various bipolar and binary sequences.
 """
 from __future__ import annotations
 
 import math
+from typing import Any, overload
 
 import numpy as np
+import numpy.typing as npt
 from typing_extensions import Literal
 
 from ._helper import export
 
 
+@overload
+def barker(length: int, output: Literal["binary"]) -> npt.NDArray[np.int_]:
+    ...
+
+
+@overload
+def barker(length: int, output: Literal["bipolar"] = "bipolar") -> npt.NDArray[np.float_]:
+    ...
+
+
 @export
-def barker(length: int, output: Literal["binary", "bipolar"] = "bipolar") -> np.ndarray:
+def barker(length: Any, output: Any = "bipolar") -> Any:
     r"""
     Returns the Barker code/sequence of length $N$.
 
     Arguments:
         length: The length $N$ of the Barker code/sequence.
         output: The output format of the Barker code/sequence.
 
@@ -81,15 +93,15 @@
     sequence = 1 - 2 * code
     sequence = sequence.astype(float)
 
     return sequence
 
 
 @export
-def zadoff_chu(length: int, root: int, shift: int = 0) -> np.ndarray:
+def zadoff_chu(length: int, root: int, shift: int = 0) -> npt.NDArray[np.complex_]:
     r"""
     Returns the root-$u$ Zadoff-Chu sequence of length $N$.
 
     Arguments:
         length: The length $N$ of the Zadoff-Chu sequence.
         root: The root $0 < u < N$ of the Zadoff-Chu sequence. The root must be relatively prime to the length,
             i.e., $\gcd(u, N) = 1$.
```

### Comparing `sdr-0.0.8/src/sdr/_signal.py` & `sdr-0.0.9/src/sdr/_signal.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import scipy.signal
 
 from ._helper import export
 
 
 @export
 def mix(
-    x: npt.ArrayLike,
+    x: npt.NDArray,
     freq: float = 0,
     phase: float = 0,
     sample_rate: float = 1,
-    complex: bool = True,  # pylint: disable=redefined-builtin
-) -> np.ndarray:
+    complex: bool = True,
+) -> npt.NDArray:
     r"""
     Mixes the time-domain signal $x[n]$ with a complex exponential or real sinusoid.
 
     Arguments:
         x: The time-domain signal $x[n]$.
         freq: The frequency $f$ of the sinusoid in Hz (or 1/samples if `sample_rate=1`).
             The frequency must satisfy $-f_s/2 \le f \le f_s/2$.
@@ -61,16 +61,14 @@
             sdr.plot.time_domain(y, sample_rate=sample_rate); \
             plt.title(r"Baseband signal with $f=0$ Hz and $\phi=0$ degrees"); \
             plt.tight_layout();
 
     Group:
         dsp-signal-manipulation
     """
-    x = np.asarray(x)
-
     if not isinstance(freq, (int, float)):
         raise TypeError(f"Argument 'freq' must be a number, not {type(freq)}.")
     if not isinstance(phase, (int, float)):
         raise TypeError(f"Argument 'phase' must be a number, not {type(phase)}.")
     if not isinstance(sample_rate, (int, float)):
         raise TypeError(f"Argument 'sample_rate' must be a number, not {type(sample_rate)}.")
     if not isinstance(complex, bool):
@@ -89,15 +87,15 @@
 
     y = x * lo
 
     return y
 
 
 @export
-def to_complex_bb(x_r: npt.ArrayLike) -> np.ndarray:
+def to_complex_bb(x_r: npt.NDArray[np.float_]) -> npt.NDArray[np.complex_]:
     r"""
     Converts the real passband signal $x_r[n]$ centered at $f_{s,r}/4$ with sample rate $f_{s,r}$ to a
     complex baseband signal $x_c[n]$ centered at $0$ with sample rate $f_{s,c} = f_{s,r}/2$.
 
     Arguments:
         x_r: The real passband signal $x_r[n]$ centered at $f_{s,r}/4$ with sample rate $f_{s,r}$.
             If the length is odd, one zero is appended to the end.
@@ -151,16 +149,14 @@
             sdr.plot.periodogram(x_c, fft=2048, sample_rate=sample_rate); \
             plt.title("Periodogram of $x_c[n]$"); \
             plt.tight_layout();
 
     Group:
         dsp-signal-manipulation
     """
-    x_r = np.asarray(x_r)
-
     if not x_r.ndim == 1:
         raise ValueError(f"Argument 'x_r' must be a 1D array, not {x_r.ndim}D.")
     if not np.isrealobj(x_r):
         raise ValueError("Argument 'x_r' must be real, not complex.")
 
     if x_r.size % 2 == 1:
         # Append one zero for the decimate by 2
@@ -176,15 +172,15 @@
     # spectrum outside +/- fs/4 is zero.
     x_c = x_c[::2]
 
     return x_c
 
 
 @export
-def to_real_pb(x_c: npt.ArrayLike) -> np.ndarray:
+def to_real_pb(x_c: npt.NDArray[np.complex_]) -> npt.NDArray[np.float_]:
     r"""
     Converts the complex baseband signal $x_c[n]$ centered at $0$ with sample rate $f_{s,c}$ to a
     real passband signal $x_r[n]$ centered at $f_{s,r}/4$ with sample rate $f_{s,r} = 2f_{s,c}$.
 
     Arguments:
         x_c: The complex baseband signal $x_c[n]$ centered at $0$ with sample rate $f_{s,c}$.
 
@@ -237,16 +233,14 @@
             sdr.plot.periodogram(x_r, fft=2048, sample_rate=sample_rate); \
             plt.title("Periodogram of $x_r[n]$"); \
             plt.tight_layout();
 
     Group:
         dsp-signal-manipulation
     """
-    x_c = np.asarray(x_c)
-
     if not x_c.ndim == 1:
         raise ValueError(f"Argument 'x_c' must be a 1D array, not {x_c.ndim}D.")
     if not np.iscomplexobj(x_c):
         raise ValueError("Argument 'x_c' must be complex, not real.")
 
     # Upsample by 2 to achieve 2*fs sample rate
     x_c = scipy.signal.resample_poly(x_c, 2, 1)
@@ -257,15 +251,15 @@
     # Only preserve the real part, which is complex-conjugate symmetric about 0 Hz.
     x_r = x_c.real
 
     return x_r
 
 
 @export
-def upsample(x: npt.ArrayLike, rate: int) -> np.ndarray:
+def upsample(x: npt.NDArray, rate: int) -> npt.NDArray:
     r"""
     Upsamples the time-domain signal $x[n]$ by the factor $r$.
 
     Warning:
         This function does not perform any anti-aliasing filtering. The upsampled signal $y[n]$ will have
         frequency components above the Nyquist frequency of the original signal $x[n]$. For efficient
         polyphase interpolation (with anti-aliasing filtering), see :class:`sdr.Interpolator`.
@@ -318,29 +312,27 @@
             plt.xlim(-sample_rate*2, sample_rate*2); \
             plt.title("Upsampled signal $y[n]$"); \
             plt.tight_layout();
 
     Group:
         dsp-signal-manipulation
     """
-    x = np.asarray(x)
-
     if not isinstance(rate, int):
         raise TypeError(f"Argument 'rate' must be an int, not {type(rate)}.")
     if not rate > 0:
         raise ValueError(f"Argument 'rate' must be positive, not {rate}.")
 
     y = np.zeros(x.size * rate, dtype=x.dtype)
     y[::rate] = x
 
     return y
 
 
 @export
-def downsample(x: npt.ArrayLike, rate: int) -> np.ndarray:
+def downsample(x: npt.NDArray, rate: int) -> npt.NDArray:
     r"""
     Downsamples the time-domain signal $x[n]$ by the factor $r$.
 
     Warning:
         This function does not perform any anti-aliasing filtering. The downsampled signal $y[n]$ will have
         spectral aliasing. For efficient polyphase decimation (with anti-aliasing filtering), see
         :class:`sdr.Decimator`.
@@ -395,16 +387,14 @@
             plt.xlim(-sample_rate/2, sample_rate/2); \
             plt.title("Downsampled signal $y[n]$"); \
             plt.tight_layout();
 
     Group:
         dsp-signal-manipulation
     """
-    x = np.asarray(x)
-
     if not isinstance(rate, int):
         raise TypeError(f"Argument 'rate' must be an int, not {type(rate)}.")
     if not rate > 0:
         raise ValueError(f"Argument 'rate' must be positive, not {rate}.")
 
     y = x[::rate]
```

### Comparing `sdr-0.0.8/src/sdr/_simulation/_channel_model.py` & `sdr-0.0.9/src/sdr/_simulation/_channel_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,27 @@
 import numpy as np
 import numpy.typing as npt
 
 from .._helper import export
 
 
 @export
-def bsc(x: npt.ArrayLike, p: float) -> np.ndarray:
+def bsc(
+    x: npt.ArrayLike,
+    p: float,
+    seed: int | None = None,
+) -> npt.NDArray[np.int_]:
     r"""
     Passes the binary input sequence $x$ through a binary symmetric channel (BSC)
     with transition probability $p$.
 
     Arguments:
         x: The input sequence $x$ with $x_i \in \{0, 1\}$.
         p: The probability $p$ of a bit flip.
+        seed: The seed for the random number generator. This is passed to :func:`numpy.random.default_rng()`.
 
     Returns:
         The output sequence $y$ with $y_i \in \{0, 1\}$.
 
     Examples:
         When 20 bits are passed through a BSC with transition probability $p=0.25$,
         roughly 5 bits are flipped at the output.
@@ -35,29 +40,35 @@
     Group:
         simulation-channel-models
     """
     if not 0 <= p <= 1:
         raise ValueError(f"Argument 'p' must be between 0 and 1, not {p}.")
 
     x = np.asarray(x)
-    flip = np.random.choice([0, 1], size=x.shape, p=[1 - p, p])
+    rng = np.random.default_rng(seed)
+    flip = rng.choice([0, 1], size=x.shape, p=[1 - p, p])
     y = x ^ flip
 
     return y if y.ndim > 0 else y.item()
 
 
 @export
-def bec(x: npt.ArrayLike, p: float) -> np.ndarray:
+def bec(
+    x: npt.ArrayLike,
+    p: float,
+    seed: int | None = None,
+) -> npt.NDArray[np.int_]:
     r"""
     Passes the binary input sequence $x$ through a binary erasure channel (BEC)
     with erasure probability $p$.
 
     Arguments:
         x: The input sequence $x$ with $x_i \in \{0, 1\}$.
         p: The probability $p$ of a bit erasure.
+        seed: The seed for the random number generator. This is passed to :func:`numpy.random.default_rng()`.
 
     Returns:
         The output sequence $y$ with $y_i \in \{0, 1, e\}$. Erasures $e$ are represented by -1.
 
     Examples:
         When 20 bits are passed through a BEC with erasure probability $p=0.25$,
         roughly 5 bits are erased at the output.
@@ -71,34 +82,41 @@
     Group:
         simulation-channel-models
     """
     if not 0 <= p <= 1:
         raise ValueError(f"Argument 'p' must be between 0 and 1, not {p}.")
 
     x = np.asarray(x)
-    y = np.where(np.random.rand(*x.shape) < p, -1, x)
+    rng = np.random.default_rng(seed)
+    random_p = rng.random(x.shape)
+    y = np.where(random_p < p, -1, x)
 
     return y if y.ndim > 0 else y.item()
 
 
 @export
 def dmc(
-    x: npt.ArrayLike, P: npt.ArrayLike, X: npt.ArrayLike | None = None, Y: npt.ArrayLike | None = None
-) -> np.ndarray:
+    x: npt.ArrayLike,
+    P: npt.ArrayLike,
+    X: npt.ArrayLike | None = None,
+    Y: npt.ArrayLike | None = None,
+    seed: int | None = None,
+) -> npt.NDArray[np.int_]:
     r"""
     Passes the input sequence $x$ through a discrete memoryless channel (DMC) with transition
     probability matrix $P$.
 
     Arguments:
         x: The input sequence $x$ with $x_i \in \mathcal{X}$.
         P: The $m \times n$ transition probability matrix $P$, where $P_{i,j} = \Pr(Y = y_j | X = x_i)$.
         X: The input alphabet $\mathcal{X}$ of size $m$. If `None`, it is assumed that
             $\mathcal{X} = \{0, 1, \ldots, m-1\}$.
         Y: The output alphabet $\mathcal{Y}$ of size $n$. If `None`, it is assumed that
             $\mathcal{Y} = \{0, 1, \ldots, n-1\}$.
+        seed: The seed for the random number generator. This is passed to :func:`numpy.random.default_rng()`.
 
     Returns:
         The output sequence $y$ with $y_i \in \mathcal{Y}$.
 
     Examples:
         Define the binary symmetric channel (BSC) with transition probability $p=0.25$.
 
@@ -143,12 +161,13 @@
     Y = np.asarray(Y) if Y is not None else np.arange(P.shape[1])
     if not Y.ndim == 1:
         raise ValueError(f"Argument 'Y' must be a 1D array, not {Y.ndim}D.")
     if not P.shape[1] == Y.shape[0]:
         raise ValueError(f"Argument 'P' must have {Y.shape[0]} columns, not {P.shape[1]}.")
 
     y = np.zeros_like(x)
+    rng = np.random.default_rng(seed)
     for i, Xi in enumerate(X):
         idxs = np.where(x == Xi)[0]
-        y[idxs] = np.random.choice(Y, size=idxs.shape, p=P[i])
+        y[idxs] = rng.choice(Y, size=idxs.shape, p=P[i])
 
     return y if y.ndim > 0 else y.item()
```

### Comparing `sdr-0.0.8/src/sdr/_simulation/_impairment.py` & `sdr-0.0.9/src/sdr/_simulation/_impairment.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from .._farrow import FarrowResampler
 from .._helper import export
 from .._measurement import average_power
 
 
 @export
 def awgn(
-    x: npt.ArrayLike,
+    x: npt.NDArray,
     snr: float | None = None,
     noise: float | None = None,
     seed: int | None = None,
-) -> np.ndarray:
+) -> npt.NDArray:
     r"""
     Adds additive white Gaussian noise (AWGN) to the time-domain signal $x[n]$.
 
     Arguments:
         x: The time-domain signal $x[n]$ to which AWGN is added.
         snr: The desired signal-to-noise ratio (SNR) in dB. If specified, the average signal power is measured
             explicitly. It is assumed that $x[n]$ contains signal only. If the signal power is known, the
@@ -81,15 +81,14 @@
             sdr.plot.constellation(y, label="$y[n]$", zorder=1); \
             plt.title(f"QPSK constellations for $x[n]$ with $\infty$ dB $E_s/N_0$\nand $y[n]$ with 10 dB $E_s/N_0$"); \
             plt.tight_layout()
 
     Group:
         simulation-impairments
     """
-    x = np.asarray(x)
     if snr is not None:
         snr_linear = linear(snr)
         signal_power = average_power(x)
         noise_power = signal_power / snr_linear
     elif noise is not None:
         noise_power = noise
     else:
@@ -101,15 +100,15 @@
     else:
         w = rng.normal(0, np.sqrt(noise_power), x.shape)
 
     return x + w
 
 
 @export
-def iq_imbalance(x: npt.ArrayLike, amplitude: float, phase: float = 0) -> np.ndarray:
+def iq_imbalance(x: npt.NDArray, amplitude: float, phase: float = 0) -> npt.NDArray:
     r"""
     Applies IQ imbalance to the complex time-domain signal $x[n]$.
 
     Arguments:
         x: The complex time-domain signal $x[n]$ to which IQ imbalance is applied.
         amplitude: The amplitude imbalance $A$ in dB. A positive value indicates that the in-phase component is
             larger than the quadrature component.
@@ -171,15 +170,14 @@
             sdr.plot.constellation(y2, label="$y_2[n]$"); \
             plt.legend(); \
             plt.title("-20 deg phase imbalance");
 
     Group:
         simulation-impairments
     """
-    x = np.asarray(x)
     if not np.iscomplexobj(x):
         raise ValueError("Argument 'x' must be complex.")
 
     phase = np.deg2rad(phase)
 
     # TODO: Should the phase be negative for I?
     gain_i = linear(0.5 * amplitude, type="voltage") * np.exp(1j * -0.5 * phase)
@@ -187,15 +185,15 @@
 
     y = gain_i * x.real + 1j * gain_q * x.imag
 
     return y
 
 
 @export
-def sample_rate_offset(x: npt.ArrayLike, ppm: float) -> np.ndarray:
+def sample_rate_offset(x: npt.NDArray, ppm: float) -> npt.NDArray:
     r"""
     Applies a sample rate offset to the time-domain signal $x[n]$.
 
     Arguments:
         x: The time-domain signal $x[n]$ to which the sample rate offset is applied.
         ppm: The sample rate offset $f_{s,\text{new}} / f_s$ in parts per million (ppm).
 
@@ -238,15 +236,14 @@
             sdr.plot.constellation(y, label="$y[n]$", zorder=1); \
             plt.title(f"{ppm} ppm sample rate offset"); \
             plt.tight_layout()
 
     Group:
         simulation-impairments
     """
-    x = np.asarray(x)
     if not x.ndim == 1:
         raise ValueError(f"Argument 'x' must be 1D, not {x.ndim}D.")
 
     rate = 1 + ppm * 1e-6
 
     # TODO: Add ppm_rate
     # if ppm_rate:
@@ -256,20 +253,20 @@
     y = farrow(x, rate)
 
     return y
 
 
 @export
 def frequency_offset(
-    x: npt.ArrayLike,
+    x: npt.NDArray,
     freq: npt.ArrayLike,
     freq_rate: npt.ArrayLike = 0,
     phase: npt.ArrayLike = 0,
     sample_rate: float = 1,
-) -> np.ndarray:
+) -> npt.NDArray:
     r"""
     Applies a frequency and phase offset to the time-domain signal $x[n]$.
 
     Arguments:
         x: The time-domain signal $x[n]$ to which the frequency offset is applied.
         freq: The frequency offset $f$ in Hz (or in cycles/sample if `sample_rate=1`).
         freq_rate: The frequency offset rate $f_{\text{rate}}$ in Hz/s (or in cycles/sample^2 if `sample_rate=1`).
@@ -316,15 +313,14 @@
             sdr.plot.constellation(y, label="$y[n]$", zorder=1); \
             plt.title(f"{freq} cycles/sample frequency and {phase} deg offset"); \
             plt.tight_layout()
 
     Group:
         simulation-impairments
     """
-    x = np.asarray(x)
     if not x.ndim == 1:
         raise ValueError(f"Argument 'x' must be 1D, not {x.ndim}D.")
 
     freq = np.asarray(freq)
     if not (freq.ndim == 0 or freq.shape == x.shape):
         raise ValueError(f"Argument 'freq' must be scalar or have shape {x.shape}, not {freq.shape}.")
```

### Comparing `sdr-0.0.8/src/sdr/plot/_detection.py` & `sdr-0.0.9/src/sdr/plot/_detection.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from .._helper import export
 from ._rc_params import RC_PARAMS
 
 
 @export
 def roc(
     p_fa: npt.ArrayLike,
-    p_d: npt.ArrayLike,  # pylint: disable=redefined-outer-name
-    type: Literal["linear", "semilogx", "semilogy", "loglog"] = "semilogx",  # pylint: disable=redefined-builtin
+    p_d: npt.ArrayLike,
+    type: Literal["linear", "semilogx", "semilogy", "loglog"] = "semilogx",
     **kwargs,
 ):
     r"""
     Plots the receiver operating characteristic (ROC) curve as a function of $P_{FA}$.
 
     Arguments:
         p_fa: The probability of false alarm $P_{FA}$.
@@ -57,15 +57,15 @@
         plt.title("Receiver operating characteristic (ROC) curve")
         plt.tight_layout()
 
 
 @export
 def p_d(
     x: npt.ArrayLike,
-    p_d: npt.ArrayLike,  # pylint: disable=redefined-outer-name
+    p_d: npt.ArrayLike,
     x_label: Literal["snr", "enr"] = "snr",
     **kwargs,
 ):
     r"""
     Plots the probability of detection $P_D$ as a function of received SNR or ENR.
 
     Arguments:
```

### Comparing `sdr-0.0.8/src/sdr/plot/_filter.py` & `sdr-0.0.9/src/sdr/plot/_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 from typing_extensions import Literal
 
 from .._filter import FIR, IIR
 from .._helper import export
 from ._rc_params import RC_PARAMS
 from ._units import freq_units, time_units
 
-# pylint: disable=redefined-builtin,redefined-outer-name
-
 
 def _convert_to_taps(
     filter: FIR | IIR | npt.ArrayLike | tuple[npt.ArrayLike, npt.ArrayLike]
-) -> tuple[np.ndarray, np.ndarray]:
+) -> tuple[npt.NDArray, npt.NDArray]:
     if isinstance(filter, FIR):
         b = filter.taps
         a = np.array([1])
     elif isinstance(filter, IIR):
         b = filter.b_taps
         a = filter.a_taps
     elif isinstance(filter, tuple):
```

### Comparing `sdr-0.0.8/src/sdr/plot/_modulation.py` & `sdr-0.0.9/src/sdr/plot/_modulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .._modulation import LinearModulation, PiMPSK
 from ._rc_params import RC_PARAMS
 from ._time_domain import raster
 
 
 @export
 def constellation(
-    x_hat: npt.ArrayLike,
+    x_hat: npt.NDArray[np.complex_],
     heatmap: bool = False,
     limits: tuple[float, float] | None = None,
     **kwargs,
 ):
     r"""
     Plots the constellation of the complex symbols $\hat{x}[k]$.
 
@@ -62,16 +62,14 @@
             @savefig sdr_plot_constellation_2.png
             plt.figure(figsize=(8, 4)); \
             sdr.plot.constellation(x_hat, heatmap=True);
 
     Group:
         plot-modulation
     """
-    x_hat = np.asarray(x_hat)
-
     # Set the axis limits to 10% larger than the maximum value
     if limits is None:
         lim = np.max(np.abs(x_hat)) * 1.1
         limits = (-lim, lim)
 
     with plt.rc_context(RC_PARAMS):
         if heatmap:
@@ -99,15 +97,15 @@
         plt.ylabel("Quadrature channel, $Q$")
         plt.title("Constellation")
         plt.tight_layout()
 
 
 @export
 def symbol_map(
-    modulation: LinearModulation | npt.ArrayLike,
+    modulation: LinearModulation | npt.NDArray[np.complex_],
     annotate: bool | Literal["bin"] = True,
     limits: tuple[float, float] | None = None,
     **kwargs,
 ):
     r"""
     Plots the symbol map of the complex symbols $\hat{x}[k]$.
 
@@ -199,15 +197,15 @@
         plt.ylabel("Quadrature channel, $Q$")
         plt.title("Symbol Map")
         plt.tight_layout()
 
 
 @export
 def eye(
-    x: npt.ArrayLike,
+    x: npt.NDArray,
     sps: int,
     span: int = 2,
     sample_rate: float | None = None,
     color: Literal["index"] | str = "index",
     **kwargs,
 ):
     r"""
@@ -273,15 +271,15 @@
     ymin, ymax = ax.get_ylim()
     ylim = max(np.abs(ymin), np.abs(ymax))
     ax.set_ylim(-ylim, ylim)
 
 
 @export
 def phase_tree(
-    x: npt.ArrayLike,
+    x: npt.NDArray,
     sps: int,
     span: int = 4,
     sample_rate: float | None = None,
     color: Literal["index"] | str = "index",
     **kwargs,
 ):
     r"""
@@ -340,16 +338,16 @@
     ax.set_yticks(np.arange(-ylim, ylim + 1, 180))
 
     ax.set_ylabel("Phase (deg)")
 
 
 @export
 def ber(
-    ebn0: npt.ArrayLike,
-    ber: npt.ArrayLike,  # pylint: disable=redefined-outer-name
+    ebn0: npt.NDArray[np.float_],
+    ber: npt.NDArray[np.float_],
     **kwargs,
 ):
     r"""
     Plots the bit error rate (BER) as a function of $E_b/N_0$.
 
     Arguments:
         ebn0: The bit energy $E_b$ to noise PSD $N_0$ ratio (dB).
@@ -392,16 +390,16 @@
         plt.ylabel("Probability of bit error, $P_{be}$")
         plt.title("Bit error rate curve")
         plt.tight_layout()
 
 
 @export
 def ser(
-    esn0: npt.ArrayLike,
-    ser: npt.ArrayLike,  # pylint: disable=redefined-outer-name
+    esn0: npt.NDArray[np.float_],
+    ser: npt.NDArray[np.float_],
     **kwargs,
 ):
     r"""
     Plots the symbol error rate (SER) as a function of $E_s/N_0$.
 
     Arguments:
         esn0: The symbol energy $E_s$ to noise PSD $N_0$ ratio (dB).
```

### Comparing `sdr-0.0.8/src/sdr/plot/_rc_params.py` & `sdr-0.0.9/src/sdr/plot/_rc_params.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/src/sdr/plot/_spectral_estimation.py` & `sdr-0.0.9/src/sdr/plot/_spectral_estimation.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/src/sdr/plot/_time_domain.py` & `sdr-0.0.9/src/sdr/plot/_time_domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .._helper import export
 from ._rc_params import RC_PARAMS
 from ._units import time_units
 
 
 @export
 def time_domain(
-    x: npt.ArrayLike,
+    x: npt.NDArray,
     sample_rate: float | None = None,
     centered: bool = False,
     offset: float = 0,
     diff: Literal["color", "line"] = "color",
     **kwargs,
 ):
     r"""
@@ -74,15 +74,14 @@
             sdr.plot.time_domain(y, sample_rate=10e3); \
             plt.title("SRRC pulse-shaped QPSK"); \
             plt.tight_layout()
 
     Group:
         plot-time-domain
     """
-    x = np.asarray(x)
     if not x.ndim == 1:
         raise ValueError(f"Argument 'x' must be 1-D, not {x.ndim}-D.")
 
     if sample_rate is None:
         sample_rate_provided = False
         sample_rate = 1
     else:
@@ -131,15 +130,15 @@
             plt.xlabel("Samples")
         plt.ylabel("Amplitude")
         plt.tight_layout()
 
 
 @export
 def raster(
-    x: npt.ArrayLike,
+    x: npt.NDArray,
     length: int | None = None,
     stride: int | None = None,
     sample_rate: float | None = None,
     color: Literal["index"] | str = "index",
     colorbar: bool = True,
     **kwargs,
 ):
@@ -163,16 +162,14 @@
             - `"linewidths"`: 1
             - `"linestyles"`: `"solid"`
             - `"cmap"`: `"rainbow"`
 
     Group:
         plot-time-domain
     """
-    # pylint: disable=too-many-statements
-    x = np.asarray(x)
     if not x.ndim in [1, 2]:
         raise ValueError(f"Argument 'x' must be 1-D or 2-D, not {x.ndim}-D.")
 
     if x.ndim == 1:
         if not length is not None:
             raise ValueError("Argument 'length' must be specified if 'x' is 1-D.")
         if not isinstance(length, int):
```

### Comparing `sdr-0.0.8/src/sdr/plot/_units.py` & `sdr-0.0.9/src/sdr/plot/_units.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 """
 from __future__ import annotations
 
 import numpy as np
 import numpy.typing as npt
 
 
-def time_units(time: npt.ArrayLike) -> tuple[str, float]:
+def time_units(time: npt.NDArray[np.float_]) -> tuple[str, float]:
     """
     Determines the appropriate time units to use for a given time array.
     """
-    time = np.asarray(time)
     max_time = np.nanmax(np.abs(time))
 
     if max_time > 1:
         scalar = 1
         units = "s"
     elif max_time > 1e-3:
         scalar = 1e3
@@ -32,19 +31,18 @@
     else:
         scalar = 1e15
         units = "fs"
 
     return units, scalar
 
 
-def freq_units(freq: npt.ArrayLike) -> tuple[str, float]:
+def freq_units(freq: npt.NDArray[np.float_]) -> tuple[str, float]:
     """
     Determines the appropriate frequency units to use for a given frequency array.
     """
-    freq = np.asarray(freq)
     max_freq = np.nanmax(np.abs(freq))
 
     if max_freq > 10e12:
         scalar = 1e-12
         units = "THz"
     elif max_freq > 10e9:
         scalar = 1e-9
```

### Comparing `sdr-0.0.8/src/sdr.egg-info/PKG-INFO` & `sdr-0.0.9/src/sdr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdr
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for software-defined radio
 Author-email: Matt Hostetter <matthostetter@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mhostetter/sdr
 Project-URL: Source, https://github.com/mhostetter/sdr
 Project-URL: Issues, https://github.com/mhostetter/sdr/issues
 Project-URL: Documentation, https://mhostetter.github.io/sdr/latest/
@@ -57,15 +57,15 @@
 The `sdr` library is a Python 3 package for software-defined radio (SDR).
 
 The goal of `sdr` is to provide tools to design, analyze, build, and test digital communication systems
 in Python. The library relies on and is designed to be interoperable with NumPy, SciPy, and Matplotlib.
 Performance is also very important. So, where possible, Numba is used to accelerate computationally-intensive
 functions.
 
-Additionally, the library aims to replicate relevant functionality from Matlab's Communications and
+Additionally, the library aims to replicate relevant functionality from MATLAB's Communications and
 DSP Toolboxes.
 
 We are progressively adding functionality to the library. If there is something you'd like to see included
 in `sdr`, please open an issue on GitHub.
 
 > Enjoying the library? Give us a :star: on [GitHub](https://github.com/mhostetter/sdr)!
 
@@ -83,27 +83,26 @@
 
 ## Features
 
 View all available classes and functions in the [API Reference](https://mhostetter.github.io/sdr/latest/api/dsp/).
 
 - **Digital signal processing**: Finite impulse response (FIR) filters, infinite impulse response (IIR) filters,
   polyphase interpolator, polyphase decimator, polyphase resampler, Farrow arbitrary resampler,
-  complex mixing, real/complex conversion.
+  FIR differentiator, IIR integrator, complex mixing, real/complex conversion.
 - **Sequences**: Barker, Zadoff-Chu.
 - **Modulation**: Phase-shift keying (PSK), $\pi/M$ PSK, offset QPSK, rectangular pulse shape, half-sine pulse shape,
   raised cosine pulse shape, root raised cosine pulse shape, Gaussian pulse shape, binary and Gray symbol mapping,
   differential encoding.
-- **Synchronization**: Numerically-controlled oscillators (NCO), direct digital synthesizers (DDS), loop filters,
-  closed-loop PLL analysis.
+- **Synchronization**: Numerically-controlled oscillators (NCO), loop filters, closed-loop PLL analysis.
 - **Measurement**: Energy, power, voltage, bit/symbol error rate, error vector magnitude (EVM).
 - **Conversions**: Between linear units and decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$.
 - **Simulation**: Binary symmetric channel (BSC), binary erasure channel (BEC), discrete memoryless channel (DMC),
   additive white Gaussian noise (AWGN), frequency offset, sample rate offset, IQ imbalance.
 - **Link budgets**: Channel capacities, free-space path loss, antenna gains.
-- **Data manipulation**: Packing and unpacking binary data, hexdumping binary data.
+- **Data manipulation**: Packing and unpacking binary data, hexdump of binary data.
 - **Plotting**: Time-domain, raster, periodogram, spectrogram, constellation, symbol map, eye diagram,
   bit error rate (BER), symbol error rate (SER), impulse response, step response, magnitude response, phase response,
   phase delay, group delay, and zeros/poles.
 
 ## Examples
 
 There are detailed examples published at <https://mhostetter.github.io/sdr/latest/examples/pulse-shapes/>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdr Version: 0.0.8 Summary: A Python package for
+Metadata-Version: 2.1 Name: sdr Version: 0.0.9 Summary: A Python package for
 software-defined radio Author-email: Matt Hostetter
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/mhostetter/
 sdr Project-URL: Source, https://github.com/mhostetter/sdr Project-URL: Issues,
 https://github.com/mhostetter/sdr/issues Project-URL: Documentation, https://
 mhostetter.github.io/sdr/latest/ Project-URL: Discuss, https://github.com/
 mhostetter/sdr/discussions Project-URL: Twitter, https://twitter.com/sdr_py
 Keywords: software-defined radio,sdr,digital communications,wireless
@@ -35,39 +35,39 @@
                           _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_F_J_M_L_7_9_Z_U_K_]
 The `sdr` library is a Python 3 package for software-defined radio (SDR). The
 goal of `sdr` is to provide tools to design, analyze, build, and test digital
 communication systems in Python. The library relies on and is designed to be
 interoperable with NumPy, SciPy, and Matplotlib. Performance is also very
 important. So, where possible, Numba is used to accelerate computationally-
 intensive functions. Additionally, the library aims to replicate relevant
-functionality from Matlab's Communications and DSP Toolboxes. We are
+functionality from MATLAB's Communications and DSP Toolboxes. We are
 progressively adding functionality to the library. If there is something you'd
 like to see included in `sdr`, please open an issue on GitHub. > Enjoying the
 library? Give us a :star: on [GitHub](https://github.com/mhostetter/sdr)! ##
 Documentation The documentation for `sdr` is located at
 mhostetter.github.io/sdr/latest/>. ## Installation The latest version of `sdr`
 can be installed from [PyPI](https://pypi.org/project/sdr/) using `pip`.
 ```console python3 -m pip install sdr ``` ## Features View all available
 classes and functions in the [API Reference](https://mhostetter.github.io/sdr/
 latest/api/dsp/). - **Digital signal processing**: Finite impulse response
 (FIR) filters, infinite impulse response (IIR) filters, polyphase interpolator,
-polyphase decimator, polyphase resampler, Farrow arbitrary resampler, complex
-mixing, real/complex conversion. - **Sequences**: Barker, Zadoff-Chu. -
-**Modulation**: Phase-shift keying (PSK), $\pi/M$ PSK, offset QPSK, rectangular
-pulse shape, half-sine pulse shape, raised cosine pulse shape, root raised
-cosine pulse shape, Gaussian pulse shape, binary and Gray symbol mapping,
-differential encoding. - **Synchronization**: Numerically-controlled
-oscillators (NCO), direct digital synthesizers (DDS), loop filters, closed-loop
-PLL analysis. - **Measurement**: Energy, power, voltage, bit/symbol error rate,
-error vector magnitude (EVM). - **Conversions**: Between linear units and
-decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$. - **Simulation**: Binary
-symmetric channel (BSC), binary erasure channel (BEC), discrete memoryless
-channel (DMC), additive white Gaussian noise (AWGN), frequency offset, sample
-rate offset, IQ imbalance. - **Link budgets**: Channel capacities, free-space
-path loss, antenna gains. - **Data manipulation**: Packing and unpacking binary
-data, hexdumping binary data. - **Plotting**: Time-domain, raster, periodogram,
-spectrogram, constellation, symbol map, eye diagram, bit error rate (BER),
-symbol error rate (SER), impulse response, step response, magnitude response,
-phase response, phase delay, group delay, and zeros/poles. ## Examples There
-are detailed examples published at
+polyphase decimator, polyphase resampler, Farrow arbitrary resampler, FIR
+differentiator, IIR integrator, complex mixing, real/complex conversion. -
+**Sequences**: Barker, Zadoff-Chu. - **Modulation**: Phase-shift keying (PSK),
+$\pi/M$ PSK, offset QPSK, rectangular pulse shape, half-sine pulse shape,
+raised cosine pulse shape, root raised cosine pulse shape, Gaussian pulse
+shape, binary and Gray symbol mapping, differential encoding. -
+**Synchronization**: Numerically-controlled oscillators (NCO), loop filters,
+closed-loop PLL analysis. - **Measurement**: Energy, power, voltage, bit/symbol
+error rate, error vector magnitude (EVM). - **Conversions**: Between linear
+units and decibels. Between $E_b/N_0$, $E_s/N_0$, and $S/N$. - **Simulation**:
+Binary symmetric channel (BSC), binary erasure channel (BEC), discrete
+memoryless channel (DMC), additive white Gaussian noise (AWGN), frequency
+offset, sample rate offset, IQ imbalance. - **Link budgets**: Channel
+capacities, free-space path loss, antenna gains. - **Data manipulation**:
+Packing and unpacking binary data, hexdump of binary data. - **Plotting**:
+Time-domain, raster, periodogram, spectrogram, constellation, symbol map, eye
+diagram, bit error rate (BER), symbol error rate (SER), impulse response, step
+response, magnitude response, phase response, phase delay, group delay, and
+zeros/poles. ## Examples There are detailed examples published at
 mhostetter.github.io/sdr/latest/examples/pulse-shapes/>. The Jupyter notebooks
 behind the examples are available for experimentation in `docs/examples/`.
```

### Comparing `sdr-0.0.8/src/sdr.egg-info/SOURCES.txt` & `sdr-0.0.9/src/sdr.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 requirements-dev.txt
 .github/workflows/build.yaml
 .github/workflows/docs.yaml
 .github/workflows/lint.yaml
@@ -26,16 +27,16 @@
 docs/api/modulation.rst
 docs/api/plotting.rst
 docs/api/probability.rst
 docs/api/sequences.rst
 docs/api/simulation.rst
 docs/api/synchronization.rst
 docs/development/documentation.rst
+docs/development/formatting.rst
 docs/development/installation.rst
-docs/development/linter.rst
 docs/development/unit-tests.rst
 docs/examples/farrow-resampler.ipynb
 docs/examples/fir-filters.ipynb
 docs/examples/iir-filters.ipynb
 docs/examples/peak-to-average-power.ipynb
 docs/examples/phase-locked-loop.ipynb
 docs/examples/psk.ipynb
@@ -43,17 +44,14 @@
 docs/release-notes/v0.0.md
 docs/release-notes/versioning.rst
 src/sdr/__init__.py
 src/sdr/_conversion.py
 src/sdr/_data.py
 src/sdr/_farrow.py
 src/sdr/_helper.py
-src/sdr/_loop_filter.py
-src/sdr/_nco.py
-src/sdr/_pll.py
 src/sdr/_probability.py
 src/sdr/_sequence.py
 src/sdr/_signal.py
 src/sdr/_version.py
 src/sdr.egg-info/PKG-INFO
 src/sdr.egg-info/SOURCES.txt
 src/sdr.egg-info/dependency_links.txt
@@ -83,75 +81,98 @@
 src/sdr/_modulation/_psk.py
 src/sdr/_modulation/_pulse_shapes.py
 src/sdr/_modulation/_symbol_encoding.py
 src/sdr/_modulation/_symbol_mapping.py
 src/sdr/_simulation/__init__.py
 src/sdr/_simulation/_channel_model.py
 src/sdr/_simulation/_impairment.py
+src/sdr/_synchronization/__init__.py
+src/sdr/_synchronization/_loop_filter.py
+src/sdr/_synchronization/_nco.py
+src/sdr/_synchronization/_pll.py
 src/sdr/plot/__init__.py
 src/sdr/plot/_detection.py
 src/sdr/plot/_filter.py
 src/sdr/plot/_modulation.py
 src/sdr/plot/_rc_params.py
 src/sdr/plot/_spectral_estimation.py
 src/sdr/plot/_time_domain.py
 src/sdr/plot/_units.py
+tests/conversions/__init__.py
 tests/conversions/test_ebn0_to_esn0.py
 tests/conversions/test_ebn0_to_snr.py
 tests/conversions/test_esn0_to_ebn0.py
 tests/conversions/test_esn0_to_snr.py
+tests/conversions/test_percent.py
+tests/conversions/test_ppb.py
+tests/conversions/test_ppm.py
 tests/conversions/test_snr_to_ebn0.py
 tests/conversions/test_snr_to_esn0.py
+tests/data_manipulation/__init__.py
 tests/data_manipulation/test_hexdump.py
 tests/data_manipulation/test_pack.py
 tests/data_manipulation/test_unpack.py
+tests/detection/__init__.py
 tests/detection/test_albersheim.py
+tests/dsp/__init__.py
 tests/dsp/test_decimator.py
+tests/dsp/test_differentiator.py
 tests/dsp/test_downsample.py
 tests/dsp/test_farrow.py
 tests/dsp/test_fir.py
 tests/dsp/test_iir.py
+tests/dsp/test_integrator.py
 tests/dsp/test_interpolator.py
 tests/dsp/test_mix.py
 tests/dsp/test_multirate_taps.py
+tests/dsp/test_resampler.py
 tests/dsp/test_to_complex_bb.py
 tests/dsp/test_to_real_pb.py
 tests/dsp/test_upsample.py
+tests/link_budgets/__init__.py
 tests/link_budgets/test_awgn_capacity.py
 tests/link_budgets/test_bec_capacity.py
 tests/link_budgets/test_bsc_capacity.py
 tests/link_budgets/test_fspl.py
+tests/measurements/__init__.py
 tests/measurements/test_crest_factor.py
 tests/measurements/test_energy.py
 tests/measurements/test_error_rate.py
 tests/measurements/test_evm.py
 tests/measurements/test_papr.py
 tests/measurements/test_power.py
 tests/measurements/test_voltage.py
+tests/modulation/__init__.py
 tests/modulation/test_binary_code.py
 tests/modulation/test_diff_decode.py
 tests/modulation/test_diff_encode.py
 tests/modulation/test_gaussian.py
 tests/modulation/test_gray_code.py
 tests/modulation/test_half_sine.py
 tests/modulation/test_raised_cosine.py
 tests/modulation/test_rectangular.py
 tests/modulation/test_root_raised_cosine.py
+tests/modulation/cpm/__init__.py
+tests/modulation/msk/__init__.py
+tests/modulation/psk/__init__.py
 tests/modulation/psk/test_ber.py
 tests/modulation/psk/test_ber_diff.py
 tests/modulation/psk/test_decide_symbols.py
 tests/modulation/psk/test_demodulate.py
 tests/modulation/psk/test_map_symbols.py
 tests/modulation/psk/test_modulate.py
 tests/modulation/psk/test_ser.py
 tests/modulation/psk/test_ser_diff.py
+tests/probability/__init__.py
 tests/probability/test_normal.py
+tests/sequences/__init__.py
 tests/sequences/test_barker.py
 tests/sequences/test_zadoff_chu.py
+tests/simulation/__init__.py
 tests/simulation/test_awgn.py
 tests/simulation/test_bec.py
 tests/simulation/test_bsc.py
 tests/simulation/test_dmc.py
 tests/simulation/test_iq_imbalance.py
-tests/synchronization/test_dds.py
+tests/synchronization/__init__.py
 tests/synchronization/test_loop_filter.py
 tests/synchronization/test_nco.py
```

### Comparing `sdr-0.0.8/tests/conversions/test_ebn0_to_esn0.py` & `sdr-0.0.9/tests/conversions/test_ebn0_to_esn0.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 import sdr
 
 
 def test_1():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'ebno', 'esno', 'BitsPerSymbol', 2, 'CodingRate', 1/3)'
     """
     ebn0 = np.arange(0, 11)
     esn0 = sdr.ebn0_to_esn0(ebn0, 2, rate=1 / 3)
     esn0_truth = np.array(
         [
             -1.760912590556813,
@@ -26,15 +26,15 @@
         ]
     )
     assert np.allclose(esn0, esn0_truth)
 
 
 def test_2():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'ebno', 'esno', 'BitsPerSymbol', 3, 'CodingRate', 1/2)'
     """
     ebn0 = np.arange(0, 11)
     esn0 = sdr.ebn0_to_esn0(ebn0, 3, rate=1 / 2)
     esn0_truth = np.array(
         [
             1.760912590556812,
@@ -51,15 +51,15 @@
         ]
     )
     assert np.allclose(esn0, esn0_truth)
 
 
 def test_3():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'ebno', 'esno', 'BitsPerSymbol', 4, 'CodingRate', 2/3)'
     """
     ebn0 = np.arange(0, 11)
     esn0 = sdr.ebn0_to_esn0(ebn0, 4, rate=2 / 3)
     esn0_truth = np.array(
         [
             4.259687322722811,
```

### Comparing `sdr-0.0.8/tests/conversions/test_ebn0_to_snr.py` & `sdr-0.0.9/tests/conversions/test_ebn0_to_snr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 import sdr
 
 
 def test_1():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'ebno', 'snr', 'BitsPerSymbol', 2, 'CodingRate', 1/3, 'SamplesPerSymbol', 1)'
     """
     ebn0 = np.arange(0, 11)
     snr = sdr.ebn0_to_snr(ebn0, 2, rate=1 / 3, sps=1)
     snr_truth = np.array(
         [
             -1.760912590556813,
@@ -26,15 +26,15 @@
         ]
     )
     assert np.allclose(snr, snr_truth)
 
 
 def test_2():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'ebno', 'snr', 'BitsPerSymbol', 3, 'CodingRate', 1/2, 'SamplesPerSymbol', 2)'
     """
     ebn0 = np.arange(0, 11)
     snr = sdr.ebn0_to_snr(ebn0, 3, rate=1 / 2, sps=2)
     snr_truth = np.array(
         [
             -1.249387366082999,
@@ -51,15 +51,15 @@
         ]
     )
     assert np.allclose(snr, snr_truth)
 
 
 def test_3():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'ebno', 'snr', 'BitsPerSymbol', 4, 'CodingRate', 2/3, 'SamplesPerSymbol', 4)'
     """
     ebn0 = np.arange(0, 11)
     snr = sdr.ebn0_to_snr(ebn0, 4, rate=2 / 3, sps=4)
     snr_truth = np.array(
         [
             -1.760912590556813,
```

### Comparing `sdr-0.0.8/tests/conversions/test_esn0_to_ebn0.py` & `sdr-0.0.9/tests/conversions/test_esn0_to_ebn0.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 import sdr
 
 
 def test_1():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'esno', 'ebno', 'BitsPerSymbol', 2, 'CodingRate', 1/3)'
     """
     esn0 = np.arange(0, 11)
     ebn0 = sdr.esn0_to_ebn0(esn0, 2, rate=1 / 3)
     ebn0_truth = np.array(
         [
             1.760912590556813,
@@ -26,15 +26,15 @@
         ]
     )
     assert np.allclose(ebn0, ebn0_truth)
 
 
 def test_2():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'esno', 'ebno', 'BitsPerSymbol', 3, 'CodingRate', 1/2)'
     """
     esn0 = np.arange(0, 11)
     ebn0 = sdr.esn0_to_ebn0(esn0, 3, rate=1 / 2)
     ebn0_truth = np.array(
         [
             -1.760912590556812,
@@ -51,15 +51,15 @@
         ]
     )
     assert np.allclose(ebn0, ebn0_truth)
 
 
 def test_3():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'esno', 'ebno', 'BitsPerSymbol', 4, 'CodingRate', 2/3)'
     """
     esn0 = np.arange(0, 11)
     ebn0 = sdr.esn0_to_ebn0(esn0, 4, rate=2 / 3)
     ebn0_truth = np.array(
         [
             -4.259687322722811,
```

### Comparing `sdr-0.0.8/tests/conversions/test_esn0_to_snr.py` & `sdr-0.0.9/tests/conversions/test_esn0_to_snr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 import sdr
 
 
 def test_1():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'esno', 'snr', 'SamplesPerSymbol', 1)'
     """
     esn0 = np.arange(0, 11)
     snr = sdr.esn0_to_snr(esn0, sps=1)
     snr_truth = np.array(
         [
             0,
@@ -26,15 +26,15 @@
         ]
     )
     assert np.allclose(snr, snr_truth)
 
 
 def test_2():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'esno', 'snr', 'SamplesPerSymbol', 2)'
     """
     esn0 = np.arange(0, 11)
     snr = sdr.esn0_to_snr(esn0, sps=2)
     snr_truth = np.array(
         [
             -3.010299956639812,
@@ -51,15 +51,15 @@
         ]
     )
     assert np.allclose(snr, snr_truth)
 
 
 def test_3():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'esno', 'snr', 'SamplesPerSymbol', 4)'
     """
     esn0 = np.arange(0, 11)
     snr = sdr.esn0_to_snr(esn0, sps=4)
     snr_truth = np.array(
         [
             -6.020599913279624,
```

### Comparing `sdr-0.0.8/tests/conversions/test_snr_to_ebn0.py` & `sdr-0.0.9/tests/conversions/test_snr_to_ebn0.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 import sdr
 
 
 def test_1():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'snr', 'ebno', 'BitsPerSymbol', 2, 'CodingRate', 1/3, 'SamplesPerSymbol', 1)'
     """
     snr = np.arange(0, 11)
     ebn0 = sdr.snr_to_ebn0(snr, 2, rate=1 / 3, sps=1)
     ebn0_truth = np.array(
         [
             1.760912590556812,
@@ -26,15 +26,15 @@
         ]
     )
     assert np.allclose(ebn0, ebn0_truth)
 
 
 def test_2():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'snr', 'ebno', 'BitsPerSymbol', 3, 'CodingRate', 1/2, 'SamplesPerSymbol', 2)'
     """
     snr = np.arange(0, 11)
     ebn0 = sdr.snr_to_ebn0(snr, 3, rate=1 / 2, sps=2)
     ebn0_truth = np.array(
         [
             1.249387366082999,
@@ -51,15 +51,15 @@
         ]
     )
     assert np.allclose(ebn0, ebn0_truth)
 
 
 def test_3():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'snr', 'ebno', 'BitsPerSymbol', 4, 'CodingRate', 2/3, 'SamplesPerSymbol', 4)'
     """
     snr = np.arange(0, 11)
     ebn0 = sdr.snr_to_ebn0(snr, 4, rate=2 / 3, sps=4)
     ebn0_truth = np.array(
         [
             1.760912590556812,
```

### Comparing `sdr-0.0.8/tests/conversions/test_snr_to_esn0.py` & `sdr-0.0.9/tests/conversions/test_snr_to_esn0.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 import sdr
 
 
 def test_1():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'snr', 'esno', 'SamplesPerSymbol', 1)'
     """
     snr = np.arange(0, 11)
     esn0 = sdr.snr_to_esn0(snr, sps=1)
     esn0_truth = np.array(
         [
             0,
@@ -26,15 +26,15 @@
         ]
     )
     assert np.allclose(esn0, esn0_truth)
 
 
 def test_2():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'snr', 'esno', 'SamplesPerSymbol', 2)'
     """
     snr = np.arange(0, 11)
     esn0 = sdr.snr_to_esn0(snr, sps=2)
     esn0_truth = np.array(
         [
             3.010299956639812,
@@ -51,15 +51,15 @@
         ]
     )
     assert np.allclose(esn0, esn0_truth)
 
 
 def test_3():
     """
-    Matlab:
+    MATLAB:
         >> convertSNR(0:10, 'snr', 'esno', 'SamplesPerSymbol', 4)'
     """
     snr = np.arange(0, 11)
     esn0 = sdr.snr_to_esn0(snr, sps=4)
     esn0_truth = np.array(
         [
             6.020599913279624,
```

### Comparing `sdr-0.0.8/tests/data_manipulation/test_hexdump.py` & `sdr-0.0.9/tests/data_manipulation/test_hexdump.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/data_manipulation/test_pack.py` & `sdr-0.0.9/tests/data_manipulation/test_pack.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/data_manipulation/test_unpack.py` & `sdr-0.0.9/tests/data_manipulation/test_unpack.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/detection/test_albersheim.py` & `sdr-0.0.9/tests/detection/test_albersheim.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/dsp/test_decimator.py` & `sdr-0.0.9/tests/dsp/test_decimator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-import math
-
-import matplotlib.pyplot as plt
 import numpy as np
-import pytest
-import scipy.signal
 
 import sdr
 
+
+def debug_plot(y, y_truth):
+    import matplotlib.pyplot as plt
+
+    plt.figure()
+    sdr.plot.time_domain(y, label="Test")
+    sdr.plot.time_domain(y_truth, label="Truth")
+    plt.legend()
+    plt.show()
+
+
 # def test_non_streaming_rate():
 #     mode = "rate"
 #     N = 50
 #     x = np.random.randn(N) + 1j * np.random.randn(N)  # Input signal
 #     r = np.random.randint(3, 7)  # Interpolation rate
 
 #     fir = sdr.Decimator(r)
@@ -62,15 +68,15 @@
     # plt.show()
 
     np.testing.assert_array_almost_equal(y_full, y_stream)
 
 
 def test_3_kaiser():
     """
-    Matlab:
+    MATLAB:
         >> x = cos(pi/7.123456*(0:359)');
         >> fir = dsp.FIRDecimator(3);
         >> y = fir(x);
     """
     x = np.cos(np.pi / 7.123456 * np.arange(360))
     y_truth = np.array(
         [
@@ -196,20 +202,21 @@
             -0.980854783192394,
         ]
     )
 
     fir = sdr.Decimator(3, streaming=True)
     y = fir(x)
 
+    # debug_plot(y, y_truth)
     np.testing.assert_almost_equal(y, y_truth)
 
 
 def test_4_kaiser():
     """
-    Matlab:
+    MATLAB:
         >> x = cos(pi/7.123456*(0:359)');
         >> fir = dsp.FIRDecimator(4);
         >> y = fir(x);
     """
     x = np.cos(np.pi / 7.123456 * np.arange(360))
     y_truth = np.array(
         [
@@ -305,20 +312,21 @@
             -0.734464884875273,
         ]
     )
 
     fir = sdr.Decimator(4, streaming=True)
     y = fir(x)
 
+    # debug_plot(y, y_truth)
     np.testing.assert_almost_equal(y, y_truth)
 
 
 def test_5_kaiser():
     """
-    Matlab:
+    MATLAB:
         >> x = cos(pi/7.123456*(0:359)');
         >> fir = dsp.FIRDecimator(5);
         >> y = fir(x);
     """
     x = np.cos(np.pi / 7.123456 * np.arange(360))
     y_truth = np.array(
         [
@@ -396,20 +404,21 @@
             -0.271492123589855,
         ]
     )
 
     fir = sdr.Decimator(5, streaming=True)
     y = fir(x)
 
+    # debug_plot(y, y_truth)
     np.testing.assert_almost_equal(y, y_truth)
 
 
 def test_6_kaiser():
     """
-    Matlab:
+    MATLAB:
         >> x = cos(pi/7.123456*(0:359)');
         >> fir = dsp.FIRDecimator(6);
         >> y = fir(x);
     """
     x = np.cos(np.pi / 7.123456 * np.arange(360))
     y_truth = np.array(
         [
@@ -475,8 +484,9 @@
             0.268518722443338,
         ]
     )
 
     fir = sdr.Decimator(6, streaming=True)
     y = fir(x)
 
+    # debug_plot(y, y_truth)
     np.testing.assert_almost_equal(y, y_truth)
```

### Comparing `sdr-0.0.8/tests/dsp/test_downsample.py` & `sdr-0.0.9/tests/dsp/test_downsample.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     with pytest.raises(ValueError):
         # Rate must be positive
         sdr.downsample(x, 0)
 
 
 def test_1():
     """
-    Matlab:
+    MATLAB:
         >> x = 0:39;
         >> downsample(x, 4)'
     """
     x = np.arange(40)
     y = sdr.downsample(x, 4)
     y_truth = np.array([0, 4, 8, 12, 16, 20, 24, 28, 32, 36])
     assert np.array_equal(y, y_truth)
```

### Comparing `sdr-0.0.8/tests/dsp/test_farrow.py` & `sdr-0.0.9/tests/dsp/test_farrow.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/dsp/test_fir.py` & `sdr-0.0.9/tests/dsp/test_fir.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/dsp/test_iir.py` & `sdr-0.0.9/tests/dsp/test_iir.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/dsp/test_interpolator.py` & `sdr-0.0.9/tests/dsp/test_interpolator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,56 @@
-import math
-
-import matplotlib.pyplot as plt
 import numpy as np
-import pytest
 import scipy.signal
 
 import sdr
 
 
+def debug_plot(y, y_truth):
+    import matplotlib.pyplot as plt
+
+    plt.figure()
+    sdr.plot.time_domain(y, label="Test")
+    sdr.plot.time_domain(y_truth, label="Truth")
+    plt.legend()
+    plt.show()
+
+
 def test_non_streaming_rate():
     mode = "rate"
     N = 50
     x = np.random.randn(N) + 1j * np.random.randn(N)  # Input signal
     r = np.random.randint(3, 7)  # Interpolation rate
 
     fir = sdr.Interpolator(r)
     y = fir(x, mode)
 
     # The output should align with the input. Every r-th sample should match.
-    np.testing.assert_array_almost_equal(y[::r], x)
+    y = y[::r]
+    y_truth = x
+
+    # debug_plot(y, y_truth)
+    np.testing.assert_array_almost_equal(y, y_truth)
 
 
 def test_non_streaming_full():
     mode = "full"
     N = 50
     x = np.random.randn(N) + 1j * np.random.randn(N)  # Input signal
     r = np.random.randint(3, 7)  # Interpolation rate
 
     fir = sdr.Interpolator(r)
     y = fir(x, mode)
 
     xr = np.zeros(N * r, dtype=complex)
     xr[::r] = x[:]
-    y_truth = scipy.signal.convolve(xr, fir.taps, mode=mode)
-
     # Given the polyphase decomposition, the polyphase output is slightly shorter
-    np.testing.assert_array_almost_equal(y, y_truth[: y.size])
+    y_truth = scipy.signal.convolve(xr, fir.taps, mode=mode)[: y.size]
+
+    # debug_plot(y, y_truth)
+    np.testing.assert_array_almost_equal(y, y_truth)
 
 
 def test_streaming():
     N = 50
     x = np.random.randn(N) + 1j * np.random.randn(N)  # Input signal
     r = np.random.randint(3, 7)  # Interpolation rate
 
@@ -50,14 +61,15 @@
     for i in range(0, N, d):
         y[i * r : (i + d) * r] = fir(x[i : i + d])
 
     xr = np.zeros(N * r, dtype=complex)
     xr[::r] = x[:]
     y_truth = scipy.signal.convolve(xr, fir.taps, mode="full")[0 : N * r]
 
+    # debug_plot(y, y_truth)
     np.testing.assert_array_almost_equal(y, y_truth)
 
 
 def test_streaming_match_full():
     N = 50
     x = np.random.randn(N) + 1j * np.random.randn(N)  # Input signal
     r = np.random.randint(3, 7)  # Interpolation rate
@@ -73,15 +85,15 @@
     y_stream[(i + d) * r :] = fir2.flush()
 
     np.testing.assert_array_almost_equal(y_full, y_stream)
 
 
 def test_3_kaiser():
     """
-    Matlab:
+    MATLAB:
         >> x = cos(pi/4*(0:19)');
         >> fir = dsp.Interpolator(3);
         >> y = fir(x);
     """
     x = np.cos(np.pi / 4 * np.arange(20))
     y_truth = np.array(
         [
@@ -147,20 +159,21 @@
             0.963802028619039,
         ]
     )
 
     fir = sdr.Interpolator(3, streaming=True)
     y = fir(x)
 
+    # debug_plot(y, y_truth)
     np.testing.assert_almost_equal(y, y_truth)
 
 
 def test_3_linear():
     """
-    Matlab:
+    MATLAB:
         >> x = cos(pi/4*(0:19)');
         >> fir = dsp.Interpolator(3, 'Linear');
         >> y = fir(x);
     """
     x = np.cos(np.pi / 4 * np.arange(20))
     y_truth = np.array(
         [
@@ -223,25 +236,24 @@
             0.000000000000001,
             -0.235702260395515,
             -0.471404520791031,
             -0.707106781186546,
         ]
     )
 
-    fir = sdr.Interpolator(3, "linear", streaming=True)
+    fir = sdr.Interpolator(3, "linear-matlab", streaming=True)
     y = fir(x)
 
-    # NOTE: Matlab starts with the first interpolated sample as 1/N not 0/N.
-    #       We are using 0/N since it aligns better with the input data.
-    np.testing.assert_almost_equal(y[1:], y_truth[:-1])
+    # debug_plot(y, y_truth)
+    np.testing.assert_almost_equal(y, y_truth)
 
 
 def test_3_zoh():
     """
-    Matlab:
+    MATLAB:
         >> x = cos(pi/4*(0:19)');
         >> fir = dsp.Interpolator(3, 'ZOH');
         >> y = fir(x);
     """
     x = np.cos(np.pi / 4 * np.arange(20))
     y_truth = np.array(
         [
@@ -307,20 +319,21 @@
             -0.707106781186546,
         ]
     )
 
     fir = sdr.Interpolator(3, "zoh", streaming=True)
     y = fir(x)
 
+    # debug_plot(y, y_truth)
     np.testing.assert_almost_equal(y, y_truth)
 
 
 def test_srrc_0p5_6():
     """
-    Matlab:
+    MATLAB:
         >> sps = 4;
         >> h = rcosdesign(0.5, 6, sps);
         >> s = randi([0 3], 10, 1);
         >> x = pskmod(s, 4);
         >> fir = dsp.Interpolator(sps, h);
         >> y = fir(x);
     """
@@ -411,20 +424,21 @@
             -0.549807892644904 + 0.086170934639173j,
         ]
     )
 
     fir = sdr.Interpolator(4, h, streaming=True)
     y = fir(x)
 
+    # debug_plot(y, y_truth)
     np.testing.assert_almost_equal(y, y_truth)
 
 
 def test_srrc_0p9_4():
     """
-    Matlab:
+    MATLAB:
         >> sps = 5;
         >> h = rcosdesign(0.9, 4, sps);
         >> s = randi([0 3], 10, 1);
         >> x = pskmod(s, 4);
         >> fir = dsp.Interpolator(sps, h);
         >> y = fir(x);
     """
@@ -521,20 +535,21 @@
             0.031449795150026 + 0.482516490375424j,
         ]
     )
 
     fir = sdr.Interpolator(5, h, streaming=True)
     y = fir(x)
 
+    # debug_plot(y, y_truth)
     np.testing.assert_almost_equal(y, y_truth)
 
 
 def test_srrc_0p1_7():
     """
-    Matlab:
+    MATLAB:
         >> sps = 6;
         >> h = rcosdesign(0.1, 7, sps);
         >> s = randi([0 3], 10, 1);
         >> x = pskmod(s, 4);
         >> fir = dsp.Interpolator(sps, h);
         >> y = fir(x);
     """
@@ -663,8 +678,9 @@
             0.083427205679682 - 0.242450393098225j,
         ]
     )
 
     fir = sdr.Interpolator(6, h, streaming=True)
     y = fir(x)
 
+    # debug_plot(y, y_truth)
     np.testing.assert_almost_equal(y, y_truth)
```

### Comparing `sdr-0.0.8/tests/dsp/test_mix.py` & `sdr-0.0.9/tests/dsp/test_mix.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/dsp/test_multirate_taps.py` & `sdr-0.0.9/tests/dsp/test_multirate_taps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 import sdr
 
 
 def test_3_1():
     """
-    Matlab:
+    MATLAB:
         >> transpose(designMultirateFIR(3, 1))
     """
     h = sdr.multirate_taps(3, 1)
     h_truth = np.array(
         [
             0,
             -0.000129061486200,
@@ -86,15 +86,15 @@
         ]
     )
     np.testing.assert_array_almost_equal(h, h_truth)
 
 
 def test_1_3():
     """
-    Matlab:
+    MATLAB:
         >> transpose(designMultirateFIR(1, 3))
     """
     h = sdr.multirate_taps(1, 3)
     h_truth = np.array(
         [
             0,
             -0.000043020495400,
@@ -171,15 +171,15 @@
         ]
     )
     np.testing.assert_array_almost_equal(h, h_truth)
 
 
 def test_3_2():
     """
-    Matlab:
+    MATLAB:
         >> transpose(designMultirateFIR(3, 2))
     """
     h = sdr.multirate_taps(3, 2)
     h_truth = np.array(
         [
             0,
             -0.000129061486200,
@@ -256,15 +256,15 @@
         ]
     )
     np.testing.assert_array_almost_equal(h, h_truth)
 
 
 def test_2_3():
     """
-    Matlab:
+    MATLAB:
         >> transpose(designMultirateFIR(2, 3))
     """
     h = sdr.multirate_taps(2, 3)
     h_truth = np.array(
         [
             0,
             -0.000174137520857,
@@ -317,15 +317,15 @@
         ]
     )
     np.testing.assert_array_almost_equal(h, h_truth)
 
 
 def test_3_2_20():
     """
-    Matlab:
+    MATLAB:
         >> transpose(designMultirateFIR(3, 2, 20))
     """
     h = sdr.multirate_taps(3, 2, half_length=20)
     h_truth = np.array(
         [
             0,
             -0.000059208485371,
@@ -450,15 +450,15 @@
         ]
     )
     np.testing.assert_array_almost_equal(h, h_truth)
 
 
 def test_2_3_20():
     """
-    Matlab:
+    MATLAB:
         >> transpose(designMultirateFIR(2, 3, 20))
     """
     h = sdr.multirate_taps(2, 3, half_length=20)
     h_truth = np.array(
         [
             -0.000036875262276,
             0,
@@ -544,15 +544,15 @@
         ]
     )
     np.testing.assert_array_almost_equal(h, h_truth)
 
 
 def test_3_2_15_120():
     """
-    Matlab:
+    MATLAB:
         >> transpose(designMultirateFIR(3, 2, 15, 120))
     """
     h = sdr.multirate_taps(3, 2, half_length=15, A_stop=120)
     h_truth = np.array(
         [
             0,
             0.000002676045758,
@@ -647,15 +647,15 @@
         ]
     )
     np.testing.assert_array_almost_equal(h, h_truth)
 
 
 def test_2_3_15_120():
     """
-    Matlab:
+    MATLAB:
         >> transpose(designMultirateFIR(2, 3, 15, 120))
     """
     h = sdr.multirate_taps(2, 3, half_length=15, A_stop=120)
     h_truth = np.array(
         [
             0,
             -0.000004262029874,
```

### Comparing `sdr-0.0.8/tests/dsp/test_upsample.py` & `sdr-0.0.9/tests/dsp/test_upsample.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     with pytest.raises(ValueError):
         # Rate must be positive
         sdr.upsample(x, 0)
 
 
 def test_1():
     """
-    Matlab:
+    MATLAB:
         >> x = 0:9;
         >> upsample(x, 4)'
     """
     x = np.arange(10)
     y = sdr.upsample(x, 4)
     y_truth = np.array(
         [
```

### Comparing `sdr-0.0.8/tests/link_budgets/test_bec_capacity.py` & `sdr-0.0.9/tests/link_budgets/test_bec_capacity.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/link_budgets/test_bsc_capacity.py` & `sdr-0.0.9/tests/link_budgets/test_bsc_capacity.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/link_budgets/test_fspl.py` & `sdr-0.0.9/tests/link_budgets/test_fspl.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pytest
 
 import sdr
 
 
 def test_250_MHz():
     """
-    Matlab:
+    MATLAB:
         >> d = logspace(1, 6, 20); d'
         >> L = fspl(d, physconst('LightSpeed')/250e6); L'
     """
     d = np.logspace(1, 6, 20)
     fspl = sdr.fspl(d, 250e6)
     fspl_truth = np.array(
         [
@@ -43,15 +43,15 @@
     fspl = sdr.fspl(d[i], 250e6)
     assert isinstance(fspl, float)
     assert fspl == pytest.approx(fspl_truth[i])
 
 
 def test_7p5_GHz():
     """
-    Matlab:
+    MATLAB:
         >> d = logspace(1, 6, 20); d'
         >> L = fspl(d, physconst('LightSpeed')/7.5e9); L'
     """
     d = np.logspace(1, 6, 20)
     fspl = sdr.fspl(d, 7.5e9)
     fspl_truth = np.array(
         [
@@ -84,15 +84,15 @@
     fspl = sdr.fspl(d[i], 7.5e9)
     assert isinstance(fspl, float)
     assert fspl == pytest.approx(fspl_truth[i])
 
 
 def test_28p25_GHz():
     """
-    Matlab:
+    MATLAB:
         >> d = logspace(1, 6, 20); d'
         >> L = fspl(d, physconst('LightSpeed')/28.25e9); L'
     """
     d = np.logspace(1, 6, 20)
     fspl = sdr.fspl(d, 28.25e9)
     fspl_truth = np.array(
         [
@@ -125,15 +125,15 @@
     fspl = sdr.fspl(d[i], 28.25e9)
     assert isinstance(fspl, float)
     assert fspl == pytest.approx(fspl_truth[i])
 
 
 def test_300_MHz_near_field():
     """
-    Matlab:
+    MATLAB:
         >> d = linspace(0, 0.25, 20); d'
         >> L = fspl(d, physconst('LightSpeed')/300e6); L'
     """
     d = np.linspace(0, 0.25, 20)
     fspl = sdr.fspl(d, 300e6)
     fspl_truth = np.array(
         [
```

### Comparing `sdr-0.0.8/tests/measurements/test_crest_factor.py` & `sdr-0.0.9/tests/measurements/test_crest_factor.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/measurements/test_error_rate.py` & `sdr-0.0.9/tests/measurements/test_error_rate.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/measurements/test_evm.py` & `sdr-0.0.9/tests/measurements/test_evm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Matlab:
+MATLAB:
     symbol_map = pskmod(0:3, 4, pi/4, "gray");
     s = randi([0 3], 50, 1);
     x = pskmod(s, 4, pi/4, "gray");
     x_hat = awgn(x, 20);
     disp(s)
     disp(x_hat)
     evm = comm.EVM( ...
@@ -154,23 +154,23 @@
     ]
 )
 
 
 def test_exceptions():
     psk = sdr.PSK(4, phase_offset=45)
     with pytest.raises(ValueError):
-        evm = sdr.evm(X_HAT, psk.symbol_map, norm="invalid")
+        sdr.evm(X_HAT, psk.symbol_map, norm="invalid")
     with pytest.raises(ValueError):
-        evm = sdr.evm(X_HAT, psk.symbol_map, output="invalid")
+        sdr.evm(X_HAT, psk.symbol_map, output="invalid")
     with pytest.raises(ValueError):
         # Output percentile must be in [0, 100]
-        evm = sdr.evm(X_HAT, psk.symbol_map, output=-1)
+        sdr.evm(X_HAT, psk.symbol_map, output=-1)
     with pytest.raises(ValueError):
         # Output percentile must be in [0, 100]
-        evm = sdr.evm(X_HAT, psk.symbol_map, output=101)
+        sdr.evm(X_HAT, psk.symbol_map, output=101)
 
 
 def test_average_power_ref():
     psk = sdr.PSK(4, phase_offset=45)
     evm = sdr.evm(X_HAT, psk.symbol_map, norm="average-power-ref")
     assert evm == pytest.approx(9.913846806617736)
 
@@ -195,15 +195,15 @@
     assert evm == pytest.approx(8.102616784925608)
 
     x = psk.map_symbols(S)
     evm = sdr.evm(X_HAT, x, norm="peak-power")
     assert evm == pytest.approx(8.102616784925608)
 
 
-# TODO: For some reason Matlab computes percentiles differently??
+# TODO: For some reason MATLAB computes percentiles differently??
 
 # def test_10th_percentile():
 #     psk = sdr.PSK(4, phase_offset=45)
 #     evm = sdr.evm(X_HAT, psk.symbol_map, output=10)
 #     assert evm == pytest.approx(2.835000000000000)
```

### Comparing `sdr-0.0.8/tests/measurements/test_papr.py` & `sdr-0.0.9/tests/measurements/test_papr.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/modulation/psk/test_ber.py` & `sdr-0.0.9/tests/modulation/psk/test_ber.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Matlab:
+MATLAB:
     for M = [2 4 8 16]
         disp(M)
         ebn0 = -10:0.5:10;
         [ber, ser] = berawgn(ebn0, 'psk', M, 'nondiff');
         disp(ber')
     end
 """
```

### Comparing `sdr-0.0.8/tests/modulation/psk/test_ber_diff.py` & `sdr-0.0.9/tests/modulation/psk/test_ber_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Matlab:
+MATLAB:
     for M = [2 4]
         disp(M)
         ebn0 = -10:0.5:10;
         [ber, ser] = berawgn(ebn0, 'psk', M, 'diff');
         disp(ber')
     end
 """
```

### Comparing `sdr-0.0.8/tests/modulation/psk/test_decide_symbols.py` & `sdr-0.0.9/tests/modulation/psk/test_decide_symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Matlab:
+MATLAB:
     x_hat = exp(1i * 2 * pi * rand(1, 20));
     disp(transpose(x_hat))
     for M = [2 4 8 16]
         for map = ["bin", "gray"]
             disp(M)
             disp(map)
             phi = 2*pi*(rand - 0.5);
```

### Comparing `sdr-0.0.8/tests/modulation/psk/test_demodulate.py` & `sdr-0.0.9/tests/modulation/psk/test_demodulate.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/modulation/psk/test_map_symbols.py` & `sdr-0.0.9/tests/modulation/psk/test_map_symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Matlab:
+MATLAB:
     for M = [2 4 8 16]
         for map = ["bin", "gray"]
             disp(M)
             disp(map)
             phi = 2*pi*(rand - 0.5);
             s = [0:M-1 randi([0 M-1], 1, 2*M)];
             x = pskmod(s, M, phi, map);
```

### Comparing `sdr-0.0.8/tests/modulation/psk/test_modulate.py` & `sdr-0.0.9/tests/modulation/psk/test_modulate.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/modulation/psk/test_ser.py` & `sdr-0.0.9/tests/modulation/psk/test_ser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Matlab:
+MATLAB:
     for M = [2 4 8 16]
         disp(M)
         ebn0 = -10:0.5:10;
         [ber, ser] = berawgn(ebn0, 'psk', M, 'nondiff');
         disp(ser')
     end
 """
```

### Comparing `sdr-0.0.8/tests/modulation/psk/test_ser_diff.py` & `sdr-0.0.9/tests/modulation/psk/test_ser_diff.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Matlab:
+MATLAB:
     for M = [2 4]
         disp(M)
         ebn0 = -10:0.5:10;
         [ber, ser] = berawgn(ebn0, 'psk', M, 'diff');
         disp(ser')
     end
 """
@@ -114,8 +114,8 @@
             0.000048434400120,
             0.000015488312917,
         ]
     )
     np.testing.assert_almost_equal(ser, ser_truth)
 
 
-# NOTE: Matlab only support DE-BPSK and DE-QPSK
+# NOTE: MATLAB only support DE-BPSK and DE-QPSK
```

### Comparing `sdr-0.0.8/tests/modulation/test_binary_code.py` & `sdr-0.0.9/tests/modulation/test_binary_code.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/modulation/test_diff_decode.py` & `sdr-0.0.9/tests/modulation/test_diff_decode.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     with pytest.raises(ValueError):
         # y_prev must be non-negative
         sdr.diff_decode([0, 1, 0], y_prev=-1)
 
 
 def test_decode_1():
     """
-    Matlab:
+    MATLAB:
         >> diff_dec = comm.DifferentialDecoder;
         >> y = randi([0 1], 10, 1); y
         >> diff_dec(y)
     """
     y = [1, 0, 1, 1, 0, 0, 0, 0, 0, 1]
     x = sdr.diff_decode(y)
     x_truth = [1, 1, 1, 0, 1, 0, 0, 0, 0, 1]
     assert np.array_equal(x, x_truth)
 
 
-# TODO: Add more Matlab tests
+# TODO: Add more MATLAB tests
```

### Comparing `sdr-0.0.8/tests/modulation/test_diff_encode.py` & `sdr-0.0.9/tests/modulation/test_diff_encode.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     with pytest.raises(ValueError):
         # y_prev must be non-negative
         sdr.diff_encode([0, 1, 0], y_prev=-1)
 
 
 def test_encode_1():
     """
-    Matlab:
+    MATLAB:
         >> diff_enc = comm.DifferentialEncoder;
         >> x = randi([0 1], 10, 1); x
         >> diff_enc(x)
     """
     x = [0, 1, 0, 0, 1, 1, 0, 0, 0, 0]
     y = sdr.diff_encode(x)
     y_truth = [0, 1, 1, 1, 0, 1, 1, 1, 1, 1]
     assert np.array_equal(y, y_truth)
 
 
-# TODO: Add more Matlab tests
+# TODO: Add more MATLAB tests
```

### Comparing `sdr-0.0.8/tests/modulation/test_gaussian.py` & `sdr-0.0.9/tests/modulation/test_gaussian.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     with pytest.raises(ValueError):
         # The filter must have even order
         sdr.gaussian(0.5, 3, 5)
 
 
 def test_0p1_4_8():
     """
-    Matlab:
+    MATLAB:
         >> h = gaussdesign(0.1, 4, 8); h'
     """
     h = sdr.gaussian(0.1, 4, 8)
     h_truth = np.array(
         [
             0.013681118327446,
             0.015704625974656,
@@ -70,15 +70,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p2_5_8():
     """
-    Matlab:
+    MATLAB:
         >> h = gaussdesign(0.2, 5, 8); h'
     """
     h = sdr.gaussian(0.2, 5, 8)
     h_truth = np.array(
         [
             0.000060917392374,
             0.000121956162037,
@@ -124,15 +124,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p3_4_9():
     """
-    Matlab:
+    MATLAB:
         >> h = gaussdesign(0.3, 4, 9); h'
     """
     h = sdr.gaussian(0.3, 4, 9)
     h_truth = np.array(
         [
             0.000003541513313,
             0.000010719008155,
```

### Comparing `sdr-0.0.8/tests/modulation/test_gray_code.py` & `sdr-0.0.9/tests/modulation/test_gray_code.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/modulation/test_half_sine.py` & `sdr-0.0.9/tests/modulation/test_half_sine.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/modulation/test_raised_cosine.py` & `sdr-0.0.9/tests/modulation/test_raised_cosine.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ##############################################################################
 # Test across alpha, even/odd span, even/odd sos
 ##############################################################################
 
 
 def test_0p1_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.1, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.1, 6, 4)
     h_truth = np.array(
         [
             0.000000000000000,
             0.038872406382003,
@@ -67,15 +67,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p5_5_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.5, 5, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.5, 5, 4)
     h_truth = np.array(
         [
             0.009166733389206,
             0.012160554155472,
@@ -101,15 +101,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p9_6_5():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.9, 6, 5, 'normal'); h'
     """
     h = sdr.raised_cosine(0.9, 6, 5)
     h_truth = np.array(
         [
             0.000000000000000,
             0.000087347868337,
@@ -150,15 +150,15 @@
 ##############################################################################
 # More detailed testing across alpha
 ##############################################################################
 
 
 def test_0p0_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.0, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.0, 6, 4)
     h_truth = np.array(
         [
             0.000000000000000,
             0.041628469482581,
@@ -191,15 +191,15 @@
 
 
 # Already tested 0.1
 
 
 def test_0p2_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.2, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.2, 6, 4)
     h_truth = np.array(
         [
             0.000000000000000,
             0.031348652416305,
@@ -229,15 +229,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p3_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.3, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.3, 6, 4)
     h_truth = np.array(
         [
             0.000000000000000,
             0.021071527141773,
@@ -267,15 +267,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p4_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.4, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.4, 6, 4)
     h_truth = np.array(
         [
             0.000000000000000,
             0.010684193926980,
@@ -305,15 +305,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p5_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.5, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.5, 6, 4)
     h_truth = np.array(
         [
             0.000000000000000,
             0.002551224846890,
@@ -343,15 +343,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p6_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.6, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.6, 6, 4)
     h_truth = np.array(
         [
             -0.000000000000000,
             -0.002037611604380,
@@ -381,15 +381,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p7_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.7, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.7, 6, 4)
     h_truth = np.array(
         [
             -0.000000000000000,
             -0.003169510215030,
@@ -419,15 +419,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p8_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.8, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.8, 6, 4)
     h_truth = np.array(
         [
             -0.000000000000000,
             -0.002016108589650,
@@ -457,15 +457,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p9_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.9, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(0.9, 6, 4)
     h_truth = np.array(
         [
             0.000000000000000,
             -0.000155185964730,
@@ -495,15 +495,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_1p0_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(1.0, 6, 4, 'normal'); h'
     """
     h = sdr.raised_cosine(1.0, 6, 4)
     h_truth = np.array(
         [
             0.000000000000000,
             0.001142355611194,
```

### Comparing `sdr-0.0.8/tests/modulation/test_rectangular.py` & `sdr-0.0.9/tests/modulation/test_rectangular.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/modulation/test_root_raised_cosine.py` & `sdr-0.0.9/tests/modulation/test_root_raised_cosine.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ##############################################################################
 # Test across alpha, even/odd span, even/odd sos
 ##############################################################################
 
 
 def test_0p1_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.1, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.1, 6, 4)
     h_truth = np.array(
         [
             -0.012584683717650,
             0.027659902370502,
@@ -67,15 +67,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p5_5_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.5, 5, 4); h'
     """
     h = sdr.root_raised_cosine(0.5, 5, 4)
     h_truth = np.array(
         [
             -0.007504512238300,
             0.007736024298795,
@@ -101,15 +101,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p9_6_5():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.9, 6, 5); h'
     """
     h = sdr.root_raised_cosine(0.9, 6, 5)
     h_truth = np.array(
         [
             -0.002936931761839,
             0.002340139943481,
@@ -150,15 +150,15 @@
 ##############################################################################
 # More detailed testing across alpha
 ##############################################################################
 
 
 def test_0p0_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.0, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.0, 6, 4)
     h_truth = np.array(
         [
             0.000000000000000,
             0.041628469482581,
@@ -191,15 +191,15 @@
 
 
 # Already tested 0.1
 
 
 def test_0p2_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.2, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.2, 6, 4)
     h_truth = np.array(
         [
             -0.018901920032795,
             0.010651011163846,
@@ -229,15 +229,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p3_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.3, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.3, 6, 4)
     h_truth = np.array(
         [
             -0.016564663762462,
             -0.003143272710786,
@@ -267,15 +267,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p4_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.4, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.4, 6, 4)
     h_truth = np.array(
         [
             -0.007934084141152,
             -0.009551316712176,
@@ -305,15 +305,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p5_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.5, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.5, 6, 4)
     h_truth = np.array(
         [
             0.001516034308196,
             -0.008227494944468,
@@ -343,15 +343,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p6_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.6, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.6, 6, 4)
     h_truth = np.array(
         [
             0.006692349083104,
             -0.002353423155866,
@@ -381,15 +381,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p7_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.7, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.7, 6, 4)
     h_truth = np.array(
         [
             0.005857604524586,
             0.003476008701297,
@@ -419,15 +419,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p8_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.8, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.8, 6, 4)
     h_truth = np.array(
         [
             0.001173021892141,
             0.005833223478906,
@@ -457,15 +457,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_0p9_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(0.9, 6, 4); h'
     """
     h = sdr.root_raised_cosine(0.9, 6, 4)
     h_truth = np.array(
         [
             -0.003283581301483,
             0.004037629718684,
@@ -495,15 +495,15 @@
         ]
     )
     np.testing.assert_almost_equal(h, h_truth)
 
 
 def test_1p0_6_4():
     """
-    Matlab:
+    MATLAB:
         >> h = rcosdesign(1.0, 6, 4); h'
     """
     h = sdr.root_raised_cosine(1.0, 6, 4)
     h_truth = np.array(
         [
             -0.004452022763640,
             0.000000000000000,
```

### Comparing `sdr-0.0.8/tests/probability/test_normal.py` & `sdr-0.0.9/tests/probability/test_normal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 import sdr
 
 
 def test_Q():
     """
-    Matlab:
+    MATLAB:
         >> x = -3:0.2:3;
         >> qfunc(x)'
     """
     x = np.arange(-3, 3.2, 0.2)
     p = sdr.Q(x)
     p_truth = np.array(
         [
@@ -54,15 +54,15 @@
     pi = sdr.Q(x[i])
     assert isinstance(pi, float)
     assert p[i] == pi
 
 
 def test_Qinv():
     """
-    Matlab:
+    MATLAB:
         >> p = 0:0.05:1;
         >> qfuncinv(p)'
     """
     p = np.arange(0, 1.05, 0.05)
     x = sdr.Qinv(p)
     x_truth = np.array(
         [
```

### Comparing `sdr-0.0.8/tests/sequences/test_barker.py` & `sdr-0.0.9/tests/sequences/test_barker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Matlab:
+MATLAB:
     for N = [1, 2, 3, 4, 5, 7, 11, 13]
         barker = comm.BarkerCode("Length", N, "SamplesPerFrame", N);
         disp(N)
         disp(out)
         disp(barker())
     end
 """
```

### Comparing `sdr-0.0.8/tests/sequences/test_zadoff_chu.py` & `sdr-0.0.9/tests/sequences/test_zadoff_chu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Matlab:
+MATLAB:
     N = [3 5 7 9 11 13 15 17 19 21 23 25]
     R = [2 2 3 5 3  5  7  7  7  11 11 11]
     for ii = 1:length(N)
         seq = zadoffChuSeq(R(ii), N(ii));
         disp(N(ii))
         disp(R(ii))
         disp(seq)
```

### Comparing `sdr-0.0.8/tests/simulation/test_awgn.py` & `sdr-0.0.9/tests/simulation/test_awgn.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/simulation/test_bec.py` & `sdr-0.0.9/tests/simulation/test_bec.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/simulation/test_bsc.py` & `sdr-0.0.9/tests/simulation/test_bsc.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/simulation/test_dmc.py` & `sdr-0.0.9/tests/simulation/test_dmc.py`

 * *Files identical despite different names*

### Comparing `sdr-0.0.8/tests/synchronization/test_loop_filter.py` & `sdr-0.0.9/tests/synchronization/test_loop_filter.py`

 * *Files identical despite different names*

