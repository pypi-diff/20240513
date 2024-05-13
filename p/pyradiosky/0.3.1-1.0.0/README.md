# Comparing `tmp/pyradiosky-0.3.1.tar.gz` & `tmp/pyradiosky-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyradiosky-0.3.1.tar", last modified: Thu Feb 22 18:01:47 2024, max compression
+gzip compressed data, was "pyradiosky-1.0.0.tar", last modified: Mon May 13 18:52:12 2024, max compression
```

## Comparing `pyradiosky-0.3.1.tar` & `pyradiosky-1.0.0.tar`

### file list

```diff
@@ -1,108 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.659993 pyradiosky-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.635992 pyradiosky-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.635992 pyradiosky-0.3.1/.github/original_pr_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/original_pr_templates/bug_fix.md
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/original_pr_templates/build_ci_change.md
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/original_pr_templates/documentation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/original_pr_templates/new_feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/original_pr_templates/other.md
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/original_pr_templates/version_change.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.635992 pyradiosky-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/workflows/externaltests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/workflows/publish-to-test-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.github/workflows/testsuite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-02-22 18:01:47.659993 pyradiosky-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.635992 pyradiosky-0.3.1/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/ci/full_deps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/ci/min_deps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/ci/min_versions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/ci/publish.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.639992 pyradiosky-0.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.643993 pyradiosky-0.3.1/docs/Images/
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/fhd_catalog_extended_models_fluxcounts.png
--rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/fhd_catalog_extended_models_radec.png
--rw-r--r--   0 runner    (1001) docker     (127)    41347 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/fhd_catalog_extended_models_radec_picA.png
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/fhd_catalog_extended_models_refspec.png
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/fhd_catalog_specind_atfreqs.png
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gleam_50srcs_fluxcounts.png
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gleam_50srcs_fluxcounts_fluxselect.png
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gleam_50srcs_freqflux.png
--rw-r--r--   0 runner    (1001) docker     (127)    34724 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gleam_50srcs_radec.png
--rw-r--r--   0 runner    (1001) docker     (127)    28175 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gleam_50srcs_radec_fluxselect.png
--rw-r--r--   0 runner    (1001) docker     (127)    29353 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gleam_50srcs_radec_raselect.png
--rw-r--r--   0 runner    (1001) docker     (127)    53618 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gleam_subband_spectra_atfreqs.png
--rw-r--r--   0 runner    (1001) docker     (127)    57457 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gsm_gal_coneselect_molliwede.png
--rw-r--r--   0 runner    (1001) docker     (127)    51002 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gsm_gal_neighborselect_molliwede.png
--rw-r--r--   0 runner    (1001) docker     (127)   130348 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gsm_galactic_flux_molliwede.png
--rw-r--r--   0 runner    (1001) docker     (127)   130557 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gsm_icrs_flux_molliwede.png
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gsm_icrs_fluxcounts.png
--rw-r--r--   0 runner    (1001) docker     (127)    55631 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gsm_icrs_indselect_molliwede.png
--rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gsm_icrs_radec.png
--rw-r--r--   0 runner    (1001) docker     (127)   133242 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/gsm_point_galactic_flux_molliwede.png
--rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/pointsource_catalog_radec.png
--rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Images/pointsource_catalog_radec_concat.png
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/developer_docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/make_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/make_skymodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.643993 pyradiosky-0.3.1/docs/references/
--rw-r--r--   0 runner    (1001) docker     (127)   171209 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/references/skyh5_memo.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    15558 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/references/skyh5_memo.tex
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44095 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/docs/utility_functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.643993 pyradiosky-0.3.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/scripts/download_gleam.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/scripts/make_flat_spectrum_eor.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-22 18:01:47.663993 pyradiosky-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.631992 pyradiosky-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.643993 pyradiosky-0.3.1/src/pyradiosky/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.655992 pyradiosky-0.3.1/src/pyradiosky/data/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/extended_source_test.sav
--rw-r--r--   0 runner    (1001) docker     (127)   630964 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/fhd_catalog.sav
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/fhd_catalog_bad.sav
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/fhd_catalog_no_extend.sav
--rw-r--r--   0 runner    (1001) docker     (127)   574180 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/fhd_catalog_with_beam_values.sav
--rw-r--r--   0 runner    (1001) docker     (127)    62584 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/fhd_source_array.sav
--rw-r--r--   0 runner    (1001) docker     (127)    81302 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/gleam_50srcs.vot
--rw-r--r--   0 runner    (1001) docker     (127)   280816 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/gsm_galactic.skyh5
--rw-r--r--   0 runner    (1001) docker     (127)   280816 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/gsm_icrs.skyh5
--rw-r--r--   0 runner    (1001) docker     (127)  4055984 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/healpix_disk.skyh5
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/mock_hera_text_2458098.27471.txt
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/old_skyh5_point_sources.skyh5
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/pointsource_catalog.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/simple_test.vot
--rw-r--r--   0 runner    (1001) docker     (127)    19623 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/data/single_source_old.vot
--rw-r--r--   0 runner    (1001) docker     (127)   212563 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/skymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/spherical_coords_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/src/pyradiosky/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.659993 pyradiosky-0.3.1/src/pyradiosky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-02-22 18:01:47.000000 pyradiosky-0.3.1/src/pyradiosky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-02-22 18:01:47.000000 pyradiosky-0.3.1/src/pyradiosky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 18:01:47.000000 pyradiosky-0.3.1/src/pyradiosky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-22 18:01:47.000000 pyradiosky-0.3.1/src/pyradiosky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-22 18:01:47.000000 pyradiosky-0.3.1/src/pyradiosky.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:01:47.659993 pyradiosky-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)   141668 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/tests/test_skymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/tests/test_spherical_coords_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-02-22 18:01:08.000000 pyradiosky-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.655836 pyradiosky-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.631837 pyradiosky-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.631837 pyradiosky-1.0.0/.github/original_pr_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/original_pr_templates/bug_fix.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/original_pr_templates/build_ci_change.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/original_pr_templates/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/original_pr_templates/new_feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/original_pr_templates/other.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/original_pr_templates/version_change.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.631837 pyradiosky-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/workflows/externaltests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/workflows/publish-to-test-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.github/workflows/testsuite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-13 18:52:12.655836 pyradiosky-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.631837 pyradiosky-1.0.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/ci/full_deps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/ci/min_deps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/ci/min_versions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/ci/publish.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.635836 pyradiosky-1.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.639836 pyradiosky-1.0.0/docs/Images/
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/fhd_catalog_extended_models_fluxcounts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/fhd_catalog_extended_models_radec.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41347 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/fhd_catalog_extended_models_radec_picA.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/fhd_catalog_extended_models_refspec.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/fhd_catalog_specind_atfreqs.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gleam_50srcs_fluxcounts.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gleam_50srcs_fluxcounts_fluxselect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gleam_50srcs_freqflux.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34724 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gleam_50srcs_radec.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28175 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gleam_50srcs_radec_fluxselect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29353 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gleam_50srcs_radec_raselect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53618 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gleam_subband_spectra_atfreqs.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57457 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gsm_gal_coneselect_molliwede.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51002 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gsm_gal_neighborselect_molliwede.png
+-rw-r--r--   0 runner    (1001) docker     (127)   130348 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gsm_galactic_flux_molliwede.png
+-rw-r--r--   0 runner    (1001) docker     (127)   130557 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gsm_icrs_flux_molliwede.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gsm_icrs_fluxcounts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55631 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gsm_icrs_indselect_molliwede.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18703 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gsm_icrs_radec.png
+-rw-r--r--   0 runner    (1001) docker     (127)   133242 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/gsm_point_galactic_flux_molliwede.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/pointsource_catalog_radec.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Images/pointsource_catalog_radec_concat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/developer_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/make_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/make_skymodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.639836 pyradiosky-1.0.0/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (127)   171209 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/references/skyh5_memo.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    15558 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/references/skyh5_memo.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    44095 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/docs/utility_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.639836 pyradiosky-1.0.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/scripts/download_gleam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/scripts/make_flat_spectrum_eor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 18:52:12.655836 pyradiosky-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.627836 pyradiosky-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.639836 pyradiosky-1.0.0/src/pyradiosky/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.651836 pyradiosky-1.0.0/src/pyradiosky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/extended_source_test.sav
+-rw-r--r--   0 runner    (1001) docker     (127)   630964 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/fhd_catalog.sav
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/fhd_catalog_bad.sav
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/fhd_catalog_no_extend.sav
+-rw-r--r--   0 runner    (1001) docker     (127)   574180 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/fhd_catalog_with_beam_values.sav
+-rw-r--r--   0 runner    (1001) docker     (127)    62584 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/fhd_source_array.sav
+-rw-r--r--   0 runner    (1001) docker     (127)    81302 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/gleam_50srcs.vot
+-rw-r--r--   0 runner    (1001) docker     (127)   280816 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/gsm_galactic.skyh5
+-rw-r--r--   0 runner    (1001) docker     (127)   280816 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/gsm_icrs.skyh5
+-rw-r--r--   0 runner    (1001) docker     (127)  4055984 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/healpix_disk.skyh5
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/mock_hera_text_2458098.27471.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/old_skyh5_point_sources.skyh5
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/pointsource_catalog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/simple_test.vot
+-rw-r--r--   0 runner    (1001) docker     (127)    19623 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/data/single_source_old.vot
+-rw-r--r--   0 runner    (1001) docker     (127)   212679 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/spherical_coords_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/src/pyradiosky/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.651836 pyradiosky-1.0.0/src/pyradiosky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-13 18:52:12.000000 pyradiosky-1.0.0/src/pyradiosky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-13 18:52:12.000000 pyradiosky-1.0.0/src/pyradiosky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:52:12.000000 pyradiosky-1.0.0/src/pyradiosky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-13 18:52:12.000000 pyradiosky-1.0.0/src/pyradiosky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 18:52:12.000000 pyradiosky-1.0.0/src/pyradiosky.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:52:12.651836 pyradiosky-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141926 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/tests/test_skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/tests/test_spherical_coords_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-13 18:51:35.000000 pyradiosky-1.0.0/tests/test_utils.py
```

### Comparing `pyradiosky-0.3.1/.github/CONTRIBUTING.md` & `pyradiosky-1.0.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.github/PULL_REQUEST_TEMPLATE.md` & `pyradiosky-1.0.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.github/original_pr_templates/bug_fix.md` & `pyradiosky-1.0.0/.github/original_pr_templates/bug_fix.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.github/original_pr_templates/build_ci_change.md` & `pyradiosky-1.0.0/.github/original_pr_templates/build_ci_change.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.github/original_pr_templates/documentation.md` & `pyradiosky-1.0.0/.github/original_pr_templates/documentation.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.github/original_pr_templates/new_feature.md` & `pyradiosky-1.0.0/.github/original_pr_templates/new_feature.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.github/original_pr_templates/other.md` & `pyradiosky-1.0.0/.github/original_pr_templates/other.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.github/original_pr_templates/version_change.md` & `pyradiosky-1.0.0/.github/original_pr_templates/version_change.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.github/workflows/externaltests.yaml` & `pyradiosky-1.0.0/.github/workflows/externaltests.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     name: pyuvsim
     runs-on: ubuntu-latest
     defaults:
       run:
         # Adding -l {0} helps ensure conda can be found properly.
         shell: bash -l {0}
     env:
-      ENV_NAME: pyuvsim_tests
+      ENV_NAME: pyuvsim_tests_openmpi
       PYTHON: "3.11"
 
     steps:
       - uses: actions/checkout@main
         with:
           fetch-depth: 0
 
@@ -50,8 +50,8 @@
       - name: run pyuvsim tests
         run: |
           pip install --no-deps .
           cd ../
           cd pyuvsim
           pip install --no-deps .
           mkdir test-reports
-          python -m pytest pyuvsim --junitxml=test-reports/xunit.xml
+          python -m pytest --junitxml=test-reports/xunit.xml
```

### Comparing `pyradiosky-0.3.1/.github/workflows/publish-to-test-pypi.yaml` & `pyradiosky-1.0.0/.github/workflows/publish-to-test-pypi.yaml`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.github/workflows/testsuite.yaml` & `pyradiosky-1.0.0/.github/workflows/testsuite.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       run:
         # Adding -l {0} helps ensure conda can be found properly.
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.9, "3.10", "3.11", "3.12"]
+        python-version: ["3.10", "3.11", "3.12"]
     steps:
       - uses: actions/checkout@main
         with:
           fetch-depth: 1
 
       - name: Setup Minimamba
         uses: conda-incubator/setup-miniconda@v2
@@ -119,15 +119,15 @@
         with:
           token: ${{secrets.CODECOV_TOKEN}} #required
           files: ./coverage.xml #optional
 
   min_versions:
     env:
       ENV_NAME: min_versions
-      PYTHON: 3.9
+      PYTHON: "3.10"
     name: Min Versions Testing
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     defaults:
       run:
         # Adding -l {0} helps ensure conda can be found properly.
@@ -174,15 +174,15 @@
         with:
           token: ${{secrets.CODECOV_TOKEN}} #required
           files: ./coverage.xml #optional
 
   # Use pip for diversity
   warning_test:
     env:
-      PYTHON: "3.10"
+      PYTHON: "3.11"
     name: Warning Test
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@main
         with:
           fetch-depth: 0
```

### Comparing `pyradiosky-0.3.1/.gitignore` & `pyradiosky-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/.pre-commit-config.yaml` & `pyradiosky-1.0.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: '(^docs/conf.py|^user_data/External_tables/)'
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
         - id: trailing-whitespace
         - id: check-added-large-files
         - id: check-ast
         - id: check-json
         - id: check-merge-conflict
         - id: check-xml
@@ -25,20 +25,20 @@
           - flake8-comprehensions
           - flake8-docstrings
           - flake8-pytest-style
           - flake8-rst-docstrings
           - pep8-naming
 
   - repo: https://github.com/psf/black
-    rev: 24.2.0
+    rev: 24.4.2
     hooks:
         - id: black
 
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.7
+    rev: 1.7.8
     hooks:
       - id: bandit
         args: [--skip, "B101", --recursive, pyuvdata]
 
   - repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
```

### Comparing `pyradiosky-0.3.1/.readthedocs.yml` & `pyradiosky-1.0.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/CHANGELOG.md` & `pyradiosky-1.0.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 ## [Unreleased]
 
+## [1.0.0] - 2024-05-09
+
+### Changed
+- Updated minimum dependency versions: astropy>=6.0, h5py>=3.4, numpy>=1.23,
+pyuvdata>=2.4.3, scipy>=1.7.3, python>=3.10
+- Updated minimum optional dependency versions: astropy-healpix>=1.0.2, lunarsky>=0.2.2
+
 ## [0.3.1] - 2024-02-22
 
 ### Added
 - A memo describing the SkyH5 format in docs/references.
 
 ### Changed
 - Added support for more types of FHD catalog files and better error messages.
```

### Comparing `pyradiosky-0.3.1/CODE_OF_CONDUCT.md` & `pyradiosky-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/LICENSE` & `pyradiosky-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/PKG-INFO` & `pyradiosky-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 Metadata-Version: 2.1
 Name: pyradiosky
-Version: 0.3.1
+Version: 1.0.0
 Summary: Python objects and interfaces for representing diffuse, extended and compact astrophysical radio sources
 Home-page: https://github.com/RadioAstronomySoftwareGroup/pyradiosky
 Author: Radio Astronomy Software Group
 License: BSD
 Keywords: radio astronomy
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.20
-Requires-Dist: scipy>=1.5
-Requires-Dist: astropy>=5.2
-Requires-Dist: h5py>=3.1
-Requires-Dist: pyuvdata>=2.4.1
+Requires-Dist: astropy>=6.0
+Requires-Dist: h5py>=3.4
+Requires-Dist: numpy>=1.23
+Requires-Dist: pyuvdata>=2.4.3
+Requires-Dist: scipy>=1.7.3
+Requires-Dist: setuptools>=61
 Requires-Dist: setuptools_scm>=7.0.3
 Provides-Extra: healpix
-Requires-Dist: astropy-healpix>=0.6; extra == "healpix"
+Requires-Dist: astropy-healpix>=1.0.2; extra == "healpix"
 Provides-Extra: astroquery
 Requires-Dist: astroquery>=0.4.4; extra == "astroquery"
 Provides-Extra: lunarsky
-Requires-Dist: lunarsky>=0.2.1; extra == "lunarsky"
+Requires-Dist: lunarsky>=0.2.2; extra == "lunarsky"
 Provides-Extra: all
-Requires-Dist: astropy-healpix>=0.6; extra == "all"
+Requires-Dist: astropy-healpix>=1.0.2; extra == "all"
 Requires-Dist: astroquery>=0.4.4; extra == "all"
-Requires-Dist: lunarsky>=0.2.1; extra == "all"
+Requires-Dist: lunarsky>=0.2.2; extra == "all"
 Provides-Extra: test
-Requires-Dist: astropy-healpix>=0.6; extra == "test"
+Requires-Dist: astropy-healpix>=1.0.2; extra == "test"
 Requires-Dist: astroquery>=0.4.4; extra == "test"
-Requires-Dist: lunarsky>=0.2.1; extra == "test"
+Requires-Dist: lunarsky>=0.2.2; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: doc
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: pypandoc; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Provides-Extra: dev
-Requires-Dist: astropy-healpix>=0.6; extra == "dev"
+Requires-Dist: astropy-healpix>=1.0.2; extra == "dev"
 Requires-Dist: astroquery>=0.4.4; extra == "dev"
-Requires-Dist: lunarsky>=0.2.1; extra == "dev"
+Requires-Dist: lunarsky>=0.2.2; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: pypandoc; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
@@ -59,22 +60,20 @@
 # pyradiosky
 ![](https://github.com/RadioAstronomySoftwareGroup/pyradiosky/workflows/Tests/badge.svg?branch=main)
 [![codecov](https://codecov.io/gh/RadioAstronomySoftwareGroup/pyradiosky/branch/main/graph/badge.svg)](https://codecov.io/gh/RadioAstronomySoftwareGroup/pyradiosky)
 
 Python objects and interfaces for representing diffuse, extended and compact
 astrophysical radio sources.
 
-pyradiosky is currently in a very early development stage, interfaces are changing rapidly.
-
 The primary user class is `SkyModel`, which supports:
 
   - catalogs of point sources (read/write to hd5 and text files, read VOTables)
   - diffuse models as HEALPix maps (read/write to hd5 files)
-  - conversion between RA/Dec and Azimuth/Elevation including calculating full
-  polarization coherencies in Az/El.
+  - conversion between any astropy supported coordinates (e.g. J2000 RA/Dec) and
+  Azimuth/Elevation including calculating full polarization coherencies in Az/El.
 
 # File formats
 
 pyradiosky supports reading in catalogs from several formats, including VO Table files,
 text files, [FHD](https://github.com/EoRImaging/FHD) catalog files and SkyH5 files and
 supports writing to SkyH5 and text files. SkyH5 is an HDF5-based file format defined by
 the pyradiosky team, a full description is in the [SkyH5 memo](docs/references/skyh5_memo.pdf).
@@ -84,19 +83,18 @@
 issues in the [issue log](https://github.com/RadioAstronomySoftwareGroup/pyradiosky/issues)
 are very welcome, as are bug reports and feature requests.
 Please see our [guide on contributing](.github/CONTRIBUTING.md)
 
 # Versioning
 We use a `generation.major.minor` version number format. We use the `generation`
 number for very significant improvements or major rewrites, the `major` number
-to indicate substantial package changes (intended to be released every ~6 months)
-and the `minor` number to release smaller incremental updates (intended to be
-released approximately monthly and which usually do not include breaking API
-changes). We do our best to provide a significant period (usually 2 major
-generations) of deprecation warnings for all breaking changes to the API.
+to indicate substantial package changes and the `minor` number to release smaller
+incremental updates (which do not include breaking API changes). We do our best
+to provide a significant period (usually 2 major generations) of deprecation
+warnings for all breaking changes to the API.
 We track all changes in our [changelog](https://github.com/RadioAstronomySoftwareGroup/pyradiosky/blob/main/CHANGELOG.md).
 
 # Documentation
 Developer API documentation is hosted [here](https://pyradiosky.readthedocs.io/en/latest/).
 
 # Installation
 Simple installation via pip is available for users, developers should follow
@@ -112,26 +110,26 @@
 ## Dependencies
 
 If you are using `conda` to manage your environment, you may wish to install the
 following packages before installing `pyradiosky`:
 
 Required:
 
-* astropy>=5.2
-* h5py>=3.1
-* numpy>=1.20
-* scipy>=1.5
-* pyuvdata>=2.4.1
+* astropy>=6.0
+* h5py>=3.4
+* numpy>=1.23
+* scipy>=1.7.3
+* pyuvdata>=2.4.3
 * setuptools_scm>=7.0.3
 
 Optional:
 
-* astropy-healpix>=0.6 (for working with beams in HEALPix formats)
+* astropy-healpix>=1.0.2 (for working with beams in HEALPix formats)
 * astroquery>=0.4.4 (for downloading GLEAM and other VizieR catalogs)
-* lunarsky>=0.2.1 (for supporting telescope locations on the moon)
+* lunarsky>=0.2.2 (for supporting telescope locations on the moon)
 
 We suggest using conda to install all the dependencies. To install
 pyuvdata, astropy-healpix and astroquery, you'll need to add conda-forge as a channel
 (```conda config --add channels conda-forge```).
 
 If you do not want to use conda, the packages are also available on PyPI.
 You can install the optional dependencies via pip by specifying an option
@@ -174,15 +172,15 @@
 and documentation development.
 
 To use pre-commit to prevent committing code that does not follow our style,
 you'll need to run `pre-commit install` in the top level `pyradiosky` directory.
 
 # Tests
 Uses the `pytest` package to execute test suite.
-From the source pyradiosky directory run ```pytest``` or ```python -m pytest```.
+From the pyradiosky directory run ```pytest``` or ```python -m pytest```.
 
 # Maintainers
 pyradiosky is maintained by the RASG Managers, which currently include:
 
  - Adam Beardsley (Arizona State University)
  - Bryna Hazelton (University of Washington)
  - Daniel Jacobs (Arizona State University)
```

### Comparing `pyradiosky-0.3.1/README.md` & `pyradiosky-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # pyradiosky
 ![](https://github.com/RadioAstronomySoftwareGroup/pyradiosky/workflows/Tests/badge.svg?branch=main)
 [![codecov](https://codecov.io/gh/RadioAstronomySoftwareGroup/pyradiosky/branch/main/graph/badge.svg)](https://codecov.io/gh/RadioAstronomySoftwareGroup/pyradiosky)
 
 Python objects and interfaces for representing diffuse, extended and compact
 astrophysical radio sources.
 
-pyradiosky is currently in a very early development stage, interfaces are changing rapidly.
-
 The primary user class is `SkyModel`, which supports:
 
   - catalogs of point sources (read/write to hd5 and text files, read VOTables)
   - diffuse models as HEALPix maps (read/write to hd5 files)
-  - conversion between RA/Dec and Azimuth/Elevation including calculating full
-  polarization coherencies in Az/El.
+  - conversion between any astropy supported coordinates (e.g. J2000 RA/Dec) and
+  Azimuth/Elevation including calculating full polarization coherencies in Az/El.
 
 # File formats
 
 pyradiosky supports reading in catalogs from several formats, including VO Table files,
 text files, [FHD](https://github.com/EoRImaging/FHD) catalog files and SkyH5 files and
 supports writing to SkyH5 and text files. SkyH5 is an HDF5-based file format defined by
 the pyradiosky team, a full description is in the [SkyH5 memo](docs/references/skyh5_memo.pdf).
@@ -26,19 +24,18 @@
 issues in the [issue log](https://github.com/RadioAstronomySoftwareGroup/pyradiosky/issues)
 are very welcome, as are bug reports and feature requests.
 Please see our [guide on contributing](.github/CONTRIBUTING.md)
 
 # Versioning
 We use a `generation.major.minor` version number format. We use the `generation`
 number for very significant improvements or major rewrites, the `major` number
-to indicate substantial package changes (intended to be released every ~6 months)
-and the `minor` number to release smaller incremental updates (intended to be
-released approximately monthly and which usually do not include breaking API
-changes). We do our best to provide a significant period (usually 2 major
-generations) of deprecation warnings for all breaking changes to the API.
+to indicate substantial package changes and the `minor` number to release smaller
+incremental updates (which do not include breaking API changes). We do our best
+to provide a significant period (usually 2 major generations) of deprecation
+warnings for all breaking changes to the API.
 We track all changes in our [changelog](https://github.com/RadioAstronomySoftwareGroup/pyradiosky/blob/main/CHANGELOG.md).
 
 # Documentation
 Developer API documentation is hosted [here](https://pyradiosky.readthedocs.io/en/latest/).
 
 # Installation
 Simple installation via pip is available for users, developers should follow
@@ -54,26 +51,26 @@
 ## Dependencies
 
 If you are using `conda` to manage your environment, you may wish to install the
 following packages before installing `pyradiosky`:
 
 Required:
 
-* astropy>=5.2
-* h5py>=3.1
-* numpy>=1.20
-* scipy>=1.5
-* pyuvdata>=2.4.1
+* astropy>=6.0
+* h5py>=3.4
+* numpy>=1.23
+* scipy>=1.7.3
+* pyuvdata>=2.4.3
 * setuptools_scm>=7.0.3
 
 Optional:
 
-* astropy-healpix>=0.6 (for working with beams in HEALPix formats)
+* astropy-healpix>=1.0.2 (for working with beams in HEALPix formats)
 * astroquery>=0.4.4 (for downloading GLEAM and other VizieR catalogs)
-* lunarsky>=0.2.1 (for supporting telescope locations on the moon)
+* lunarsky>=0.2.2 (for supporting telescope locations on the moon)
 
 We suggest using conda to install all the dependencies. To install
 pyuvdata, astropy-healpix and astroquery, you'll need to add conda-forge as a channel
 (```conda config --add channels conda-forge```).
 
 If you do not want to use conda, the packages are also available on PyPI.
 You can install the optional dependencies via pip by specifying an option
@@ -116,15 +113,15 @@
 and documentation development.
 
 To use pre-commit to prevent committing code that does not follow our style,
 you'll need to run `pre-commit install` in the top level `pyradiosky` directory.
 
 # Tests
 Uses the `pytest` package to execute test suite.
-From the source pyradiosky directory run ```pytest``` or ```python -m pytest```.
+From the pyradiosky directory run ```pytest``` or ```python -m pytest```.
 
 # Maintainers
 pyradiosky is maintained by the RASG Managers, which currently include:
 
  - Adam Beardsley (Arizona State University)
  - Bryna Hazelton (University of Washington)
  - Daniel Jacobs (Arizona State University)
```

### Comparing `pyradiosky-0.3.1/docs/Images/fhd_catalog_extended_models_fluxcounts.png` & `pyradiosky-1.0.0/docs/Images/fhd_catalog_extended_models_fluxcounts.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/fhd_catalog_extended_models_radec.png` & `pyradiosky-1.0.0/docs/Images/fhd_catalog_extended_models_radec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/fhd_catalog_extended_models_radec_picA.png` & `pyradiosky-1.0.0/docs/Images/fhd_catalog_extended_models_radec_picA.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/fhd_catalog_extended_models_refspec.png` & `pyradiosky-1.0.0/docs/Images/fhd_catalog_extended_models_refspec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/fhd_catalog_specind_atfreqs.png` & `pyradiosky-1.0.0/docs/Images/fhd_catalog_specind_atfreqs.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gleam_50srcs_fluxcounts.png` & `pyradiosky-1.0.0/docs/Images/gleam_50srcs_fluxcounts.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gleam_50srcs_fluxcounts_fluxselect.png` & `pyradiosky-1.0.0/docs/Images/gleam_50srcs_fluxcounts_fluxselect.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gleam_50srcs_freqflux.png` & `pyradiosky-1.0.0/docs/Images/gleam_50srcs_freqflux.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gleam_50srcs_radec.png` & `pyradiosky-1.0.0/docs/Images/gleam_50srcs_radec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gleam_50srcs_radec_fluxselect.png` & `pyradiosky-1.0.0/docs/Images/gleam_50srcs_radec_fluxselect.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gleam_50srcs_radec_raselect.png` & `pyradiosky-1.0.0/docs/Images/gleam_50srcs_radec_raselect.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gleam_subband_spectra_atfreqs.png` & `pyradiosky-1.0.0/docs/Images/gleam_subband_spectra_atfreqs.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gsm_gal_coneselect_molliwede.png` & `pyradiosky-1.0.0/docs/Images/gsm_gal_coneselect_molliwede.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gsm_gal_neighborselect_molliwede.png` & `pyradiosky-1.0.0/docs/Images/gsm_gal_neighborselect_molliwede.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gsm_galactic_flux_molliwede.png` & `pyradiosky-1.0.0/docs/Images/gsm_galactic_flux_molliwede.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gsm_icrs_flux_molliwede.png` & `pyradiosky-1.0.0/docs/Images/gsm_icrs_flux_molliwede.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gsm_icrs_fluxcounts.png` & `pyradiosky-1.0.0/docs/Images/gsm_icrs_fluxcounts.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gsm_icrs_indselect_molliwede.png` & `pyradiosky-1.0.0/docs/Images/gsm_icrs_indselect_molliwede.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gsm_icrs_radec.png` & `pyradiosky-1.0.0/docs/Images/gsm_icrs_radec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/gsm_point_galactic_flux_molliwede.png` & `pyradiosky-1.0.0/docs/Images/gsm_point_galactic_flux_molliwede.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/pointsource_catalog_radec.png` & `pyradiosky-1.0.0/docs/Images/pointsource_catalog_radec.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Images/pointsource_catalog_radec_concat.png` & `pyradiosky-1.0.0/docs/Images/pointsource_catalog_radec_concat.png`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/Makefile` & `pyradiosky-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/conf.py` & `pyradiosky-1.0.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,8 +159,9 @@
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "pyuvdata": ("https://pyuvdata.readthedocs.io/en/latest/", None),
     "astropy": ("https://docs.astropy.org/en/stable/", None),
     "astropy_healpix": ("https://astropy-healpix.readthedocs.io/en/latest/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
+    # "lunarsky": (None), lunarsky is not on RTD yet. Add it here when it is.
 }
```

### Comparing `pyradiosky-0.3.1/docs/conftest.py` & `pyradiosky-1.0.0/docs/conftest.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/make.bat` & `pyradiosky-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/make_index.py` & `pyradiosky-1.0.0/docs/make_index.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/make_skymodel.py` & `pyradiosky-1.0.0/docs/make_skymodel.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/references/skyh5_memo.pdf` & `pyradiosky-1.0.0/docs/references/skyh5_memo.pdf`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/references/skyh5_memo.tex` & `pyradiosky-1.0.0/docs/references/skyh5_memo.tex`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/docs/tutorial.rst` & `pyradiosky-1.0.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/scripts/download_gleam.py` & `pyradiosky-1.0.0/scripts/download_gleam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /usr/bin/env python
 # Copyright (c) 2019 Radio Astronomy Software Group
-# Licensed under the 3-clause BSD License
+# Licensed under the 2-clause BSD License
 
 """Download the gleam catalog as a VOTable from Vizier."""
 
 import argparse
 
 import pyradiosky.utils as utils
```

### Comparing `pyradiosky-0.3.1/scripts/make_flat_spectrum_eor.py` & `pyradiosky-1.0.0/scripts/make_flat_spectrum_eor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-#!/bin/env python
+#! /usr/bin/env python
+# Copyright (c) 2024 Radio Astronomy Software Group
+# Licensed under the 2-clause BSD License
 
 """Utility function for making noiselike EoR models."""
 
 
 import argparse
 
 import numpy as np
```

### Comparing `pyradiosky-0.3.1/setup.py` & `pyradiosky-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         else:
             return version.format_choice("+{node}.{branch}", "+{node}.{branch}.dirty")
 
 
 with io.open("README.md", "r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
-healpix_reqs = ["astropy-healpix>=0.6"]
+healpix_reqs = ["astropy-healpix>=1.0.2"]
 astroquery_reqs = ["astroquery>=0.4.4"]
-lunarsky_reqs = ["lunarsky>=0.2.1"]
+lunarsky_reqs = ["lunarsky>=0.2.2"]
 all_optional_reqs = healpix_reqs + astroquery_reqs + lunarsky_reqs
 
 doc_reqs = ["matplotlib", "pypandoc", "sphinx"]
 test_reqs = all_optional_reqs + ["coverage", "pre-commit", "pytest", "pytest-cov"]
 
 
 setup_args = {
@@ -47,20 +47,22 @@
     "long_description": readme,
     "long_description_content_type": "text/markdown",
     "package_dir": {"": "src"},
     "packages": find_packages(where="src"),
     "scripts": glob.glob("scripts/*"),
     "use_scm_version": {"local_scheme": branch_scheme},
     "include_package_data": True,
+    "python_requires": ">=3.10",
     "install_requires": [
-        "numpy>=1.20",
-        "scipy>=1.5",
-        "astropy>=5.2",
-        "h5py>=3.1",
-        "pyuvdata>=2.4.1",
+        "astropy>=6.0",
+        "h5py>=3.4",
+        "numpy>=1.23",
+        "pyuvdata>=2.4.3",
+        "scipy>=1.7.3",
+        "setuptools>=61",
         "setuptools_scm>=7.0.3",
     ],
     "extras_require": {
         "healpix": healpix_reqs,
         "astroquery": astroquery_reqs,
         "lunarsky": lunarsky_reqs,
         "all": all_optional_reqs,
@@ -68,15 +70,14 @@
         "doc": doc_reqs,
         "dev": test_reqs + doc_reqs,
     },
     "classifiers": [
         "Development Status :: 1 - Planning",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering :: Astronomy",
     ],
     "keywords": "radio astronomy",
 }
```

### Comparing `pyradiosky-0.3.1/src/pyradiosky/__init__.py` & `pyradiosky-1.0.0/src/pyradiosky/__init__.py`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/extended_source_test.sav` & `pyradiosky-1.0.0/src/pyradiosky/data/extended_source_test.sav`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/fhd_catalog.sav` & `pyradiosky-1.0.0/src/pyradiosky/data/fhd_catalog.sav`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/fhd_catalog_bad.sav` & `pyradiosky-1.0.0/src/pyradiosky/data/fhd_catalog_bad.sav`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/fhd_catalog_no_extend.sav` & `pyradiosky-1.0.0/src/pyradiosky/data/fhd_catalog_no_extend.sav`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/fhd_catalog_with_beam_values.sav` & `pyradiosky-1.0.0/src/pyradiosky/data/fhd_catalog_with_beam_values.sav`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/fhd_source_array.sav` & `pyradiosky-1.0.0/src/pyradiosky/data/fhd_source_array.sav`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/gleam_50srcs.vot` & `pyradiosky-1.0.0/src/pyradiosky/data/gleam_50srcs.vot`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/gsm_galactic.skyh5` & `pyradiosky-1.0.0/src/pyradiosky/data/gsm_galactic.skyh5`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/gsm_icrs.skyh5` & `pyradiosky-1.0.0/src/pyradiosky/data/gsm_icrs.skyh5`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/healpix_disk.skyh5` & `pyradiosky-1.0.0/src/pyradiosky/data/healpix_disk.skyh5`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/mock_hera_text_2458098.27471.txt` & `pyradiosky-1.0.0/src/pyradiosky/data/mock_hera_text_2458098.27471.txt`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/old_skyh5_point_sources.skyh5` & `pyradiosky-1.0.0/src/pyradiosky/data/old_skyh5_point_sources.skyh5`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/simple_test.vot` & `pyradiosky-1.0.0/src/pyradiosky/data/simple_test.vot`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/data/single_source_old.vot` & `pyradiosky-1.0.0/src/pyradiosky/data/single_source_old.vot`

 * *Files identical despite different names*

### Comparing `pyradiosky-0.3.1/src/pyradiosky/skymodel.py` & `pyradiosky-1.0.0/src/pyradiosky/skymodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- mode: python; coding: utf-8 -*
 # Copyright (c) 2019 Radio Astronomy Software Group
-# Licensed under the 3-clause BSD License
+# Licensed under the 2-clause BSD License
 """Define SkyModel class and helper functions."""
 
 import os
 import re
 import warnings
 
 import astropy.units as units
@@ -2321,16 +2321,18 @@
             * ``alt_az``
             * ``time``
 
         Parameters
         ----------
         time : :class:`astropy.time.Time`
             Time to update positions for.
-        telescope_location : :class:`astropy.coordinates.EarthLocation`
-            Telescope location to update positions for.
+        telescope_location : EarthLocation or MoonLocation
+            Telescope location to update positions for, must be either an
+            :class:`astropy.coordinates.EarthLocation` or a
+            :class:`lunarsky.MoonLocation` object.
         """
         if not isinstance(time, Time):
             raise ValueError(
                 "time must be an astropy Time object. value was: {t}".format(t=time)
             )
 
         if not (
```

### Comparing `pyradiosky-0.3.1/src/pyradiosky/spherical_coords_transforms.py` & `pyradiosky-1.0.0/src/pyradiosky/spherical_coords_transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- mode: python; coding: utf-8 -*
 # Copyright (c) 2019 Radio Astronomy Software Group
-# Licensed under the 3-clause BSD License
+# Licensed under the 2-clause BSD License
 """Methods for doing spherical coordinate transformations on vectors."""
 
 import numpy as np
 
 
 def r_hat(theta, phi):
     """
```

### Comparing `pyradiosky-0.3.1/src/pyradiosky/utils.py` & `pyradiosky-1.0.0/src/pyradiosky/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- mode: python; coding: utf-8 -*
 # Copyright (c) 2019 Radio Astronomy Software Group
-# Licensed under the 3-clause BSD License
+# Licensed under the 2-clause BSD License
 """Utility methods."""
 import os
 
 import astropy.units as units
 import erfa
 import numpy as np
 from astropy.coordinates import Angle
```

### Comparing `pyradiosky-0.3.1/src/pyradiosky.egg-info/PKG-INFO` & `pyradiosky-1.0.0/src/pyradiosky.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 Metadata-Version: 2.1
 Name: pyradiosky
-Version: 0.3.1
+Version: 1.0.0
 Summary: Python objects and interfaces for representing diffuse, extended and compact astrophysical radio sources
 Home-page: https://github.com/RadioAstronomySoftwareGroup/pyradiosky
 Author: Radio Astronomy Software Group
 License: BSD
 Keywords: radio astronomy
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.20
-Requires-Dist: scipy>=1.5
-Requires-Dist: astropy>=5.2
-Requires-Dist: h5py>=3.1
-Requires-Dist: pyuvdata>=2.4.1
+Requires-Dist: astropy>=6.0
+Requires-Dist: h5py>=3.4
+Requires-Dist: numpy>=1.23
+Requires-Dist: pyuvdata>=2.4.3
+Requires-Dist: scipy>=1.7.3
+Requires-Dist: setuptools>=61
 Requires-Dist: setuptools_scm>=7.0.3
 Provides-Extra: healpix
-Requires-Dist: astropy-healpix>=0.6; extra == "healpix"
+Requires-Dist: astropy-healpix>=1.0.2; extra == "healpix"
 Provides-Extra: astroquery
 Requires-Dist: astroquery>=0.4.4; extra == "astroquery"
 Provides-Extra: lunarsky
-Requires-Dist: lunarsky>=0.2.1; extra == "lunarsky"
+Requires-Dist: lunarsky>=0.2.2; extra == "lunarsky"
 Provides-Extra: all
-Requires-Dist: astropy-healpix>=0.6; extra == "all"
+Requires-Dist: astropy-healpix>=1.0.2; extra == "all"
 Requires-Dist: astroquery>=0.4.4; extra == "all"
-Requires-Dist: lunarsky>=0.2.1; extra == "all"
+Requires-Dist: lunarsky>=0.2.2; extra == "all"
 Provides-Extra: test
-Requires-Dist: astropy-healpix>=0.6; extra == "test"
+Requires-Dist: astropy-healpix>=1.0.2; extra == "test"
 Requires-Dist: astroquery>=0.4.4; extra == "test"
-Requires-Dist: lunarsky>=0.2.1; extra == "test"
+Requires-Dist: lunarsky>=0.2.2; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: doc
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: pypandoc; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Provides-Extra: dev
-Requires-Dist: astropy-healpix>=0.6; extra == "dev"
+Requires-Dist: astropy-healpix>=1.0.2; extra == "dev"
 Requires-Dist: astroquery>=0.4.4; extra == "dev"
-Requires-Dist: lunarsky>=0.2.1; extra == "dev"
+Requires-Dist: lunarsky>=0.2.2; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: pypandoc; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
@@ -59,22 +60,20 @@
 # pyradiosky
 ![](https://github.com/RadioAstronomySoftwareGroup/pyradiosky/workflows/Tests/badge.svg?branch=main)
 [![codecov](https://codecov.io/gh/RadioAstronomySoftwareGroup/pyradiosky/branch/main/graph/badge.svg)](https://codecov.io/gh/RadioAstronomySoftwareGroup/pyradiosky)
 
 Python objects and interfaces for representing diffuse, extended and compact
 astrophysical radio sources.
 
-pyradiosky is currently in a very early development stage, interfaces are changing rapidly.
-
 The primary user class is `SkyModel`, which supports:
 
   - catalogs of point sources (read/write to hd5 and text files, read VOTables)
   - diffuse models as HEALPix maps (read/write to hd5 files)
-  - conversion between RA/Dec and Azimuth/Elevation including calculating full
-  polarization coherencies in Az/El.
+  - conversion between any astropy supported coordinates (e.g. J2000 RA/Dec) and
+  Azimuth/Elevation including calculating full polarization coherencies in Az/El.
 
 # File formats
 
 pyradiosky supports reading in catalogs from several formats, including VO Table files,
 text files, [FHD](https://github.com/EoRImaging/FHD) catalog files and SkyH5 files and
 supports writing to SkyH5 and text files. SkyH5 is an HDF5-based file format defined by
 the pyradiosky team, a full description is in the [SkyH5 memo](docs/references/skyh5_memo.pdf).
@@ -84,19 +83,18 @@
 issues in the [issue log](https://github.com/RadioAstronomySoftwareGroup/pyradiosky/issues)
 are very welcome, as are bug reports and feature requests.
 Please see our [guide on contributing](.github/CONTRIBUTING.md)
 
 # Versioning
 We use a `generation.major.minor` version number format. We use the `generation`
 number for very significant improvements or major rewrites, the `major` number
-to indicate substantial package changes (intended to be released every ~6 months)
-and the `minor` number to release smaller incremental updates (intended to be
-released approximately monthly and which usually do not include breaking API
-changes). We do our best to provide a significant period (usually 2 major
-generations) of deprecation warnings for all breaking changes to the API.
+to indicate substantial package changes and the `minor` number to release smaller
+incremental updates (which do not include breaking API changes). We do our best
+to provide a significant period (usually 2 major generations) of deprecation
+warnings for all breaking changes to the API.
 We track all changes in our [changelog](https://github.com/RadioAstronomySoftwareGroup/pyradiosky/blob/main/CHANGELOG.md).
 
 # Documentation
 Developer API documentation is hosted [here](https://pyradiosky.readthedocs.io/en/latest/).
 
 # Installation
 Simple installation via pip is available for users, developers should follow
@@ -112,26 +110,26 @@
 ## Dependencies
 
 If you are using `conda` to manage your environment, you may wish to install the
 following packages before installing `pyradiosky`:
 
 Required:
 
-* astropy>=5.2
-* h5py>=3.1
-* numpy>=1.20
-* scipy>=1.5
-* pyuvdata>=2.4.1
+* astropy>=6.0
+* h5py>=3.4
+* numpy>=1.23
+* scipy>=1.7.3
+* pyuvdata>=2.4.3
 * setuptools_scm>=7.0.3
 
 Optional:
 
-* astropy-healpix>=0.6 (for working with beams in HEALPix formats)
+* astropy-healpix>=1.0.2 (for working with beams in HEALPix formats)
 * astroquery>=0.4.4 (for downloading GLEAM and other VizieR catalogs)
-* lunarsky>=0.2.1 (for supporting telescope locations on the moon)
+* lunarsky>=0.2.2 (for supporting telescope locations on the moon)
 
 We suggest using conda to install all the dependencies. To install
 pyuvdata, astropy-healpix and astroquery, you'll need to add conda-forge as a channel
 (```conda config --add channels conda-forge```).
 
 If you do not want to use conda, the packages are also available on PyPI.
 You can install the optional dependencies via pip by specifying an option
@@ -174,15 +172,15 @@
 and documentation development.
 
 To use pre-commit to prevent committing code that does not follow our style,
 you'll need to run `pre-commit install` in the top level `pyradiosky` directory.
 
 # Tests
 Uses the `pytest` package to execute test suite.
-From the source pyradiosky directory run ```pytest``` or ```python -m pytest```.
+From the pyradiosky directory run ```pytest``` or ```python -m pytest```.
 
 # Maintainers
 pyradiosky is maintained by the RASG Managers, which currently include:
 
  - Adam Beardsley (Arizona State University)
  - Bryna Hazelton (University of Washington)
  - Daniel Jacobs (Arizona State University)
```

### Comparing `pyradiosky-0.3.1/src/pyradiosky.egg-info/SOURCES.txt` & `pyradiosky-1.0.0/src/pyradiosky.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 .readthedocs.yml
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.md
 environment.yaml
+paper.bib
+paper.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/CONTRIBUTING.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/original_pr_templates/bug_fix.md
 .github/original_pr_templates/build_ci_change.md
```

### Comparing `pyradiosky-0.3.1/tests/conftest.py` & `pyradiosky-1.0.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- mode: python; coding: utf-8 -*
 # Copyright (c) 2020 Radio Astronomy Software Group
-# Licensed under the 3-clause BSD License
+# Licensed under the 2-clause BSD License
 
 import pytest
 from astropy.time import Time
 from astropy.utils import iers
 
 
 @pytest.fixture(autouse=True, scope="session")
```

### Comparing `pyradiosky-0.3.1/tests/test_skymodel.py` & `pyradiosky-1.0.0/tests/test_skymodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- mode: python; coding: utf-8 -*
 # Copyright (c) 2019 Radio Astronomy Software Group
-# Licensed under the 3-clause BSD License
+# Licensed under the 2-clause BSD License
 
 import copy
 import fileinput
 import os
 import re
 import warnings
 
@@ -95,14 +95,15 @@
 
 @pytest.fixture
 def moonsky():
     pytest.importorskip("lunarsky")
 
     from lunarsky import MoonLocation
     from lunarsky import SkyCoord as LunarSkyCoord
+    from spiceypy.utils.exceptions import SpiceUNKNOWNFRAME
 
     # Tranquility base
     array_location = MoonLocation(lat="00d41m15s", lon="23d26m00s", height=0.0)
 
     time = Time.now()
     zen_coord = LunarSkyCoord(
         alt=Angle(90, unit=units.deg),
@@ -115,16 +116,18 @@
     icrs_coord = zen_coord.transform_to("icrs")
 
     names = "zen_source"
     stokes = [1.0, 0, 0, 0] * units.Jy
     zenith_source = SkyModel(
         name=names, skycoord=icrs_coord, stokes=stokes, spectral_type="flat"
     )
-
-    zenith_source.update_positions(time, array_location)
+    try:
+        zenith_source.update_positions(time, array_location)
+    except SpiceUNKNOWNFRAME as err:
+        pytest.skip("SpiceUNKNOWNFRAME error: " + str(err))
 
     yield zenith_source
 
 
 @pytest.fixture
 def healpix_data():
     astropy_healpix = pytest.importorskip("astropy_healpix")
@@ -2081,16 +2084,14 @@
 
     src_l = np.sin(src_az.rad) * np.sin(src_za.rad)
     src_m = np.cos(src_az.rad) * np.sin(src_za.rad)
     src_n = np.cos(src_za.rad)
 
     sky2 = SkyModel.from_file(filename)
 
-    time.location = array_location
-
     sky2.update_positions(time, array_location)
     src_alt_az = sky2.alt_az
     assert np.isclose(src_alt_az[0][ipix], src_alt.rad)
     assert np.isclose(src_alt_az[1][ipix], src_az.rad)
 
     src_lmn = sky2.pos_lmn
     assert np.isclose(src_lmn[0][ipix], src_l)
@@ -3095,19 +3096,21 @@
         alt=Angle(90, unit=units.deg),
         az=Angle(0, unit=units.deg),
         obstime=time,
         frame="altaz",
         location=array_location,
     )
     frame_coord = source_coord.transform_to(frame)
+    # make a new coord to get rid of obstime
+    input_coord = SkyCoord(ra=frame_coord.ra, dec=frame_coord.dec, frame=frame)
 
     names = "zen_source"
     stokes = [1.0, 0, 0, 0] * units.Jy
     zenith_source = SkyModel(
-        name=names, skycoord=frame_coord, stokes=stokes, spectral_type="flat"
+        name=names, skycoord=input_coord, stokes=stokes, spectral_type="flat"
     )
 
     fname = os.path.join(tmp_path, "temp_cat.txt")
 
     if isinstance(frame, str) and frame == "cirs":
         with pytest.raises(
             ValueError, match="cirs is not supported for writing text files."
```

### Comparing `pyradiosky-0.3.1/tests/test_spherical_coords_transforms.py` & `pyradiosky-1.0.0/tests/test_spherical_coords_transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- mode: python; coding: utf-8 -*
 # Copyright (c) 2019 Radio Astronomy Software Group
-# Licensed under the 3-clause BSD License
+# Licensed under the 2-clause BSD License
 
 import numpy as np
 import pytest
 from astropy import units
 from astropy.coordinates import EarthLocation, SkyCoord
 from astropy.time import Time
 from scipy.linalg import orthogonal_procrustes as ortho_procr
```

### Comparing `pyradiosky-0.3.1/tests/test_utils.py` & `pyradiosky-1.0.0/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- mode: python; coding: utf-8 -*
 # Copyright (c) 2019 Radio Astronomy Software Group
-# Licensed under the 3-clause BSD License
+# Licensed under the 2-clause BSD License
 import os
 
 import astropy.units as units
 import numpy as np
 import pytest
 from astropy.coordinates import Angle
 from astropy.time import Time
@@ -73,19 +73,23 @@
         "First two dimensions of coherency_matrix must be length 2."
     )
 
 
 @pytest.mark.parametrize("stype", ["subband", "spectral_index", "flat"])
 def test_download_gleam(tmp_path, stype):
     pytest.importorskip("astroquery")
+    import requests  # a dependency of astroquery
 
     fname = "gleam_cat.vot"
     filename = os.path.join(tmp_path, fname)
 
-    skyutils.download_gleam(path=tmp_path, filename=fname, row_limit=10)
+    try:
+        skyutils.download_gleam(path=tmp_path, filename=fname, row_limit=10)
+    except requests.exceptions.ConnectionError:
+        pytest.skip("Connection error w/ Vizier")
 
     sky = SkyModel()
     sky.read_gleam_catalog(filename, spectral_type=stype)
     assert sky.Ncomponents == 10
 
     # check there's not an error if the file exists and overwrite is False
     # and that the file is not replaced
```

