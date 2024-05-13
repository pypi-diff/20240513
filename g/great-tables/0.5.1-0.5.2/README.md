# Comparing `tmp/great_tables-0.5.1.tar.gz` & `tmp/great_tables-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_tables-0.5.1.tar", last modified: Fri May  3 19:41:20 2024, max compression
+gzip compressed data, was "great_tables-0.5.2.tar", last modified: Mon May 13 17:52:50 2024, max compression
```

## Comparing `great_tables-0.5.1.tar` & `great_tables-0.5.2.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.708802 great_tables-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.652801 great_tables-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.652801 great_tables-0.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.652801 great_tables-0.5.1/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/scripts/no_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.652801 great_tables-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/workflows/ci-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/workflows/code-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-03 19:41:15.000000 great_tables-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-03 19:41:15.000000 great_tables-0.5.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.656801 great_tables-0.5.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 19:41:15.000000 great_tables-0.5.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-03 19:41:15.000000 great_tables-0.5.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-03 19:41:15.000000 great_tables-0.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-03 19:41:15.000000 great_tables-0.5.1/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     5243 2024-05-03 19:41:15.000000 great_tables-0.5.1/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2259 2024-05-03 19:41:15.000000 great_tables-0.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 19:41:15.000000 great_tables-0.5.1/HISTORY.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1081 2024-05-03 19:41:15.000000 great_tables-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-03 19:41:15.000000 great_tables-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-03 19:41:15.000000 great_tables-0.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-03 19:41:20.708802 great_tables-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-03 19:41:15.000000 great_tables-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.656801 great_tables-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.648801 great_tables-0.5.1/docs/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.648801 great_tables-0.5.1/docs/_extensions/machow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.656801 great_tables-0.5.1/docs/_extensions/machow/interlinks/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.656801 great_tables-0.5.1/docs/articles/
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/articles/intro.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.660801 great_tables-0.5.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/GT_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)  2325288 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/datasets.png
--rw-r--r--   0 runner    (1001) docker     (127)   136430 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/gt_parts_of_a_table.svg
--rw-r--r--   0 runner    (1001) docker     (127)   342328 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/gt_sp500_table.svg
--rw-r--r--   0 runner    (1001) docker     (127)    74998 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/gt_workflow_diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)   209904 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/tables_from_the_web.png
--rw-r--r--   0 runner    (1001) docker     (127)   139817 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/the_components_of_a_table.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.660801 great_tables-0.5.1/docs/blog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.660801 great_tables-0.5.1/docs/blog/bring-your-own-df/
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/bring-your-own-df/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.668801 great_tables-0.5.1/docs/blog/design-philosophy/
--rw-r--r--   0 runner    (1001) docker     (127)   241842 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/a_simple_table.png
--rw-r--r--   0 runner    (1001) docker     (127)   195558 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/cave_grids.png
--rw-r--r--   0 runner    (1001) docker     (127)   656631 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/composition_of_a_table_in_GT.png
--rw-r--r--   0 runner    (1001) docker     (127)   801735 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/computer_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)  1486510 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/nippur_cuneiform_tablet.png
--rw-r--r--   0 runner    (1001) docker     (127)  1629638 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png
--rw-r--r--   0 runner    (1001) docker     (127)   458471 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/uruk_tablet_with_annotations.png
--rw-r--r--   0 runner    (1001) docker     (127)   812542 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/visicalc.png
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.668801 great_tables-0.5.1/docs/blog/introduction-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/introduction-0.2.0/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.668801 great_tables-0.5.1/docs/blog/introduction-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/introduction-0.3.0/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.668801 great_tables-0.5.1/docs/blog/introduction-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/introduction-0.4.0/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/introduction_great_tables.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.672801 great_tables-0.5.1/docs/blog/polars-styling/
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/polars-styling/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)   132380 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/polars-styling/table-preview.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.672801 great_tables-0.5.1/docs/blog/superbowl-squares/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/superbowl-squares/_code.py
--rw-r--r--   0 runner    (1001) docker     (127)  1949299 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/superbowl-squares/games.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/superbowl-squares/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.672801 great_tables-0.5.1/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.672801 great_tables-0.5.1/docs/examples/_data/
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/_data/power_cie_prepared_tbl.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.676801 great_tables-0.5.1/docs/examples/sports-earnings/
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/basketball.png
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/boxing.png
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/golf.png
--rw-r--r--   0 runner    (1001) docker     (127)    76604 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/soccer.png
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/sports_earnings.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/tennis.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.676801 great_tables-0.5.1/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-column-labels.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-formatting.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-header.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-stub.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-styling.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/colorizing-with-data.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/column-selection.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/nanoplots.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/row-selection.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/table-theme-options.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/table-theme-premade.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.684801 great_tables-0.5.1/great_tables/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_boxhead.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.684801 great_tables-0.5.1/great_tables/_data_color/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_data_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_data_color/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_data_color/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_data_color/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_databackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_export.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)   148122 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    40689 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_formats_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)    43858 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_gt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_heading.py
--rw-r--r--   0 runner    (1001) docker     (127)    32690 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_locale.py
--rw-r--r--   0 runner    (1001) docker     (127)    14766 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    74156 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_render.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_row_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_scss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_source_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24908 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_spanners.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_stubhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_tab_create_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_tbl_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    55215 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_utils_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)    27299 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_utils_render_html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.684801 great_tables-0.5.1/great_tables/css/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/css/gt_colors.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/css/gt_styles_default.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.692802 great_tables-0.5.1/great_tables/data/
--rw-r--r--   0 runner    (1001) docker     (127)   412361 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/01-countrypops.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/02-sza.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/03-gtcars.csv
--rw-r--r--   0 runner    (1001) docker     (127)   906055 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/04-sp500.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2848391 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/05-pizzaplace.csv
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/06-exibble.csv
--rw-r--r--   0 runner    (1001) docker     (127)    81025 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/07-towny.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20916 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/08-metro.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21007 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/09-constants.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/10-illness.csv
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/11-islands.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28127 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.700801 great_tables-0.5.1/great_tables/data/metro_images/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_10.svg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_11.svg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_12.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_13.svg
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_14.svg
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_3.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_3bis.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_4.svg
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_7.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_7bis.svg
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_8.svg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_9.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_A.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_B.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_C.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_D.svg
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_E.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T11.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T13.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T3a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T3b.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T4.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T5.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T6.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T7.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T8.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T9.svg
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_H.svg
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_J.svg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_K.svg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_L.svg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_N.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_P.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_R.svg
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_U.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x-airquality.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x_currencies.csv
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x_currency_symbols.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x_default_locales.csv
--rw-r--r--   0 runner    (1001) docker     (127)   255709 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x_locales.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/gt.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/loc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/shiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/utils_render_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/vals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/great_tables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-03 19:41:15.000000 great_tables-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 19:41:15.000000 great_tables-0.5.1/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:41:20.708802 great_tables-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_export.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_formats.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_locations.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_options.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_repr.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_scss.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_tbl_data.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_utils_render_html.ambr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/tests/data_color/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/tests/data_color/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/data_color/__snapshots__/test_data_color.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/data_color/test_data_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/data_color/test_data_color_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test__boxhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test__formats_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test__stubhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    54510 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test__utils_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_boxhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    55203 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_formats_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_gt.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_gt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_heading.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_scss.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_shiny.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_spanners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_tab_create_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_tbl_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_utils_render_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_utils_render_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.086212 great_tables-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/scripts/no_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/workflows/ci-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/workflows/code-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-13 17:52:45.000000 great_tables-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 17:52:45.000000 great_tables-0.5.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 17:52:45.000000 great_tables-0.5.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-13 17:52:45.000000 great_tables-0.5.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 17:52:45.000000 great_tables-0.5.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-13 17:52:45.000000 great_tables-0.5.2/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5243 2024-05-13 17:52:45.000000 great_tables-0.5.2/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2259 2024-05-13 17:52:45.000000 great_tables-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 17:52:45.000000 great_tables-0.5.2/HISTORY.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1081 2024-05-13 17:52:45.000000 great_tables-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 17:52:45.000000 great_tables-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-13 17:52:45.000000 great_tables-0.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-13 17:52:50.086212 great_tables-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-13 17:52:45.000000 great_tables-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.014210 great_tables-0.5.2/docs/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.014210 great_tables-0.5.2/docs/_extensions/machow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/docs/_extensions/machow/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/docs/articles/
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/articles/intro.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.030211 great_tables-0.5.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/GT_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)  2325288 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/datasets.png
+-rw-r--r--   0 runner    (1001) docker     (127)   136430 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/gt_parts_of_a_table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   342328 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/gt_sp500_table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    74998 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/gt_workflow_diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   209904 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/tables_from_the_web.png
+-rw-r--r--   0 runner    (1001) docker     (127)   139817 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/the_components_of_a_table.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.030211 great_tables-0.5.2/docs/blog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.030211 great_tables-0.5.2/docs/blog/bring-your-own-df/
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/bring-your-own-df/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/design-philosophy/
+-rw-r--r--   0 runner    (1001) docker     (127)   241842 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/a_simple_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)   195558 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/cave_grids.png
+-rw-r--r--   0 runner    (1001) docker     (127)   656631 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/composition_of_a_table_in_GT.png
+-rw-r--r--   0 runner    (1001) docker     (127)   801735 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/computer_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)  1486510 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/nippur_cuneiform_tablet.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1629638 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   458471 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/uruk_tablet_with_annotations.png
+-rw-r--r--   0 runner    (1001) docker     (127)   812542 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/visicalc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/introduction-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/introduction-0.2.0/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/introduction-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/introduction-0.3.0/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/introduction-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/introduction-0.4.0/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/introduction_great_tables.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/polars-styling/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/polars-styling/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)   132380 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/polars-styling/table-preview.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.042211 great_tables-0.5.2/docs/blog/superbowl-squares/
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/superbowl-squares/_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1949299 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/superbowl-squares/games.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/superbowl-squares/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.042211 great_tables-0.5.2/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.042211 great_tables-0.5.2/docs/examples/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/_data/power_cie_prepared_tbl.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.046211 great_tables-0.5.2/docs/examples/sports-earnings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/basketball.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/boxing.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/golf.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76604 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/soccer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/sports_earnings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/tennis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.046211 great_tables-0.5.2/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-column-labels.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-formatting.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-header.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-stub.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-styling.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/colorizing-with-data.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/column-selection.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/nanoplots.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/row-selection.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/table-theme-options.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/table-theme-premade.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.054211 great_tables-0.5.2/great_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_boxhead.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.058211 great_tables-0.5.2/great_tables/_data_color/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_data_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_data_color/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_data_color/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_data_color/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_databackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151729 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40689 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_formats_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43858 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_gt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32944 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74939 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_row_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_scss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_source_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25402 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_spanners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_stubhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_tab_create_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16622 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_tbl_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55726 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_utils_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27299 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_utils_render_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.058211 great_tables-0.5.2/great_tables/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/css/gt_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/css/gt_styles_default.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.066212 great_tables-0.5.2/great_tables/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   412361 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/01-countrypops.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/02-sza.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/03-gtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   906055 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/04-sp500.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2848391 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/05-pizzaplace.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/06-exibble.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    81025 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/07-towny.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20916 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/08-metro.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21007 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/09-constants.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/10-illness.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/11-islands.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28127 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.074212 great_tables-0.5.2/great_tables/data/metro_images/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_10.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_11.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_12.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_14.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_3bis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_7bis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_A.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_B.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_C.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_D.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_E.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T11.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T3a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T3b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_H.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_J.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_K.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_L.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_N.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_P.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_R.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_U.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x-airquality.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x_currencies.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x_currency_symbols.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x_default_locales.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   255709 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x_locales.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/loc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/shiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/utils_render_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/vals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.082212 great_tables-0.5.2/great_tables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-13 17:52:49.000000 great_tables-0.5.2/great_tables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-13 17:52:50.000000 great_tables-0.5.2/great_tables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:52:49.000000 great_tables-0.5.2/great_tables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-13 17:52:49.000000 great_tables-0.5.2/great_tables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 17:52:49.000000 great_tables-0.5.2/great_tables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-13 17:52:45.000000 great_tables-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 17:52:45.000000 great_tables-0.5.2/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:52:50.086212 great_tables-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.078212 great_tables-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.082212 great_tables-0.5.2/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_export.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    14024 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_formats.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_locations.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_options.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_repr.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_scss.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_tbl_data.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_utils_render_html.ambr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.082212 great_tables-0.5.2/tests/data_color/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.082212 great_tables-0.5.2/tests/data_color/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/data_color/__snapshots__/test_data_color.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/data_color/test_data_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/data_color/test_data_color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test__boxhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test__formats_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test__stubhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54571 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test__utils_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_boxhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55851 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_formats_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_gt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_scss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_shiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_spanners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_tab_create_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_tbl_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_utils_render_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_utils_render_html.py
```

### Comparing `great_tables-0.5.1/.github/CODE_OF_CONDUCT.md` & `great_tables-0.5.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.github/CONTRIBUTING.md` & `great_tables-0.5.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.github/ISSUE_TEMPLATE/bug.md` & `great_tables-0.5.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.github/ISSUE_TEMPLATE/feature.md` & `great_tables-0.5.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.github/ISSUE_TEMPLATE/question.md` & `great_tables-0.5.2/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.github/PULL_REQUEST_TEMPLATE.md` & `great_tables-0.5.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.github/scripts/no_pandas.py` & `great_tables-0.5.2/.github/scripts/no_pandas.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.github/workflows/ci-docs.yaml` & `great_tables-0.5.2/.github/workflows/ci-docs.yaml`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.github/workflows/ci-tests.yaml` & `great_tables-0.5.2/.github/workflows/ci-tests.yaml`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.github/workflows/code-checks.yaml` & `great_tables-0.5.2/.github/workflows/code-checks.yaml`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.gitignore` & `great_tables-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/.pre-commit-config.yaml` & `great_tables-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/CODE_OF_CONDUCT.md` & `great_tables-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/CONTRIBUTING.md` & `great_tables-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/LICENSE` & `great_tables-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/Makefile` & `great_tables-0.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/PKG-INFO` & `great_tables-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great-tables
-Version: 0.5.1
+Version: 0.5.2
 Summary: Easily generate information-rich, publication-quality tables from Python.
 Author-email: Richard Iannone <rich@posit.co>, Michael Chow <michael.chow@posit.co>
 License: MIT License
         
         Copyright (c) 2022-2024 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,15 +50,14 @@
 License-File: AUTHORS.rst
 Requires-Dist: commonmark>=0.9.1
 Requires-Dist: htmltools>=0.4.1
 Requires-Dist: importlib-metadata
 Requires-Dist: typing_extensions>=3.10.0.0
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: Babel>=2.13.1
-Requires-Dist: webcolors>=1.13
 Requires-Dist: importlib-resources
 Provides-Extra: all
 Requires-Dist: great_tables[extra]; extra == "all"
 Requires-Dist: great_tables[dev]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: selenium>=4.18.1; extra == "extra"
 Requires-Dist: Pillow>=10.2.0; extra == "extra"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: great-tables Version: 0.5.1 Summary: Easily
+Metadata-Version: 2.1 Name: great-tables Version: 0.5.2 Summary: Easily
 generate information-rich, publication-quality tables from Python. Author-
 email: Richard Iannone
 posit.co>, Michael Chow
 posit.co> License: MIT License Copyright (c) 2022-2024 Posit Software, PBC
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -30,26 +30,25 @@
 Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
 :: Markup :: HTML Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE License-File: AUTHORS.rst Requires-Dist: commonmark>=0.9.1 Requires-
 Dist: htmltools>=0.4.1 Requires-Dist: importlib-metadata Requires-Dist:
 typing_extensions>=3.10.0.0 Requires-Dist: numpy>=1.22.4 Requires-Dist:
-Babel>=2.13.1 Requires-Dist: webcolors>=1.13 Requires-Dist: importlib-resources
-Provides-Extra: all Requires-Dist: great_tables[extra]; extra == "all"
-Requires-Dist: great_tables[dev]; extra == "all" Provides-Extra: extra
-Requires-Dist: selenium>=4.18.1; extra == "extra" Requires-Dist:
-Pillow>=10.2.0; extra == "extra" Provides-Extra: dev Requires-Dist:
-great_tables[dev-no-pandas]; extra == "dev" Requires-Dist: pandas; extra ==
-"dev" Provides-Extra: dev-no-pandas Requires-Dist: black; extra == "dev-no-
-pandas" Requires-Dist: jupyter; extra == "dev-no-pandas" Requires-Dist:
-quartodoc>=0.7.1; python_version >= "3.9" and extra == "dev-no-pandas"
-Requires-Dist: griffe==0.38.1; extra == "dev-no-pandas" Requires-Dist: polars;
-extra == "dev-no-pandas" Requires-Dist: pre-commit==2.15.0; extra == "dev-no-
-pandas" Requires-Dist: pyarrow; extra == "dev-no-pandas" Requires-Dist:
+Babel>=2.13.1 Requires-Dist: importlib-resources Provides-Extra: all Requires-
+Dist: great_tables[extra]; extra == "all" Requires-Dist: great_tables[dev];
+extra == "all" Provides-Extra: extra Requires-Dist: selenium>=4.18.1; extra ==
+"extra" Requires-Dist: Pillow>=10.2.0; extra == "extra" Provides-Extra: dev
+Requires-Dist: great_tables[dev-no-pandas]; extra == "dev" Requires-Dist:
+pandas; extra == "dev" Provides-Extra: dev-no-pandas Requires-Dist: black;
+extra == "dev-no-pandas" Requires-Dist: jupyter; extra == "dev-no-pandas"
+Requires-Dist: quartodoc>=0.7.1; python_version >= "3.9" and extra == "dev-no-
+pandas" Requires-Dist: griffe==0.38.1; extra == "dev-no-pandas" Requires-Dist:
+polars; extra == "dev-no-pandas" Requires-Dist: pre-commit==2.15.0; extra ==
+"dev-no-pandas" Requires-Dist: pyarrow; extra == "dev-no-pandas" Requires-Dist:
 pyright>=1.1.244; extra == "dev-no-pandas" Requires-Dist: pytest>=3; extra ==
 "dev-no-pandas" Requires-Dist: pytest-cov; extra == "dev-no-pandas" Requires-
 Dist: shiny; extra == "dev-no-pandas" Requires-Dist: syrupy; extra == "dev-no-
 pandas"
  _[_._/_d_o_c_s_/_a_s_s_e_t_s_/_G_T___l_o_g_o_._s_v_g_]_Absolutely Delightful Table-making in Python_ [!
   [Python Versions](https://img.shields.io/pypi/pyversions/great_tables.svg)]
  (https://pypi.python.org/pypi/great_tables) [![PyPI](https://img.shields.io/
```

### Comparing `great_tables-0.5.1/README.md` & `great_tables-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/_extensions/machow/interlinks/interlinks.lua` & `great_tables-0.5.2/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/_quarto.yml` & `great_tables-0.5.2/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/articles/intro.qmd` & `great_tables-0.5.2/docs/articles/intro.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/assets/GT_logo.svg` & `great_tables-0.5.2/docs/assets/GT_logo.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/assets/datasets.png` & `great_tables-0.5.2/docs/assets/datasets.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/assets/gt_parts_of_a_table.svg` & `great_tables-0.5.2/docs/assets/gt_parts_of_a_table.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/assets/gt_sp500_table.svg` & `great_tables-0.5.2/docs/assets/gt_sp500_table.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/assets/gt_workflow_diagram.svg` & `great_tables-0.5.2/docs/assets/gt_workflow_diagram.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/assets/tables_from_the_web.png` & `great_tables-0.5.2/docs/assets/tables_from_the_web.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/assets/the_components_of_a_table.svg` & `great_tables-0.5.2/docs/assets/the_components_of_a_table.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/bring-your-own-df/index.qmd` & `great_tables-0.5.2/docs/blog/bring-your-own-df/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/design-philosophy/a_simple_table.png` & `great_tables-0.5.2/docs/blog/design-philosophy/a_simple_table.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/design-philosophy/cave_grids.png` & `great_tables-0.5.2/docs/blog/design-philosophy/cave_grids.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/design-philosophy/composition_of_a_table_in_GT.png` & `great_tables-0.5.2/docs/blog/design-philosophy/composition_of_a_table_in_GT.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/design-philosophy/computer_tables.png` & `great_tables-0.5.2/docs/blog/design-philosophy/computer_tables.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/design-philosophy/index.qmd` & `great_tables-0.5.2/docs/blog/design-philosophy/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/design-philosophy/nippur_cuneiform_tablet.png` & `great_tables-0.5.2/docs/blog/design-philosophy/nippur_cuneiform_tablet.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png` & `great_tables-0.5.2/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/design-philosophy/uruk_tablet_with_annotations.png` & `great_tables-0.5.2/docs/blog/design-philosophy/uruk_tablet_with_annotations.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/design-philosophy/visicalc.png` & `great_tables-0.5.2/docs/blog/design-philosophy/visicalc.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/introduction-0.2.0/index.qmd` & `great_tables-0.5.2/docs/blog/introduction-0.2.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/introduction-0.3.0/index.qmd` & `great_tables-0.5.2/docs/blog/introduction-0.3.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/introduction-0.4.0/index.qmd` & `great_tables-0.5.2/docs/blog/introduction-0.4.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/introduction_great_tables.qmd` & `great_tables-0.5.2/docs/blog/introduction_great_tables.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/polars-styling/index.qmd` & `great_tables-0.5.2/docs/blog/polars-styling/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/polars-styling/table-preview.png` & `great_tables-0.5.2/docs/blog/polars-styling/table-preview.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/superbowl-squares/_code.py` & `great_tables-0.5.2/docs/blog/superbowl-squares/_code.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/superbowl-squares/games.csv` & `great_tables-0.5.2/docs/blog/superbowl-squares/games.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/blog/superbowl-squares/index.qmd` & `great_tables-0.5.2/docs/blog/superbowl-squares/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/examples/_data/power_cie_prepared_tbl.csv` & `great_tables-0.5.2/docs/examples/_data/power_cie_prepared_tbl.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/examples/index.qmd` & `great_tables-0.5.2/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/examples/sports-earnings/basketball.png` & `great_tables-0.5.2/docs/examples/sports-earnings/basketball.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/examples/sports-earnings/boxing.png` & `great_tables-0.5.2/docs/examples/sports-earnings/boxing.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/examples/sports-earnings/golf.png` & `great_tables-0.5.2/docs/examples/sports-earnings/golf.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/examples/sports-earnings/index.ipynb` & `great_tables-0.5.2/docs/examples/sports-earnings/index.ipynb`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/examples/sports-earnings/soccer.png` & `great_tables-0.5.2/docs/examples/sports-earnings/soccer.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/examples/sports-earnings/sports_earnings.csv` & `great_tables-0.5.2/docs/examples/sports-earnings/sports_earnings.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/examples/sports-earnings/tennis.png` & `great_tables-0.5.2/docs/examples/sports-earnings/tennis.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/basic-column-labels.qmd` & `great_tables-0.5.2/docs/get-started/basic-column-labels.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/basic-formatting.qmd` & `great_tables-0.5.2/docs/get-started/basic-formatting.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/basic-header.qmd` & `great_tables-0.5.2/docs/get-started/basic-header.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/basic-stub.qmd` & `great_tables-0.5.2/docs/get-started/basic-stub.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/basic-styling.qmd` & `great_tables-0.5.2/docs/get-started/basic-styling.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/colorizing-with-data.qmd` & `great_tables-0.5.2/docs/get-started/colorizing-with-data.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/column-selection.qmd` & `great_tables-0.5.2/docs/get-started/column-selection.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/index.qmd` & `great_tables-0.5.2/docs/get-started/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/nanoplots.qmd` & `great_tables-0.5.2/docs/get-started/nanoplots.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/overview.qmd` & `great_tables-0.5.2/docs/get-started/overview.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/row-selection.qmd` & `great_tables-0.5.2/docs/get-started/row-selection.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/table-theme-options.qmd` & `great_tables-0.5.2/docs/get-started/table-theme-options.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/get-started/table-theme-premade.qmd` & `great_tables-0.5.2/docs/get-started/table-theme-premade.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/docs/styles.css` & `great_tables-0.5.2/docs/styles.css`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/__init__.py` & `great_tables-0.5.2/great_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_boxhead.py` & `great_tables-0.5.2/great_tables/_boxhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_data_color/base.py` & `great_tables-0.5.2/great_tables/_data_color/base.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_data_color/constants.py` & `great_tables-0.5.2/great_tables/_data_color/constants.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_data_color/palettes.py` & `great_tables-0.5.2/great_tables/_data_color/palettes.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_databackend.py` & `great_tables-0.5.2/great_tables/_databackend.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_export.py` & `great_tables-0.5.2/great_tables/_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,26 @@
     gt
         A GT object.
 
     Returns
     -------
     str
         An HTML fragment containing a table.
+
+    Examples:
+    ------
+    Let's use the `row` column of `exibble` dataset to create a table. With the `as_raw_html()`
+    method, we're able to output the HTML content.
+
+    ```{python}
+    from great_tables import GT, exibble
+
+    GT(exibble[["row"]]).as_raw_html()
+    ```
+
     """
     built_table = self._build_data(context="html")
 
     html_table = built_table._render_as_html(
         make_page=make_page,
         all_important=all_important,
     )
```

### Comparing `great_tables-0.5.1/great_tables/_formats.py` & `great_tables-0.5.2/great_tables/_formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,24 @@
 from babel.dates import format_date, format_datetime, format_time
 from typing_extensions import TypeAlias
 
 from ._gt_data import FormatFn, FormatFns, FormatInfo, GTData
 from ._helpers import px
 from ._locale import _get_currencies_data, _get_default_locales_data, _get_locales_data
 from ._locations import resolve_cols_c, resolve_rows_i
-from ._tbl_data import PlExpr, SelectExpr, _get_column_dtype, is_na, to_list
+from ._tbl_data import (
+    Agnostic,
+    DataFrameLike,
+    PlExpr,
+    SelectExpr,
+    is_na,
+    is_series,
+    to_list,
+    _get_column_dtype,
+)
 from ._text import _md_html
 from ._utils import _str_detect, _str_replace
 from ._utils_nanoplots import _generate_nanoplot
 
 
 if TYPE_CHECKING:
     from ._types import GTSelf
@@ -94,14 +103,28 @@
         Whether the formatter is a substitution. Substitutions are run last, after other formatters.
 
     Returns
     -------
     GT
         The GT object is returned. This is the same object that the method is called on so that we
         can facilitate method chaining.
+
+    Examples
+    --------
+    Let's use the `exibble` dataset to create a table. With the `fmt()` method, we'll add a prefix
+    `^` and a suffix `$` to the `row` and `group` columns.
+
+    ```{python}
+    from great_tables import GT, exibble
+
+    (
+        GT(exibble)
+        .fmt(lambda x: f"^{x}$", columns=["row", "group"])
+    )
+    ```
     """
 
     # If a single function is supplied to `fns` then
     # repackage that into a list as the `default` function
     if isinstance(fns, Callable):
         fns = FormatFns(default=fns)
 
@@ -868,14 +891,32 @@
     any values be provided in `sep_mark` or `dec_mark`, they will be overridden by the locale's
     preferred values.
 
     Note that a `locale` value provided here will override any global locale setting performed in
     [`GT()`](`great_tables.GT`)'s own `locale` argument (it is settable there as a value received by
     all other methods that have a `locale` argument).
 
+    Examples
+    --------
+    Let’s use the `towny` dataset as the input table. With the `fmt_percent()` method, we'll format
+    the `pop_change_2016_2021_pct` column to to display values as percentages (to two decimal
+    places).
+
+    ```{python}
+    from great_tables import GT
+    from great_tables.data import towny
+
+    towny_mini = (
+        towny[["name", "pop_change_2016_2021_pct"]]
+        .head(10)
+    )
+
+    (GT(towny_mini).fmt_percent("pop_change_2016_2021_pct", decimals=2))
+    ```
+
     See Also
     --------
     The functional version of this method,
     [`val_fmt_percent()`](`great_tables._formats_vals.val_fmt_percent`), allows you to format a
     single numerical value (or a list of them).
     """
 
@@ -2016,14 +2057,45 @@
 
     Returns
     -------
     GT
         The GT object is returned. This is the same object that the method is called on so that we
         can facilitate method chaining.
 
+    Examples:
+    -------
+    Let’s first create a DataFrame containing some text that is Markdown-formatted and then introduce
+    that to [`GT()`](`great_tables.GT`). We’ll then transform the `md` column with the
+    `fmt_markdown()` method.
+
+    ```{python}
+    import pandas as pd
+    from great_tables import GT
+    from great_tables.data import towny
+
+    text_1 = \"""
+    ### This is Markdown.
+
+    Markdown’s syntax is comprised entirely of
+    punctuation characters, which punctuation
+    characters have been carefully chosen so as
+    to look like what they mean... assuming
+    you’ve ever used email.
+    \"""
+
+    text_2 = \"""
+    Info on Markdown syntax can be found
+    [here](https://daringfireball.net/projects/markdown/).
+    \"""
+
+    df = pd.DataFrame({"md": [text_1, text_2]})
+
+    (GT(df).fmt_markdown("md"))
+    ```
+
     See Also
     --------
     The functional version of this method,
     [`val_fmt_markdown()`](`great_tables._formats_vals.val_fmt_markdown`), allows you to format a
     single string value (or a list of them).
     """
 
@@ -2170,15 +2242,15 @@
     formatted_value = ("-" if is_negative else "") + _insert_decimal_mark(
         digits=sig_digits, power=power, dec_mark="."
     )
 
     # Get integer and decimal parts
     # Split number at `.` and obtain the integer and decimal parts
     number_parts = formatted_value.split(".")
-    integer_part = number_parts[0]
+    integer_part = number_parts[0].lstrip("-")
     decimal_part = number_parts[1] if len(number_parts) > 1 else ""
 
     # Initialize formatted representations of integer and decimal parts
     formatted_integer = ""
     formatted_decimal = dec_mark + decimal_part if decimal_part else ""
 
     if preserve_integer and "." not in formatted_value:
@@ -2191,14 +2263,18 @@
             if count and count % 3 == 0:
                 formatted_integer = sep_mark + formatted_integer
             formatted_integer = digit + formatted_integer
             count += 1
     else:
         formatted_integer = integer_part
 
+    # Add back the negative sign if the number is negative
+    if is_negative:
+        formatted_integer = "-" + formatted_integer
+
     # Combine the integer and decimal parts
     result = formatted_integer + formatted_decimal
 
     return result
 
 
 def _format_number_fixed_decimals(
@@ -3240,41 +3316,44 @@
             "fmt_image currently does not support polars expressions for arguments other than"
             " columns and rows"
         )
 
     if height is None and width is None:
         height = "2em"
 
-    formatter = FmtImage(height, width, sep, str(path), file_pattern, encode)
+    formatter = FmtImage(self._tbl_data, height, width, sep, str(path), file_pattern, encode)
     return fmt(self, fns=formatter.to_html, columns=columns, rows=rows)
 
 
 from dataclasses import dataclass
 
 
 @dataclass
 class FmtImage:
+    dispatch_on: DataFrameLike | Agnostic = Agnostic()
     height: str | int | None = None
     width: str | None = None
     sep: str = " "
     path: str | None = None
     file_pattern: str = "{}"
     encode: bool = True
 
     SPAN_TEMPLATE: ClassVar = '<span style="white-space:nowrap;">{}</span>'
 
     def to_html(self, val: Any):
         import re
         from pathlib import Path
 
-        # TODO: handle NA values
         # TODO: are we assuming val is a string? (or coercing?)
 
         # otherwise...
 
+        if is_na(self.dispatch_on, val):
+            return val
+
         if "," in val:
             files = re.split(r",\s*", val)
         else:
             files = [val]
 
         # TODO: if we allowing height and width to be set based on column values, then
         # they could end up as bespoke types like np int64, etc..
@@ -3504,14 +3583,58 @@
             columns="bars",
             plot_type="bar",
             reference_line="max",
             reference_area=["max", "median"])
     )
     ```
 
+    Here's an example to adjust some of the options using
+    [`nanoplot_options()`](`great_tables.nanoplot_options`).
+
+    ```{python}
+    from great_tables import nanoplot_options
+
+    (
+        GT(random_numbers_df, rowname_col="i")
+        .fmt_nanoplot(
+            columns="lines",
+            reference_line="mean",
+            reference_area=["min", "q1"],
+            options=nanoplot_options(
+                data_point_radius=8,
+                data_point_stroke_color="black",
+                data_point_stroke_width=2,
+                data_point_fill_color="white",
+                data_line_type="straight",
+                data_line_stroke_color="brown",
+                data_line_stroke_width=2,
+                data_area_fill_color="orange",
+                vertical_guide_stroke_color="green",
+            ),
+        )
+        .fmt_nanoplot(
+            columns="bars",
+            plot_type="bar",
+            reference_line="max",
+            reference_area=["max", "median"],
+            options=nanoplot_options(
+                data_bar_stroke_color="gray",
+                data_bar_stroke_width=2,
+                data_bar_fill_color="orange",
+                data_bar_negative_stroke_color="blue",
+                data_bar_negative_stroke_width=1,
+                data_bar_negative_fill_color="lightblue",
+                reference_line_color="pink",
+                reference_area_fill_color="bisque",
+                vertical_guide_stroke_color="blue",
+            ),
+        )
+    )
+    ```
+
     Single-value bar plots and line plots can be made with `fmt_nanoplot()`. These run in the
     horizontal direction, which is ideal for tabular presentation. The key thing here is that
     `fmt_nanoplot()` expects a column of numeric values. These plots are meant for comparison
     across rows so the method automatically scales the horizontal bars to facilitate this type of
     display. The following example shows how `fmt_nanoplot()` can be used to create single-value bar
     and line plots.
 
@@ -3688,14 +3811,17 @@
 
     Returns:
         list[Any]: A list of data values.
     """
 
     import re
 
+    if is_series(data_vals):
+        data_vals = to_list(data_vals)
+
     if isinstance(data_vals, list):
 
         # If the list contains string values, determine whether they are date values
         if all(isinstance(val, str) for val in data_vals):
             if not is_x_axis:
                 raise ValueError("Only the x-axis of a nanoplot allows strings.")
             if re.search(r"\d{1,4}-\d{2}-\d{2}", data_vals[0]):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `great_tables-0.5.1/great_tables/_formats_vals.py` & `great_tables-0.5.2/great_tables/_formats_vals.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_gt_data.py` & `great_tables-0.5.2/great_tables/_gt_data.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_heading.py` & `great_tables-0.5.2/great_tables/_heading.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_helpers.py` & `great_tables-0.5.2/great_tables/_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,18 @@
     text
         The text that is understood to contain Markdown formatting.
 
     Returns
     -------
     Text
         An instance of the Text class is returned, where the text `type` is `"from_markdown"`.
+
+    Examples
+    ------
+    See [`GT.tab_header()`](`great_tables.GT.tab_header`).
     """
     return Text(text=text, type="from_markdown")
 
 
 def html(text: str) -> Text:
     """Interpret input text as HTML-formatted text.
 
@@ -113,14 +117,18 @@
     text
         The text that is understood to contain HTML formatting.
 
     Returns
     -------
     Text
         An instance of the Text class is returned, where the text `type` is `"html"`.
+
+    Examples
+    ------
+    See [`GT.tab_header()`](`great_tables.GT.tab_header`).
     """
     return Text(text=text, type="html")
 
 
 def random_id(n: int = 10) -> str:
     """Helper for creating a random `id` for an output table
 
@@ -683,14 +691,18 @@
     y_ref_line_fmt_fn
         Providing a function for `y_ref_line_fmt_fn=` yields customized formatting of the reference
         line (if present).
     currency
         If the values are to be displayed as currency values, supply either: (1) a 3-letter currency
         code (e.g., `"USD"` for U.S. Dollars, `"EUR"` for the Euro currency), or (2) a common
         currency name (e.g., `"dollar"`, `"pound"`, `"yen"`, etc.).
+
+    Examples
+    --------
+    See [`fmt_nanoplot()`](`great_tables.GT.fmt_nanoplot`)
     """
 
     data_point_radius = _normalize_listable_nanoplot_options(
         nano_opt=data_point_radius, option_type=int
     )
     data_point_stroke_color = _normalize_listable_nanoplot_options(
         nano_opt=data_point_stroke_color, option_type=str
```

### Comparing `great_tables-0.5.1/great_tables/_locale.py` & `great_tables-0.5.2/great_tables/_locale.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_locations.py` & `great_tables-0.5.2/great_tables/_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,18 @@
         The rows to target. Can either be a single row name or a series of row names provided in a
         list.
 
     Returns
     -------
     LocBody
         A LocBody object, which is used for a `locations` argument if specifying the table body.
+
+    Examples
+    ------
+    See [`GT.tab_style()`](`great_tables.GT.tab_style`).
     """
     columns: SelectExpr = None
     rows: RowSelectExpr = None
 
 
 @dataclass
 class LocSummary(Loc):
```

### Comparing `great_tables-0.5.1/great_tables/_options.py` & `great_tables-0.5.2/great_tables/_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -997,14 +997,40 @@
         hexadecimal color code or a color name.
 
     Returns
     -------
     GT
         The GT object is returned. This is the same object that the method is called on so that we
         can facilitate method chaining.
+
+    Examples
+    --------
+    Using select columns from the `exibble` dataset, let's create a table with a number of
+    components added. Following that, we'll put an outline around the entire table using the
+    `opt_table_outline()` method.
+
+    ```{python}
+    from great_tables import GT, exibble, md
+
+    (
+      GT(
+        exibble[["num", "char", "currency", "row", "group"]],
+        rowname_col="row",
+        groupname_col="group"
+      )
+      .tab_header(
+        title=md("Data listing from **exibble**"),
+        subtitle=md("`exibble` is a **Great Tables** dataset.")
+      )
+      .fmt_number(columns="num")
+      .fmt_currency(columns="currency")
+      .tab_source_note(source_note="This is only a subset of the dataset.")
+      .opt_table_outline()
+    )
+    ```
     """
 
     # Validate the `style` argument
     style = _utils._match_arg(x=style, lst=["solid", "dashed", "dotted", "none"])
 
     # Create a dictionary of parameters to pass to the `tab_options()` method
     params = {
```

### Comparing `great_tables-0.5.1/great_tables/_render.py` & `great_tables-0.5.2/great_tables/_render.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_scss.py` & `great_tables-0.5.2/great_tables/_scss.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_source_notes.py` & `great_tables-0.5.2/great_tables/_source_notes.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_spanners.py` & `great_tables-0.5.2/great_tables/_spanners.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,14 +396,15 @@
 
     We can also move multiple columns at a time. With the same `countrypops`-based table
     (`countrypops_mini`), let's move both the `year` and `country_name` columns to the end of the
     column series.
 
     ```{python}
     GT(countrypops_mini).cols_move_to_end(columns=["year", "country_name"])
+    ```
     """
 
     # If `columns` is a string, convert it to a list
     if isinstance(columns, str):
         columns = [columns]
 
     sel_cols = resolve_cols_c(data=data, expr=columns)
@@ -441,14 +442,31 @@
 
     Returns
     -------
     GT
         The GT object is returned. This is the same object that the method is called on so that we
         can facilitate method chaining.
 
+
+    Examples
+    --------
+    For this example, we'll use a portion of the `countrypops` dataset to create a simple table.
+    Let's hide the `year` column with the `cols_hide()` method.
+
+    ```{python}
+    from great_tables import GT
+    from great_tables.data import countrypops
+
+    countrypops_mini = countrypops.loc[countrypops["country_name"] == "Benin"][
+        ["country_name", "year", "population"]
+    ].tail(5)
+
+    GT(countrypops_mini).cols_hide(columns="year")
+    ```
+
     Details
     -------
     The hiding of columns is internally a rendering directive, so, all columns that are 'hidden' are
     still accessible and useful in any expression provided to a `rows` argument. Furthermore, the
     `cols_hide()` method (as with many of the methods available in **Great Tables**) can be placed
     anywhere in a chain of calls (acting as a promise to hide columns when the timing is right).
     However there's perhaps greater readability when placing this call closer to the end of such a
```

### Comparing `great_tables-0.5.1/great_tables/_stub.py` & `great_tables-0.5.2/great_tables/_stub.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_stubhead.py` & `great_tables-0.5.2/great_tables/_stubhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_styles.py` & `great_tables-0.5.2/great_tables/_styles.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,18 @@
         `"pre-wrap"`, `"pre-line"`, and `"break-spaces"`.
 
     Returns
     -------
     CellStyleText
         A CellStyleText object, which is used for a `styles` argument if specifying any cell text
         properties.
+
+    Examples
+    ------
+    See [`GT.tab_style()`](`great_tables.GT.tab_style`).
     """
 
     color: str | ColumnExpr | None = None
     font: str | ColumnExpr | None = None
     size: str | ColumnExpr | None = None
     align: Literal["center", "left", "right", "justify"] | ColumnExpr | None = None
     v_align: Literal["middle", "top", "bottom"] | ColumnExpr | None = None
@@ -259,14 +263,18 @@
         as a hex code, a named color, or an RGB value.
 
     Returns
     -------
     CellStyleFill
         A CellStyleFill object, which is used for a `styles` argument if specifying a cell fill
         value.
+
+    Examples
+    ------
+    See [`GT.tab_style()`](`great_tables.GT.tab_style`).
     """
 
     color: str | ColumnExpr
     # alpha: float | None = None
 
     def _to_html_style(self) -> str:
         return f"background-color: {self.color};"
@@ -296,14 +304,18 @@
         The default value for `weight` is `"1px"` and higher values will become more visually
         prominent.
 
     Returns
     -------
     CellStyleBorders
         A CellStyleBorders object, which is used for a `styles` argument if specifying cell borders.
+
+    Examples
+    ------
+    See [`GT.tab_style()`](`great_tables.GT.tab_style`).
     """
 
     sides: (
         Literal["all", "top", "bottom", "left", "right"]
         | list[Literal["all", "top", "bottom", "left", "right"]]
         | ColumnExpr
     ) = "all"
@@ -318,15 +330,20 @@
 
         # If self.sides is a string, convert to a list
         if isinstance(self.sides, str):
             self.sides = [self.sides]
 
         # If 'all' is provided then call the function recursively with all sides
         if "all" in self.sides:
-            return CellStyleBorders(sides=["top", "bottom", "left", "right"])._to_html_style()
+            return CellStyleBorders(
+                sides=["top", "bottom", "left", "right"],
+                color=self.color,
+                style=self.style,
+                weight=self.weight,
+            )._to_html_style()
 
         weight = self.weight
         if isinstance(weight, int):
             weight = px(weight)
 
         color = self.color
         style = self.style
```

### Comparing `great_tables-0.5.1/great_tables/_substitution.py` & `great_tables-0.5.2/great_tables/_substitution.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_tab_create_modify.py` & `great_tables-0.5.2/great_tables/_tab_create_modify.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,20 @@
         The styles to use for the cells at the targeted `locations`. The `style.text()`,
         `style.fill()`, and `style.borders()` classes can be used here to more easily generate valid
         styles.
     locations
         The cell or set of cells to be associated with the style. The `loc.body()` class can be used
         here to easily target body cell locations.
 
+    Returns
+    -------
+    GT
+        The GT object is returned. This is the same object that the method is called on so that we
+        can facilitate method chaining.
+
     Examples
     --------
     Let's use a small subset of the `exibble` dataset to demonstrate how to use `tab_style()` to
     target specific cells and apply styles to them. We'll start by creating the `exibble_sm` table
     (a subset of the `exibble` table) and then use `tab_style()` to apply a light cyan background
     color to the cells in the `num` column for the first two rows of the table. We'll then apply a
     larger font size to the cells in the `fctr` column for the last four rows of the table.
@@ -63,19 +69,22 @@
             style=style.text(size="22px"),
             locations=loc.body(columns=["fctr"], rows=[4, 5, 6, 7]),
         )
     )
     ```
 
     Let's use `exibble` once again to create a simple, two-column output table (keeping only the
-    `num` and `currency` columns). With the `tab_style()` method (called twice), we'll add style to
+    `num` and `currency` columns). With the `tab_style()` method (called thrice), we'll add style to
     the values already formatted by `fmt_number()` and `fmt_currency()`. In the `style` argument of
-    each `tab_style()` call, we can define multiple types of styling with the `style.fill()` and
-    `style.text()` classes (enclosing these in a list). The cells to be targeted for styling require
-    the use of `loc.body()`, which is used here with different columns being targeted.
+    the first two `tab_style()` call, we can define multiple types of styling with the
+    `style.fill()` and `style.text()` classes (enclosing these in a list). The cells to be targeted
+    for styling require the use of `loc.body()`, which is used here with different columns being
+    targeted. For the final `tab_style()` call, we demonstrate the use of `style.borders()` class
+    as the `style` argument, which is employed in conjunction with `loc.body()` to locate the row to
+    be styled.
 
     ```{python}
     from great_tables import GT, style, loc, exibble
 
     (
         GT(exibble[["num", "currency"]])
         .fmt_number(columns="num", decimals=1)
@@ -90,22 +99,20 @@
         .tab_style(
             style=[
                 style.fill(color="#F9E3D6"),
                 style.text(style="italic")
             ],
             locations=loc.body(columns="currency")
         )
+        .tab_style(
+            style=style.borders(sides=["top", "bottom"], weight='2px', color="red"),
+            locations=loc.body(rows=[4])
+        )
     )
     ```
-
-    Returns
-    -------
-    GT
-        The GT object is returned. This is the same object that the method is called on so that we
-        can facilitate method chaining.
     """
 
     if not isinstance(style, list):
         style = [style]
 
     if not isinstance(locations, list):
         locations = [locations]
```

### Comparing `great_tables-0.5.1/great_tables/_tbl_data.py` & `great_tables-0.5.2/great_tables/_tbl_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,16 +401,24 @@
 def _(df: PdDataFrame):
     return df.astype("string")
 
 
 @cast_frame_to_string.register
 def _(df: PlDataFrame):
     import polars as pl
+    import polars.selectors as cs
 
-    return df.cast(pl.Utf8)
+    list_cols = [
+        name for name, dtype in zip(df.columns, df.dtypes) if issubclass(dtype.base_type(), pl.List)
+    ]
+
+    return df.with_columns(
+        cs.by_name(list_cols).map_elements(lambda x: str(x.to_list())),
+        cs.all().exclude(list_cols).cast(pl.Utf8),
+    )
 
 
 # replace_null_frame ----
 
 
 @singledispatch
 def replace_null_frame(df: DataFrameLike, replacement: DataFrameLike) -> DataFrameLike:
@@ -442,14 +450,32 @@
 
 
 @to_list.register
 def _(ser: PlSeries) -> list[Any]:
     return ser.to_list()
 
 
+# is_series ----
+
+
+@singledispatch
+def is_series(ser: Any) -> bool:
+    False
+
+
+@is_series.register
+def _(ser: PdSeries) -> bool:
+    return True
+
+
+@is_series.register
+def _(ser: PlSeries) -> bool:
+    return True
+
+
 # mutate ----
 
 
 @singledispatch
 def eval_transform(df: DataFrameLike, expr: Any) -> list[Any]:
     raise NotImplementedError(f"Unsupported type: {type(df)}")
```

### Comparing `great_tables-0.5.1/great_tables/_text.py` & `great_tables-0.5.2/great_tables/_text.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_utils.py` & `great_tables-0.5.2/great_tables/_utils.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/_utils_nanoplots.py` & `great_tables-0.5.2/great_tables/_utils_nanoplots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1592,22 +1592,32 @@
     return isinstance(n, numbers.Real) and ((n * scaled_by - int(n) * scaled_by) == 0)
 
 
 def _get_n_intlike(nums: list[Any]) -> int:
     return len([n for n in nums if _is_intlike(n)])
 
 
-def _remove_exponent(n: "str | int | float") -> int:
+def _remove_exponent(n: "str | int | float") -> str:
     """
     https://docs.python.org/3/library/decimal.html#decimal-faq
     """
-    from decimal import Decimal
+    from decimal import Decimal, InvalidOperation
 
     if isinstance(n, str):
         # Replacement of minus sign (U+2212) with hyphen (necessary in some locales)
-        n = str(n).replace("−", "-")
-    d = Decimal(n)
-    if d == d.to_integral():
-        x = d.quantize(Decimal(1))
-    else:
-        x = d.normalize()
-    return int(x)
+        n = n.replace("−", "-")
+
+    # TODO: note that in the nanoplot code, this function only runs when
+    # GT believes everything is an integer. However, _format_number_compactly
+    # may have run on each value and formatted them compactly (e.g. 7045 to "704K")
+    # The InvalidOperation catch prevents errors on compact numbers, but is a
+    # hacky patch. We need to consolidate the processing steps run for value
+    # formatting.
+    try:
+        d = Decimal(n)
+        if d == d.to_integral():
+            x = d.quantize(Decimal(1))
+        else:
+            x = d.normalize()
+        return str(int(x))
+    except InvalidOperation:
+        return str(n)
```

### Comparing `great_tables-0.5.1/great_tables/_utils_render_html.py` & `great_tables-0.5.2/great_tables/_utils_render_html.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/css/gt_colors.scss` & `great_tables-0.5.2/great_tables/css/gt_colors.scss`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/css/gt_styles_default.scss` & `great_tables-0.5.2/great_tables/css/gt_styles_default.scss`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/01-countrypops.csv` & `great_tables-0.5.2/great_tables/data/01-countrypops.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/02-sza.csv` & `great_tables-0.5.2/great_tables/data/02-sza.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/03-gtcars.csv` & `great_tables-0.5.2/great_tables/data/03-gtcars.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/04-sp500.csv` & `great_tables-0.5.2/great_tables/data/04-sp500.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/05-pizzaplace.csv` & `great_tables-0.5.2/great_tables/data/05-pizzaplace.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/06-exibble.csv` & `great_tables-0.5.2/great_tables/data/06-exibble.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/07-towny.csv` & `great_tables-0.5.2/great_tables/data/07-towny.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/08-metro.csv` & `great_tables-0.5.2/great_tables/data/08-metro.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/09-constants.csv` & `great_tables-0.5.2/great_tables/data/09-constants.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/10-illness.csv` & `great_tables-0.5.2/great_tables/data/10-illness.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/11-islands.csv` & `great_tables-0.5.2/great_tables/data/11-islands.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/__init__.py` & `great_tables-0.5.2/great_tables/data/__init__.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_10.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_10.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_11.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_11.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_12.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_12.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_13.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_13.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_14.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_14.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_2.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_2.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_3.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_3.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_3bis.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_3bis.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_5.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_5.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_6.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_6.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_7bis.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_7bis.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_8.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_8.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/metro_9.svg` & `great_tables-0.5.2/great_tables/data/metro_images/metro_9.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/rer_A.svg` & `great_tables-0.5.2/great_tables/data/metro_images/rer_A.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/rer_B.svg` & `great_tables-0.5.2/great_tables/data/metro_images/rer_B.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/rer_C.svg` & `great_tables-0.5.2/great_tables/data/metro_images/rer_C.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/rer_D.svg` & `great_tables-0.5.2/great_tables/data/metro_images/rer_D.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/rer_E.svg` & `great_tables-0.5.2/great_tables/data/metro_images/rer_E.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T1.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T1.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T11.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T11.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T13.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T13.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T2.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T2.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T3a.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T3a.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T3b.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T3b.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T4.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T4.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T5.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T5.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T6.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T6.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T7.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T7.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T8.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T8.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/tram_T9.svg` & `great_tables-0.5.2/great_tables/data/metro_images/tram_T9.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/transilien_H.svg` & `great_tables-0.5.2/great_tables/data/metro_images/transilien_H.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/transilien_J.svg` & `great_tables-0.5.2/great_tables/data/metro_images/transilien_J.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/transilien_K.svg` & `great_tables-0.5.2/great_tables/data/metro_images/transilien_K.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/transilien_L.svg` & `great_tables-0.5.2/great_tables/data/metro_images/transilien_L.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/transilien_N.svg` & `great_tables-0.5.2/great_tables/data/metro_images/transilien_N.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/transilien_P.svg` & `great_tables-0.5.2/great_tables/data/metro_images/transilien_P.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/transilien_R.svg` & `great_tables-0.5.2/great_tables/data/metro_images/transilien_R.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/metro_images/transilien_U.svg` & `great_tables-0.5.2/great_tables/data/metro_images/transilien_U.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/x-airquality.csv` & `great_tables-0.5.2/great_tables/data/x-airquality.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/x_currencies.csv` & `great_tables-0.5.2/great_tables/data/x_currencies.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/x_default_locales.csv` & `great_tables-0.5.2/great_tables/data/x_default_locales.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/data/x_locales.csv` & `great_tables-0.5.2/great_tables/data/x_locales.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/gt.py` & `great_tables-0.5.2/great_tables/gt.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/shiny.py` & `great_tables-0.5.2/great_tables/shiny.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables/utils_render_common.py` & `great_tables-0.5.2/great_tables/utils_render_common.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/great_tables.egg-info/PKG-INFO` & `great_tables-0.5.2/great_tables.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great-tables
-Version: 0.5.1
+Version: 0.5.2
 Summary: Easily generate information-rich, publication-quality tables from Python.
 Author-email: Richard Iannone <rich@posit.co>, Michael Chow <michael.chow@posit.co>
 License: MIT License
         
         Copyright (c) 2022-2024 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,15 +50,14 @@
 License-File: AUTHORS.rst
 Requires-Dist: commonmark>=0.9.1
 Requires-Dist: htmltools>=0.4.1
 Requires-Dist: importlib-metadata
 Requires-Dist: typing_extensions>=3.10.0.0
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: Babel>=2.13.1
-Requires-Dist: webcolors>=1.13
 Requires-Dist: importlib-resources
 Provides-Extra: all
 Requires-Dist: great_tables[extra]; extra == "all"
 Requires-Dist: great_tables[dev]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: selenium>=4.18.1; extra == "extra"
 Requires-Dist: Pillow>=10.2.0; extra == "extra"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: great-tables Version: 0.5.1 Summary: Easily
+Metadata-Version: 2.1 Name: great-tables Version: 0.5.2 Summary: Easily
 generate information-rich, publication-quality tables from Python. Author-
 email: Richard Iannone
 posit.co>, Michael Chow
 posit.co> License: MIT License Copyright (c) 2022-2024 Posit Software, PBC
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -30,26 +30,25 @@
 Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
 :: Markup :: HTML Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE License-File: AUTHORS.rst Requires-Dist: commonmark>=0.9.1 Requires-
 Dist: htmltools>=0.4.1 Requires-Dist: importlib-metadata Requires-Dist:
 typing_extensions>=3.10.0.0 Requires-Dist: numpy>=1.22.4 Requires-Dist:
-Babel>=2.13.1 Requires-Dist: webcolors>=1.13 Requires-Dist: importlib-resources
-Provides-Extra: all Requires-Dist: great_tables[extra]; extra == "all"
-Requires-Dist: great_tables[dev]; extra == "all" Provides-Extra: extra
-Requires-Dist: selenium>=4.18.1; extra == "extra" Requires-Dist:
-Pillow>=10.2.0; extra == "extra" Provides-Extra: dev Requires-Dist:
-great_tables[dev-no-pandas]; extra == "dev" Requires-Dist: pandas; extra ==
-"dev" Provides-Extra: dev-no-pandas Requires-Dist: black; extra == "dev-no-
-pandas" Requires-Dist: jupyter; extra == "dev-no-pandas" Requires-Dist:
-quartodoc>=0.7.1; python_version >= "3.9" and extra == "dev-no-pandas"
-Requires-Dist: griffe==0.38.1; extra == "dev-no-pandas" Requires-Dist: polars;
-extra == "dev-no-pandas" Requires-Dist: pre-commit==2.15.0; extra == "dev-no-
-pandas" Requires-Dist: pyarrow; extra == "dev-no-pandas" Requires-Dist:
+Babel>=2.13.1 Requires-Dist: importlib-resources Provides-Extra: all Requires-
+Dist: great_tables[extra]; extra == "all" Requires-Dist: great_tables[dev];
+extra == "all" Provides-Extra: extra Requires-Dist: selenium>=4.18.1; extra ==
+"extra" Requires-Dist: Pillow>=10.2.0; extra == "extra" Provides-Extra: dev
+Requires-Dist: great_tables[dev-no-pandas]; extra == "dev" Requires-Dist:
+pandas; extra == "dev" Provides-Extra: dev-no-pandas Requires-Dist: black;
+extra == "dev-no-pandas" Requires-Dist: jupyter; extra == "dev-no-pandas"
+Requires-Dist: quartodoc>=0.7.1; python_version >= "3.9" and extra == "dev-no-
+pandas" Requires-Dist: griffe==0.38.1; extra == "dev-no-pandas" Requires-Dist:
+polars; extra == "dev-no-pandas" Requires-Dist: pre-commit==2.15.0; extra ==
+"dev-no-pandas" Requires-Dist: pyarrow; extra == "dev-no-pandas" Requires-Dist:
 pyright>=1.1.244; extra == "dev-no-pandas" Requires-Dist: pytest>=3; extra ==
 "dev-no-pandas" Requires-Dist: pytest-cov; extra == "dev-no-pandas" Requires-
 Dist: shiny; extra == "dev-no-pandas" Requires-Dist: syrupy; extra == "dev-no-
 pandas"
  _[_._/_d_o_c_s_/_a_s_s_e_t_s_/_G_T___l_o_g_o_._s_v_g_]_Absolutely Delightful Table-making in Python_ [!
   [Python Versions](https://img.shields.io/pypi/pyversions/great_tables.svg)]
  (https://pypi.python.org/pypi/great_tables) [![PyPI](https://img.shields.io/
```

### Comparing `great_tables-0.5.1/great_tables.egg-info/SOURCES.txt` & `great_tables-0.5.2/great_tables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/pyproject.toml` & `great_tables-0.5.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 dependencies = [
     "commonmark>=0.9.1",
     "htmltools>=0.4.1",
     "importlib-metadata",
     "typing_extensions>=3.10.0.0",
     "numpy>=1.22.4",
     "Babel>=2.13.1",
-    "webcolors>=1.13",
     "importlib-resources"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 all = [
     "great_tables[extra]",
```

### Comparing `great_tables-0.5.1/tests/__snapshots__/test_export.ambr` & `great_tables-0.5.2/tests/__snapshots__/test_export.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/__snapshots__/test_options.ambr` & `great_tables-0.5.2/tests/__snapshots__/test_options.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/__snapshots__/test_repr.ambr` & `great_tables-0.5.2/tests/__snapshots__/test_repr.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/__snapshots__/test_scss.ambr` & `great_tables-0.5.2/tests/__snapshots__/test_scss.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/__snapshots__/test_utils_render_html.ambr` & `great_tables-0.5.2/tests/__snapshots__/test_utils_render_html.ambr`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,23 @@
     <tr>
       <th class="gt_row gt_left gt_stub">3</th>
       <td class="gt_row gt_right">33</td>
     </tr>
   </tbody>
   '''
 # ---
+# name: test_render_polars_list_col
+  '''
+  <tbody class="gt_table_body">
+    <tr>
+      <td class="gt_row gt_center">[1, 2]</td>
+    </tr>
+  </tbody>
+  '''
+# ---
 # name: test_source_notes_snap
   '''
     <tfoot class="gt_sourcenotes">
     
     <tr>
       <td class="gt_sourcenote" colspan="9">An <strong>important</strong> note.</td>
     </tr>
```

### Comparing `great_tables-0.5.1/tests/data_color/__snapshots__/test_data_color.ambr` & `great_tables-0.5.2/tests/data_color/__snapshots__/test_data_color.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/data_color/test_data_color.py` & `great_tables-0.5.2/tests/data_color/test_data_color.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/data_color/test_data_color_utils.py` & `great_tables-0.5.2/tests/data_color/test_data_color_utils.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test__boxhead.py` & `great_tables-0.5.2/tests/test__boxhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test__stubhead.py` & `great_tables-0.5.2/tests/test__stubhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test__utils_nanoplots.py` & `great_tables-0.5.2/tests/test__utils_nanoplots.py`

 * *Files 0% similar despite different names*

```diff
@@ -2048,17 +2048,18 @@
 def test_get_n_intlike(nums: list[Any], n: int):
     assert _get_n_intlike(nums) == n
 
 
 @pytest.mark.parametrize(
     "n, result",
     [
-        ("1.0", 1),
-        (2.0, 2),
-        (3.00, 3),
-        (Decimal(4), 4),
-        ("-5.0", -5),
-        ("−5.0", -5),  # not regular `-`
+        ("1.0", "1"),
+        (2.0, "2"),
+        (3.00, "3"),
+        (Decimal(4), "4"),
+        ("-5.0", "-5"),
+        ("−5.0", "-5"),  # not regular `-`
+        ("-7.04K", "-7.04K"),  # not regular `-`
     ],
 )
 def test_remove_exponent(n: "int | float | str", result: int):
     assert _remove_exponent(n) == result
```

### Comparing `great_tables-0.5.1/tests/test_export.py` & `great_tables-0.5.2/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_formats.py` & `great_tables-0.5.2/tests/test_formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import polars as pl
 import pytest
 from great_tables import GT, _locale
 from great_tables._data_color.base import _html_color
 from great_tables._formats import (
     FmtImage,
     _expand_exponential_to_full_string,
+    _format_number_n_sigfig,
     _format_number_fixed_decimals,
     _get_currency_str,
     _get_locale_currency_code,
     _get_locale_dec_mark,
     _get_locale_sep_mark,
     _normalize_locale,
     _validate_locale,
@@ -999,22 +1000,35 @@
         (5.234523, "5.23"),
         (0, "0.00"),
         (0.1, "0.10"),
         (0.01, "0.01"),
         (0.00023, "0.00"),
         (0.000033, "0.00"),
         (0.00000000446453, "0.00"),
+        (-325, "-325.00"),
     ],
 )
 def test_format_number_fixed_decimals(value: Union[int, float], x_out: str):
     x = _format_number_fixed_decimals(value=value, decimals=2, sep_mark=",")
     assert x == x_out
 
 
 @pytest.mark.parametrize(
+    "value, out",
+    [
+        (325, "325"),
+        (-325, "-325"),
+        (-1320, "-1,320"),
+    ],
+)
+def test_format_number_n_sigfig_3(value, out: str):
+    assert _format_number_n_sigfig(value, 3) == out
+
+
+@pytest.mark.parametrize(
     "str_number,x_out",
     [
         ("1e-5", "0.00001"),
         ("1.5e-5", "0.000015"),
         ("-1e-5", "-0.00001"),
         ("-1.5e-5", "-0.000015"),
         ("1E-5", "0.00001"),
@@ -1393,14 +1407,22 @@
     formatter = FmtImage(sep=" ", file_pattern="{}.svg", encode=False)
     res = formatter.to_html("/a")
     dst = formatter.SPAN_TEMPLATE.format('<img src="/a.svg" style="vertical-align: middle;">')
 
     assert res == dst
 
 
+def test_fmt_image_missing():
+    formatter = FmtImage()
+    assert formatter.to_html(None) is None
+
+    formatter_pd = FmtImage(pd.DataFrame())
+    assert formatter_pd.to_html(pd.NA) is pd.NA
+
+
 def test_fmt_image_multiple():
     formatter = FmtImage(sep="---", file_pattern="{}.svg", encode=False)
     res = formatter.to_html("/a,/b")
     dst = formatter.SPAN_TEMPLATE.format(
         '<img src="/a.svg" style="vertical-align: middle;">'
         "---"
         '<img src="/b.svg" style="vertical-align: middle;">'
@@ -1862,14 +1884,20 @@
             ("stroke-width", "2"),
             ("fill", "#A6E6F2"),
             ("fill-opacity", "0.8"),
         ],
     )
 
 
+def test_fmt_nanoplot_polars_listcol(snapshot):
+    gt = GT(pl.DataFrame({"x": [[1, 2], [3, 4]]})).fmt_nanoplot("x")
+
+    assert_rendered_body(snapshot, gt)
+
+
 def test_normalize_locale():
     assert _normalize_locale("af-ZA") == "af"
 
 
 def test_normalize_locale_noops_none():
     assert _normalize_locale(None) is None
```

### Comparing `great_tables-0.5.1/tests/test_formats_nanoplots.py` & `great_tables-0.5.2/tests/test_formats_nanoplots.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 from typing import Any
 
+import polars as pl
 import pytest
 from great_tables._formats import _generate_data_vals, _process_number_stream
 
 
 @pytest.mark.parametrize(
-    "src", ["1 2 3", "1  2, 3", "a1 b2 c3", [1, 2, 3], {"x": [1, 2, 3]}, {"any_name": [1, 2, 3]}]
+    "src",
+    [
+        "1 2 3",
+        "1  2, 3",
+        "a1 b2 c3",
+        [1, 2, 3],
+        {"x": [1, 2, 3]},
+        {"any_name": [1, 2, 3]},
+        pl.Series([1, 2, 3]),
+    ],
 )
 def test_generate_data_vals(src: Any):
     assert _generate_data_vals(src) == [1, 2, 3]
 
 
 @pytest.mark.xfail
 def test_generate_data_vals_fails_ambig():
```

### Comparing `great_tables-0.5.1/tests/test_gt.py` & `great_tables-0.5.2/tests/test_gt.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_gt_data.py` & `great_tables-0.5.2/tests/test_gt_data.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_helpers.py` & `great_tables-0.5.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_locations.py` & `great_tables-0.5.2/tests/test_locations.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_options.py` & `great_tables-0.5.2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_repr.py` & `great_tables-0.5.2/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_scss.py` & `great_tables-0.5.2/tests/test_scss.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_spanners.py` & `great_tables-0.5.2/tests/test_spanners.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_styles.py` & `great_tables-0.5.2/tests/test_styles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import polars as pl
-from great_tables._styles import CellStyleText, FromColumn
+from great_tables._styles import CellStyleText, CellStyleBorders, FromColumn
 
 
 def test_from_column_replace():
     """FromColumn is replaced by the specified column's value in a row of data"""
 
     df = pd.DataFrame({"x": [1, 2], "color": ["red", "blue"]})
     from_col = FromColumn("color")
@@ -38,7 +38,18 @@
 def test_cell_value_from_polars_expr():
     df = pl.DataFrame({"x": [1, 2], "color": ["red", "blue"]})
 
     style = CellStyleText(color=pl.col("color").str.to_uppercase())
     new_style = style._evaluate_expressions(df)._from_row(df, 0)
 
     assert new_style.color == "RED"
+
+
+def test_cell_style_borders_all():
+    res = CellStyleBorders(sides=["all"], color="blue")._to_html_style()
+    assert res.split(";") == [
+        "border-top: 1px solid blue",
+        "border-bottom: 1px solid blue",
+        "border-left: 1px solid blue",
+        "border-right: 1px solid blue",
+        "",
+    ]
```

### Comparing `great_tables-0.5.1/tests/test_substitutions.py` & `great_tables-0.5.2/tests/test_substitutions.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_tab_create_modify.py` & `great_tables-0.5.2/tests/test_tab_create_modify.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_tbl_data.py` & `great_tables-0.5.2/tests/test_tbl_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import pytest
 from great_tables._tbl_data import (
     DataFrameLike,
     SeriesLike,
     _get_cell,
     _get_column_dtype,
     _set_cell,
+    cast_frame_to_string,
     create_empty_frame,
     eval_select,
     get_column_names,
+    is_series,
     reorder,
     to_frame,
     validate_frame,
 )
 
 params_frames = [pytest.param(pd.DataFrame, id="pandas"), pytest.param(pl.DataFrame, id="polars")]
 params_series = [pytest.param(pd.Series, id="pandas"), pytest.param(pl.Series, id="polars")]
@@ -132,7 +134,24 @@
 
     if isinstance(ser, pl.Series):
         assert_frame_equal(df, pl.DataFrame({"x": [1.0, 2.0, None]}))
     elif isinstance(ser, pd.Series):
         assert_frame_equal(df, pd.DataFrame({"x": [1.0, 2.0, None]}))
     else:
         raise AssertionError(f"Unexpected series type: {type(ser)}")
+
+
+def test_is_series(ser: SeriesLike):
+    assert is_series(ser)
+
+
+def test_is_series_false():
+    assert not is_series(1)
+
+
+def test_cast_frame_to_string_polars_list_col():
+    df = pl.DataFrame({"x": [[1, 2], [3]], "y": [1, None], "z": [{"a": 1}, {"a": 2}]})
+    new_df = cast_frame_to_string(df)
+
+    assert new_df["x"].dtype.is_(pl.String)
+    assert new_df["y"].dtype.is_(pl.String)
+    assert new_df["z"].dtype.is_(pl.String)
```

### Comparing `great_tables-0.5.1/tests/test_utils.py` & `great_tables-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_utils_render_common.py` & `great_tables-0.5.2/tests/test_utils_render_common.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.1/tests/test_utils_render_html.py` & `great_tables-0.5.2/tests/test_utils_render_html.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import polars as pl
 from great_tables import GT, exibble, html, loc, md, style
 from great_tables._utils_render_html import create_body_component_h, create_source_notes_component_h
 
 small_exibble = exibble[["num", "char"]].head(3)
 
 
 def assert_rendered_source_notes(snapshot, gt):
@@ -146,7 +147,13 @@
 def test_styling_data_10(snapshot):
     new_gt = GT(small_exibble).tab_style(
         style=style.borders(sides="all"),
         locations=loc.body(columns="char", rows=[0, 2]),
     )
 
     assert_rendered_body(snapshot, new_gt)
+
+
+def test_render_polars_list_col(snapshot):
+    gt = GT(pl.DataFrame({"x": [[1, 2]]}))
+
+    assert_rendered_body(snapshot, gt)
```

