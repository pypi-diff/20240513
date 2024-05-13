# Comparing `tmp/anemoi_datasets-0.1.7.tar.gz` & `tmp/anemoi_datasets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi_datasets-0.1.7.tar", last modified: Tue May  7 09:21:59 2024, max compression
+gzip compressed data, was "anemoi_datasets-0.2.0.tar", last modified: Mon May 13 09:26:05 2024, max compression
```

## Comparing `anemoi_datasets-0.1.7.tar` & `anemoi_datasets-0.2.0.tar`

### file list

```diff
@@ -1,280 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.389526 anemoi_datasets-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.341527 anemoi_datasets-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.345527 anemoi_datasets-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.349527 anemoi_datasets-0.1.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/.vscode/spellright.dict
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-05-07 09:21:59.389526 anemoi_datasets-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.349527 anemoi_datasets-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.349527 anemoi_datasets-0.1.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.349527 anemoi_datasets-0.1.7/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/_templates/.gitkeep
--rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/apply-fmt.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.353527 anemoi_datasets-0.1.7/docs/building/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.353527 anemoi_datasets-0.1.7/docs/building/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/filters/empty.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/filters/noop.rst
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/filters/rename.rst
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/filters/rotate_winds.rst
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/filters/select.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/filters/unrotate_winds.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/filters.rst
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/handling-missing-dates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/handling-missing-values.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/naming-variables.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/operations.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.353527 anemoi_datasets-0.1.7/docs/building/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/accumulations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/accumulations1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/accumulations2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/forcings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/forcings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/grib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/mars.rst
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/mars1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/mars2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/netcdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/netcdf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/opendap.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/opendap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/perturbations.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.357527 anemoi_datasets-0.1.7/docs/building/sources/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/yaml/grib1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/yaml/grib2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/yaml/grib3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/yaml/grib4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources/yaml/perturbations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/sources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/statistics.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/syntax.rst
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/syntax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.357527 anemoi_datasets-0.1.7/docs/building/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/building1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/building1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/building2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/building2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/building3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/building3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/concat.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/input.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/missing_dates.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/building/yaml/pipe.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/check-index.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.357527 anemoi_datasets-0.1.7/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/cli/compare.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/cli/copy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/cli/create.rst
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/cli/inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/cli/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/images.pptx
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/overview_.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.361527 anemoi_datasets-0.1.7/docs/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   106709 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/schemas/matrix.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)    53069 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/schemas/matrix.png
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/schemas/overview.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/schemas/overview.png
--rw-r--r--   0 runner    (1001) docker     (127)    42125 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/schemas/recipe.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)    43845 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/schemas/recipe.png
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.361527 anemoi_datasets-0.1.7/docs/using/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.369526 anemoi_datasets-0.1.7/docs/using/code/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/area1_.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/area2_.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/chain_.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/combine_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/concat1.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/cutout_.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/drop_.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/end_.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/ensembles1_.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/frequency_.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/grids1_.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/join1.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/matching0_.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/matching1_.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/matching2_.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/matching3_.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/matching4_.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/misc1.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/misc2.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/missing_.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_combine1_.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_combine2_.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_dict_.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_first_.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_list_.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_other.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_path.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/open_yaml_.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/rename_.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/reorder1_.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/reorder2_.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/select1_.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/select2_.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/shuffle_.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/some_attributes_.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/start_.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/statistics_.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/subset_example.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/thinning_.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/zip1_.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/code/zip2_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/combining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/configuration.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/grids.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.373527 anemoi_datasets-0.1.7/docs/using/images/
--rw-r--r--   0 runner    (1001) docker     (127)   108038 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/area-1.png
--rw-r--r--   0 runner    (1001) docker     (127)    40564 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/concat.png
--rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/cutout-1.png
--rw-r--r--   0 runner    (1001) docker     (127)   122139 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/cutout-2.png
--rw-r--r--   0 runner    (1001) docker     (127)   129758 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/cutout-3.png
--rw-r--r--   0 runner    (1001) docker     (127)   151858 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/cutout-4.png
--rw-r--r--   0 runner    (1001) docker     (127)    38066 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/join.png
--rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/overlay.png
--rw-r--r--   0 runner    (1001) docker     (127)   109206 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/thinning-after.png
--rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/images/thinning-before.png
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/matching.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/methods.rst
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/miscellaneous.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/opening.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/other.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/selecting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/statistics.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/docs/using/subsetting.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:21:59.389526 anemoi_datasets-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.345527 anemoi_datasets-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.345527 anemoi_datasets-0.1.7/src/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.373527 anemoi_datasets-0.1.7/src/anemoi/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 09:21:59.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.373527 anemoi_datasets-0.1.7/src/anemoi/datasets/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/commands/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/commands/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.373527 anemoi_datasets-0.1.7/src/anemoi/datasets/commands/inspect/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/commands/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/commands/inspect/zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/commands/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.373527 anemoi_datasets-0.1.7/src/anemoi/datasets/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/compute/perturbations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.377527 anemoi_datasets-0.1.7/src/anemoi/datasets/create/
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.377527 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.377527 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/rotate_winds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/unrotate_winds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.381527 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/accumulations.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/forcings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/grib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/opendap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/tendencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    27981 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    28020 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/loaders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3682 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.381527 anemoi_datasets-0.1.7/src/anemoi/datasets/create/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/statistics/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/create/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.381527 anemoi_datasets-0.1.7/src/anemoi/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/debug.css
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/forewards.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/masked.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/data/unchecked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.381527 anemoi_datasets-0.1.7/src/anemoi/datasets/dates/
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/dates/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/grids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.385527 anemoi_datasets-0.1.7/src/anemoi/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/src/anemoi/datasets/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.389526 anemoi_datasets-0.1.7/src/anemoi_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-05-07 09:21:59.000000 anemoi_datasets-0.1.7/src/anemoi_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-07 09:21:59.000000 anemoi_datasets-0.1.7/src/anemoi_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:21:59.000000 anemoi_datasets-0.1.7/src/anemoi_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 09:21:59.000000 anemoi_datasets-0.1.7/src/anemoi_datasets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 09:21:59.000000 anemoi_datasets-0.1.7/src/anemoi_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 09:21:59.000000 anemoi_datasets-0.1.7/src/anemoi_datasets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.385527 anemoi_datasets-0.1.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.385527 anemoi_datasets-0.1.7/tests/create/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create/concat.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create/data_sources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create/join.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create/missing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create/nan.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create/perturbations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create/pipe.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     7619 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create-perturbations-full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/create-shift.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/test_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)    36578 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tests/test_indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.385527 anemoi_datasets-0.1.7/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tools/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.385527 anemoi_datasets-0.1.7/tools/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tools/examples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tools/examples/an-oper-2023-2023-2p5-6h-v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:21:59.389526 anemoi_datasets-0.1.7/tools/grids/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tools/grids/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tools/grids/grids.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tools/grids/grids1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-07 09:21:44.000000 anemoi_datasets-0.1.7/tools/grids/grids2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.599055 anemoi_datasets-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.551056 anemoi_datasets-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.555056 anemoi_datasets-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.555056 anemoi_datasets-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/.vscode/spellright.dict
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-05-13 09:26:05.599055 anemoi_datasets-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.559056 anemoi_datasets-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.559056 anemoi_datasets-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.559056 anemoi_datasets-0.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/_templates/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/apply-fmt.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.559056 anemoi_datasets-0.2.0/docs/building/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.563056 anemoi_datasets-0.2.0/docs/building/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/filters/empty.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/filters/noop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/filters/rename.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/filters/rotate_winds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/filters/select.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/filters/unrotate_winds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/handling-missing-dates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/handling-missing-values.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/naming-variables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/operations.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.563056 anemoi_datasets-0.2.0/docs/building/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/accumulations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/accumulations1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/accumulations2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/forcings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/forcings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/mars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/mars1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/mars2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/netcdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/netcdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/opendap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/opendap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/perturbations.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.563056 anemoi_datasets-0.2.0/docs/building/sources/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/yaml/grib1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/yaml/grib2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/yaml/grib3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/yaml/grib4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources/yaml/perturbations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/sources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/statistics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/syntax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/syntax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.567056 anemoi_datasets-0.2.0/docs/building/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/building1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/building1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/building2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/building2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/building3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/building3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/concat.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/input.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/missing_dates.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/nan.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/building/yaml/pipe.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/check-index.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.567056 anemoi_datasets-0.2.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/cli/compare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/cli/copy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/cli/create.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/cli/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/cli/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/images.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/overview_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.567056 anemoi_datasets-0.2.0/docs/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   106709 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/schemas/matrix.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)    53069 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/schemas/matrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/schemas/overview.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/schemas/overview.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42125 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/schemas/recipe.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)    43845 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/schemas/recipe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.571056 anemoi_datasets-0.2.0/docs/using/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.575056 anemoi_datasets-0.2.0/docs/using/code/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/area1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/area2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/chain_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/combine_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/concat1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/cutout_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/drop_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/end_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/ensembles1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/frequency_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/grids1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/join1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/matching0_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/matching1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/matching2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/matching3_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/matching4_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/misc1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/misc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/missing_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_combine1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_combine2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_dict_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_first_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_list_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/open_yaml_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/rename_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/reorder1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/reorder2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/select1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/select2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/shuffle_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/some_attributes_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/start_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/statistics_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/subset_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/thinning_.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/zip1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/code/zip2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/combining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/configuration.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/grids.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.579056 anemoi_datasets-0.2.0/docs/using/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   108038 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/area-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40564 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/concat.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/cutout-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122139 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/cutout-2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   129758 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/cutout-3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151858 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/cutout-4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38066 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/join.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/overlay.png
+-rw-r--r--   0 runner    (1001) docker     (127)   109206 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/thinning-after.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141221 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/images/thinning-before.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/matching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/miscellaneous.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/opening.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/other.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/selecting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/statistics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/docs/using/subsetting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:26:05.599055 anemoi_datasets-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.555056 anemoi_datasets-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.555056 anemoi_datasets-0.2.0/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.579056 anemoi_datasets-0.2.0/src/anemoi/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 09:26:05.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.579056 anemoi_datasets-0.2.0/src/anemoi/datasets/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/commands/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/commands/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.579056 anemoi_datasets-0.2.0/src/anemoi/datasets/commands/inspect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/commands/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/commands/inspect/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/commands/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.583056 anemoi_datasets-0.2.0/src/anemoi/datasets/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/compute/perturbations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.583056 anemoi_datasets-0.2.0/src/anemoi/datasets/create/
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.583056 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.583056 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/rotate_winds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/unrotate_winds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.587056 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/accumulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/forcings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/opendap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/tendencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27981 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28416 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/loaders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3682 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.587056 anemoi_datasets-0.2.0/src/anemoi/datasets/create/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/statistics/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/create/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.591055 anemoi_datasets-0.2.0/src/anemoi/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/debug.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/forewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/masked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/data/unchecked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.591055 anemoi_datasets-0.2.0/src/anemoi/datasets/dates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/dates/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.591055 anemoi_datasets-0.2.0/src/anemoi/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/src/anemoi/datasets/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.595055 anemoi_datasets-0.2.0/src/anemoi_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-05-13 09:26:05.000000 anemoi_datasets-0.2.0/src/anemoi_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-13 09:26:05.000000 anemoi_datasets-0.2.0/src/anemoi_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:26:05.000000 anemoi_datasets-0.2.0/src/anemoi_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 09:26:05.000000 anemoi_datasets-0.2.0/src/anemoi_datasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 09:26:05.000000 anemoi_datasets-0.2.0/src/anemoi_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 09:26:05.000000 anemoi_datasets-0.2.0/src/anemoi_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.591055 anemoi_datasets-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.595055 anemoi_datasets-0.2.0/tests/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create/concat.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create/data_sources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create/join.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create/missing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create/nan.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create/perturbations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create/pipe.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7700 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create-perturbations-full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/create-shift.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/test_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36578 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tests/test_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.595055 anemoi_datasets-0.2.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tools/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.595055 anemoi_datasets-0.2.0/tools/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tools/examples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tools/examples/an-oper-2023-2023-2p5-6h-v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:26:05.595055 anemoi_datasets-0.2.0/tools/grids/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tools/grids/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tools/grids/grids.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tools/grids/grids1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-13 09:25:55.000000 anemoi_datasets-0.2.0/tools/grids/grids2.yaml
```

### Comparing `anemoi_datasets-0.1.7/.github/workflows/python-publish.yml` & `anemoi_datasets-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/.gitignore` & `anemoi_datasets-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/.pre-commit-config.yaml` & `anemoi_datasets-0.2.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   rev: v4.4.0
   hooks:
   - id: check-yaml # Check YAML files for syntax errors only
     args: [--unsafe, --allow-multiple-documents]
   - id: debug-statements # Check for debugger imports and py37+ breakpoint()
   - id: end-of-file-fixer # Ensure files end in a newline
   - id: trailing-whitespace # Trailing whitespace checker
-  - id: no-commit-to-branch # Prevent committing to main / master
+#  - id: no-commit-to-branch # Prevent committing to main / master
   - id: check-added-large-files # Check for large files added to git
   - id: check-merge-conflict # Check for files that contain merge conflict
 
 - repo: https://github.com/psf/black-pre-commit-mirror
   rev: 24.1.1
   hooks:
     - id: black
```

### Comparing `anemoi_datasets-0.1.7/LICENSE` & `anemoi_datasets-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/PKG-INFO` & `anemoi_datasets-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-datasets
-Version: 0.1.7
+Version: 0.2.0
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,15 +219,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: anemoi-utils[provenance]>=0.1.7
-Requires-Dist: zarr
+Requires-Dist: zarr<=2.17.0
 Requires-Dist: pyyaml
 Requires-Dist: numpy
 Requires-Dist: tqdm
 Requires-Dist: semantic-version
 Provides-Extra: remote
 Requires-Dist: boto3; extra == "remote"
 Requires-Dist: requests; extra == "remote"
```

### Comparing `anemoi_datasets-0.1.7/README.md` & `anemoi_datasets-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/Makefile` & `anemoi_datasets-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/_static/logo.png` & `anemoi_datasets-0.2.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/_static/style.css` & `anemoi_datasets-0.2.0/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/handling-missing-dates.rst` & `anemoi_datasets-0.2.0/docs/building/handling-missing-dates.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/introduction.rst` & `anemoi_datasets-0.2.0/docs/building/introduction.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/operations.rst` & `anemoi_datasets-0.2.0/docs/building/operations.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/sources/accumulations.rst` & `anemoi_datasets-0.2.0/docs/building/sources/accumulations.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/sources/forcings.rst` & `anemoi_datasets-0.2.0/docs/building/sources/forcings.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/sources/grib.rst` & `anemoi_datasets-0.2.0/docs/building/sources/grib.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/sources/mars.rst` & `anemoi_datasets-0.2.0/docs/building/sources/mars.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/sources/perturbations.rst` & `anemoi_datasets-0.2.0/docs/building/sources/perturbations.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/statistics.rst` & `anemoi_datasets-0.2.0/docs/building/statistics.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 algorithm:
 
    -  If the dataset covers 20 years or more, the last 3 years are
       excluded.
    -  If the dataset covers 10 years or more, the last year is excluded.
    -  Otherwise, 80% of the dataset is used.
 
-You can override this behaviour by setting the `start` and `end`
+You can override this behaviour by setting the `start` or `end`
 parameters in the `statistics` config.
 
 .. code:: yaml
 
    statistics:
        start: 2000
        end: 2020
```

### Comparing `anemoi_datasets-0.1.7/docs/building/yaml/building1.txt` & `anemoi_datasets-0.2.0/docs/building/yaml/building1.txt`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/yaml/building2.txt` & `anemoi_datasets-0.2.0/docs/building/yaml/building2.txt`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/building/yaml/building3.txt` & `anemoi_datasets-0.2.0/docs/building/yaml/building3.txt`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/conf.py` & `anemoi_datasets-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/images.pptx` & `anemoi_datasets-0.2.0/docs/images.pptx`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/index.rst` & `anemoi_datasets-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/installing.rst` & `anemoi_datasets-0.2.0/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/overview.rst` & `anemoi_datasets-0.2.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/schemas/matrix.excalidraw` & `anemoi_datasets-0.2.0/docs/schemas/matrix.excalidraw`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/schemas/matrix.png` & `anemoi_datasets-0.2.0/docs/schemas/matrix.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/schemas/overview.excalidraw` & `anemoi_datasets-0.2.0/docs/schemas/overview.excalidraw`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/schemas/overview.png` & `anemoi_datasets-0.2.0/docs/schemas/overview.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/schemas/recipe.excalidraw` & `anemoi_datasets-0.2.0/docs/schemas/recipe.excalidraw`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/schemas/recipe.png` & `anemoi_datasets-0.2.0/docs/schemas/recipe.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/test.ipynb` & `anemoi_datasets-0.2.0/docs/test.ipynb`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/combining.rst` & `anemoi_datasets-0.2.0/docs/using/combining.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/configuration.rst` & `anemoi_datasets-0.2.0/docs/using/configuration.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/grids.rst` & `anemoi_datasets-0.2.0/docs/using/grids.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/area-1.png` & `anemoi_datasets-0.2.0/docs/using/images/area-1.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/concat.png` & `anemoi_datasets-0.2.0/docs/using/images/concat.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/cutout-1.png` & `anemoi_datasets-0.2.0/docs/using/images/cutout-1.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/cutout-2.png` & `anemoi_datasets-0.2.0/docs/using/images/cutout-2.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/cutout-3.png` & `anemoi_datasets-0.2.0/docs/using/images/cutout-3.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/cutout-4.png` & `anemoi_datasets-0.2.0/docs/using/images/cutout-4.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/join.png` & `anemoi_datasets-0.2.0/docs/using/images/join.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/overlay.png` & `anemoi_datasets-0.2.0/docs/using/images/overlay.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/thinning-after.png` & `anemoi_datasets-0.2.0/docs/using/images/thinning-after.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/images/thinning-before.png` & `anemoi_datasets-0.2.0/docs/using/images/thinning-before.png`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/introduction.rst` & `anemoi_datasets-0.2.0/docs/using/introduction.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/matching.rst` & `anemoi_datasets-0.2.0/docs/using/matching.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/methods.rst` & `anemoi_datasets-0.2.0/docs/using/methods.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/miscellaneous.rst` & `anemoi_datasets-0.2.0/docs/using/miscellaneous.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/opening.rst` & `anemoi_datasets-0.2.0/docs/using/opening.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/other.rst` & `anemoi_datasets-0.2.0/docs/using/other.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/selecting.rst` & `anemoi_datasets-0.2.0/docs/using/selecting.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/docs/using/subsetting.rst` & `anemoi_datasets-0.2.0/docs/using/subsetting.rst`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/pyproject.toml` & `anemoi_datasets-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "anemoi-utils[provenance]>=0.1.7",
-    "zarr",
+    "zarr<=2.17.0",
     "pyyaml",
     "numpy",
     "tqdm",
     "semantic-version",
 ]
 
 [project.optional-dependencies]
```

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/__init__.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/__main__.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/commands/__init__.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/commands/compare.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/commands/compare.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/commands/copy.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/commands/copy.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/commands/create.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/commands/create.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/commands/inspect/__init__.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/commands/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/commands/inspect/zarr.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/commands/inspect/zarr.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/commands/scan.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/commands/scan.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/compute/perturbations.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/compute/perturbations.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "sf",
     "swl4",
     "swl3",
     "swl2",
     "swl1",
 )
 
-SKIP = ("class", "stream", "type", "number", "expver", "_leg_number")
+SKIP = ("class", "stream", "type", "number", "expver", "_leg_number", "anoffset")
 
 
 def check_compatible(f1, f2, center_field_as_mars, ensemble_field_as_mars):
     assert f1.mars_grid == f2.mars_grid, (f1.mars_grid, f2.mars_grid)
     assert f1.mars_area == f2.mars_area, (f1.mars_area, f2.mars_area)
     assert f1.shape == f2.shape, (f1.shape, f2.shape)
```

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/__init__.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,45 +90,45 @@
         cleaner.registry.clean()
 
     def patch(self, **kwargs):
         from .patch import apply_patch
 
         apply_patch(self.path, **kwargs)
 
-    def init_additions(self, delta=[1, 3, 6, 12]):
+    def init_additions(self, delta=[1, 3, 6, 12, 24]):
         from .loaders import StatisticsAddition
         from .loaders import TendenciesStatisticsAddition
         from .loaders import TendenciesStatisticsDeltaNotMultipleOfFrequency
 
         a = StatisticsAddition.from_dataset(path=self.path, print=self.print)
         a.initialise()
 
         for d in delta:
             try:
                 a = TendenciesStatisticsAddition.from_dataset(path=self.path, print=self.print, delta=d)
                 a.initialise()
             except TendenciesStatisticsDeltaNotMultipleOfFrequency:
                 self.print(f"Skipping delta={d} as it is not a multiple of the frequency.")
 
-    def run_additions(self, parts=None, delta=[1, 3, 6, 12]):
+    def run_additions(self, parts=None, delta=[1, 3, 6, 12, 24]):
         from .loaders import StatisticsAddition
         from .loaders import TendenciesStatisticsAddition
         from .loaders import TendenciesStatisticsDeltaNotMultipleOfFrequency
 
         a = StatisticsAddition.from_dataset(path=self.path, print=self.print)
         a.run(parts)
 
         for d in delta:
             try:
                 a = TendenciesStatisticsAddition.from_dataset(path=self.path, print=self.print, delta=d)
                 a.run(parts)
             except TendenciesStatisticsDeltaNotMultipleOfFrequency:
                 self.print(f"Skipping delta={d} as it is not a multiple of the frequency.")
 
-    def finalise_additions(self, delta=[1, 3, 6, 12]):
+    def finalise_additions(self, delta=[1, 3, 6, 12, 24]):
         from .loaders import StatisticsAddition
         from .loaders import TendenciesStatisticsAddition
         from .loaders import TendenciesStatisticsDeltaNotMultipleOfFrequency
 
         a = StatisticsAddition.from_dataset(path=self.path, print=self.print)
         a.finalise()
 
@@ -146,18 +146,18 @@
     def create(self):
         self.init()
         self.load()
         self.finalise()
         self.additions()
         self.cleanup()
 
-    def additions(self):
-        self.init_additions()
-        self.run_additions()
-        self.finalise_additions()
+    def additions(self, delta=[1, 3, 6, 12, 24]):
+        self.init_additions(delta=delta)
+        self.run_additions(delta=delta)
+        self.finalise_additions(delta=delta)
 
     def _cache_context(self):
         from .utils import cache_context
 
         return cache_context(self.cache)
 
     def _path_readable(self):
```

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/check.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/check.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/chunks.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/chunks.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/config.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/config.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/__init__.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/empty.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/empty.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/rename.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/rename.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/rotate_winds.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/rotate_winds.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/filters/unrotate_winds.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/filters/unrotate_winds.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/accumulations.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/accumulations.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/constants.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/constants.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/forcings.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/forcings.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/grib.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/grib.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/mars.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/mars.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/netcdf.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/netcdf.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/opendap.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/opendap.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/perturbations.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/perturbations.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/source.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/source.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/functions/sources/tendencies.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/functions/sources/tendencies.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/input.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/input.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/loaders.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -542,20 +542,25 @@
         LOG.info(f"Wrote statistics in {self.path}")
 
     def write_stats_to_stdout(self, stats):
         LOG.info(stats)
 
 
 class GenericAdditions(GenericDatasetHandler):
-    def __init__(self, name="", **kwargs):
+    def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = name
+        self.tmp_storage = build_storage(directory=self.tmp_storage_path, create=True)
 
-        storage_path = f"{self.path}.tmp_storage_{name}"
-        self.tmp_storage = build_storage(directory=storage_path, create=True)
+    @property
+    def tmp_storage_path(self):
+        raise NotImplementedError
+
+    @property
+    def final_storage_path(self):
+        raise NotImplementedError
 
     def initialise(self):
         self.tmp_storage.delete()
         self.tmp_storage.create()
         LOG.info(f"Dataset {self.path} additions initialized.")
 
     @cached_property
@@ -585,15 +590,15 @@
             minimum=np.full(shape, np.nan, dtype=np.float64),
             maximum=np.full(shape, np.nan, dtype=np.float64),
             sums=np.full(shape, np.nan, dtype=np.float64),
             squares=np.full(shape, np.nan, dtype=np.float64),
             count=np.full(shape, -1, dtype=np.int64),
             has_nans=np.full(shape, False, dtype=np.bool_),
         )
-        LOG.info(f"Aggregating {self.name} statistics on shape={shape}. Variables : {self.variables}")
+        LOG.info(f"Aggregating {self.__class__.__name__} statistics on shape={shape}. Variables : {self.variables}")
 
         found = set()
         ifound = set()
         missing = set()
         for _date, (date, i, stats) in self.tmp_storage.items():
             assert _date == date
             if stats == "missing":
@@ -655,37 +660,45 @@
         LOG.info(f"Dataset {self.path} additions finalized.")
         self.check_statistics()
         self._write(self.summary)
         self.tmp_storage.delete()
 
     def _write(self, summary):
         for k in ["mean", "stdev", "minimum", "maximum", "sums", "squares", "count", "has_nans"]:
-            self._add_dataset(name=k, array=summary[k])
-        self.registry.add_to_history("compute_statistics_end")
-        LOG.info(f"Wrote {self.name} additions in {self.path}")
+            name = self.final_storage_name(k)
+            self._add_dataset(name=name, array=summary[k])
+        self.registry.add_to_history(f"compute_statistics_{self.__class__.__name__.lower()}_end")
+        LOG.info(f"Wrote additions in {self.path} ({self.final_storage_name('*')})")
 
     def check_statistics(self):
         pass
 
 
 class StatisticsAddition(GenericAdditions):
     def __init__(self, **kwargs):
-        super().__init__("statistics_", **kwargs)
+        super().__init__(**kwargs)
 
         z = zarr.open(self.path, mode="r")
         start = z.attrs["statistics_start_date"]
         end = z.attrs["statistics_end_date"]
         self.ds = open_dataset(self.path, start=start, end=end)
 
         self.variables = self.ds.variables
         self.dates = self.ds.dates
 
         assert len(self.variables) == self.ds.shape[1], self.ds.shape
         self.total = len(self.dates)
 
+    @property
+    def tmp_storage_path(self):
+        return f"{self.path}.tmp_storage_statistics"
+
+    def final_storage_name(self, k):
+        return k
+
     def run(self, parts):
         chunk_filter = ChunkFilter(parts=parts, total=self.total)
         for i in range(0, self.total):
             if not chunk_filter(i):
                 continue
             date = self.dates[i]
             try:
@@ -721,56 +734,64 @@
 
 
 class TendenciesStatisticsDeltaNotMultipleOfFrequency(ValueError):
     pass
 
 
 class TendenciesStatisticsAddition(GenericAdditions):
-    DATASET_NAME_PATTERN = "statistics_tendencies_{delta}"
-
     def __init__(self, path, delta=None, **kwargs):
         full_ds = open_dataset(path)
         self.variables = full_ds.variables
 
         frequency = full_ds.frequency
         if delta is None:
             delta = frequency
         assert isinstance(delta, int), delta
         if not delta % frequency == 0:
             raise TendenciesStatisticsDeltaNotMultipleOfFrequency(
                 f"Delta {delta} is not a multiple of frequency {frequency}"
             )
+        self.delta = delta
         idelta = delta // frequency
 
-        super().__init__(path=path, name=self.DATASET_NAME_PATTERN.format(delta=f"{delta}h"), **kwargs)
+        super().__init__(path=path, **kwargs)
 
         z = zarr.open(self.path, mode="r")
         start = z.attrs["statistics_start_date"]
         end = z.attrs["statistics_end_date"]
         start = datetime.datetime.fromisoformat(start)
         ds = open_dataset(self.path, start=start + datetime.timedelta(hours=delta), end=end)
         self.dates = ds.dates
         self.total = len(self.dates)
 
         ds = open_dataset(self.path, start=start, end=end)
         self.ds = DeltaDataset(ds, idelta)
 
+    @property
+    def tmp_storage_path(self):
+        return f"{self.path}.tmp_storage_statistics_{self.delta}h"
+
+    def final_storage_name(self, k):
+        return self.final_storage_name_from_delta(k, delta=self.delta)
+
+    @classmethod
+    def final_storage_name_from_delta(_, k, delta):
+        if isinstance(delta, int):
+            delta = str(delta)
+        if not delta.endswith("h"):
+            delta = delta + "h"
+        return f"statistics_tendencies_{delta}_{k}"
+
     def run(self, parts):
         chunk_filter = ChunkFilter(parts=parts, total=self.total)
         for i in range(0, self.total):
             if not chunk_filter(i):
                 continue
             date = self.dates[i]
             try:
                 arr = self.ds[i]
                 stats = compute_statistics(arr, self.variables, allow_nan=self.allow_nan)
                 self.tmp_storage.add([date, i, stats], key=date)
             except MissingDateError:
                 self.tmp_storage.add([date, i, "missing"], key=date)
         self.tmp_storage.flush()
         LOG.info(f"Dataset {self.path} additions run.")
-
-    def _write(self, summary):
-        for k in ["mean", "stdev", "minimum", "maximum", "sums", "squares", "count", "has_nans"]:
-            self._add_dataset(name=f"{self.name}_{k}", array=summary[k])
-        self.registry.add_to_history(f"compute_{self.name}_end")
-        LOG.info(f"Wrote {self.name} additions in {self.path}")
```

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/patch.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/patch.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/persistent.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/persistent.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/size.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/size.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import logging
 import os
 
+from anemoi.utils.humanize import bytes
+
 from anemoi.datasets.create.utils import progress_bar
 
 LOG = logging.getLogger(__name__)
 
 
 def compute_directory_sizes(path):
     if not os.path.isdir(path):
```

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/statistics/__init__.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/statistics/summary.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/statistics/summary.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/template.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/template.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/utils.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/utils.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/writer.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/writer.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/create/zarr.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/create/zarr.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/__init__.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/concat.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/concat.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/dataset.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/dataset.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/debug.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/debug.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/ensemble.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/ensemble.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/forewards.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/forewards.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/grids.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/grids.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/indexing.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/indexing.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/join.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/join.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/masked.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/masked.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/misc.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/misc.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/select.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/select.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/statistics.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/statistics.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/stores.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/stores.py`

 * *Files 7% similar despite different names*

```diff
@@ -221,20 +221,20 @@
     def statistics_tendencies(self, delta=None):
         if delta is None:
             delta = self.frequency
         if isinstance(delta, int):
             delta = f"{delta}h"
         from anemoi.datasets.create.loaders import TendenciesStatisticsAddition
 
-        prefix = TendenciesStatisticsAddition.DATASET_NAME_PATTERN.format(delta=delta) + "_"
+        func = TendenciesStatisticsAddition.final_storage_name_from_delta
         return dict(
-            mean=self.z[f"{prefix}mean"][:],
-            stdev=self.z[f"{prefix}stdev"][:],
-            maximum=self.z[f"{prefix}maximum"][:],
-            minimum=self.z[f"{prefix}minimum"][:],
+            mean=self.z[func("mean", delta)][:],
+            stdev=self.z[func("stdev", delta)][:],
+            maximum=self.z[func("maximum", delta)][:],
+            minimum=self.z[func("minimum", delta)][:],
         )
 
     @property
     def resolution(self):
         return self.z.attrs["resolution"]
 
     @property
```

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/subset.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/subset.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/data/unchecked.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/data/unchecked.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/dates/__init__.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/dates/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/dates/groups.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/dates/groups.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi/datasets/grids.py` & `anemoi_datasets-0.2.0/src/anemoi/datasets/grids.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/src/anemoi_datasets.egg-info/PKG-INFO` & `anemoi_datasets-0.2.0/src/anemoi_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-datasets
-Version: 0.1.7
+Version: 0.2.0
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,15 +219,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: anemoi-utils[provenance]>=0.1.7
-Requires-Dist: zarr
+Requires-Dist: zarr<=2.17.0
 Requires-Dist: pyyaml
 Requires-Dist: numpy
 Requires-Dist: tqdm
 Requires-Dist: semantic-version
 Provides-Extra: remote
 Requires-Dist: boto3; extra == "remote"
 Requires-Dist: requests; extra == "remote"
```

### Comparing `anemoi_datasets-0.1.7/src/anemoi_datasets.egg-info/SOURCES.txt` & `anemoi_datasets-0.2.0/src/anemoi_datasets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 docs/building/yaml/building2.txt
 docs/building/yaml/building2.yaml
 docs/building/yaml/building3.txt
 docs/building/yaml/building3.yaml
 docs/building/yaml/concat.yaml
 docs/building/yaml/input.yaml
 docs/building/yaml/missing_dates.yaml
+docs/building/yaml/nan.yaml
 docs/building/yaml/pipe.yaml
 docs/cli/compare.rst
 docs/cli/copy.rst
 docs/cli/create.rst
 docs/cli/inspect.rst
 docs/cli/introduction.rst
 docs/schemas/matrix.excalidraw
```

### Comparing `anemoi_datasets-0.1.7/tests/create/concat.yaml` & `anemoi_datasets-0.2.0/tests/create/concat.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tests/create/join.yaml` & `anemoi_datasets-0.2.0/tests/create/join.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tests/create/perturbations.yaml` & `anemoi_datasets-0.2.0/tests/create/perturbations.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tests/create/pipe.yaml` & `anemoi_datasets-0.2.0/tests/create/pipe.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tests/create/test_create.py` & `anemoi_datasets-0.2.0/tests/create/test_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,19 @@
 @mockup_load_source
 def test_run(name):
     config = os.path.join(HERE, name + ".yaml")
     output = os.path.join(HERE, name + ".zarr")
 
     # cache=None is using the default cache
     c = Creator(output, config=config, cache=None, overwrite=True)
-    c.create()
+    c.init()
+    c.load()
+    c.finalise()
+    c.additions(delta=[1, 3, 6, 12])
+    c.cleanup()
 
     comparer = Comparer(name, output_path=output)
     comparer.compare()
 
 
 if __name__ == "__main__":
     import argparse
```

### Comparing `anemoi_datasets-0.1.7/tests/create-perturbations-full.yaml` & `anemoi_datasets-0.2.0/tests/create-perturbations-full.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tests/create-shift.yaml` & `anemoi_datasets-0.2.0/tests/create-shift.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tests/test_chunks.py` & `anemoi_datasets-0.2.0/tests/test_chunks.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tests/test_data.py` & `anemoi_datasets-0.2.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tests/test_dates.py` & `anemoi_datasets-0.2.0/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tests/test_indexing.py` & `anemoi_datasets-0.2.0/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tools/examples/an-oper-2023-2023-2p5-6h-v1.yaml` & `anemoi_datasets-0.2.0/tools/examples/an-oper-2023-2023-2p5-6h-v1.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tools/grids/grids.ipynb` & `anemoi_datasets-0.2.0/tools/grids/grids.ipynb`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tools/grids/grids1.yaml` & `anemoi_datasets-0.2.0/tools/grids/grids1.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_datasets-0.1.7/tools/grids/grids2.yaml` & `anemoi_datasets-0.2.0/tools/grids/grids2.yaml`

 * *Files identical despite different names*

