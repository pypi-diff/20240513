# Comparing `tmp/erlab-2.4.2.tar.gz` & `tmp/erlab-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.4.2.tar", last modified: Tue May  7 12:07:35 2024, max compression
+gzip compressed data, was "erlab-2.5.0.tar", last modified: Mon May 13 08:15:48 2024, max compression
```

## Comparing `erlab-2.4.2.tar` & `erlab-2.5.0.tar`

### file list

```diff
@@ -1,185 +1,186 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.013511 erlab-2.4.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.965511 erlab-2.4.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.973511 erlab-2.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)     2200 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/ISSUE_TEMPLATE/feature-request.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.973511 erlab-2.4.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-07 12:07:26.000000 erlab-2.4.2/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-07 12:07:26.000000 erlab-2.4.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-05-07 12:07:26.000000 erlab-2.4.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      793 2024-05-07 12:07:26.000000 erlab-2.4.2/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   124266 2024-05-07 12:07:30.000000 erlab-2.4.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-05-07 12:07:26.000000 erlab-2.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48438 2024-05-07 12:07:35.013511 erlab-2.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-05-07 12:07:26.000000 erlab-2.4.2/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     5147 2024-05-07 12:07:26.000000 erlab-2.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.973511 erlab-2.4.2/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.977511 erlab-2.4.2/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    17977 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    15203 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     5039 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.985511 erlab-2.4.2/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   328062 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   328737 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3119 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.985511 erlab-2.4.2/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2604 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.989511 erlab-2.4.2/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    41238 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     2598 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/imagetool.rst
--rw-r--r--   0 root         (0) root         (0)     1291 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)    12039 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    54817 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)    10710 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    27564 2024-05-07 12:07:26.000000 erlab-2.4.2/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-07 12:07:26.000000 erlab-2.4.2/environment.yml
--rw-r--r--   0 root         (0) root         (0)     5353 2024-05-07 12:07:26.000000 erlab-2.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      315 2024-05-07 12:07:26.000000 erlab-2.4.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 12:07:35.013511 erlab-2.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.969511 erlab-2.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.989511 erlab-2.4.2/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-07 12:07:30.000000 erlab-2.4.2/src/erlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.989511 erlab-2.4.2/src/erlab/accessors/
--rw-r--r--   0 root         (0) root         (0)      792 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/accessors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26123 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/accessors/fit.py
--rw-r--r--   0 root         (0) root         (0)    30007 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/accessors/kspace.py
--rw-r--r--   0 root         (0) root         (0)     7071 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/accessors/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5322 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10779 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     9594 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    12739 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    20223 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    18221 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)    14968 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5397 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8505 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     5443 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.993511 erlab-2.4.2/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.997511 erlab-2.4.2/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      526 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14330 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21371 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    23024 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11891 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)    19282 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.997511 erlab-2.4.2/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    20018 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.997511 erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52053 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114641 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27909 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    57841 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    14551 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25660 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    15911 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19321 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     2749 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    55581 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.001511 erlab-2.4.2/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2194 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.001511 erlab-2.4.2/src/erlab/io/characterization/
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)    43727 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    12313 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/exampledata.py
--rw-r--r--   0 root         (0) root         (0)     6998 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.001511 erlab-2.4.2/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     8166 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7667 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6737 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     1522 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.001511 erlab-2.4.2/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.005511 erlab-2.4.2/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2113 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30641 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18686 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4420 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    39760 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    37467 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.005511 erlab-2.4.2/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-05-07 12:07:26.000000 erlab-2.4.2/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.009511 erlab-2.4.2/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48438 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4937 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-07 12:07:34.000000 erlab-2.4.2/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.005511 erlab-2.4.2/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-07 12:07:26.000000 erlab-2.4.2/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-07 12:07:26.000000 erlab-2.4.2/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-07 12:07:26.000000 erlab-2.4.2/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:34.969511 erlab-2.4.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.009511 erlab-2.4.2/tests/accessors/
--rw-r--r--   0 root         (0) root         (0)     5785 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/accessors/test_fit.py
--rw-r--r--   0 root         (0) root         (0)     4035 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/accessors/test_kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.009511 erlab-2.4.2/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4497 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     6035 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_fit_models.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)     3126 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     1513 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/analysis/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 12:07:35.009511 erlab-2.4.2/tests/io/
--rw-r--r--   0 root         (0) root         (0)     9385 2024-05-07 12:07:26.000000 erlab-2.4.2/tests/io/test_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.800446 erlab-2.5.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.756446 erlab-2.5.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.760446 erlab-2.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/ISSUE_TEMPLATE/feature-request.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.760446 erlab-2.5.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-13 08:15:39.000000 erlab-2.5.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-05-13 08:15:39.000000 erlab-2.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      793 2024-05-13 08:15:39.000000 erlab-2.5.0/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   126450 2024-05-13 08:15:44.000000 erlab-2.5.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-05-13 08:15:39.000000 erlab-2.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    48438 2024-05-13 08:15:48.800446 erlab-2.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-05-13 08:15:39.000000 erlab-2.5.0/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     5147 2024-05-13 08:15:39.000000 erlab-2.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.760446 erlab-2.5.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.764446 erlab-2.5.0/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    18220 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    15203 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     5039 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.772446 erlab-2.5.0/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   328062 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   328737 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.772446 erlab-2.5.0/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.776446 erlab-2.5.0/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    42435 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     2598 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/imagetool.rst
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)    12039 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    54817 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)    10710 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    27572 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-13 08:15:39.000000 erlab-2.5.0/environment.yml
+-rw-r--r--   0 root         (0) root         (0)     5369 2024-05-13 08:15:39.000000 erlab-2.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-13 08:15:39.000000 erlab-2.5.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 08:15:48.800446 erlab-2.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.756446 erlab-2.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.776446 erlab-2.5.0/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-13 08:15:44.000000 erlab-2.5.0/src/erlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.780446 erlab-2.5.0/src/erlab/accessors/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/accessors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26123 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/accessors/fit.py
+-rw-r--r--   0 root         (0) root         (0)    30007 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/accessors/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    14898 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/accessors/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.780446 erlab-2.5.0/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.780446 erlab-2.5.0/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.780446 erlab-2.5.0/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10779 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    12739 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    20223 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    27520 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)    14968 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.784446 erlab-2.5.0/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5397 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8505 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.784446 erlab-2.5.0/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.784446 erlab-2.5.0/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      526 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14330 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21371 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    23024 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11891 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)    19282 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.784446 erlab-2.5.0/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    20451 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.788446 erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52053 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114641 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27909 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    57841 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    14551 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25642 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19321 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    56647 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.788446 erlab-2.5.0/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.788446 erlab-2.5.0/src/erlab/io/characterization/
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    12313 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)     6998 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.788446 erlab-2.5.0/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     8166 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7667 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.792446 erlab-2.5.0/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.792446 erlab-2.5.0/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30641 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18686 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    39760 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    38515 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.796446 erlab-2.5.0/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.800446 erlab-2.5.0/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    48438 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4973 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.796446 erlab-2.5.0/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-13 08:15:39.000000 erlab-2.5.0/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-13 08:15:39.000000 erlab-2.5.0/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-13 08:15:39.000000 erlab-2.5.0/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.756446 erlab-2.5.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.796446 erlab-2.5.0/tests/accessors/
+-rw-r--r--   0 root         (0) root         (0)     5785 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/accessors/test_fit.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/accessors/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.796446 erlab-2.5.0/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_fit_models.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_image_savgol.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.800446 erlab-2.5.0/tests/io/
+-rw-r--r--   0 root         (0) root         (0)     9385 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/io/test_dataloader.py
```

### Comparing `erlab-2.4.2/.github/ISSUE_TEMPLATE/bug-report.yml` & `erlab-2.5.0/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/.github/ISSUE_TEMPLATE/feature-request.yml` & `erlab-2.5.0/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/.github/workflows/pr.yml` & `erlab-2.5.0/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/.github/workflows/release.yml` & `erlab-2.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/.gitignore` & `erlab-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/.pre-commit-config.yaml` & `erlab-2.5.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+ci:
+  autoupdate_commit_msg: "ci(pre-commit): pre-commit autoupdate"
+  autofix_commit_msg: "style: pre-commit auto fixes [...]"
+
 repos:
 
   # Meta hooks
   - repo: meta
     hooks:
       - id: check-hooks-apply
       - id: check-useless-excludes
```

### Comparing `erlab-2.4.2/.readthedocs.yaml` & `erlab-2.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/CHANGELOG.md` & `erlab-2.5.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,57 @@
 # CHANGELOG
 
 
 
+## v2.5.0 (2024-05-13)
+
+### Chore
+
+* (**deps**) unpin PyQt6 ([`55a8ce5`](https://github.com/kmnhan/erlabpy/commit/55a8ce5e0c74c38c22a44f4f385c5ee87ee5fdcb))
+
+### Ci
+
+* (**pre-commit**) update commit messages ([`0321ec1`](https://github.com/kmnhan/erlabpy/commit/0321ec131b61e8bf6881f1f72fdc550937d96959))
+
+### Documentation
+
+* make view button point to github ([`f968c37`](https://github.com/kmnhan/erlabpy/commit/f968c3777ed796011338f7ff14b0561d9fada05e))
+
+### Feature
+
+* extended interactive accessor ([`f6f19ab`](https://github.com/kmnhan/erlabpy/commit/f6f19abd8edfb33585b5e19040a2ebaff39b2b70))
+
+  The `qshow` accessor has been updated so that it calls `hvplot` (if installed) for data not supported by ImageTool.
+  Also, the `qshow` accessor has been introduced to Datasets. For valid fit result datasets produced by the `modelfit` accessor, calling `qshow` will now show an `hvplot`-based interactive visualization of the fit result.
+
+* (**itool**) make itool accept Datasets ([`f77b699`](https://github.com/kmnhan/erlabpy/commit/f77b699abdf312a23832611052d67e8c4c8d4930))
+
+  When a Dataset is passed to `itool`, each data variable will be shown in a separate ImageTool window.
+
+* (**analysis.image**) add multidimensional Savitzky-Golay filter ([`131b32d`](https://github.com/kmnhan/erlabpy/commit/131b32d9e562693e98a2f9e45cf6db4635405b44))
+
+### Fix
+
+* (**itool**) add input data dimension check ([`984f2db`](https://github.com/kmnhan/erlabpy/commit/984f2db0f69db2b5b99211728840447d9617f8bf))
+
+* (**analysis.image**) correct argument order parsing in some filters ([`6043413`](https://github.com/kmnhan/erlabpy/commit/60434136224c0875ed8fba41d24e32fc6868127c))
+
+* (**interactive**) improve formatting for code copied to clipboard ([`d8b6d91`](https://github.com/kmnhan/erlabpy/commit/d8b6d91a4d2688486886f2464426935fdf8cabc2))
+
+### Refactor
+
+* (**plotting**) update `clean_labels` to use `Axes.label_outer` ([`0c64756`](https://github.com/kmnhan/erlabpy/commit/0c647564c6027f5b60f9ff288f13019e0e5933b6))
+
+### Unknown
+
+* Merge pull request #33 from kmnhan/dev-2.5 ([`dc9a9a8`](https://github.com/kmnhan/erlabpy/commit/dc9a9a84a6c1e5424d6994ce02a678b6a0a30db2))
+
+  2.5 Update
+
+
 ## v2.4.2 (2024-05-07)
 
 ### Fix
 
 * (**ktool**) resolve ktool initialization problem, closes #32 ([`e88a58e`](https://github.com/kmnhan/erlabpy/commit/e88a58e6aaed326af1a68aa33322d6ea9f0e800d))
 
 * (**itool**) disable flag checking for non-numpy arrays ([`da6eb1d`](https://github.com/kmnhan/erlabpy/commit/da6eb1db9e81d51b52d4b361de938bcf7ba45e68))
```

### Comparing `erlab-2.4.2/LICENSE` & `erlab-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/PKG-INFO` & `erlab-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.4.2
+Version: 2.5.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.4.2/PythonInterface.ipf` & `erlab-2.5.0/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/README.md` & `erlab-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/Makefile` & `erlab-2.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/environment.yml` & `erlab-2.5.0/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/make.bat` & `erlab-2.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/conf.py` & `erlab-2.5.0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,16 @@
     "pandas": ("https://pandas.pydata.org/docs/", None),
     "pyqtgraph": ("https://pyqtgraph.readthedocs.io/en/latest/", None),
     "csaps": ("https://csaps.readthedocs.io/en/latest/", None),
     "iminuit": ("https://scikit-hep.org/iminuit/", None),
     "cmasher": ("https://cmasher.readthedocs.io/", None),
     "ipywidgets": ("https://ipywidgets.readthedocs.io/en/stable/", None),
     "joblib": ("https://joblib.readthedocs.io/en/latest/", None),
+    "panel": ("https://panel.holoviz.org/", None),
+    "hvplot": ("https://hvplot.holoviz.org/", None),
 }
 
 
 # -- Plot configuration ------------------------------------------------------
 
 plot_formats = ["pdf"]
 plot_basedir = "pyplots"
@@ -474,14 +476,17 @@
     #     "color-brand-primary": "#6d50bf",
     #     "color-brand-content": "#6d50bf",
     # },
     # "dark_css_variables": {
     #     "color-brand-primary": "#a180ff",
     #     "color-brand-content": "#a180ff",
     # },
+    "source_repository": "https://github.com/kmnhan/erlabpy/",
+    "source_branch": f"v{version}",
+    "source_directory": "docs/source/",
 }
 
 # -- LaTeX options -----------------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#latex-options
 
 latex_engine = "lualatex"
 latex_show_pagerefs = True
```

### Comparing `erlab-2.4.2/docs/source/contributing.rst` & `erlab-2.5.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/getting-started.rst` & `erlab-2.5.0/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/images/flowchart_multiple.pdf` & `erlab-2.5.0/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/images/flowchart_single.pdf` & `erlab-2.5.0/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/images/imagetool_dark.png` & `erlab-2.5.0/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/images/imagetool_light.png` & `erlab-2.5.0/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/images/ktool_1_dark.png` & `erlab-2.5.0/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/images/ktool_1_light.png` & `erlab-2.5.0/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/images/ktool_2_dark.png` & `erlab-2.5.0/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/images/ktool_2_light.png` & `erlab-2.5.0/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/index.rst` & `erlab-2.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/pyplots/norms.py` & `erlab-2.5.0/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/reference.rst` & `erlab-2.5.0/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/refs.bib` & `erlab-2.5.0/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.5.0/docs/source/user-guide/curve-fitting.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960897435897436%*

 * *Differences: {"'cells'": "{53: {'source': {insert: [(0, 'result_ds = darr.modelfit(\\n'), (11, ')\\n'), (12, "*

 * *            "'result_ds')], delete: [11, 0]}}, insert: [(54, OrderedDict([('cell_type', 'raw'), "*

 * *            "('metadata', OrderedDict([('editable', True), ('raw_mimetype', "*

 * *            "'text/restructuredtext'), ('slideshow', OrderedDict([('slide_type', '')])), ('tags', "*

 * *            "[]), ('vscode', OrderedDict([('languageId', 'raw')]))])), ('source', ['Visualizing "*

 * *            "fits\\n', '~~~~~~~~~~~~~~~~ […]*

```diff
@@ -780,26 +780,61 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "darr.modelfit(\n",
+                "result_ds = darr.modelfit(\n",
                 "    coords=\"alpha\",\n",
                 "    model=GaussianModel() + LinearModel(),\n",
                 "    params={\n",
                 "        \"center\": {\n",
                 "            \"value\": xr.DataArray([-2, 0, 2], coords=[darr.beta]),\n",
                 "            \"min\": -5.0,\n",
                 "            \"max\": xr.DataArray([0, 2, 5], coords=[darr.beta]),\n",
                 "        },\n",
                 "        \"slope\": -0.1,\n",
                 "    },\n",
-                ")"
+                ")\n",
+                "result_ds"
+            ]
+        },
+        {
+            "cell_type": "raw",
+            "metadata": {
+                "editable": true,
+                "raw_mimetype": "text/restructuredtext",
+                "slideshow": {
+                    "slide_type": ""
+                },
+                "tags": [],
+                "vscode": {
+                    "languageId": "raw"
+                }
+            },
+            "source": [
+                "Visualizing fits\n",
+                "~~~~~~~~~~~~~~~~\n",
+                "\n",
+                "If `hvplot <https://github.com/holoviz/hvplot>`_ is installed, we can visualize the fit\n",
+                "results interactively with the `qshow` accessor.\n",
+                "\n",
+                ".. note::\n",
+                "\n",
+                "    If you are viewing this documentation online, the plot will not be interactive. Run the code locally to try it out."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "result_ds.qshow(plot_components=True)"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
```

### Comparing `erlab-2.4.2/docs/source/user-guide/imagetool.rst` & `erlab-2.5.0/docs/source/user-guide/imagetool.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/user-guide/index.rst` & `erlab-2.5.0/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/user-guide/indexing.ipynb` & `erlab-2.5.0/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/user-guide/io.ipynb` & `erlab-2.5.0/docs/source/user-guide/io.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/user-guide/kconv.ipynb` & `erlab-2.5.0/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/docs/source/user-guide/plotting.ipynb` & `erlab-2.5.0/docs/source/user-guide/plotting.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994212962962963%*

 * *Differences: {"'cells'": "{12: {'source': [':func:`plot_array <erlab.plotting.general.plot_array>` can also be "*

 * *            'accessed (for 2D data) through the :class:`qplot '*

 * *            "<erlab.accessors.utils.PlotAccessor>` accessor.']}, 19: {'source': {insert: [(2, "*

 * *            "'some annotations, we can use :func:`clean_labels "*

 * *            "<erlab.plotting.general.clean_labels>`\\n')], delete: [2]}}}"}*

```diff
@@ -200,15 +200,15 @@
                 },
                 "tags": [],
                 "vscode": {
                     "languageId": "raw"
                 }
             },
             "source": [
-                ":func:`plot_array <erlab.plotting.general.plot_array>` can also be accessed (for 2D data) through an :class:`accessor <erlab.accessors.utils.PlotAccessor>`."
+                ":func:`plot_array <erlab.plotting.general.plot_array>` can also be accessed (for 2D data) through the :class:`qplot <erlab.accessors.utils.PlotAccessor>` accessor."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -312,15 +312,15 @@
                 "vscode": {
                     "languageId": "raw"
                 }
             },
             "source": [
                 "Here, we plotted each constant energy surface with :func:`plot_array\n",
                 "<erlab.plotting.general.plot_array>`. To remove the duplicated y axis labels and add\n",
-                "some annotations, we can use :func:`clean_labels <erlab.plotting.erplot.clean_labels>`\n",
+                "some annotations, we can use :func:`clean_labels <erlab.plotting.general.clean_labels>`\n",
                 "and :func:`label_subplot_properties\n",
                 "<erlab.plotting.annotations.label_subplot_properties>`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `erlab-2.4.2/pyproject.toml` & `erlab-2.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,15 @@
     "io/plugins/",
 ]
 
 [[tool.mypy.overrides]]
 module = [
     "astropy.*",
     "h5netcdf.*",
+    "hvplot.*",
     "igor2.*",
     "iminuit.*",
     "ipywidgets.*",
     "joblib.*",
     "lmfit.*",
     "mpl_toolkits.*",
     "numba.*",
```

### Comparing `erlab-2.4.2/src/erlab/accessors/__init__.py` & `erlab-2.5.0/src/erlab/accessors/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,16 @@
    utils
    kspace
    fit
 
 """  # noqa: D205
 
 __all__ = [
-    "ImageToolAccessor",
+    "InteractiveDataArrayAccessor",
+    "InteractiveDatasetAccessor",
     "ModelFitDataArrayAccessor",
     "ModelFitDatasetAccessor",
     "MomentumAccessor",
     "OffsetView",
     "ParallelFitDataArrayAccessor",
     "PlotAccessor",
     "SelectionAccessor",
@@ -30,8 +31,13 @@
 
 from erlab.accessors.fit import (
     ModelFitDataArrayAccessor,
     ModelFitDatasetAccessor,
     ParallelFitDataArrayAccessor,
 )
 from erlab.accessors.kspace import MomentumAccessor, OffsetView
-from erlab.accessors.utils import ImageToolAccessor, PlotAccessor, SelectionAccessor
+from erlab.accessors.utils import (
+    InteractiveDataArrayAccessor,
+    InteractiveDatasetAccessor,
+    PlotAccessor,
+    SelectionAccessor,
+)
```

### Comparing `erlab-2.4.2/src/erlab/accessors/fit.py` & `erlab-2.5.0/src/erlab/accessors/fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/accessors/kspace.py` & `erlab-2.5.0/src/erlab/accessors/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/accessors/utils.py` & `erlab-2.5.0/src/erlab/io/plugins/ssrl52.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,219 +1,234 @@
-__all__ = [
-    "ImageToolAccessor",
-    "PlotAccessor",
-    "SelectionAccessor",
-]
-
-import warnings
-from collections.abc import Hashable, Mapping
-from typing import Any, TypeGuard, TypeVar, cast
+"""Data loader for beamline 5-2 at SSRL."""
 
-import matplotlib.pyplot as plt
+import datetime
+import os
+import re
+from typing import ClassVar
+
+import h5netcdf
+import numpy as np
+import pandas as pd
 import xarray as xr
 
-import erlab.plotting.erplot as eplt
+import erlab.io.utilities
+from erlab.io.dataloader import LoaderBase
 
-T = TypeVar("T")
 
-# Used as the key corresponding to a DataArray's variable when converting
-# arbitrary DataArray objects to datasets, from xarray.core.dataarray
-_THIS_ARRAY: str = "<this-array>"
+class SSRL52Loader(LoaderBase):
+    name = "ssrl"
+    aliases = ("ssrl52", "bl5-2")
+
+    name_map: ClassVar[dict] = {
+        "eV": "Kinetic Energy",
+        "alpha": "ThetaX",
+        "beta": ["ThetaY", "YDeflection", "DeflectionY"],
+        "delta": ["A", "a"],  # azi
+        "chi": ["T", "t"],  # polar
+        "xi": ["F", "f"],  # tilt
+        "x": "X",
+        "y": "Y",
+        "z": "Z",
+        "hv": ["BL_energy", "BL_photon_energy"],
+        "temp_sample": ["TB", "sample_stage_temperature"],
+        "sample_workfunction": "WorkFunction",
+    }
+
+    coordinate_attrs = ("beta", "delta", "chi", "xi", "hv", "x", "y", "z")
+
+    additional_attrs: ClassVar[dict] = {
+        "configuration": 3,
+        "sample_workfunction": 4.5,
+    }
+
+    always_single: bool = True
+    skip_validate: bool = True
+
+    def load_single(self, file_path: str | os.PathLike) -> xr.DataArray:
+        with h5netcdf.File(file_path, mode="r", phony_dims="sort") as ncf:
+            attrs = dict(ncf.attrs)
+            compat_mode = "data" in ncf.groups  # Compatibility with older data
+            for k, v in ncf.groups.items():
+                ds = xr.open_dataset(xr.backends.H5NetCDFStore(v, autoclose=True))
+
+                if k.casefold() == "Beamline".casefold():
+                    attrs[k] = ds.attrs
+                    hv = ds.attrs.get("energy", None)
+                    hv = ds.attrs.get("photon_energy", hv)
+                    if hv is not None:
+                        attrs["hv"] = hv
 
+                    attrs["polarization"] = ds.attrs.get("polarization")
 
-class ERLabDataArrayAccessor:
-    """Base class for accessors."""
-
-    def __init__(self, xarray_obj: xr.DataArray):
-        self._obj = xarray_obj
-
-
-class ERLabDatasetAccessor:
-    """Base class for accessors."""
-
-    def __init__(self, xarray_obj: xr.Dataset):
-        self._obj = xarray_obj
-
-
-def is_dict_like(value: Any) -> TypeGuard[Mapping[Any, Any]]:
-    return hasattr(value, "keys") and hasattr(value, "__getitem__")
-
-
-def either_dict_or_kwargs(
-    pos_kwargs: Mapping[Any, T] | None,
-    kw_kwargs: Mapping[str, T],
-    func_name: str,
-) -> Mapping[Hashable, T]:
-    if pos_kwargs is None or pos_kwargs == {}:
-        # Need an explicit cast to appease mypy due to invariance; see
-        # https://github.com/python/mypy/issues/6228
-        return cast(Mapping[Hashable, T], kw_kwargs)
-
-    if not is_dict_like(pos_kwargs):
-        raise ValueError(f"the first argument to .{func_name} must be a dictionary")
-    if kw_kwargs:
-        raise ValueError(
-            f"cannot specify both keyword and positional arguments to .{func_name}"
-        )
-    return pos_kwargs
-
-
-@xr.register_dataarray_accessor("qplot")
-class PlotAccessor(ERLabDataArrayAccessor):
-    """`xarray.DataArray.qplot` accessor for plotting data."""
-
-    def __call__(self, *args, **kwargs):
-        """Plot the data.
-
-        If a 2D data array is provided, it is plotted using :func:`plot_array
-        <erlab.plotting.general.plot_array>`. Otherwise, it is equivalent to calling
-        :meth:`xarray.DataArray.plot`.
-
-        Parameters
-        ----------
-        *args
-            Positional arguments to be passed to the plotting function.
-        **kwargs
-            Keyword arguments to be passed to the plotting function.
-
-        """
-        if len(self._obj.dims) == 2:
-            return eplt.plot_array(self._obj, *args, **kwargs)
-        else:
-            ax = kwargs.pop("ax", None)
-            if ax is None:
-                ax = plt.gca()
-            kwargs["ax"] = ax
-
-            out = self._obj.plot(*args, **kwargs)
-            eplt.fancy_labels(ax)
-            return out
-
-
-@xr.register_dataarray_accessor("qshow")
-class ImageToolAccessor(ERLabDataArrayAccessor):
-    """`xarray.DataArray.qshow` accessor for interactive visualization."""
-
-    def __call__(self, *args, **kwargs):
-        from erlab.interactive.imagetool import itool
+                else:
+                    # Merge group attributes
+                    attrs = attrs | ds.attrs
 
-        if len(self._obj.dims) >= 2:
-            return itool(self._obj, *args, **kwargs)
+                if k.casefold() == "Data".casefold():
+                    if compat_mode:
+                        if "exposure" in ds.variables:
+                            ds = ds.rename_vars(counts="spectrum", exposure="time")
+                        else:
+                            ds = ds.rename_vars(counts="spectrum")
+                    elif "Time" in ds.variables:
+                        ds = ds.rename_vars(Count="spectrum", Time="time")
+                    else:
+                        ds = ds.rename_vars(Count="spectrum")
+
+                    # List of dicts containing scale and label info for each axis
+                    axes: list[dict[str, float | int | str]] = [
+                        dict(v.groups[g].attrs) for g in v.groups
+                    ]
+
+                    for i, ax in enumerate(axes):
+                        # Unify case for compatibility with old data
+                        axes[i] = {name.lower(): val for name, val in ax.items()}
+
+                    # Apply dim labels
+                    data = ds.rename_dims(
+                        {f"phony_dim_{i}": ax["label"] for i, ax in enumerate(axes)}
+                    ).load()
+
+                    # Apply coordinates
+                    for i, ax in enumerate(axes):
+                        if compat_mode:
+                            cnt = v.dimensions[f"phony_dim_{i}"].size
+                        else:
+                            cnt = ax["count"]
+                        mn, mx = (
+                            ax["offset"],
+                            ax["offset"] + (cnt - 1) * ax["delta"],
+                        )
+                        data = data.assign_coords(
+                            {ax["label"]: np.linspace(mn, mx, cnt)}
+                        )
+
+        if "time" in data.variables:
+            # Normalize by dwell time
+            data = data["spectrum"] / data["time"]
         else:
-            raise ValueError("Data must have at leasst two dimensions.")
-
+            data = data["spectrum"]
 
-@xr.register_dataarray_accessor("qsel")
-class SelectionAccessor(ERLabDataArrayAccessor):
-    """`xarray.DataArray.qsel` accessor for convenient selection and averaging."""
+        data = data.assign_attrs(attrs)
+        return self.process_keys(data)
 
-    def __call__(
+    def identify(
         self,
-        indexers: Mapping[Hashable, float | slice] | None = None,
-        *,
-        verbose: bool = False,
-        **indexers_kwargs,
+        num: int,
+        data_dir: str | os.PathLike,
+        zap: bool = False,
     ):
-        """Select and average data along specified dimensions.
-
-        Parameters
-        ----------
-        indexers
-            Dictionary specifying the dimensions and their values or slices.
-            Position along a dimension can be specified in three ways:
-
-            - As a scalar value: `alpha=-1.2`
-
-              If no width is specified, the data is selected along the nearest value. It
-              is equivalent to `xarray.DataArray.sel` with `method='nearest'`.
-
-            - As a value and width: `alpha=5, alpha_width=0.5`
-
-              The data is *averaged* over a slice of width `alpha_width`, centered at
-              `alpha`.
-
-            - As a slice: `alpha=slice(-10, 10)`
-
-              The data is selected over the specified slice. No averaging is performed.
-
-            One of `indexers` or `indexers_kwargs` must be provided.
-        verbose
-            If `True`, print information about the selected data and averaging process.
-            Default is `False`.
-        **indexers_kwargs
-            The keyword arguments form of `indexers`. One of `indexers` or
-            `indexers_kwargs` must be provided.
-
-        Returns
-        -------
-        xarray.DataArray
-            The selected and averaged data.
-
-        Raises
-        ------
-        ValueError
-            If a specified dimension is not present in the data.
-        """
-        indexers = either_dict_or_kwargs(indexers, indexers_kwargs, "qsel")
-
-        # Bin widths for each dimension, zero if width not specified
-        bin_widths: dict[Hashable, float] = {}
-
-        for dim in indexers:
-            if not str(dim).endswith("_width"):
-                width = indexers.get(f"{dim}_width", 0.0)
-                if isinstance(width, slice):
-                    raise ValueError(
-                        f"Slice not allowed for width of dimension `{dim}`"
-                    )
-                else:
-                    bin_widths[dim] = float(width)
-                if dim not in self._obj.dims:
-                    raise ValueError(f"Dimension `{dim}` not found in data.")
-
-        scalars: dict[Hashable, float] = {}
-        slices: dict[Hashable, slice] = {}
-        avg_dims: list[Hashable] = []
-
-        for dim, width in bin_widths.items():
-            value = indexers[dim]
-
-            if width == 0.0:
-                if isinstance(value, slice):
-                    slices[dim] = value
-                else:
-                    scalars[dim] = float(value)
-            else:
-                if isinstance(value, slice):
-                    raise ValueError(
-                        f"Slice not allowed for value of dimension `{dim}` "
-                        "with width specified"
-                    )
-                slices[dim] = slice(value - width / 2, value + width / 2)
-                avg_dims.append(dim)
-
-        if len(scalars) >= 1:
-            for k, v in scalars.items():
-                if v < self._obj[k].min() or v > self._obj[k].max():
-                    warnings.warn(
-                        f"Selected value {v} for `{k}` is outside coordinate bounds",
-                        stacklevel=2,
-                    )
-            out = self._obj.sel(
-                {str(k): v for k, v in scalars.items()}, method="nearest"
+        if zap:
+            target_files = erlab.io.utilities.get_files(
+                data_dir, extensions=(".h5",), contains="zap"
             )
         else:
-            out = self._obj
+            target_files = erlab.io.utilities.get_files(
+                data_dir, extensions=(".h5",), notcontains="zap"
+            )
 
-        if len(slices) >= 1:
-            out = out.sel(slices)
+        for file in target_files:
+            match = re.match(r"(.*?)_" + str(num).zfill(4) + r".h5", file)
+            if match is not None:
+                return [file], {}
+
+        raise FileNotFoundError(f"No files found for scan {num} in {data_dir}")
+
+    # def post_process(
+    #     self, data: xr.DataArray | xr.Dataset
+    # ) -> xr.DataArray | xr.Dataset:
+    #     data = super().post_process(data)
+
+    #     if "eV" in data.coords:
+    #         data = data.assign_coords(eV=-data.eV.values)
+
+    #     return data
+
+    def load_zap(self, identifier, data_dir):
+        return self.load(identifier, data_dir, zap=True)
+
+    def generate_summary(
+        self, data_dir: str | os.PathLike, exclude_zap: bool = False
+    ) -> pd.DataFrame:
+        files: dict[str, str] = {}
+
+        if exclude_zap:
+            target_files = erlab.io.utilities.get_files(
+                data_dir, extensions=(".h5",), notcontains="zap"
+            )
+        else:
+            target_files = erlab.io.utilities.get_files(data_dir, extensions=(".h5",))
 
-            lost_coords = {k: out[k].mean() for k in avg_dims}
-            out = out.mean(dim=avg_dims, keep_attrs=True)
-            out = out.assign_coords(lost_coords)
-
-        if verbose:
-            print(
-                f"Selected data with {scalars} and {slices}, averaging over {avg_dims}"
+        for pth in target_files:
+            base_name = os.path.splitext(os.path.basename(pth))[0]
+            files[base_name] = pth
+
+        summary_attrs: dict[str, str] = {
+            "Type": "Description",
+            "Lens Mode": "LensModeName",
+            "Region": "RegionName",
+            "T(K)": "temp_sample",
+            "Pass E": "PassEnergy",
+            "Polarization": "polarization",
+            "hv": "hv",
+            # "Entrance Slit": "Entrance Slit",
+            # "Exit Slit": "Exit Slit",
+            "x": "x",
+            "y": "y",
+            "z": "z",
+            "polar": "chi",
+            "tilt": "xi",
+            "azi": "delta",
+            "DA": "beta",
+        }
+
+        cols = ["File Name", "Path", "Time", *summary_attrs.keys()]
+
+        data_info = []
+
+        for name, path in files.items():
+            data = self.load(path)
+
+            data_info.append(
+                [
+                    name,
+                    path,
+                    datetime.datetime.fromtimestamp(data.attrs["CreationTimeStamp"]),
+                ]
             )
 
-        return out
+            for k, v in summary_attrs.items():
+                try:
+                    val = data.attrs[v]
+                except KeyError:
+                    try:
+                        val = data.coords[v].values
+                        if val.size == 1:
+                            val = val.item()
+                    except KeyError:
+                        val = ""
+
+                if k == "Pass E":
+                    val = round(val)
+
+                elif k == "Polarization":
+                    if np.iterable(val):
+                        val = np.round(np.asarray(val), 3).astype(float)
+                    else:
+                        val = [float(np.round(val, 3))]
+                    val = [
+                        {0.0: "LH", 0.5: "LV", 0.25: "RC", -0.25: "LC"}.get(v, v)
+                        for v in val
+                    ]
+
+                    if len(val) == 1:
+                        val = val[0]
+
+                data_info[-1].append(val)
+
+            del data
+
+        return (
+            pd.DataFrame(data_info, columns=cols)
+            .sort_values("Time")
+            .set_index("File Name")
+        )
```

### Comparing `erlab-2.4.2/src/erlab/analysis/__init__.py` & `erlab-2.5.0/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/correlation.py` & `erlab-2.5.0/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.5.0/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.5.0/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/fit/functions/general.py` & `erlab-2.5.0/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/fit/minuit.py` & `erlab-2.5.0/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/fit/models.py` & `erlab-2.5.0/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/fit/spline.py` & `erlab-2.5.0/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/gold.py` & `erlab-2.5.0/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/image.py` & `erlab-2.5.0/src/erlab/analysis/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,79 @@
 """
 Various image processing functions including tools for visualizing dispersive features.
 
-Note
-----
-For scipy-based filter functions, the default value of the `mode` argument is 'nearest',
-unlike the scipy default of 'reflect'.
+Some filter functions in `scipy.ndimage` and `scipy.signal` are extended to work with
+regularly spaced xarray DataArrays.
+
+Notes
+-----
+- For many scipy-based filter functions, the default value of the `mode` argument is
+  different from scipy.
+- Many functions in this module has conflicting names with the SciPy functions. It is
+  good practice to avoid direct imports.
+
 """
 
-from collections.abc import Collection, Hashable, Mapping, Sequence, Sized
+import itertools
+import math
+from collections.abc import Collection, Hashable, Mapping, Sequence
+from typing import Literal
 
 import numpy as np
 import numpy.typing as npt
 import scipy
 import scipy.ndimage
 import xarray as xr
 from numba import carray, cfunc, types
 
 
+def _parse_dict_arg(
+    dims: Sequence[Hashable],
+    sigma: float | Collection[float] | Mapping[Hashable, float],
+    arg_name: str,
+    reference_name: str,
+    allow_subset: bool = False,
+) -> dict[Hashable, float]:
+    if isinstance(sigma, Mapping):
+        sigma_dict = dict(sigma)
+
+    elif np.isscalar(sigma):
+        sigma_dict = dict.fromkeys(dims, sigma)
+
+    elif isinstance(sigma, Collection):
+        if len(sigma) != len(dims):
+            raise ValueError(
+                f"`{arg_name}` does not match dimensions of {reference_name}"
+            )
+
+        sigma_dict = dict(zip(dims, sigma, strict=True))
+
+    else:
+        raise TypeError(f"`{arg_name}` must be a scalar, sequence, or mapping")
+
+    if not allow_subset and len(sigma_dict) != len(dims):
+        required_dims = set(dims) - set(sigma_dict.keys())
+        raise ValueError(
+            f"`{arg_name}` missing for the following dimension"
+            f"{'' if len(required_dims) == 1 else 's'}: {required_dims}"
+        )
+
+    else:
+        for d in sigma_dict.keys():
+            if d not in dims:
+                raise ValueError(
+                    f"Dimension `{d}` in {arg_name} not found in {reference_name}"
+                )
+
+    # Make sure that sigma_dict is ordered in temrs of data dims
+    sigma_dict = {d: sigma_dict[d] for d in dims if d in sigma_dict.keys()}
+
+    return sigma_dict
+
+
 def gaussian_filter(
     darr: xr.DataArray,
     sigma: float | Collection[float] | Mapping[Hashable, float],
     order: int | Sequence[int] | Mapping[Hashable, int] = 0,
     mode: str | Sequence[str] | Mapping[Hashable, str] = "nearest",
     cval: float = 0.0,
     truncate: float = 4.0,
@@ -95,43 +148,36 @@
         [10, 12, 14, 15, 17],
         [20, 22, 24, 25, 27],
         [29, 31, 33, 34, 36],
         [36, 38, 40, 41, 43]])
     Dimensions without coordinates: x, y
 
     """
-    if isinstance(sigma, Mapping):
-        sigma_dict = dict(sigma)
-    elif np.isscalar(sigma):
-        sigma_dict = dict.fromkeys(darr.dims, sigma)
-    elif isinstance(sigma, Collection):
-        sigma_dict = dict(zip(darr.dims, sigma, strict=True))
-    else:
-        raise TypeError("`sigma` must be a scalar, sequence, or mapping")
+    sigma_dict: dict[Hashable, float] = _parse_dict_arg(
+        darr.dims,
+        sigma,
+        arg_name="sigma",
+        reference_name="DataArray",
+        allow_subset=True,
+    )
 
     # Get the axis indices to apply the filter
     axes = tuple(darr.get_axis_num(d) for d in sigma_dict.keys())
 
     # Convert arguments to tuples acceptable by scipy
     if isinstance(order, Mapping):
         order = tuple(order.get(str(d), 0) for d in sigma_dict.keys())
+
     if isinstance(mode, Mapping):
         mode = tuple(mode[str(d)] for d in sigma_dict.keys())
 
     if radius is not None:
-        if isinstance(radius, Mapping):
-            radius_dict = dict(radius)
-        elif isinstance(radius, Sized):
-            if len(radius) != len(sigma_dict):
-                raise ValueError("`radius` does not match dimensions of `sigma`")
-            radius_dict = dict(zip(sigma_dict.keys(), radius, strict=True))
-        elif np.isscalar(radius):
-            radius_dict = dict.fromkeys(sigma_dict.keys(), radius)
-        else:
-            raise TypeError("`radius` must be a scalar, sequence, or mapping")
+        radius_dict = _parse_dict_arg(
+            tuple(sigma_dict.keys()), radius, "radius", "`sigma`"
+        )
 
         # Calculate radius in pixels
         radius_pix: tuple[int, ...] | None = tuple(
             round(r / (darr[d].values[1] - darr[d].values[0]))
             for d, r in radius_dict.items()
         )
     else:
@@ -154,15 +200,15 @@
             axes=axes,
         )
     )
 
 
 def gaussian_laplace(
     darr: xr.DataArray,
-    sigma: float | Collection[float] | Mapping[str, float],
+    sigma: float | Collection[float] | Mapping[Hashable, float],
     mode: str | Sequence[str] | Mapping[str, str] = "nearest",
     cval: float = 0.0,
     **kwargs,
 ) -> xr.DataArray:
     """Coordinate-aware wrapper around `scipy.ndimage.gaussian_laplace`.
 
     This function calculates the Laplacian of the given array using Gaussian second
@@ -201,29 +247,21 @@
     - The input array is assumed to be regularly spaced.
 
     See Also
     --------
     :func:`scipy.ndimage.gaussian_laplace` : The underlying function used to apply the
         filter.
     """
-    if isinstance(sigma, Mapping):
-        sigma_dict = dict(sigma)
-    elif np.isscalar(sigma):
-        sigma_dict = dict.fromkeys(darr.dims, sigma)
-    elif isinstance(sigma, Collection):
-        sigma_dict = dict(zip(darr.dims, sigma, strict=True))
-    else:
-        raise TypeError("`sigma` must be a scalar, sequence, or mapping")
-
-    if len(sigma_dict) != darr.ndim:
-        required_dims = set(darr.dims) - set(sigma_dict.keys())
-        raise ValueError(
-            "`sigma` missing for the following dimension"
-            f"{'' if len(required_dims) == 1 else 's'}: {required_dims}"
-        )
+    sigma_dict: dict[Hashable, float] = _parse_dict_arg(
+        darr.dims,
+        sigma,
+        arg_name="sigma",
+        reference_name="DataArray",
+        allow_subset=False,
+    )
 
     # Convert mode to tuple acceptable by scipy
     if isinstance(mode, dict):
         mode = tuple(mode[d] for d in sigma_dict.keys())
 
     # Calculate sigma in pixels
     sigma_pix: tuple[float, ...] = tuple(
@@ -233,14 +271,251 @@
     return darr.copy(
         data=scipy.ndimage.gaussian_laplace(
             darr.values, sigma=sigma_pix, mode=mode, cval=cval, **kwargs
         )
     )
 
 
+def _ndpoly_degree_combinations(polyorder: int, ndim: int) -> list[tuple[int, ...]]:
+    degrees = [range(polyorder + 1)] * ndim
+    return [d for d in itertools.product(*degrees) if sum(d) <= polyorder]
+
+
+def _ndsavgol_vandermonde(window_shape: tuple[int, ...], polyorder: int):
+    """Calculate the Vandermonde matrix for Savitzky-Golay filtering."""
+    # Get the number of dimensions
+    ndim: int = len(window_shape)
+
+    # Half of the window size
+    half_sizes = np.array([[s // 2 for s in window_shape]], dtype=np.float64).T
+
+    # Create an array of indices for each dimension
+    indices = (
+        np.indices(window_shape, dtype=np.float64).reshape((ndim, -1)) - half_sizes
+    ).T
+
+    # Create all combinations of degrees
+    degree_combinations = np.array(
+        _ndpoly_degree_combinations(polyorder, ndim), dtype=np.float64
+    )
+
+    # Create the Vandermonde matrix
+    vander = np.prod(
+        np.power(indices[:, None, :], degree_combinations[None, :, :]), axis=-1
+    )
+    return vander
+
+
+def _ndsavgol_scale(deriv_idx: int, delta: tuple[float, ...], polyorder: int):
+    """Calculate the scale factor for the Savitzky-Golay filter."""
+    # Get the derivative order for each axis
+    deriv_for_ax = _ndpoly_degree_combinations(polyorder, len(delta))[deriv_idx]
+
+    # Calculate the correction factor for the derivative order and sample point spacing
+    scale = math.factorial(sum(deriv_for_ax)) / sum(np.power(delta, deriv_for_ax))
+
+    return scale
+
+
+def _ndsavgol_coeffs(
+    window_shape: tuple[int, ...],
+    polyorder: int,
+    deriv_idx: int,
+    delta: tuple[float, ...],
+):
+    """Calculate the Savitzky-Golay filter coefficients."""
+    vander = _ndsavgol_vandermonde(window_shape, polyorder)
+    scale = _ndsavgol_scale(deriv_idx, delta, polyorder)
+
+    # Invert the Vandermonde matrix to get the filter coefficients
+    coeffs = np.linalg.pinv(vander)[deriv_idx] * scale
+
+    # SciPy uses lstsq for this, but calculating the pseudo-inverse directly seems to
+    # return more accurate results
+
+    return coeffs
+
+
+def ndsavgol(
+    arr: npt.NDArray[np.float64],
+    window_shape: int | tuple[int, ...],
+    polyorder: int,
+    deriv: int | tuple[int, ...] = 0,
+    delta: float | tuple[float, ...] = 1.0,
+    mode: Literal["mirror", "constant", "nearest", "wrap"] = "mirror",
+    cval: float = 0.0,
+    method: Literal["pinv", "lstsq"] = "pinv",
+):
+    """Apply a Savitzky-Golay filter to an N-dimensional array.
+
+    Unlike `scipy.signal.savgol_filter` which is limited to 1D arrays, this function
+    calculates multi-dimensional Savitzky-Golay filters. There are some subtle
+    differences in the implementation, so the results may not be identical. See Notes.
+
+    Parameters
+    ----------
+    arr
+        The input N-dimensional array to be filtered. The array will be cast to float64
+        before filtering.
+    window_shape
+        The shape of the window used for filtering. If an integer, the same size will be
+        used across all axes.
+    polyorder
+        The order of the polynomial used to fit the samples. `polyorder` must be less
+        than the minimum of `window_shape`.
+    deriv
+        The order of the derivative to compute given as a single integer or a tuple of
+        integers. If an integer, the derivative of that order is computed along all
+        axes. If a tuple of integers, the derivative of each order is computed along the
+        corresponding dimension. The default is 0, which means to filter the data
+        without differentiating.
+    delta
+        The spacing of the samples to which the filter will be applied. If a float, the
+        same value is used for all axes. If a tuple, the values are used in the same
+        order as in `deriv`. The default is 1.0.
+    mode
+        Must be 'mirror', 'constant', 'nearest', or 'wrap'. This determines the type of
+        extension to use for the padded signal to which the filter is applied.  When
+        `mode` is 'constant', the padding value is given by `cval`.
+    cval
+        Value to fill past the edges of the input if `mode` is 'constant'. Default is
+        0.0.
+    method
+        Must be 'pinv' or 'lstsq'. Determines the method used to calculate the filter
+        coefficients. 'pinv' uses the pseudoinverse of the Vandermonde matrix, while
+        'lstsq' uses least squares for each window position. 'lstsq' is much slower but
+        may be more numerically stable in some cases. The difference is more pronounced
+        for higher dimensions, larger window size, and higher polynomial orders. The
+        default is 'pinv'.
+
+    Returns
+    -------
+    numpy.ndarray
+        The filtered array.
+
+    See Also
+    --------
+    :func:`scipy.signal.savgol_filter` : The 1D Savitzky-Golay filter function in SciPy.
+
+    Notes
+    -----
+    - For even window sizes, the results may differ slightly from
+      `scipy.signal.savgol_filter` due to differences in the implementation.
+    - This function is not suitable for cases where accumulated floating point errors
+      are comparable to the filter coefficients, i.e., for high number of dimensions and
+      large window sizes.
+    - ``mode='interp'`` is not implemented as it is not clear how to handle the edge
+      cases in higher dimensions.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> import erlab.analysis as era
+
+    >>> arr = np.array([1, 2, 3, 4, 5])
+    >>> era.image.ndsavgol(arr, (3,), polyorder=2)
+    array([1., 2., 3., 4., 5.])
+
+    >>> era.image.ndsavgol(arr, (3,), polyorder=2, deriv=1)
+    array([0., 1., 1., 1., 0.])
+
+    >>> arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
+    >>> era.image.ndsavgol(arr, (3, 3), polyorder=2)
+    array([[0.5, 1. , 1.5],
+           [2. , 2.5, 3. ],
+           [3.5, 4. , 4.5]])
+
+    """
+    if mode not in ["mirror", "constant", "nearest", "wrap"]:
+        raise ValueError("mode must be 'mirror', 'constant', 'nearest', or 'wrap'")
+
+    if method not in ["pinv", "lstsq"]:
+        raise ValueError("method must be 'pinv' or 'lstsq'")
+
+    if method == "lstsq":
+        accurate = True
+    else:
+        accurate = False
+
+    if isinstance(window_shape, int):
+        window_shape = (window_shape,) * arr.ndim
+
+    # Convert deriv to a tuple for 2D or higher arrays
+    if isinstance(deriv, int) and arr.ndim > 1:
+        deriv = (deriv,) * arr.ndim
+
+    # Convert to an index of the list of combinations
+    if not isinstance(deriv, int):
+        if len(deriv) != arr.ndim:
+            raise ValueError(
+                "`deriv` must have the same length as the number of dimensions"
+            )
+        deriv_idx = _ndpoly_degree_combinations(polyorder, arr.ndim).index(tuple(deriv))
+    else:
+        # 1D case, the two are equivalent
+        deriv_idx = deriv
+
+    # Ensure delta is a tuple
+    if isinstance(delta, int | float | np.floating):
+        delta = (float(delta),) * arr.ndim
+
+    if len(delta) != arr.ndim:
+        raise ValueError(
+            "`delta` must have the same length as the number of dimensions"
+        )
+
+    if accurate:
+        vander = _ndsavgol_vandermonde(window_shape, polyorder)
+        scale = _ndsavgol_scale(deriv_idx, delta, polyorder)
+
+    else:
+        # Invert the Vandermonde matrix to get the filter coefficients
+        coeffs = _ndsavgol_coeffs(window_shape, polyorder, deriv_idx, delta)
+
+    if arr.ndim == 1:
+        # Cfunc definition overhead is a bottleneck for small arrays
+        # Python function is faster for 1D arrays of reasonable size
+
+        def _func(values):
+            if accurate:
+                out, _, _, _ = np.linalg.lstsq(vander, values, rcond=-1.0)
+                return out[deriv_idx] * scale
+            else:
+                return np.dot(coeffs, values)
+
+    else:
+
+        @cfunc(
+            types.intc(
+                types.CPointer(types.float64),
+                types.intp,
+                types.CPointer(types.float64),
+                types.voidptr,
+            )
+        )
+        def _calc_savgol(values_ptr, len_values, result, data):
+            values = carray(values_ptr, (len_values,), dtype=types.float64)
+
+            if accurate:
+                out, _, _, _ = np.linalg.lstsq(vander, values, rcond=-1.0)
+                result[0] = out[deriv_idx] * scale
+            else:
+                result[0] = np.dot(coeffs, values)
+
+            return 1
+
+        _func = scipy.LowLevelCallable(
+            _calc_savgol.ctypes, signature="int (double *, npy_intp, double *, void *)"
+        )
+
+    return scipy.ndimage.generic_filter(
+        arr.astype(np.float64), _func, size=window_shape, mode=mode, cval=cval
+    )
+
+
 def gradient_magnitude(
     input: npt.NDArray[np.float64],
     dx: np.float64,
     dy: np.float64,
     mode: str = "nearest",
     cval: float = 0.0,
 ) -> npt.NDArray[np.float64]:
```

### Comparing `erlab-2.4.2/src/erlab/analysis/interpolate.py` & `erlab-2.5.0/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/kspace.py` & `erlab-2.5.0/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/mask/__init__.py` & `erlab-2.5.0/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/mask/polygon.py` & `erlab-2.5.0/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/transform.py` & `erlab-2.5.0/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/analysis/utilities.py` & `erlab-2.5.0/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/constants.py` & `erlab-2.5.0/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/__init__.py` & `erlab-2.5.0/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/bzplot.py` & `erlab-2.5.0/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/colors.py` & `erlab-2.5.0/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/curvefittingtool.py` & `erlab-2.5.0/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/derivative.py` & `erlab-2.5.0/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/dtool.ui` & `erlab-2.5.0/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/fermiedge.py` & `erlab-2.5.0/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.5.0/src/erlab/interactive/imagetool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,24 @@
     ItoolCrosshairControls,
 )
 from erlab.interactive.imagetool.core import ImageSlicerArea, SlicerLinkProxy
 from erlab.interactive.utilities import DictMenuBar, copy_to_clipboard
 from erlab.io.plugins.merlin import BL403Loader
 
 if TYPE_CHECKING:
-    from collections.abc import Callable, Sequence
+    from collections.abc import Callable, Collection
 
     from erlab.interactive.imagetool.slicer import ArraySlicer
 
 
 def itool(
-    data: Sequence[xr.DataArray | npt.NDArray] | xr.DataArray | npt.NDArray,
+    data: Collection[xr.DataArray | npt.NDArray]
+    | xr.DataArray
+    | npt.NDArray
+    | xr.Dataset,
     link: bool = False,
     link_colors: bool = True,
     execute: bool | None = None,
     **kwargs,
 ) -> ImageTool | list[ImageTool] | None:
     """Create and display an ImageTool window.
 
@@ -77,30 +80,38 @@
     ImageTool or list of ImageTool
         The created ImageTool window(s).
 
     Notes
     -----
     - If `data` is a sequence of valid data, multiple ImageTool windows will be created
       and displayed.
+    - If `data` is a Dataset, each DataArray in the Dataset will be displayed in a
+      separate ImageTool window. Data variables with 2 to 4 dimensions are considered as
+      valid. Other variables are ignored.
     - If `link` is True, the ImageTool windows will be synchronized.
 
     Examples
     --------
     >>> itool(data, cmap="gray", gamma=0.5)
     >>> itool(data_list, link=True)
     """
     qapp = QtWidgets.QApplication.instance()
     if not qapp:
         qapp = QtWidgets.QApplication(sys.argv)
 
     if isinstance(qapp, QtWidgets.QApplication):
         qapp.setStyle("Fusion")
 
+    if isinstance(data, xr.Dataset):
+        data = [d for d in data.data_vars.values() if d.ndim >= 2 and d.ndim <= 4]
+        if len(data) == 0:
+            raise ValueError("No valid data for ImageTool found in the Dataset")
+
     if isinstance(data, np.ndarray | xr.DataArray):
-        data = cast(list[npt.NDArray | xr.DataArray], [data])
+        data = (data,)
 
     itool_list = [ImageTool(d, **kwargs) for d in data]
 
     for w in itool_list:
         w.show()
 
     if len(itool_list) == 0:
```

### Comparing `erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/imagetool/controls.py` & `erlab-2.5.0/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/imagetool/core.py` & `erlab-2.5.0/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.5.0/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.5.0/src/erlab/interactive/imagetool/slicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import numba
 import numpy as np
 import numpy.typing as npt
 from qtpy import QtCore
 
 from erlab.interactive.imagetool.fastbinning import fast_nanmean_skipcheck
+from erlab.interactive.utilities import format_kwargs
 
 if TYPE_CHECKING:
     from collections.abc import Hashable, Sequence
 
     import xarray as xr
 
 VALID_NDIM = (2, 3, 4)
@@ -249,14 +250,20 @@
 
         Returns
         -------
         xarray.DataArray
             The converted data.
 
         """
+        if data.ndim < 2:
+            raise ValueError("Data must have at least two dimensions.")
+
+        if data.ndim > 4:
+            raise ValueError("Data must have at most four dimensions.")
+
         # convert coords to C-contiguous float32
         data = data.assign_coords(
             {d: data[d].astype(np.float32, order="C") for d in data.dims}
         )
 
         if data.dtype not in (np.float32, np.float64):
             data = data.astype(np.float64)
@@ -628,26 +635,18 @@
             return self.isel_code(cursor, disp)
 
         try:
             qsel_kw = self.qsel_args(cursor, disp)
         except ValueError:
             return self.isel_code(cursor, disp)
 
-        dict_repr: str = ""
-        for k, v in qsel_kw.items():
-            dict_repr += f"{k}={v!s}, "
-        dict_repr = dict_repr.rstrip(", ")
-        return f".qsel({dict_repr})"
+        return f".qsel({format_kwargs(qsel_kw)})"
 
     def isel_code(self, cursor: int, disp: Sequence[int]) -> str:
-        dict_repr: str = ""
-        for k, v in self.isel_args(cursor, disp, int_if_one=True).items():
-            dict_repr += f"{k}={v!s}, "
-        dict_repr = dict_repr.rstrip(", ")
-        return f".isel({dict_repr})"
+        return f".isel({format_kwargs(self.isel_args(cursor, disp, int_if_one=True))})"
 
     def xslice(self, cursor: int, disp: Sequence[int]) -> xr.DataArray:
         isel_kw = self.isel_args(cursor, disp, int_if_one=False)
         binned_coord_average: dict[str, xr.DataArray] = {
             str(k): self._obj[k][isel_kw[str(k)]].mean()
             for k, v in zip(self._obj.dims, self.get_binned(cursor), strict=True)
             if v
```

### Comparing `erlab-2.4.2/src/erlab/interactive/kspace.py` & `erlab-2.5.0/src/erlab/interactive/kspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,17 +258,19 @@
         out_lines: list[str] = []
 
         if self.data.kspace.has_hv:
             out_lines.append(
                 f"{input_name}.kspace.inner_potential"
                 f" = {self._offset_spins['V0'].value()}"
             )
+
+        offset_dict_repr = str(self.offset_dict).replace("'", '"')
         out_lines.extend(
             (
-                f"{input_name}.kspace.offsets = {self.offset_dict}",
+                f"{input_name}.kspace.offsets = {offset_dict_repr}",
                 gen_function_code(
                     copy=False,
                     **{f"{input_name}_kconv = {input_name}.kspace.convert": [arg_dict]},
                 ),
             )
         )
```

### Comparing `erlab-2.4.2/src/erlab/interactive/ktool.ui` & `erlab-2.5.0/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/masktool.py` & `erlab-2.5.0/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/interactive/utilities.py` & `erlab-2.5.0/src/erlab/interactive/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,28 +76,38 @@
     """
     if isinstance(content, list):
         content = "\n".join(content)
     pyperclip.copy(content)
     return content
 
 
-def process_arg(arg):
+def _parse_single_arg(arg):
     if isinstance(arg, str):
         if arg.startswith("|") and arg.endswith("|"):
+            # If the string is surrounded by vertical bars, remove them
             arg = arg[1:-1]
+
         else:
+            # Otherwise, quote the string
             arg = f'"{arg}"'
+
+    elif isinstance(arg, dict):
+        # If the argument is a dict, convert to string with double quotes
+        arg = str(arg).replace("'", '"')
+
     return arg
 
 
 def gen_single_function_code(funcname: str, *args: tuple, **kwargs):
     """Generate the string for a Python function call.
 
-    The first argument is the name of the function, and subsequent arguments are
-    passed as positional arguments. Keyword arguments are also supported.
+    The first argument is the name of the function, and subsequent arguments are passed
+    as positional arguments. Keyword arguments are also supported. For strings in
+    arguments and keyword arguments, surrounding the string with vertical bars (``|``)
+    will prevent the string from being quoted.
 
     Parameters
     ----------
     funcname
         Name of the function.
     *args
         Mandatory arguments passed onto the function.
@@ -107,37 +117,39 @@
     Returns
     -------
     code : str
         generated code.
 
     """
     if len(args) == 0 and len(kwargs) == 0:
+        # If no arguments are passed, return the function name
         return f"{funcname}()"
-    tab = "    "
+
+    TAB = "    "
+
+    # Start with function call and open parenthesis
     code = f"{funcname}(\n"
+
     for v in args:
-        if isinstance(v, str):
-            if v.startswith("|") and v.endswith("|"):
-                v = v[1:-1]
-            else:
-                v = f'"{v}"'
-        code += f"{tab}{v},\n"
+        # Add positional argument to code string
+        code += f"{TAB}{_parse_single_arg(v)},\n"
+
     for k, v in kwargs.items():
-        if isinstance(v, str):
-            if v.startswith("|") and v.endswith("|"):
-                v = v[1:-1]
-            else:
-                v = f'"{v}"'
-        code += f"{tab}{k}={v},\n"
+        # Add keyword argument to code string
+        code += f"{TAB}{k}={_parse_single_arg(v)},\n"
+
+    # Add closing parenthesis
     code += ")"
 
     if len(code.replace("\n", "")) <= 88:
         # If code fits in one line, remove newlines
         code = " ".join([s.strip() for s in code.split("\n")])
+        # Remove trailing comma and space
         code = code.replace(", )", ")").replace("( ", "(")
+
     return code
 
 
 def gen_function_code(copy: bool = True, **kwargs):
     r"""Copy the Python code for function calls to the clipboard.
 
     The result can be copied to your clipboard in a form that can be pasted into an
@@ -150,27 +162,46 @@
     **kwargs
         Dictionary where the keys are the string of the function call and the values are
         a list of function arguments. The last item, if a dictionary, is interpreted as
         keyword arguments.
 
     """
     code_list = []
-    for k, v in kwargs.items():
-        if not isinstance(v[-1], dict):
-            v.append({})
-        code_list.append(gen_single_function_code(k, *v[:-1], **v[-1]))
+    for fname, fargs in kwargs.items():
+        if not isinstance(fargs[-1], dict):
+            fargs.append({})
+        code_list.append(gen_single_function_code(fname, *fargs[:-1], **fargs[-1]))
 
     code_str = "\n".join(code_list)
 
     if copy:
         return copy_to_clipboard(code_str)
     else:
         return code_str
 
 
+def format_kwargs(d: dict[str, Any]) -> str:
+    """Format a dictionary of keyword arguments for a function call.
+
+    If the keys are valid Python identifiers, the output will be formatted as keyword
+    arguments. Otherwise, the output will be formatted as a dictionary.
+
+    Parameters
+    ----------
+    d
+        Dictionary of keyword arguments.
+
+    """
+    if all(s.isidentifier() for s in d.keys()):
+        return ", ".join(f"{k}={_parse_single_arg(v)!s}" for k, v in d.items())
+    else:
+        out = ", ".join(f'"{k}": {_parse_single_arg(v)!s}' for k, v in d.items())
+        return "{" + out + "}"
+
+
 class BetterSpinBox(QtWidgets.QAbstractSpinBox):
     """An improved spinbox.
 
     Signals
     ----------
     valueChanged
         Emitted when the value is changed.
```

### Comparing `erlab-2.4.2/src/erlab/io/__init__.py` & `erlab-2.5.0/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/characterization/resistance.py` & `erlab-2.5.0/src/erlab/io/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/characterization/xrd.py` & `erlab-2.5.0/src/erlab/io/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/dataloader.py` & `erlab-2.5.0/src/erlab/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/exampledata.py` & `erlab-2.5.0/src/erlab/io/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/igor.py` & `erlab-2.5.0/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/plugins/__init__.py` & `erlab-2.5.0/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/plugins/da30.py` & `erlab-2.5.0/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/plugins/kriss.py` & `erlab-2.5.0/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/plugins/merlin.py` & `erlab-2.5.0/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/io/utilities.py` & `erlab-2.5.0/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/lattice.py` & `erlab-2.5.0/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/parallel.py` & `erlab-2.5.0/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.5.0/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.5.0/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.5.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.5.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.5.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.5.0/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.5.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.5.0/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.5.0/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.5.0/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/__init__.py` & `erlab-2.5.0/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/annotations.py` & `erlab-2.5.0/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/atoms.py` & `erlab-2.5.0/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/bz.py` & `erlab-2.5.0/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/colors.py` & `erlab-2.5.0/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/general.py` & `erlab-2.5.0/src/erlab/plotting/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 __all__ = [
     "LabeledCursor",
     "autoscale_off",
     "autoscale_to",
+    "clean_labels",
     "fermiline",
     "figwh",
     "gradient_fill",
     "place_inset",
     "plot_array",
     "plot_array_2d",
     "plot_slices",
@@ -1130,7 +1131,42 @@
     match orientation:
         case "h":
             return ax.axhline(value, ls=ls, lw=lw, c=c, **kwargs)
         case "v":
             return ax.axvline(value, ls=ls, lw=lw, c=c, **kwargs)
         case _:
             raise ValueError("`orientation` must be either 'v' or 'h'")
+
+
+def clean_labels(
+    axes: Iterable[matplotlib.axes.Axes],
+    remove_inner_ticks: bool = False,
+    **kwargs,
+):
+    """Clean the labels of the given axes.
+
+    This function removes the labels from the axes except for the outermost axes and
+    prettifies the remaining labels with :func:`fancy_labels
+    <erlab.plotting.annotations.fancy_labels>`.
+
+    .. versionchanged:: 2.5.0
+
+       The function now calls :meth:`Axes.label_outer
+       <matplotlib.axes.Axes.label_outer>` recursively instead of setting the labels to
+       an empty string.
+
+    Parameters
+    ----------
+    axes
+        The axes to clean the labels for.
+    remove_inner_ticks
+        If `True`, remove the inner ticks as well (not only tick labels).
+    **kwargs
+        Additional keyword arguments to be passed to :func:`fancy_labels
+        <erlab.plotting.annotations.fancy_labels>`.
+
+    """
+    axes = np.asarray(axes)
+
+    for ax in axes.flat:
+        ax.label_outer(remove_inner_ticks=remove_inner_ticks)
+    fancy_labels(axes, **kwargs)
```

### Comparing `erlab-2.4.2/src/erlab/plotting/plot3d.py` & `erlab-2.5.0/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.5.0/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.5.0/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.5.0/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.5.0/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.5.0/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.5.0/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/src/erlab.egg-info/PKG-INFO` & `erlab-2.5.0/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.4.2
+Version: 2.5.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.4.2/src/erlab.egg-info/SOURCES.txt` & `erlab-2.5.0/src/erlab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -141,11 +141,12 @@
 tests/accessors/test_fit.py
 tests/accessors/test_kspace.py
 tests/analysis/test_fastbinning.py
 tests/analysis/test_fit_functions_dynamic.py
 tests/analysis/test_fit_functions_general.py
 tests/analysis/test_fit_models.py
 tests/analysis/test_image.py
+tests/analysis/test_image_savgol.py
 tests/analysis/test_interpolate.py
 tests/analysis/test_kspace.py
 tests/analysis/test_utilities.py
 tests/io/test_dataloader.py
```

### Comparing `erlab-2.4.2/src/erlab.egg-info/requires.txt` & `erlab-2.5.0/src/erlab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/templates/.macros.j2` & `erlab-2.5.0/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/accessors/test_fit.py` & `erlab-2.5.0/tests/accessors/test_fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/accessors/test_kspace.py` & `erlab-2.5.0/tests/accessors/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/analysis/test_fastbinning.py` & `erlab-2.5.0/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.5.0/tests/analysis/test_fit_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/analysis/test_fit_functions_general.py` & `erlab-2.5.0/tests/analysis/test_fit_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/analysis/test_fit_models.py` & `erlab-2.5.0/tests/analysis/test_fit_models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/analysis/test_image.py` & `erlab-2.5.0/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/analysis/test_interpolate.py` & `erlab-2.5.0/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/analysis/test_kspace.py` & `erlab-2.5.0/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/analysis/test_utilities.py` & `erlab-2.5.0/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.4.2/tests/io/test_dataloader.py` & `erlab-2.5.0/tests/io/test_dataloader.py`

 * *Files identical despite different names*

