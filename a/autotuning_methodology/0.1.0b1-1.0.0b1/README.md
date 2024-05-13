# Comparing `tmp/autotuning_methodology-0.1.0b1.tar.gz` & `tmp/autotuning_methodology-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotuning_methodology-0.1.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "autotuning_methodology-1.0.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `autotuning_methodology-0.1.0b1.tar` & `autotuning_methodology-1.0.0b1.tar`

### file list

```diff
@@ -1,72 +1,83 @@
--rw-r--r--   0        0        0      112 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/.coveragerc
--rw-r--r--   0        0        0     1410 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/.github/workflows/build-test-python-package.yml
--rw-r--r--   0        0        0      573 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/.github/workflows/publish-documentation.yml
--rw-r--r--   0        0        0     1227 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/.github/workflows/publish-package.yml
--rwxr-xr-x   0        0        0     3468 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/.gitignore
--rw-r--r--   0        0        0      171 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/.vscode/extensions.json
--rw-r--r--   0        0        0      638 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/.vscode/settings.json
--rw-r--r--   0        0        0     1077 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/LICENSE
--rw-r--r--   0        0        0     6164 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/README.md
--rw-r--r--   0        0        0     2597 2023-06-02 07:16:59.918264 autotuning_methodology-0.1.0b1/UML/.$Sequence Diagram.drawio.bkp
--rw-r--r--   0        0        0   302745 2023-06-02 07:16:59.922265 autotuning_methodology-0.1.0b1/UML/.$flowchart.drawio.bkp
--rw-r--r--   0        0        0     2585 2023-06-02 07:16:59.922265 autotuning_methodology-0.1.0b1/UML/Sequence Diagram.drawio
--rw-r--r--   0        0        0    26889 2023-06-02 07:16:59.922265 autotuning_methodology-0.1.0b1/UML/classes.pdf
--rw-r--r--   0        0        0   303637 2023-06-02 07:16:59.922265 autotuning_methodology-0.1.0b1/UML/flowchart/.$flowchart.drawio.bkp
--rw-r--r--   0        0        0   303637 2023-06-02 07:16:59.926265 autotuning_methodology-0.1.0b1/UML/flowchart/flowchart.drawio
--rw-r--r--   0        0        0   315705 2023-06-02 07:16:59.930265 autotuning_methodology-0.1.0b1/UML/flowchart/flowchart_output_generation.png
--rw-r--r--   0        0        0   267296 2023-06-02 07:16:59.930265 autotuning_methodology-0.1.0b1/UML/flowchart/flowchart_performance_curve_generation.png
--rw-r--r--   0        0        0   131133 2023-06-02 07:16:59.930265 autotuning_methodology-0.1.0b1/UML/flowchart/mini_plots/flowchart_plot_aggregated.png
--rw-r--r--   0        0        0    95756 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/UML/flowchart/mini_plots/flowchart_plot_individual.png
--rw-r--r--   0        0        0     1074 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/UML/flowchart/mini_plots/flowchart_plots.py
--rw-r--r--   0        0        0    15114 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/UML/packages.pdf
--rw-r--r--   0        0        0      634 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/Makefile
--rw-r--r--   0        0        0     1892 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/autotuning_methodology.rst
--rw-r--r--   0        0        0     2440 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/conf.py
--rw-r--r--   0        0        0      408 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/make.bat
--rw-r--r--   0        0        0      103 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/modules.rst
--rw-r--r--   0        0        0     5034 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/source/logo_autotuning_methodology.svg
--rw-r--r--   0        0        0    36351 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/source/logo_kernel_dashboard.svg
--rw-r--r--   0        0        0    42513 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/source/logo_kernel_launcher.svg
--rw-r--r--   0        0        0    39816 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/docs/source/logo_kernel_tuner.svg
--rwxr-xr-x   0        0        0      983 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/experiment_files/bootstrap_hyperparams.json
--rw-r--r--   0        0        0     1633 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/experiment_files/methodology_paper_example.json
--rw-r--r--   0        0        0     1403 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/experiment_files/presentation_comparison.json
--rw-r--r--   0        0        0     1515 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/experiment_files/test_random_calculated.json
--rw-r--r--   0        0        0     1409 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/experiment_files/test_scatter.json
--rwxr-xr-x   0        0        0     2275 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/experiment_files/test_searchspace_algorithms.json
--rw-r--r--   0        0        0      132 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/.vscode/settings.json
--rwxr-xr-x   0        0        0    18897 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/bootstrap_hyperparams_visualizer.py
--rwxr-xr-x   0        0        0    19811 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/experiments_strategies.py
--rwxr-xr-x   0        0        0   119690 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/experiments_strategies_hyperparamtuning.py
--rwxr-xr-x   0        0        0     7475 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/generate_cachefile.py
--rw-r--r--   0        0        0    20608 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/max_draw_k_from_n.py
--rw-r--r--   0        0        0     3259 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/speedtest_index_performance.py
--rw-r--r--   0        0        0     1174 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/speedtest_python_reversed_nan_sort.py
--rwxr-xr-x   0        0        0     2545 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/try_BOtorch.py
--rwxr-xr-x   0        0        0     8426 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/try_GPytorch.py
--rw-r--r--   0        0        0    20822 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/extra/try_isotonic_regression.py
--rwxr-xr-x   0        0        0      435 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/mypy.ini
--rw-r--r--   0        0        0      967 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/noxfile.py
--rwxr-xr-x   0        0        0       17 2023-06-02 07:16:59.934265 autotuning_methodology-0.1.0b1/profilings/.gitignore
--rw-r--r--   0        0        0     2727 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/src/autotuning_methodology/__init__.py
--rw-r--r--   0        0        0    16103 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/src/autotuning_methodology/baseline.py
--rwxr-xr-x   0        0        0     8418 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/src/autotuning_methodology/caching.py
--rw-r--r--   0        0        0    50283 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/src/autotuning_methodology/curves.py
--rwxr-xr-x   0        0        0     9689 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/src/autotuning_methodology/experiments.py
--rwxr-xr-x   0        0        0    16513 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/src/autotuning_methodology/runner.py
--rwxr-xr-x   0        0        0     4138 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/src/autotuning_methodology/schema.json
--rw-r--r--   0        0        0    21440 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/src/autotuning_methodology/searchspace_statistics.py
--rwxr-xr-x   0        0        0    47912 2023-06-02 07:16:59.938264 autotuning_methodology-0.1.0b1/src/autotuning_methodology/visualize_experiments.py
--rw-r--r--   0        0        0  3483805 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json
--rw-r--r--   0        0        0     3017 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py
--rw-r--r--   0        0        0     1285 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/mockfiles/test.json
--rw-r--r--   0        0        0     1284 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json
--rw-r--r--   0        0        0     1273 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/mockfiles/test_cached.json
--rw-r--r--   0        0        0     6934 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/test_run_experiment.py
--rw-r--r--   0        0        0     2888 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/test_visualization.py
--rw-r--r--   0        0        0     1978 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/release/test_toml_file.py
--rw-r--r--   0        0        0       34 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/unit/test_caching.py
--rw-r--r--   0        0        0     3464 2023-06-02 07:16:59.954264 autotuning_methodology-0.1.0b1/tests/autotuning_methodology/unit/test_curves.py
--rw-r--r--   0        0        0     7995 1970-01-01 00:00:00.000000 autotuning_methodology-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0      112 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.coveragerc
+-rw-r--r--   0        0        0     1424 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.github/workflows/build-test-python-package.yml
+-rw-r--r--   0        0        0      573 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.github/workflows/publish-documentation.yml
+-rw-r--r--   0        0        0     1227 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.github/workflows/publish-package.yml
+-rwxr-xr-x   0        0        0     3571 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.gitignore
+-rw-r--r--   0        0        0      144 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.vscode/extensions.json
+-rw-r--r--   0        0        0      605 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.vscode/settings.json
+-rw-r--r--   0        0        0     1077 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     7328 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/README.md
+-rw-r--r--   0        0        0     2597 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/UML/.$Sequence Diagram.drawio.bkp
+-rw-r--r--   0        0        0   302745 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/.$flowchart.drawio.bkp
+-rw-r--r--   0        0        0     2585 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/Sequence Diagram.drawio
+-rw-r--r--   0        0        0    26889 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/classes.pdf
+-rw-r--r--   0        0        0   303637 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/flowchart/.$flowchart.drawio.bkp
+-rw-r--r--   0        0        0   303637 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/flowchart/flowchart.drawio
+-rw-r--r--   0        0        0   315705 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/flowchart_output_generation.png
+-rw-r--r--   0        0        0   267296 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/flowchart_performance_curve_generation.png
+-rw-r--r--   0        0        0   131133 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plot_aggregated.png
+-rw-r--r--   0        0        0    95756 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plot_individual.png
+-rw-r--r--   0        0        0     1074 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plots.py
+-rw-r--r--   0        0        0    15114 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/UML/packages.pdf
+-rw-r--r--   0        0        0     5736 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py
+-rw-r--r--   0        0        0      634 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/Makefile
+-rw-r--r--   0        0        0     1722 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/autotuning_methodology.rst
+-rw-r--r--   0        0        0     2487 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/conf.py
+-rw-r--r--   0        0        0     1669 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/getting_started.rst
+-rw-r--r--   0        0        0      827 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/make.bat
+-rw-r--r--   0        0        0      128 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/modules.rst
+-rw-r--r--   0        0        0   315705 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/flowchart_output_generation.png
+-rw-r--r--   0        0        0   267296 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/flowchart_performance_curve_generation.png
+-rw-r--r--   0        0        0     5034 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/logo_autotuning_methodology.svg
+-rw-r--r--   0        0        0    36351 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/logo_kernel_dashboard.svg
+-rw-r--r--   0        0        0    42513 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/logo_kernel_launcher.svg
+-rw-r--r--   0        0        0    39816 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/docs/source/logo_kernel_tuner.svg
+-rwxr-xr-x   0        0        0      983 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/bootstrap_hyperparams.json
+-rw-r--r--   0        0        0     1625 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/example_visualizations.json
+-rw-r--r--   0        0        0     1971 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/methodology_paper_evaluation.json
+-rw-r--r--   0        0        0     1647 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/milo_hotspot.json
+-rw-r--r--   0        0        0     1403 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/presentation_comparison.json
+-rw-r--r--   0        0        0     2364 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/simple_example.json
+-rw-r--r--   0        0        0     1745 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/test_random_calculated.json
+-rw-r--r--   0        0        0     1409 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/test_scatter.json
+-rwxr-xr-x   0        0        0     2275 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/test_searchspace_algorithms.json
+-rw-r--r--   0        0        0      132 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/.vscode/settings.json
+-rwxr-xr-x   0        0        0    18897 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/bootstrap_hyperparams_visualizer.py
+-rwxr-xr-x   0        0        0    19811 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/experiments_strategies.py
+-rwxr-xr-x   0        0        0   119690 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/experiments_strategies_hyperparamtuning.py
+-rwxr-xr-x   0        0        0     7475 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/generate_cachefile.py
+-rw-r--r--   0        0        0    20608 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/max_draw_k_from_n.py
+-rw-r--r--   0        0        0     3259 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/speedtest_index_performance.py
+-rw-r--r--   0        0        0     1174 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/speedtest_python_reversed_nan_sort.py
+-rwxr-xr-x   0        0        0     2545 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/try_BOtorch.py
+-rwxr-xr-x   0        0        0     8426 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/try_GPytorch.py
+-rw-r--r--   0        0        0    20822 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/try_isotonic_regression.py
+-rwxr-xr-x   0        0        0      435 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/mypy.ini
+-rw-r--r--   0        0        0     1089 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/noxfile.py
+-rwxr-xr-x   0        0        0       17 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/profilings/.gitignore
+-rw-r--r--   0        0        0     2816 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/__init__.py
+-rw-r--r--   0        0        0    17647 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/baseline.py
+-rwxr-xr-x   0        0        0     8418 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/caching.py
+-rw-r--r--   0        0        0    51986 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/curves.py
+-rwxr-xr-x   0        0        0     9764 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/experiments.py
+-rwxr-xr-x   0        0        0    24377 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/runner.py
+-rwxr-xr-x   0        0        0     4138 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/schema.json
+-rw-r--r--   0        0        0    25701 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/searchspace_statistics.py
+-rw-r--r--   0        0        0     1787 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/validators.py
+-rwxr-xr-x   0        0        0    48490 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/visualize_experiments.py
+-rw-r--r--   0        0        0  3269061 2024-05-13 15:37:26.579071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json
+-rw-r--r--   0        0        0  3255846 2024-05-13 15:37:26.587071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json
+-rw-r--r--   0        0        0  3483805 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json
+-rw-r--r--   0        0        0     2967 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py
+-rw-r--r--   0        0        0     1489 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test.json
+-rw-r--r--   0        0        0     1476 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json
+-rw-r--r--   0        0        0     1465 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_cached.json
+-rw-r--r--   0        0        0     1453 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json
+-rw-r--r--   0        0        0     8913 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/test_run_experiment.py
+-rw-r--r--   0        0        0     2934 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/test_visualization.py
+-rw-r--r--   0        0        0     1978 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/release/test_toml_file.py
+-rw-r--r--   0        0        0       34 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/unit/test_caching.py
+-rw-r--r--   0        0        0     3464 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/unit/test_curves.py
+-rw-r--r--   0        0        0     9296 1970-01-01 00:00:00.000000 autotuning_methodology-1.0.0b1/PKG-INFO
```

### Comparing `autotuning_methodology-0.1.0b1/.github/workflows/build-test-python-package.yml` & `autotuning_methodology-1.0.0b1/.github/workflows/build-test-python-package.yml`

 * *Files 7% similar despite different names*

```diff
@@ -16,26 +16,26 @@
     build:
         runs-on: ubuntu-latest
         strategy:
             matrix:
                 python-version: ["3.9", "3.10", "3.11"]
 
         steps:
-            - uses: actions/checkout@v3
+            - uses: actions/checkout@v4
             - name: Set up Python ${{ matrix.python-version }}
-              uses: actions/setup-python@v4
+              uses: actions/setup-python@v5
               with:
                   python-version: ${{ matrix.python-version }}
             - name: Install dependencies
               run: |
                   python -m pip install --upgrade pip
                   pip install ruff pytest
                   pip install .[test]
             - name: Lint with ruff
               run: |
                   # stop the build if there are Python syntax errors or undefined names
-                  ruff --format=github --select=E9,F63,F7,F82 --config=pyproject.toml .
+                  ruff --output-format=github --select=E9,F63,F7,F82 --config=pyproject.toml .
                   # default set of ruff rules with GitHub Annotations
-                  ruff --format=github --config=pyproject.toml .
+                  ruff --output-format=github --config=pyproject.toml .
             - name: Test with pytest
               run: |
                   pytest
```

### Comparing `autotuning_methodology-0.1.0b1/.github/workflows/publish-documentation.yml` & `autotuning_methodology-1.0.0b1/.github/workflows/publish-documentation.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/.github/workflows/publish-package.yml` & `autotuning_methodology-1.0.0b1/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/.gitignore` & `autotuning_methodology-1.0.0b1/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 generated_plots/*
 
 # ignore files in cachefile folder
 cached_data_used/cachefiles/*
 cached_data_used/kernels/*
 cached_data_used/visualizations/*
 cached_data_used/last_run/*
+cached_data_used/import_runs/*
+
+# exceptions
+!cached_data_used/cachefiles/ktt_values_to_kerneltuner.py
 
 # ignore specific experiment files
 experiment_files/milo.json
 
 # ignore mypy
 mypy.ini
```

### Comparing `autotuning_methodology-0.1.0b1/.vscode/settings.json` & `autotuning_methodology-1.0.0b1/.vscode/settings.json`

 * *Files 22% similar despite different names*

```diff
@@ -6,20 +6,19 @@
     "editor.defaultFormatter": "vscode.json-language-features"
   },
   "[python]": {
     "editor.defaultFormatter": "ms-python.black-formatter",
     "editor.formatOnType": true,
     "editor.formatOnSave": true,
     "editor.codeActionsOnSave": {
-      "source.fixAll": true,
-      "source.organizeImports": true,
+        "source.fixAll": "explicit",
+        "source.organizeImports": "explicit"
     }
   },
-  "python.formatting.provider": "black",
-  "python.formatting.blackArgs": [
+  "black-formatter.args": [
     "--config=pyproject.toml"
   ],
   "ruff.args": [
     "--config=pyproject.toml"
   ],
   "autoDocstring.docstringFormat": "google-notypes",
 }
```

### Comparing `autotuning_methodology-0.1.0b1/LICENSE` & `autotuning_methodology-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/README.md` & `autotuning_methodology-1.0.0b1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,81 @@
 # Autotuning Methodology Software Package
 
 <p align="center">
-  <img width="25%" src="https://fjwillemsen.github.io/autotuning_methodology/_static/logo_autotuning_methodology.svg" />
+  <img width="25%" src="https://autotuningassociation.github.io/autotuning_methodology/_static/logo_autotuning_methodology.svg" />
 </p>
 
-[![Build Status](https://github.com/fjwillemsen/autotuning_methodology/actions/workflows/build-test-python-package.yml/badge.svg)](https://github.com/fjwillemsen/autotuning_methodology/actions/workflows/build-test-python-package.yml)
-[![Docs](https://img.shields.io/github/actions/workflow/status/fjwillemsen/autotuning_methodology/publish-documentation.yml?label=docs)](https://fjwillemsen.github.io/autotuning_methodology/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 ![PyPI - License](https://img.shields.io/pypi/l/autotuning_methodology)
+[![Build Status](https://github.com/autotuningassociation/autotuning_methodology/actions/workflows/build-test-python-package.yml/badge.svg)](https://github.com/autotuningassociation/autotuning_methodology/actions/workflows/build-test-python-package.yml)
+[![Docs](https://img.shields.io/github/actions/workflow/status/autotuningassociation/autotuning_methodology/publish-documentation.yml?label=docs)](https://autotuningassociation.github.io/autotuning_methodology/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
+![PyPI - Status](https://img.shields.io/pypi/status/autotuning_methodology)
 
-
+ 
 This repository contains the software package accompanying the paper "A Methodology for Comparing Auto-Tuning Optimization Algorithms". 
 It makes the guidelines in the methodology easy to apply: simply specify the  `.json` file, run `autotuning_visualize [path_to_json]` and wait for the results!
 
 ## Installation
-The package can be installed by cloning this repository and running `pip install .`. Python >= 3.9 is supported.  
+The package can be installed with `pip install autotuning_methodology`. 
+Alternatively, it can be installed by cloning this repository and running `pip install .` in the root of the cloned project. 
+Python >= 3.9 is supported. 
 
 ## Notable features
 - Official software by the authors of the methodology-defining paper. 
 - Supports [BAT benchmark suite](https://github.com/NTNU-HPC-Lab/BAT) and [Kernel Tuner](https://github.com/KernelTuner/kernel_tuner).
 - Split executer and visualizer to allow running the algorithms on a cluster and visualize locally. 
 - Caching built-in to avoid duplicate executions.  
 - Planned support for T1 input and T4 output files.
-- Notebook / interactive window mode; in this case, plots are shown in the notebook / window instead of written to a folder. 
+- Notebook / interactive window mode; if enabled, plots are shown in the notebook / window instead of written to a folder. 
 
 <img width="674" alt="example run in interactive window" src="https://user-images.githubusercontent.com/6725103/232880006-70a05b0e-a4e4-4cc7-bea9-473959c474c2.png">
 <img width="483" alt="example run in interactive window 2" src="https://user-images.githubusercontent.com/6725103/232881244-d432ea8e-801a-44b1-9acb-b98cc1b740ac.png">
 
 ## Usage
 
 ### Entry points
 There are two entry points defined: `autotuning_experiment` and `autotuning_visualize`. Both take one argument: the path to an experiment file (see below). 
 
 ### Input files
 To get started, all you need is an experiments file. This is a `json` file that describes the details of your comparison: which algorithms to use, which programs to tune on which devices, the graphs to output and so on. 
-You can find the API and an example `experiments.json` in the [documentation](). 
+You can find the API and an example `experiments.json` in the [documentation](https://autotuningassociation.github.io/autotuning_methodology/modules.html). 
 
 ### File references
 As we are dealing with input and output files, file references matter. 
 When calling the entrypoints, we are already providing the path to an experiments file. 
 File references in experiments files are relative to the location of the experiment file itself. 
 File references in tuning scripts are relative to the location of the tuning script itself. Tuning scripts need to have the global literals `file_path_results` and `file_path_metadata` for this package to know where to get the results. 
 Plots outputted by this package are placed in a folder called `generated_plots` relative to the current working directory. 
 
 
+## Pipeline
+The below schematics show the pipeline implemented by this tool as described in the paper. 
+
+<!-- <img width="100%" alt="flowchart performance curve generation" src="https://autotuningassociation.github.io/autotuning_methodology/_static/flowchart_performance_curve_generation.svg"> -->
+![flowchart performance curve generation](docs/source/flowchart_performance_curve_generation.png)
+The first flowchart shows the tranformation of raw, stochastic optimization algorithm data to a performance curve. 
+
+<!-- <img width="100%" alt="flowchart output generation" src="docs/source/flowchart_output_generation.svg"> -->
+![flowchart output generation](docs/source/flowchart_output_generation.png)
+The second flowchart shows the adaption of performance curves of various optimization algorithms and search spaces to the desired output.
+
+
 ## Contributing
 
 ### Setup
 If you're looking to contribute to this package: welcome!
 Start out by installing with `pip install -e .[dev]` (this installs the package in editable mode alongside the development dependencies). 
 During development, unit and integration tests can be ran with `pytest`. 
 [Black](https://pypi.org/project/black/) is used as a formatter, and [Ruff](https://pypi.org/project/ruff/) is used as a linter to check the formatting, import sorting et cetera. 
 When using Visual Studio Code, use the `settings.json` found in `.vscode` to automatically have the correct linting, formatting and sorting during development. 
 In addition, install the extensions recommended by us by searching for `@recommended:workspace` in the extensions tab for a better development experience. 
 
 ### Documentation
-The documentation can be found [here](https://fjwillemsen.github.io/autotuning_methodology/). 
+The documentation can be found [here](https://autotuningassociation.github.io/autotuning_methodology/). 
 Locally, the documentation can be build with `make clean html` from the `docs` folder, but the package must have been installed in editable mode with `pip install -e .`. 
 Upon pushing to main or publishing a version, this documentation will be built and published to the GitHub Pages. 
 The Docstring format used is Google. Type hints are to be included in the function signature and therefor omitted from the docstring. In Visual Studio Code, the `autoDocstring` extension can be used to automatically infer docstrings. When referrring to functions and parameters in the docstring outside of their definition, use double backquotes to be compatible with both MarkDown and ReStructuredText, e.g.: *"skip_draws_check: skips checking that each value in ``draws`` is in the ``dist``."*.
 
 ### Tests
 Before contributing a pull request, please run `nox` and ensure it has no errors. This will test against all Python versions explicitely supported by this package, and will check whether the correct formatting has been applied.
 Upon submitting a pull request or pushing to main, these same checks will be ran remotely via GitHub Actions.
```

### Comparing `autotuning_methodology-0.1.0b1/UML/.$Sequence Diagram.drawio.bkp` & `autotuning_methodology-1.0.0b1/UML/.$Sequence Diagram.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/.$flowchart.drawio.bkp` & `autotuning_methodology-1.0.0b1/UML/.$flowchart.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/Sequence Diagram.drawio` & `autotuning_methodology-1.0.0b1/UML/Sequence Diagram.drawio`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/classes.pdf` & `autotuning_methodology-1.0.0b1/UML/classes.pdf`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/flowchart/.$flowchart.drawio.bkp` & `autotuning_methodology-1.0.0b1/UML/flowchart/.$flowchart.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/flowchart/flowchart.drawio` & `autotuning_methodology-1.0.0b1/UML/flowchart/flowchart.drawio`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/flowchart/flowchart_output_generation.png` & `autotuning_methodology-1.0.0b1/UML/flowchart/flowchart_output_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/flowchart/flowchart_performance_curve_generation.png` & `autotuning_methodology-1.0.0b1/UML/flowchart/flowchart_performance_curve_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/flowchart/mini_plots/flowchart_plot_aggregated.png` & `autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plot_aggregated.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/flowchart/mini_plots/flowchart_plot_individual.png` & `autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plot_individual.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/flowchart/mini_plots/flowchart_plots.py` & `autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plots.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/UML/packages.pdf` & `autotuning_methodology-1.0.0b1/UML/packages.pdf`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/docs/Makefile` & `autotuning_methodology-1.0.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/docs/autotuning_methodology.rst` & `autotuning_methodology-1.0.0b1/docs/autotuning_methodology.rst`

 * *Files 25% similar despite different names*

```diff
@@ -2,71 +2,71 @@
 ---------------
 
 .. automodule:: autotuning_methodology
    :members:
    :undoc-members:
    :show-inheritance:
 
-autotuning\_methodology.baseline module
+Baseline module
 ---------------------------------------
 .. inheritance-diagram:: src.autotuning_methodology.baseline
     :parts: 1
 
 .. automodule:: autotuning_methodology.baseline
    :members:
    :undoc-members:
    :show-inheritance:
 
-autotuning\_methodology.caching module
+Caching module
 --------------------------------------
 .. inheritance-diagram:: src.autotuning_methodology.caching
     :parts: 1
 
 .. automodule:: autotuning_methodology.caching
    :members:
    :undoc-members:
    :show-inheritance:
 
-autotuning\_methodology.curves module
+Curves module
 -------------------------------------
 .. inheritance-diagram:: src.autotuning_methodology.curves
     :parts: 1
 
 .. automodule:: autotuning_methodology.curves
    :members:
    :undoc-members:
    :show-inheritance:
 
-autotuning\_methodology.experiments module
+Experiments module
 ------------------------------------------
 
 .. automodule:: autotuning_methodology.experiments
    :members:
    :undoc-members:
    :show-inheritance:
 
-autotuning\_methodology.runner module
+Runner module
 -------------------------------------
 
 .. automodule:: autotuning_methodology.runner
    :members:
    :undoc-members:
    :show-inheritance:
 
-autotuning\_methodology.searchspace\_statistics module
+Searchspace statistics module
 ------------------------------------------------------
 .. inheritance-diagram:: src.autotuning_methodology.searchspace_statistics
     :parts: 1
 
 .. automodule:: autotuning_methodology.searchspace_statistics
    :members:
    :undoc-members:
    :show-inheritance:
 
-autotuning\_methodology.visualize\_experiments module
+Visualize experiments module
 -----------------------------------------------------
 .. inheritance-diagram:: src.autotuning_methodology.visualize_experiments
     :parts: 1
 
 .. automodule:: autotuning_methodology.visualize_experiments
    :members:
    :undoc-members:
```

### Comparing `autotuning_methodology-0.1.0b1/docs/conf.py` & `autotuning_methodology-1.0.0b1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-import os
-import sys
 import time
 
 from sphinx_pyproject import SphinxConfig
 
-sys.path.insert(0, os.path.abspath(".."))
+# sys.path.insert(0, os.path.abspath(".."))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 # import data from pyproject.toml using https://github.com/sphinx-toolbox/sphinx-pyproject
 # additional data can be added with `[tool.sphinx-pyproject]` and retrieved with `config['']`.
 config = SphinxConfig("../pyproject.toml")  # add `, globalns=globals()` to directly insert in namespace
@@ -43,14 +41,16 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.graphviz",
     "sphinx.ext.inheritance_diagram",
 ]
 autosummary_generate = True  # Turn on sphinx.ext.autosummary
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+add_module_names = False
+toc_object_entries_show_parents = "hide"
 
 # -- Options for inheritance diagrams ----------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/extensions/inheritance.html
 inheritance_graph_attrs = dict(rankdir="TB", fontsize=24, ratio="compress")
 inheritance_node_attrs = dict(fontsize=24)
```

### Comparing `autotuning_methodology-0.1.0b1/docs/make.bat` & `autotuning_methodology-1.0.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/docs/source/logo_autotuning_methodology.svg` & `autotuning_methodology-1.0.0b1/docs/source/logo_autotuning_methodology.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/docs/source/logo_kernel_dashboard.svg` & `autotuning_methodology-1.0.0b1/docs/source/logo_kernel_dashboard.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/docs/source/logo_kernel_launcher.svg` & `autotuning_methodology-1.0.0b1/docs/source/logo_kernel_launcher.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/docs/source/logo_kernel_tuner.svg` & `autotuning_methodology-1.0.0b1/docs/source/logo_kernel_tuner.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/experiment_files/bootstrap_hyperparams.json` & `autotuning_methodology-1.0.0b1/experiment_files/bootstrap_hyperparams.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/experiment_files/methodology_paper_example.json` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_cached.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7512152777777777%*

 * *Differences: {"'GPUs'": '{delete: [1]}',*

 * * "'bruteforced_caches_path'": "'../../../../cached_data_used/cachefiles'",*

 * * "'cutoff_percentile'": '0.99',*

 * * "'cutoff_percentile_start'": '0.7',*

 * * "'folder_id'": "'test_output_file_writer'",*

 * * "'kernels'": '{delete: [0]}',*

 * * "'kernels_path'": "'cached_data_used/kernels'",*

 * * "'name'": "'Test output file writer'",*

 * * "'plot'": "{'plot_x_value_types': {delete: [0]}}",*

 * * "'strategies'": "{0: {'name': 'random_sample_100_iter', 'strategy': 'random_sample', "*

 * *                 "'display_name': ' […]*

```diff
@@ -1,24 +1,22 @@
 {
     "GPUs": [
-        "RTX_2080_Ti",
-        "RTX_3090"
+        "RTX_2080_Ti"
     ],
-    "bruteforced_caches_path": "../cached_data_used/cachefiles",
-    "cutoff_percentile": 0.96,
-    "cutoff_percentile_start": 0.5,
+    "bruteforced_caches_path": "../../../../cached_data_used/cachefiles",
+    "cutoff_percentile": 0.99,
+    "cutoff_percentile_start": 0.7,
     "cutoff_type": "fevals",
-    "folder_id": "methodology_paper_evaluation",
+    "folder_id": "test_output_file_writer",
     "kernels": [
-        "pnpoly",
         "convolution"
     ],
-    "kernels_path": "../cached_data_used/kernels",
+    "kernels_path": "cached_data_used/kernels",
     "minimization": true,
-    "name": "Methodology paper evaluation",
+    "name": "Test output file writer",
     "objective_performance_keys": [
         "time"
     ],
     "objective_time_keys": [
         "compilation",
         "benchmark",
         "framework",
@@ -26,50 +24,35 @@
         "validation"
     ],
     "plot": {
         "compare_baselines": false,
         "compare_split_times": false,
         "confidence_level": 0.95,
         "plot_x_value_types": [
-            "time",
             "aggregated"
         ],
         "plot_y_value_types": [
             "normalized",
             "baseline"
         ]
     },
     "resolution": 1000.0,
     "strategies": [
         {
-            "display_name": "Genetic Algorithm",
-            "name": "genetic_algorithm",
-            "strategy": "genetic_algorithm"
-        },
-        {
-            "display_name": "PSO",
-            "name": "particle_swarm_optimization",
-            "strategy": "pso"
-        },
-        {
-            "display_name": "Firefly",
-            "name": "firefly",
-            "strategy": "firefly_algorithm"
-        },
-        {
-            "display_name": "Differential Evolution",
-            "name": "differential_evolution",
-            "strategy": "diff_evo"
+            "display_name": "Random sampling 100 iters",
+            "name": "random_sample_100_iter",
+            "repeats": 5,
+            "strategy": "random_sample"
         }
     ],
     "strategy_defaults": {
         "minimum_number_of_evaluations": 20,
         "record_data": [
             "time",
             "GFLOP/s"
         ],
         "repeats": 100,
         "stochastic": true
     },
     "version": "0.1.2",
-    "visualization_caches_path": "../cached_data_used/visualizations"
+    "visualization_caches_path": "../../../../cached_data_used/visualizations"
 }
```

### Comparing `autotuning_methodology-0.1.0b1/experiment_files/presentation_comparison.json` & `autotuning_methodology-1.0.0b1/experiment_files/presentation_comparison.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/experiment_files/test_random_calculated.json` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7846064814814815%*

 * *Differences: {"'GPUs'": '{delete: [1]}',*

 * * "'bruteforced_caches_path'": "'../../../../cached_data_used/cachefiles'",*

 * * "'folder_id'": "'test_output_file_writer'",*

 * * "'kernels'": '{delete: [1]}',*

 * * "'kernels_path'": "'cached_data_used/bogus_kernels_path'",*

 * * "'name'": "'Test output file writer'",*

 * * "'objective_time_keys'": "['compilation', 'benchmark', 'framework', 'search_algorithm', "*

 * *                          "'validation']",*

 * * "'plot'": "{'plot_x_value_types': {delete: [1, 0]}}",*

 * * "'strategies'": "{0: {'name': 'random_sampl […]*

```diff
@@ -1,68 +1,58 @@
 {
     "GPUs": [
-        "RTX_2080_Ti",
-        "RTX_3090"
+        "RTX_2080_Ti"
     ],
-    "bruteforced_caches_path": "../cached_data_used/cachefiles",
+    "bruteforced_caches_path": "../../../../cached_data_used/cachefiles",
     "cutoff_percentile": 0.99,
     "cutoff_percentile_start": 0.7,
     "cutoff_type": "fevals",
-    "folder_id": "test_random_calculated",
+    "folder_id": "test_output_file_writer",
     "kernels": [
-        "convolution",
-        "gemm"
+        "convolution"
     ],
-    "kernels_path": "../cached_data_used/kernels",
+    "kernels_path": "cached_data_used/bogus_kernels_path",
     "minimization": true,
-    "name": "Test random search (calculated vs executed)",
+    "name": "Test output file writer",
     "objective_performance_keys": [
         "time"
     ],
     "objective_time_keys": [
-        "strategy_time",
-        "compile_time",
-        "benchmark_time",
-        "verification_time",
-        "framework_time"
+        "compilation",
+        "benchmark",
+        "framework",
+        "search_algorithm",
+        "validation"
     ],
     "plot": {
         "compare_baselines": false,
         "compare_split_times": false,
         "confidence_level": 0.95,
         "plot_x_value_types": [
-            "fevals",
-            "time",
             "aggregated"
         ],
         "plot_y_value_types": [
             "normalized",
             "baseline"
         ]
     },
     "resolution": 1000.0,
     "strategies": [
         {
-            "display_name": "Random sampling 500 iters",
-            "name": "random_sample_500_iter",
-            "repeats": 500,
-            "strategy": "random_sample"
-        },
-        {
-            "display_name": "Random sampling 1000 iters",
-            "name": "random_sample_1000_iter",
-            "repeats": 1000,
+            "display_name": "Random sampling 100 iters",
+            "name": "random_sample_100_iter",
+            "repeats": 5,
             "strategy": "random_sample"
         }
     ],
     "strategy_defaults": {
         "minimum_number_of_evaluations": 20,
         "record_data": [
             "time",
             "GFLOP/s"
         ],
         "repeats": 100,
         "stochastic": true
     },
     "version": "0.1.2",
-    "visualization_caches_path": "../cached_data_used/visualizations"
+    "visualization_caches_path": "../../../../cached_data_used/visualizations"
 }
```

### Comparing `autotuning_methodology-0.1.0b1/experiment_files/test_scatter.json` & `autotuning_methodology-1.0.0b1/experiment_files/test_scatter.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/experiment_files/test_searchspace_algorithms.json` & `autotuning_methodology-1.0.0b1/experiment_files/test_searchspace_algorithms.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/bootstrap_hyperparams_visualizer.py` & `autotuning_methodology-1.0.0b1/extra/bootstrap_hyperparams_visualizer.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/experiments_strategies.py` & `autotuning_methodology-1.0.0b1/extra/experiments_strategies.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/experiments_strategies_hyperparamtuning.py` & `autotuning_methodology-1.0.0b1/extra/experiments_strategies_hyperparamtuning.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/generate_cachefile.py` & `autotuning_methodology-1.0.0b1/extra/generate_cachefile.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/max_draw_k_from_n.py` & `autotuning_methodology-1.0.0b1/extra/max_draw_k_from_n.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/speedtest_index_performance.py` & `autotuning_methodology-1.0.0b1/extra/speedtest_index_performance.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/speedtest_python_reversed_nan_sort.py` & `autotuning_methodology-1.0.0b1/extra/speedtest_python_reversed_nan_sort.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/try_BOtorch.py` & `autotuning_methodology-1.0.0b1/extra/try_BOtorch.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/try_GPytorch.py` & `autotuning_methodology-1.0.0b1/extra/try_GPytorch.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/extra/try_isotonic_regression.py` & `autotuning_methodology-1.0.0b1/extra/try_isotonic_regression.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/noxfile.py` & `autotuning_methodology-1.0.0b1/noxfile.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 This allows for locally mirroring the testing occuring with GitHub-actions.
 Be careful that the general setup of tests is left to pyproject.toml.
 """
 
 
 import nox
 
+# set the test parameters
+nox.options.stop_on_first_error = True
+nox.options.error_on_missing_interpreters = True
+
+
+@nox.session
+def lint(session: nox.Session) -> None:
+    """Ensure the code is formatted as expected."""
+    session.install("ruff")
+    session.run("ruff", "--output-format=github", "--config=pyproject.toml", ".")
+
 
 # @nox.session  # uncomment this line to only run on the current python interpreter
 @nox.session(python=["3.9", "3.10", "3.11"])  # missing versions can be installed with `pyenv install ...`
 # do not forget check / set the versions with `pyenv global`, or `pyenv local` in case of virtual environment
 def tests(session: nox.Session) -> None:
     """Run the tests for the specified Python versions."""
     session.install(".[test]")
     session.run("pytest")
-
-
-@nox.session
-def lint(session: nox.Session) -> None:
-    """Ensure the code is formatted as expected."""
-    session.install("ruff")
-    session.run("ruff", "--format=github", "--config=pyproject.toml", ".")
```

### Comparing `autotuning_methodology-0.1.0b1/pyproject.toml` & `autotuning_methodology-1.0.0b1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,87 +1,83 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
-[project]   # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
+[project] # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
 name = "autotuning_methodology"
-version = "0.1.0b1"
-authors = [
-    {name = "Floris-Jan Willemsen", email = "fjwillemsen97@gmail.com"},
-]
+version = "1.0.0b1"
+authors = [{ name = "Floris-Jan Willemsen", email = "fjwillemsen97@gmail.com" }]
 description = "Software package easing implementation of the guidelines of the 2023 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'."
 keywords = ["autotuning", "auto-tuning", "methodology", "scientific"]
 readme = "README.md"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-]       # https://pypi.org/classifiers/
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+] # https://pypi.org/classifiers/
 dependencies = [
     "numpy >= 1.22.4",
+    "scipy >= 1.10.1",
     "scikit-learn >= 1.0.2",
     "matplotlib >= 3.7.1",
     "yappi >= 1.4.0",
     "progressbar2 >= 4.2.0",
     "jsonschema >= 4.17.3",
     "nonconformist >= 2.1.0",
-    "kernel_tuner >= 0.4.5",
+    "kernel_tuner >= 1.0.0b5",
 ]
 
 [project.optional-dependencies]
-dev = [
-    "pylint >=2.14.4",
-    "black >= 23.3.0",
-]
+dev = ["pylint >=2.14.4", "black >= 23.3.0"]
 docs = [
     "sphinx >= 6.2.1",
     "sphinx_rtd_theme >= 1.2.0",
     "sphinx-pyproject >= 0.1.0",
 ]
 test = [
     "ruff >= 0.0.263",
     "pep440 >= 0.1.2",
     "pytest >= 7.3.1",
     "pytest-cov >= 4.0.0",
     "nox >= 2023.4.22",
     "crepes >= 0.2.0",
-    "tomli >= 2.0.1",   # can be replaced by built-in [tomllib](https://docs.python.org/3.11/library/tomllib.html) from Python 3.11
+    "tomli >= 2.0.1",      # can be replaced by built-in [tomllib](https://docs.python.org/3.11/library/tomllib.html) from Python 3.11
 ]
 
 [project.scripts]
 autotuning_experiment = "autotuning_methodology.experiments:entry_point"
 autotuning_visualize = "autotuning_methodology.visualize_experiments:entry_point"
 
 [project.urls]
 "Repository" = "https://github.com/fjwillemsen/autotuning_methodology"
 "Documentation" = "https://fjwillemsen.github.io/autotuning_methodology/"
 "Bug Tracker" = "https://github.com/fjwillemsen/autotuning_methodology/issues"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
-pythonpath = ["src"]    # necessary to get coverage reports without installing with `-e`
+pythonpath = [
+    "src",
+] # necessary to get coverage reports without installing with `-e`
 addopts = "--cov --cov-config=.coveragerc --cov-report html --cov-report term-missing --cov-fail-under 80"
-testpaths = [
-    "tests/unit",
-    "tests/integration",
-    "tests/release",
-]
+testpaths = ["tests/unit", "tests/integration", "tests/release"]
 
 [tool.black]
 line-length = 120
 [tool.ruff]
 line-length = 120
 src = ["src"]
 respect-gitignore = true
 exclude = ["extra", "UML", "tests/autotuning_methodology/*mockfiles*"]
 select = [
-  "E",   # pycodestyle
-  "F",   # pyflakes,
-  "D",   # pydocstyle,
+    "E", # pycodestyle
+    "F", # pyflakes,
+    "D", # pydocstyle,
 ]
 # target-version = "py310"   # inferred from project.requires-python
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `autotuning_methodology-0.1.0b1/src/autotuning_methodology/baseline.py` & `autotuning_methodology-1.0.0b1/src/autotuning_methodology/baseline.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from math import ceil
 from typing import Callable, Optional
 
 import numpy as np
+from scipy.interpolate import PchipInterpolator
 
-from autotuning_methodology.curves import CurveBasis, get_indices_in_array
+from autotuning_methodology.curves import CurveBasis, get_indices_in_array, moving_average
 from autotuning_methodology.searchspace_statistics import SearchspaceStatistics
 
 
 class Baseline(CurveBasis):
     """Class to use as a baseline against Curves in plots."""
 
     label: str
@@ -105,21 +106,41 @@
         index = min(N - 1, index)
         return index
 
     def _redwhite_index_value(self, M: int, N: int, dist: np.ndarray) -> float:
         """Get the expected value in the distribution for a budget in number of function evaluations M."""
         return dist[self._redwhite_index(M, N)]
 
-    def _get_random_curve(self, fevals_range: np.ndarray) -> np.ndarray:
+    def _get_random_curve(self, fevals_range: np.ndarray, smoothing=True) -> np.ndarray:
         """Returns the drawn values of the random curve at each number of function evaluations."""
         ks = fevals_range
         dist = self._redwhite_index_dist
         N = dist.shape[0]
         draws = np.array([self._redwhite_index_value(k, N, dist) for k in ks])
-        return draws
+        if not smoothing or len(fevals_range) <= 2:
+            return draws
+
+        # the monotic interpolator does not handle duplicate values, so if present, filter them out first
+        if len(fevals_range) != len(np.unique(fevals_range)):
+            # get a boolean mask of the fevals_range-values that occur multiple times
+            # (as ediff1d only gives the difference between consecutive values, the first value is added as True)
+            first_occurance_index = np.concatenate([[True], np.where(np.ediff1d(fevals_range) > 0, True, False)])
+            assert len(first_occurance_index) == len(fevals_range) == len(draws)
+
+            # apply the boolean mask to the x and y dimensions
+            x = fevals_range[first_occurance_index]
+            y = draws[first_occurance_index]
+        else:
+            x = fevals_range
+            y = draws
+
+        # apply the monotonicity-preserving Piecewise Cubic Hermite Interpolating Polynomial
+        smooth_fevals_range = np.linspace(fevals_range[0], fevals_range[-1], len(fevals_range))
+        smooth_draws = PchipInterpolator(x, y)(smooth_fevals_range)
+        return smooth_draws
 
     def _draw_random(self, xs: np.ndarray, k: int):
         """Monte Carlo simulation over cache."""
         return np.random.choice(xs, size=k, replace=False)
 
     def _stats_max(self, xs: np.ndarray, k: int, trials: int, opt_func: Callable) -> np.ndarray:
         # print("Running for stats max size", k, end="\r", flush=True)
@@ -145,15 +166,21 @@
     ) -> np.ndarray:
         if self.simulate:
             return self._get_random_curve_means(fevals_range)
         return self._get_random_curve(fevals_range)
 
     def get_curve_over_time(self, time_range: np.ndarray, dist=None, confidence_level=None) -> np.ndarray:  # noqa: D102
         fevals_range = self.time_to_fevals(time_range)
-        return self.get_curve_over_fevals(fevals_range, dist, confidence_level)
+        curve_over_time = self.get_curve_over_fevals(fevals_range, dist, confidence_level)
+        smoothing_factor = 0.0
+        if smoothing_factor > 0.0:
+            window_size = min(time_range.size, ceil(time_range.size * smoothing_factor))
+            if time_range.size > 1 and window_size > 1:
+                curve_over_time = moving_average(curve_over_time, window_size)
+        return curve_over_time
 
     def get_standardised_curve(  # noqa: D102
         self, range: np.ndarray, strategy_curve: np.ndarray, x_type: str
     ) -> np.ndarray:
         return super().get_standardised_curve(range, strategy_curve, x_type)
 
     def get_standardised_curves(  # noqa: D102
```

### Comparing `autotuning_methodology-0.1.0b1/src/autotuning_methodology/caching.py` & `autotuning_methodology-1.0.0b1/src/autotuning_methodology/caching.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/src/autotuning_methodology/curves.py` & `autotuning_methodology-1.0.0b1/src/autotuning_methodology/curves.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Code for curve generation."""
 
-from __future__ import \
-    annotations  # for correct nested type hints e.g. list[str], tuple[dict, str]
+from __future__ import annotations  # for correct nested type hints e.g. list[str], tuple[dict, str]
 
-import warnings
 from abc import ABC, abstractmethod
 from math import ceil, floor, sqrt
+from warnings import warn
 
 import numpy as np
 from sklearn.ensemble import BaggingRegressor
 from sklearn.isotonic import IsotonicRegression
 
 from autotuning_methodology.caching import ResultsDescription
 from autotuning_methodology.searchspace_statistics import SearchspaceStatistics
@@ -43,17 +42,18 @@
         ), f"""Distribution is not sorted ascendingly,
             {np.count_nonzero(~strictly_ascending_sort)} violations in {len(dist)} values: {dist}"""
 
     # check whether each value of draws (excluding NaN) is in dist
     if not skip_draws_check:
         assert np.all(
             np.in1d(draws[~np.isnan(draws)], dist)
-        ), f"""Each value in draws should be in dist,
+        ), f"""
+            Each value in draws should be in dist,
             but {np.size(draws[~np.isnan(draws)][~np.in1d(draws[~np.isnan(draws)], dist)])} values
-             of the {np.size(draws)} are missing: {draws[~np.isnan(draws)][~np.in1d(draws[~np.isnan(draws)], dist)]}"""
+            of the {np.size(draws)} are missing: {draws[~np.isnan(draws)][~np.in1d(draws[~np.isnan(draws)], dist)]}"""
 
     # check the sorter
     if sorter is not None:
         assert sorter.shape == dist.shape, "The shape of the sorter must be the same as the distribution"
 
     # find the index of each draw in the distribution
     indices_found = np.searchsorted(dist, draws, side="left", sorter=sorter).astype(float)
@@ -89,14 +89,33 @@
     nan_mask = ~np.isnan(indices_found)
     indices_found_unsorted = np.full_like(indices_found, fill_value=np.NaN)
     indices_found_unsorted[nan_mask] = array_sorter[indices_found[nan_mask].astype(int)]
 
     return indices_found_unsorted
 
 
+def moving_average(y: np.ndarray, window_size=3) -> np.ndarray:
+    """Function to calculate the moving average over an array.
+
+    Output array is the same size as input array.
+    After https://stackoverflow.com/a/47490020.
+
+    Args:
+        y: the 1-dimensional array to calculate the moving average over.
+        window_size: the moving average window size. Defaults to 3.
+
+    Returns:
+        the smoothed 1-dimensional array with the same size as input array.
+    """
+    assert y.ndim == 1
+    y_padded = np.pad(y, (window_size // 2, window_size - 1 - window_size // 2), mode="edge")
+    y_smooth = np.convolve(y_padded, np.ones((window_size,)) / window_size, mode="valid")
+    return y_smooth
+
+
 class CurveBasis(ABC):
     """Abstract object providing minimals for visualization and analysis. Implemented by ``Curve`` and ``Baseline``."""
 
     @abstractmethod
     def get_curve(self, range: np.ndarray, x_type: str, dist: np.ndarray = None, confidence_level: float = None):
         """Get the curve over the specified range of time or function evaluations.
 
@@ -338,22 +357,15 @@
         Returns:
             _description_
         """
         return IsotonicRegression(
             increasing=not self.minimization, y_min=y_min, y_max=y_max, out_of_bounds=out_of_bounds
         )
 
-    def get_isotonic_curve(
-        self,
-        x: np.ndarray,
-        y: np.ndarray,
-        x_new: np.ndarray,
-        ymin=None,
-        ymax=None,
-    ) -> np.ndarray:
+    def get_isotonic_curve(self, x: np.ndarray, y: np.ndarray, x_new: np.ndarray, ymin=None, ymax=None) -> np.ndarray:
         """Get the isotonic regression curve fitted to x_new using package 'sklearn' or 'isotonic'.
 
         Args:
             x: x-dimension training data.
             y: y-dimension training data.
             x_new: x-dimension prediction data.
             ymin: lower bound on the lowest predicted value. Defaults to None.
@@ -364,34 +376,38 @@
         """
         # check if the assumptions that the input arrays are numpy arrays holds
         assert isinstance(x, np.ndarray)
         assert isinstance(y, np.ndarray)
         assert isinstance(x_new, np.ndarray)
         assert x_new.ndim == 1
 
+        # flatten the input arrays if necessary
         if x.ndim > 1:
             x = x.flatten()
         if y.ndim > 1:
             y = y.flatten()
 
+        # apply isotonic regression
         ir = self.get_isotonic_regressor(y_min=ymin, y_max=ymax)
         ir.fit(x, y)
-        return ir.predict(x_new)
+        isotonic_curve = ir.predict(x_new)
+        return isotonic_curve
 
 
 class StochasticOptimizationAlgorithm(Curve):
     """Class for producing a curve for stochastic optimization algorithms."""
 
     def _get_curve_split_real_fictional_parts(
         self,
         real_stopping_point_index: int,
         x_axis_range: np.ndarray,
         curve: np.ndarray,
         curve_lower_err: np.ndarray,
         curve_upper_err: np.ndarray,
+        smoothing_factor=0.0,
     ) -> tuple[int, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
         """Split the provided curves based on the real_stopping_point_index.
 
         Return real_stopping_point_index and the real and fictional part for each curve.
         """
         # select the parts of the data that are real
         x_axis_range_real = x_axis_range[:real_stopping_point_index]
@@ -407,15 +423,15 @@
         target_index = x_axis_range.shape[0] - 1
         if real_stopping_point_index <= target_index:
             x_axis_range_fictional = x_axis_range[real_stopping_point_index:]
             curve_fictional = curve[real_stopping_point_index:]
             curve_lower_err_fictional = curve_lower_err[real_stopping_point_index:]
             curve_upper_err_fictional = curve_upper_err[real_stopping_point_index:]
 
-        # check and return
+        # check the consistency
         self._check_curve_real_fictional_consistency(
             x_axis_range,
             curve,
             curve_lower_err,
             curve_upper_err,
             x_axis_range_real,
             curve_real,
@@ -423,14 +439,29 @@
             curve_upper_err_real,
             x_axis_range_fictional,
             curve_fictional,
             curve_lower_err_fictional,
             curve_upper_err_fictional,
         )
 
+        # smooth the curve if applicable
+        if smoothing_factor > 0.0:
+            if smoothing_factor >= 1:
+                raise ValueError(f"Smoothing factor can't be >= 1, is {smoothing_factor}")
+            elif smoothing_factor >= 0.05:
+                warn(
+                    f"Smoothing factor {smoothing_factor} >= 0.05, likely making curves too smooth. 0.005 recommended",
+                    category=UserWarning,
+                )
+            window_size = min(x_axis_range.size, ceil(x_axis_range.size * smoothing_factor))
+            if window_size > 1:
+                curve_real = moving_average(curve_real, window_size)
+                curve_lower_err_real = moving_average(curve_lower_err_real, window_size)
+                curve_upper_err_real = moving_average(curve_upper_err_real, window_size)
+
         return (
             real_stopping_point_index,
             x_axis_range_real,
             curve_real,
             curve_lower_err_real,
             curve_upper_err_real,
             x_axis_range_fictional,
@@ -537,15 +568,15 @@
         if not np.allclose(masked_fevals, masked_fevals[0], equal_nan=True):
             indices = np.nanargmax(masked_fevals, axis=1)  # get the index of the last non-nan value of each repeat
             num_repeats = len(indices)
             # find the repeats that end before the index
             early_ending_repeats = np.where(indices < target_index)
             greatest_common_non_NaN_index = min(floor(np.median(indices)), target_index)
             if np.count_nonzero(early_ending_repeats) > 0:
-                warnings.warn(
+                warn(
                     f"""For optimization algorithm {self.display_name},
                     {np.count_nonzero(early_ending_repeats)} of the {num_repeats} runs ended before
                      the end of fevals_range ({target_index + 1}).
                      Only data up to {greatest_common_non_NaN_index + 1} fevals will be used.
                      Perhaps increase the allotted auto-tuning time for this optimization algorithm?"""
                 )
 
@@ -630,18 +661,19 @@
             curve_lower_err = np.pad(curve_lower_err, pad_width=pad_width, constant_values=np.nan)
             curve_upper_err = np.pad(curve_upper_err, pad_width=pad_width, constant_values=np.nan)
         assert curve.shape == fevals_range.shape, "The curve shape must match the input fevals_range shape"
 
         # if necessary, extend the curves up to target_index
         target_index: int = fevals_range.shape[0] - 1
         if real_stopping_point_index < target_index:
-            warnings.warn(
+            warn(
                 f"""For optimization algorithm {self.display_name},
                 all runs end at {real_stopping_point_index + 1} fevals,
-                which is before the target number of function evals of {target_index + 1}."""
+                which is before the target number of function evals of {target_index + 1}.""",
+                category=UserWarning,
             )
             # take the last non-NaN value and overwrite the curves up to the target index with it
             curve[real_stopping_point_index : target_index + 1] = curve[real_stopping_point_index]
             curve_lower_err[real_stopping_point_index : target_index + 1] = curve_lower_err[real_stopping_point_index]
             curve_upper_err[real_stopping_point_index : target_index + 1] = curve_upper_err[real_stopping_point_index]
 
         # check whether there are no NaNs left
@@ -931,16 +963,17 @@
             _x = _x[no_nan_mask]
             _y = _y[no_nan_mask]
             assert _x.ndim == _y.ndim == 1
             assert np.all(~np.isnan(_x))
             assert np.all(~np.isnan(_y))
             fraction_valid = _y.shape[0] / num_fevals
             if fraction_valid < 0.05:
-                warnings.warn(
-                    f"{round(fraction_valid * 100, 1)}% data left after removing NaN ({_y.shape[0]} / {num_fevals})"
+                warn(
+                    f"{round(fraction_valid * 100, 1)}% data left after removing NaN ({_y.shape[0]} / {num_fevals})",
+                    category=UserWarning,
                 )
 
             # get the prediction
             predictions[run] = self.get_isotonic_curve(_x, _y, time_range)
 
         # extract the mean and prediction intervals
         assert np.all(~np.isnan(predictions))
```

### Comparing `autotuning_methodology-0.1.0b1/src/autotuning_methodology/experiments.py` & `autotuning_methodology-1.0.0b1/src/autotuning_methodology/experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     curve_segment_factor: float = experiment.get("curve_segment_factor", 0.05)
     assert isinstance(curve_segment_factor, float), f"curve_segment_factor is not float, {type(curve_segment_factor)}"
     strategies = get_strategies(experiment)
 
     # add the kernel directory to the path to import the module, relative to the experiment file
     kernels_path = experiment_folderpath / Path(experiment["kernels_path"])
     if not kernels_path.exists():
-        raise FileNotFoundError(f"No such path {kernels_path}, CWD: {getcwd()}")
+        raise FileNotFoundError(f"No such path {kernels_path.resolve()}, CWD: {getcwd()}")
     sys.path.append(str(kernels_path))
     kernel_names = experiment["kernels"]
     kernels = list(import_module(kernel_name) for kernel_name in kernel_names)
 
     # variables for comparison
     objective_time_keys: list[str] = experiment["objective_time_keys"]
     objective_performance_keys: list[str] = experiment["objective_performance_keys"]
@@ -206,15 +206,17 @@
                     visualization_caches_path=experiment_folderpath / experiment["visualization_caches_path"],
                 )
 
                 # if the strategy is in the cache, use cached data
                 if "ignore_cache" not in strategy and results_description.has_results():
                     print(" | - |-> retrieved from cache")
                 else:  # execute each strategy that is not in the cache
-                    results_description = collect_results(kernel, strategy, results_description, profiling=profiling)
+                    results_description = collect_results(
+                        kernel, strategy, results_description, searchspace_stats, profiling=profiling
+                    )
 
                 # set the results
                 results_descriptions[gpu_name][kernel_name][strategy_name] = results_description
 
     return experiment, strategies, results_descriptions
```

### Comparing `autotuning_methodology-0.1.0b1/src/autotuning_methodology/schema.json` & `autotuning_methodology-1.0.0b1/src/autotuning_methodology/schema.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/src/autotuning_methodology/searchspace_statistics.py` & `autotuning_methodology-1.0.0b1/src/autotuning_methodology/searchspace_statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Code for obtaining search space statistics."""
 
-
 from __future__ import annotations  # for correct nested type hints e.g. list[str], tuple[dict, str]
 
 import json
 from math import ceil, floor
 from pathlib import Path
 
 import numpy as np
 
-from autotuning_methodology.runner import is_invalid_objective_performance, is_invalid_objective_time
+from autotuning_methodology.validators import is_invalid_objective_performance, is_invalid_objective_time
 
 
 def nansumwrapper(array: np.ndarray, **kwargs) -> np.ndarray:
     """Wrapper around np.nansum. Ensures partials that contain only NaN are returned as NaN instead of 0.
 
     Args:
         array: values to sum.
@@ -90,17 +89,19 @@
         Args:
             time_keys: list of T4-style time keys.
 
         Returns:
             List of Kernel Tuner-style time keys.
         """
         return list(
-            self.T4_time_keys_to_kernel_tuner_time_keys_mapping[key]
-            if key in self.T4_time_keys_to_kernel_tuner_time_keys_mapping
-            else key
+            (
+                self.T4_time_keys_to_kernel_tuner_time_keys_mapping[key]
+                if key in self.T4_time_keys_to_kernel_tuner_time_keys_mapping
+                else key
+            )
             for key in time_keys
         )
 
     def total_performance_absolute_optimum(self) -> float:
         """Calculate the absolute optimum of the total performances.
 
         Returns:
@@ -116,40 +117,98 @@
 
         Returns:
             The objective performance value at which to stop.
         """
         absolute_optimum = self.total_performance_absolute_optimum()
         median = self.total_performance_median()
         objective_performance_target = absolute_optimum + ((median - absolute_optimum) * (1 - cutoff_percentile))
+        # print(f"{cutoff_percentile=}, {median=}, {absolute_optimum=}; results in {objective_performance_target=}")
         return objective_performance_target
 
+    def plot_histogram(self, cutoff_percentile: float):
+        """Plots a histogram of the distribution.
+
+        Args:
+            cutoff_percentile: the desired cutoff percentile to reach before stopping.
+        """
+        # prepare plot
+        import matplotlib.pyplot as plt
+
+        fig, axs = plt.subplots(1, 1, sharey=True, tight_layout=True)
+        if not isinstance(axs, list):
+            axs = [axs]
+
+        # prepare data
+        performances = self.objective_performances_total_sorted
+        mean = self.total_performance_mean()
+        median = self.total_performance_median()
+        cutoff_performance = self.objective_performance_at_cutoff_point(cutoff_percentile)
+
+        # plot the data
+        n_bins = 200
+        axs[0].hist(performances, bins=n_bins)
+        axs[0].set_ylabel("Number of configurations in bin")
+        axs[0].set_xlabel("Performance in miliseconds")
+        axs[0].axvline(x=[mean], label="Mean", c="red")
+        axs[0].axvline(x=[median], label="Median", c="orange")
+        axs[0].axvline(x=[cutoff_performance], label="Cutoff point", c="green")
+
+        # finalize and show plot
+        plt.legend()
+        plt.show()
+
     def cutoff_point(self, cutoff_percentile: float) -> tuple[float, int]:
         """Calculates the cutoff point.
 
         Args:
             cutoff_percentile: the desired cutoff percentile to reach before stopping.
 
         Returns:
             A tuple of the objective value at the cutoff point and the fevals to the cutoff point.
         """
-        objective_performance_at_cutoff_point = self.objective_performance_at_cutoff_point(cutoff_percentile)
         inverted_sorted_performance_arr = self.objective_performances_total_sorted[::-1]
         N = inverted_sorted_performance_arr.shape[0]
 
-        # fevals_to_cutoff_point = ceil((cutoff_percentile * N) / (1 + (1 - cutoff_percentile) * N))
+        # get the objective performance at the cutoff point
+        objective_performance_at_cutoff_point = self.objective_performance_at_cutoff_point(cutoff_percentile)
+
+        # # top 10 duplicate values
+        # uniques, counts = np.unique(inverted_sorted_performance_arr, return_counts=True)
+        # top_ten = sorted(zip(uniques, counts), key=lambda x: x[1])[-10:]
+        # print(f"Searchspace size: {N}, of which unique: {len(uniques)}")
+        # print("Top ten duplicate values (value, occurance):")
+        # print(top_ten)
+
+        # # for each number of function evaluations from 0 to N
+        # print("Calculating r_i (eq. 6) for each feval until the performance cutoff is reached:")
+        # for feval in range(0, N):
+        #     # calculate the random search index
+        #     ri = round((feval * (N + 1)) / (feval + 1))
+        #     print(f"  {feval}: {ri} ({round(ri / N * 100, 3)}%)")
+        #     # lookup if random search has reached the performance at cutoff
+        #     if inverted_sorted_performance_arr[ri] <= objective_performance_at_cutoff_point:
+        #         i = ri
+        #         fevals_to_cutoff_point = ceil(i / (N + 1 - i))
+        #         break
+
+        # fevals_to_cutoff_point_alt = ceil((cutoff_percentile * N) / (1 + (1 - cutoff_percentile) * N))
 
+        # iterate over the inverted_sorted_performance_arr until we have
         # i = next(x[0] for x in enumerate(inverted_sorted_performance_arr) if x[1] > cutoff_percentile * arr[-1])
         i = next(
             x[0] for x in enumerate(inverted_sorted_performance_arr) if x[1] <= objective_performance_at_cutoff_point
         )
         # In case of x <= (1+p) * f_opt
         # i = next(x[0] for x in enumerate(inverted_sorted_performance_arr) if x[1] <= (1 + (1 - cutoff_percentile)) * arr[-1])  # noqa: E501
         # In case of p*x <= f_opt
         # i = next(x[0] for x in enumerate(inverted_sorted_performance_arr) if cutoff_percentile * x[1] <= arr[-1])
         fevals_to_cutoff_point = ceil(i / (N + 1 - i))
+
+        # print(f"{fevals_to_cutoff_point=} ({i=})")
+        # exit(0)
         return objective_performance_at_cutoff_point, fevals_to_cutoff_point
 
     def cutoff_point_fevals_time(self, cutoff_percentile: float) -> tuple[float, int, float]:
         """Calculates the cutoff point.
 
         Args:
             cutoff_percentile: the desired cutoff percentile to reach before stopping.
@@ -157,34 +216,43 @@
         Returns:
             A tuple of the objective value at cutoff point, fevals to cutoff point, and the mean time to cutoff point.
         """
         cutoff_point_value, cutoff_point_fevals = self.cutoff_point(cutoff_percentile)
         cutoff_point_time = cutoff_point_fevals * self.total_time_median()
         return cutoff_point_value, cutoff_point_fevals, cutoff_point_time
 
-    def _get_filepath(self) -> Path:
+    def _get_filepath(self, lowercase=True) -> Path:
         """Returns the filepath."""
-        kernel_directory = self.kernel_name.lower()
-        filename = f"{self.device_name.lower()}.json"
+        kernel_directory = self.kernel_name
+        if lowercase:
+            kernel_directory = kernel_directory.lower()
+        filename = f"{self.device_name}.json"
+        if lowercase:
+            filename = filename.lower()
         return self.bruteforced_caches_path / kernel_directory / filename
 
     def get_valid_filepath(self) -> Path:
         """Returns the filepath to the Searchspace statistics .json file if it exists.
 
         Raises:
             FileNotFoundError: if filepath does not exist.
 
         Returns:
             Filepath to the Searchspace statistics .json file.
         """
         filepath = self._get_filepath()
         if not filepath.exists():
-            import os
+            filepath = self._get_filepath(lowercase=False)
+        if not filepath.exists():
+            # if the file is not found, raise an error
+            from os import getcwd
 
-            raise FileNotFoundError(f"{filepath} does not exist relative to current working directory {os.getcwd()}")
+            raise FileNotFoundError(
+                f"{filepath.resolve()} does not exist relative to current working directory {getcwd()}"
+            )
         return filepath
 
     def _is_not_invalid_value(self, value, performance: bool) -> bool:
         """Checks if a cache performance or time value is an array or is not invalid."""
         if isinstance(value, str):
             return False
         if isinstance(value, (list, tuple, np.ndarray)):
@@ -225,14 +293,15 @@
                 contents = orig_contents[:-1] + "}\n}"
                 try:
                     data = json.loads(contents)
                 except json.decoder.JSONDecodeError:
                     contents = orig_contents[:-2] + "}\n}"
                     data = json.loads(contents)
             cache: dict = data["cache"]
+            self.cache = cache
 
             # get the time values per configuration
             cache_values = list(cache.values())
             self.size = len(cache_values)
             self.objective_times = dict()
             for key in self.objective_time_keys:
                 self.objective_times[key] = self._to_valid_array(cache_values, key, performance=False)
@@ -279,22 +348,22 @@
                 list(self.objective_performances[key] for key in self.objective_performance_keys)
             )
             assert self.objective_performances_array.shape == tuple([len(self.objective_performance_keys), self.size])
 
             # get the totals
             self.objective_times_total = nansumwrapper(self.objective_times_array, axis=0)
             assert self.objective_times_total.shape == tuple([self.size])
-            # NOTE more of a test than a necessary assert
+            # more of a test than a necessary assert
             assert (
                 np.nansum(self.objective_times_array[:, 0]) == self.objective_times_total[0]
             ), f"""Sums of objective performances do not match:
                 {np.nansum(self.objective_times_array[:, 0])} vs. {self.objective_times_total[0]}"""
             self.objective_performances_total = nansumwrapper(self.objective_performances_array, axis=0)
             assert self.objective_performances_total.shape == tuple([self.size])
-            # NOTE more of a test than a necessary assert
+            # more of a test than a necessary assert
             assert (
                 np.nansum(self.objective_performances_array[:, 0]) == self.objective_performances_total[0]
             ), f"""Sums of objective performances do not match:
                 {np.nansum(self.objective_performances_array[:, 0])} vs. {self.objective_performances_total[0]}"""
 
             # sort
             self.objective_times_total_sorted = np.sort(
@@ -316,19 +385,40 @@
             )
             self.objective_performances_total_sorted_nan = np.concatenate(
                 (sorted_best_first, [np.nan] * self.objective_performances_number_of_nan)
             )
 
         return True
 
-    def get_time_per_feval(self, time_per_feval_operator: str) -> float:
+    def get_value_in_config(self, config: str, key: str):
+        """Get the value for a key given a configuration."""
+        return self.cache[config][key]
+
+    def get_num_duplicate_values(self, value: float) -> int:
+        """Get the number of duplicate values in the searchspace."""
+        duplicates = np.count_nonzero(np.where(self.objective_performances_total == value, 1, 0)) - 1
+        if duplicates < 0:
+            raise ValueError(f"Value {value} not in distribution")
+        return duplicates
+
+    def mean_strategy_time_per_feval(self) -> float:
+        """Gets the average time spent on the strategy per function evaluation."""
+        if "strategy" in self.objective_times:
+            strategy_times = self.objective_times
+            invalid_mask = np.isnan(self.objective_performances_total)
+            if not all(invalid_mask):
+                return np.mean(strategy_times)
+        return 0
+
+    def get_time_per_feval(self, time_per_feval_operator: str, strategy_offset=False) -> float:
         """Gets the average time per function evaluation. Several methods available.
 
         Args:
             time_per_feval_operator: method to use.
+            strategy_offset: whether to include a small offset to adjust for missing strategy time.
 
         Raises:
             ValueError: if invalid ``time_per_feval_operator`` is passed.
 
         Returns:
             The average time per function evaluation.
         """
@@ -341,15 +431,20 @@
         elif time_per_feval_operator == "mean_per_feval":
             time_per_feval = self.total_time_mean_per_feval()
         elif time_per_feval_operator == "median_per_feval":
             time_per_feval = self.total_time_median_per_feval()
         else:
             raise ValueError(f"Invalid {time_per_feval_operator=}")
         assert not np.isnan(time_per_feval) and time_per_feval > 0, f"Invalid {time_per_feval=}"
-        return time_per_feval
+        # add a small amount of strategy time if necessary
+        offset = 0
+        if strategy_offset and self.mean_strategy_time_per_feval() == 0:
+            # offset should not be more than 10% of actual time per feval
+            offset = min(time_per_feval * 0.1, 0.001)
+        return time_per_feval + offset
 
     def total_time_minimum(self) -> float:
         """Get the minimum value of total time."""
         return self.objective_times_total_sorted[0]
 
     def total_time_maximum(self) -> float:
         """Get the maximum value of total time."""
```

### Comparing `autotuning_methodology-0.1.0b1/src/autotuning_methodology/visualize_experiments.py` & `autotuning_methodology-1.0.0b1/src/autotuning_methodology/visualize_experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,36 +35,36 @@
             "time_partial_times": "kernel runtime",
             "time_partial_verification_time": "verification time",
         }
     )
 
     y_metric_displayname = dict(
         {
-            "objective_absolute": "Best found objective value",
-            "objective_scatter": "Best found objective value",
+            "objective_absolute": "Best-found objective value",
+            "objective_scatter": "Best-found objective value",
             "objective_relative_median": "Fraction of absolute optimum relative to median",
-            "objective_normalized": "Best found objective value normalized \n from median to absolute optimum",
-            "objective_baseline": "Best found objective value \n relative to baseline",
+            "objective_normalized": "Best-found objective value\n(normalized from median to optimum)",
+            "objective_baseline": "Best-found objective value\n(relative to baseline)",
             "objective_baseline_max": "Improvement over random sampling",
-            "aggregate_objective": "Aggregate best found objective function value relative to baseline",
+            "aggregate_objective": "Aggregate best-found objective value relative to baseline",
             "aggregate_objective_max": "Aggregate improvement over random sampling",
-            "time": "Best found kernel time in miliseconds",
+            "time": "Best-found kernel time in miliseconds",
             "GFLOP/s": "GFLOP/s",
         }
     )
 
     plot_x_value_types = ["fevals", "time", "aggregated"]  # number of function evaluations, time, aggregation
     plot_y_value_types = [
         "absolute",
         "scatter",
         "normalized",
         "baseline",
     ]  # absolute values, scatterplot, median-absolute normalized, improvement over baseline
 
-    plot_filename_prefix = "generated_plots/"
+    plot_filename_prefix_parent = "generated_plots"
 
     colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
 
     def __init__(
         self,
         experiment_filepath: str,
         save_figs=True,
@@ -87,19 +87,23 @@
         # # silently execute the experiment
         # with warnings.catch_warnings():
         #     warnings.simplefilter("ignore")
         self.experiment, self.strategies, self.results_descriptions = execute_experiment(
             experiment_filepath, profiling=False
         )
         experiment_folderpath = Path(experiment_filepath).parent
+        experiment_folder_id: str = self.experiment["folder_id"]
+        assert isinstance(experiment_folder_id, str) and len(experiment_folder_id) > 0
+        self.plot_filename_prefix = f"{self.plot_filename_prefix_parent}/{experiment_folder_id}/"
         print("\n")
         print("Visualizing")
 
         # preparing filesystem
         if save_figs or save_extra_figs:
+            Path(self.plot_filename_prefix_parent).mkdir(exist_ok=True)
             Path(self.plot_filename_prefix).mkdir(exist_ok=True)
 
         # settings
         self.minimization: bool = self.experiment.get("minimization", True)
         cutoff_percentile: float = self.experiment["cutoff_percentile"]
         cutoff_percentile_start: float = self.experiment.get("cutoff_percentile_start", 0.01)
         cutoff_type: str = self.experiment.get("cutoff_type", "fevals")
@@ -225,15 +229,15 @@
                     else:
                         raise ValueError(f"Invalid {x_type=}")
 
                     # create the figure and plots
                     fig, axs = plt.subplots(
                         nrows=len(plot_y_value_types),
                         ncols=1,
-                        figsize=(9, 3.4 * len(plot_y_value_types)),
+                        figsize=(8, 3.4 * len(plot_y_value_types)),
                         sharex=True,
                         dpi=300,
                     )
                     if not hasattr(
                         axs, "__len__"
                     ):  # if there is just one subplot, wrap it in a list so it can be passed to the plot functions
                         axs = [axs]
@@ -621,15 +625,15 @@
         if baseline_curve is not None:
             if y_type == "baseline":
                 ax.axhline(0, label="baseline trajectory", color="black", ls="--")
             elif y_type == "normalized" or y_type == "baseline":
                 baseline = baseline_curve.get_curve(x_axis_range, x_type)
                 if y_type == "normalized":
                     baseline = normalize(baseline)
-                ax.plot(x_axis_range, baseline, label="baseline curve", color="black", ls="--")
+                ax.plot(x_axis_range, baseline, label="Calculated baseline", color="black", ls="--")
 
         # plot additional baselines if provided
         baselines_extra_curves = list()
         for baseline_extra in baselines_extra:
             curve = baseline_extra.get_curve(x_axis_range, x_type)
             if y_type == "normalized":
                 curve = normalize(curve)
@@ -855,15 +859,15 @@
 
         Args:
             ax: the axis to plot on.
             aggregation_data: the aggregated data from the various searchspaces.
             plot_settings: dictionary of additional plot settings.
         """
         # plot the random baseline and absolute optimum
-        ax.axhline(0, label="Random search", c="black", ls=":")
+        ax.axhline(0, label="Calculated baseline", c="black", ls=":")
         ax.axhline(1, label="Absolute optimum", c="black", ls="-.")
 
         # get the relative aggregated performance for each strategy
         confidence_level: float = plot_settings.get("confidence_level", 0.95)
         (
             strategies_performance,
             strategies_lower_err,
@@ -896,41 +900,46 @@
                     strategy_upper_err[:real_stopping_point_index],
                     alpha=0.15,
                     antialiased=True,
                     color=color,
                 )
                 if (
                     real_stopping_point_index < time_range.shape[0]
-                    and real_stopping_point_index < len(strategies_lower_err) - 1
+                    and real_stopping_point_index < len(strategy_lower_err) - 1
                 ):
                     ax.fill_between(
                         time_range[real_stopping_point_index:],
-                        strategies_lower_err[real_stopping_point_index:],
-                        strategies_upper_err[real_stopping_point_index:],
+                        strategy_lower_err[real_stopping_point_index:],
+                        strategy_upper_err[real_stopping_point_index:],
                         alpha=0.15,
                         antialiased=True,
                         color=color,
                         ls="dashed",
                     )
 
             # plot the curve
             ax.plot(
                 time_range[:real_stopping_point_index],
                 strategy_performance[:real_stopping_point_index],
                 color=color,
                 label=displayname,
             )
-            if real_stopping_point_index < time_range.shape[0]:
+            if (
+                real_stopping_point_index < time_range.shape[0]
+                and real_stopping_point_index < len(strategy_performance) - 1
+            ):
                 ax.plot(
                     time_range[real_stopping_point_index:],
                     strategy_performance[real_stopping_point_index:],
                     color=color,
                     ls="dashed",
                 )
-            print(f" | performance of {displayname}: {round(np.mean(strategy_performance), 3)}")
+            performance_score = round(np.mean(strategy_performance), 3)
+            performance_score_std = round(np.std(strategy_performance), 3)
+            print(f" | performance of {displayname}: {performance_score} (±{performance_score_std})")
 
         # set the axis
         cutoff_percentile: float = self.experiment.get("cutoff_percentile", 1)
         cutoff_percentile_start: float = self.experiment.get("cutoff_percentile_start", 0.01)
         ax.set_xlabel(
             f"{self.x_metric_displayname['aggregate_time']} ({cutoff_percentile_start*100}% to {cutoff_percentile*100}%)",  # noqa: E501
             fontsize="large",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Test kernel to run integration tests."""
 
 #!/usr/bin/env python
 import sys
-from collections import OrderedDict
 
 import numpy
 
 import kernel_tuner
 from kernel_tuner.file_utils import store_metadata_file, store_output_file
 
 file_path_prefix = "../../../../cached_data_used"
@@ -27,21 +26,21 @@
     output_image = numpy.zeros(size).astype(numpy.float32)
     input_image = numpy.random.randn(input_size).astype(numpy.float32)
     filter_weights = numpy.random.randn(filter_width * filter_height).astype(numpy.float32)
 
     cmem_args = {"d_filter": filter_weights}
     args = [output_image, input_image, filter_weights]
 
-    metrics = OrderedDict()
+    metrics = dict()
     metrics["GFLOP/s"] = lambda p: (image_width * image_height * filter_width * filter_height * 2 / 1e9) / (
         p["time"] / 1e3
     )
 
     # setup tunable parameters
-    tune_params = OrderedDict()
+    tune_params = dict()
     tune_params["block_size_x"] = [1, 2, 4, 8, 16, 32, 48, 64, 96, 112, 128]
     tune_params["block_size_y"] = [1, 2, 4, 8, 16, 32]
     tune_params["filter_height"] = [filter_height]
     tune_params["filter_width"] = [filter_width]
     tune_params["read_only"] = [0, 1]
     tune_params["tile_size_x"] = [1, 2, 3, 4, 5, 6, 7, 8]
     tune_params["tile_size_y"] = [1, 2, 3, 4, 5, 6, 7, 8]
```

### Comparing `autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/mockfiles/test.json` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,94 @@
-00000000: 7b0a 2020 2276 6572 7369 6f6e 223a 2022  {.  "version": "
-00000010: 302e 312e 3222 2c0a 2020 226e 616d 6522  0.1.2",.  "name"
-00000020: 3a20 224d 6f63 6b20 7275 6e20 7465 7374  : "Mock run test
-00000030: 222c 0a20 2022 666f 6c64 6572 5f69 6422  ",.  "folder_id"
-00000040: 3a20 2274 6573 745f 7275 6e5f 6578 7065  : "test_run_expe
-00000050: 7269 6d65 6e74 222c 0a20 2022 6b65 726e  riment",.  "kern
-00000060: 656c 735f 7061 7468 223a 2022 2e2e 2f6d  els_path": "../m
-00000070: 6f63 6b66 696c 6573 222c 0a20 2022 6272  ockfiles",.  "br
-00000080: 7574 6566 6f72 6365 645f 6361 6368 6573  uteforced_caches
-00000090: 5f70 6174 6822 3a20 222e 2e2f 2e2e 2f2e  _path": "../../.
-000000a0: 2e2f 2e2e 2f63 6163 6865 645f 6461 7461  ./../cached_data
-000000b0: 5f75 7365 642f 6361 6368 6566 696c 6573  _used/cachefiles
-000000c0: 222c 0a20 2022 7669 7375 616c 697a 6174  ",.  "visualizat
-000000d0: 696f 6e5f 6361 6368 6573 5f70 6174 6822  ion_caches_path"
-000000e0: 3a20 222e 2e2f 2e2e 2f2e 2e2f 2e2e 2f63  : "../../../../c
-000000f0: 6163 6865 645f 6461 7461 5f75 7365 642f  ached_data_used/
-00000100: 7669 7375 616c 697a 6174 696f 6e73 222c  visualizations",
-00000110: 0a20 2022 6b65 726e 656c 7322 3a20 5b0a  .  "kernels": [.
-00000120: 2020 2020 226d 6f63 6b74 6573 745f 6b65      "mocktest_ke
-00000130: 726e 656c 5f63 6f6e 766f 6c75 7469 6f6e  rnel_convolution
-00000140: 220a 2020 5d2c 0a20 2022 4750 5573 223a  ".  ],.  "GPUs":
-00000150: 205b 0a20 2020 2022 6d6f 636b 5f47 5055   [.    "mock_GPU
-00000160: 220a 2020 5d2c 0a20 2022 6d69 6e69 6d69  ".  ],.  "minimi
-00000170: 7a61 7469 6f6e 223a 2074 7275 652c 0a20  zation": true,. 
-00000180: 2022 7265 736f 6c75 7469 6f6e 223a 2031   "resolution": 1
-00000190: 6533 2c0a 2020 2263 7574 6f66 665f 7065  e3,.  "cutoff_pe
-000001a0: 7263 656e 7469 6c65 223a 2030 2e39 392c  rcentile": 0.99,
-000001b0: 0a20 2022 6375 746f 6666 5f70 6572 6365  .  "cutoff_perce
-000001c0: 6e74 696c 655f 7374 6172 7422 3a20 302e  ntile_start": 0.
-000001d0: 372c 0a20 2022 6f62 6a65 6374 6976 655f  7,.  "objective_
-000001e0: 7469 6d65 5f6b 6579 7322 3a20 5b0a 2020  time_keys": [.  
-000001f0: 2020 2263 6f6d 7069 6c61 7469 6f6e 222c    "compilation",
-00000200: 0a20 2020 2022 6265 6e63 686d 6172 6b22  .    "benchmark"
-00000210: 2c0a 2020 2020 2266 7261 6d65 776f 726b  ,.    "framework
-00000220: 222c 0a20 2020 2022 7365 6172 6368 5f61  ",.    "search_a
-00000230: 6c67 6f72 6974 686d 222c 0a20 2020 2022  lgorithm",.    "
-00000240: 7661 6c69 6461 7469 6f6e 220a 2020 5d2c  validation".  ],
-00000250: 0a20 2022 6f62 6a65 6374 6976 655f 7065  .  "objective_pe
-00000260: 7266 6f72 6d61 6e63 655f 6b65 7973 223a  rformance_keys":
-00000270: 205b 0a20 2020 2022 7469 6d65 220a 2020   [.    "time".  
-00000280: 5d2c 0a20 2022 6375 746f 6666 5f74 7970  ],.  "cutoff_typ
-00000290: 6522 3a20 2266 6576 616c 7322 2c0a 2020  e": "fevals",.  
-000002a0: 2270 6c6f 7422 3a20 7b0a 2020 2020 2270  "plot": {.    "p
-000002b0: 6c6f 745f 785f 7661 6c75 655f 7479 7065  lot_x_value_type
-000002c0: 7322 3a20 5b0a 2020 2020 2020 2266 6576  s": [.      "fev
-000002d0: 616c 7322 2c0a 2020 2020 2020 2274 696d  als",.      "tim
-000002e0: 6522 2c0a 2020 2020 2020 2261 6767 7265  e",.      "aggre
-000002f0: 6761 7465 6422 0a20 2020 205d 2c0a 2020  gated".    ],.  
-00000300: 2020 2270 6c6f 745f 795f 7661 6c75 655f    "plot_y_value_
-00000310: 7479 7065 7322 3a20 5b0a 2020 2020 2020  types": [.      
-00000320: 226e 6f72 6d61 6c69 7a65 6422 2c0a 2020  "normalized",.  
-00000330: 2020 2020 2262 6173 656c 696e 6522 0a20      "baseline". 
-00000340: 2020 205d 2c0a 2020 2020 2263 6f6e 6669     ],.    "confi
-00000350: 6465 6e63 655f 6c65 7665 6c22 3a20 302e  dence_level": 0.
-00000360: 3935 2c0a 2020 2020 2263 6f6d 7061 7265  95,.    "compare
-00000370: 5f62 6173 656c 696e 6573 223a 2074 7275  _baselines": tru
-00000380: 652c 0a20 2020 2022 636f 6d70 6172 655f  e,.    "compare_
-00000390: 7370 6c69 745f 7469 6d65 7322 3a20 7472  split_times": tr
-000003a0: 7565 0a20 207d 2c0a 2020 2273 7472 6174  ue.  },.  "strat
-000003b0: 6567 795f 6465 6661 756c 7473 223a 207b  egy_defaults": {
-000003c0: 0a20 2020 2022 7265 7065 6174 7322 3a20  .    "repeats": 
-000003d0: 3130 2c0a 2020 2020 226d 696e 696d 756d  10,.    "minimum
-000003e0: 5f6e 756d 6265 725f 6f66 5f65 7661 6c75  _number_of_evalu
-000003f0: 6174 696f 6e73 223a 2032 302c 0a20 2020  ations": 20,.   
-00000400: 2022 7374 6f63 6861 7374 6963 223a 2074   "stochastic": t
-00000410: 7275 652c 0a20 2020 2022 7265 636f 7264  rue,.    "record
-00000420: 5f64 6174 6122 3a20 5b0a 2020 2020 2020  _data": [.      
-00000430: 2274 696d 6522 2c0a 2020 2020 2020 2247  "time",.      "G
-00000440: 464c 4f50 2f73 220a 2020 2020 5d0a 2020  FLOP/s".    ].  
-00000450: 7d2c 0a20 2022 7374 7261 7465 6769 6573  },.  "strategies
-00000460: 223a 205b 0a20 2020 207b 0a20 2020 2020  ": [.    {.     
-00000470: 2022 6e61 6d65 223a 2022 7261 6e64 6f6d   "name": "random
-00000480: 5f73 616d 706c 655f 3130 5f69 7465 7222  _sample_10_iter"
-00000490: 2c0a 2020 2020 2020 2273 7472 6174 6567  ,.      "strateg
-000004a0: 7922 3a20 2272 616e 646f 6d5f 7361 6d70  y": "random_samp
-000004b0: 6c65 222c 0a20 2020 2020 2022 6469 7370  le",.      "disp
-000004c0: 6c61 795f 6e61 6d65 223a 2022 5261 6e64  lay_name": "Rand
-000004d0: 6f6d 2073 616d 706c 696e 6720 3130 2069  om sampling 10 i
-000004e0: 7465 7273 222c 0a20 2020 2020 2022 7265  ters",.      "re
-000004f0: 7065 6174 7322 3a20 330a 2020 2020 7d0a  peats": 3.    }.
-00000500: 2020 5d0a 7d                               ].}
+00000000: 7b0a 2020 2020 2276 6572 7369 6f6e 223a  {.    "version":
+00000010: 2022 302e 312e 3222 2c0a 2020 2020 226e   "0.1.2",.    "n
+00000020: 616d 6522 3a20 224d 6f63 6b20 7275 6e20  ame": "Mock run 
+00000030: 7465 7374 222c 0a20 2020 2022 666f 6c64  test",.    "fold
+00000040: 6572 5f69 6422 3a20 2274 6573 745f 7275  er_id": "test_ru
+00000050: 6e5f 6578 7065 7269 6d65 6e74 222c 0a20  n_experiment",. 
+00000060: 2020 2022 6b65 726e 656c 735f 7061 7468     "kernels_path
+00000070: 223a 2022 2e2e 2f6d 6f63 6b66 696c 6573  ": "../mockfiles
+00000080: 222c 0a20 2020 2022 6272 7574 6566 6f72  ",.    "brutefor
+00000090: 6365 645f 6361 6368 6573 5f70 6174 6822  ced_caches_path"
+000000a0: 3a20 222e 2e2f 2e2e 2f2e 2e2f 2e2e 2f63  : "../../../../c
+000000b0: 6163 6865 645f 6461 7461 5f75 7365 642f  ached_data_used/
+000000c0: 6361 6368 6566 696c 6573 222c 0a20 2020  cachefiles",.   
+000000d0: 2022 7669 7375 616c 697a 6174 696f 6e5f   "visualization_
+000000e0: 6361 6368 6573 5f70 6174 6822 3a20 222e  caches_path": ".
+000000f0: 2e2f 2e2e 2f2e 2e2f 2e2e 2f63 6163 6865  ./../../../cache
+00000100: 645f 6461 7461 5f75 7365 642f 7669 7375  d_data_used/visu
+00000110: 616c 697a 6174 696f 6e73 222c 0a20 2020  alizations",.   
+00000120: 2022 6b65 726e 656c 7322 3a20 5b0a 2020   "kernels": [.  
+00000130: 2020 2020 2020 226d 6f63 6b74 6573 745f        "mocktest_
+00000140: 6b65 726e 656c 5f63 6f6e 766f 6c75 7469  kernel_convoluti
+00000150: 6f6e 220a 2020 2020 5d2c 0a20 2020 2022  on".    ],.    "
+00000160: 4750 5573 223a 205b 0a20 2020 2020 2020  GPUs": [.       
+00000170: 2022 6d6f 636b 5f47 5055 220a 2020 2020   "mock_GPU".    
+00000180: 5d2c 0a20 2020 2022 6d69 6e69 6d69 7a61  ],.    "minimiza
+00000190: 7469 6f6e 223a 2074 7275 652c 0a20 2020  tion": true,.   
+000001a0: 2022 7265 736f 6c75 7469 6f6e 223a 2031   "resolution": 1
+000001b0: 6533 2c0a 2020 2020 2263 7574 6f66 665f  e3,.    "cutoff_
+000001c0: 7065 7263 656e 7469 6c65 223a 2030 2e39  percentile": 0.9
+000001d0: 392c 0a20 2020 2022 6375 746f 6666 5f70  9,.    "cutoff_p
+000001e0: 6572 6365 6e74 696c 655f 7374 6172 7422  ercentile_start"
+000001f0: 3a20 302e 372c 0a20 2020 2022 6f62 6a65  : 0.7,.    "obje
+00000200: 6374 6976 655f 7469 6d65 5f6b 6579 7322  ctive_time_keys"
+00000210: 3a20 5b0a 2020 2020 2020 2020 2263 6f6d  : [.        "com
+00000220: 7069 6c61 7469 6f6e 222c 0a20 2020 2020  pilation",.     
+00000230: 2020 2022 6265 6e63 686d 6172 6b22 2c0a     "benchmark",.
+00000240: 2020 2020 2020 2020 2266 7261 6d65 776f          "framewo
+00000250: 726b 222c 0a20 2020 2020 2020 2022 7365  rk",.        "se
+00000260: 6172 6368 5f61 6c67 6f72 6974 686d 222c  arch_algorithm",
+00000270: 0a20 2020 2020 2020 2022 7661 6c69 6461  .        "valida
+00000280: 7469 6f6e 220a 2020 2020 5d2c 0a20 2020  tion".    ],.   
+00000290: 2022 6f62 6a65 6374 6976 655f 7065 7266   "objective_perf
+000002a0: 6f72 6d61 6e63 655f 6b65 7973 223a 205b  ormance_keys": [
+000002b0: 0a20 2020 2020 2020 2022 7469 6d65 220a  .        "time".
+000002c0: 2020 2020 5d2c 0a20 2020 2022 6375 746f      ],.    "cuto
+000002d0: 6666 5f74 7970 6522 3a20 2266 6576 616c  ff_type": "feval
+000002e0: 7322 2c0a 2020 2020 2270 6c6f 7422 3a20  s",.    "plot": 
+000002f0: 7b0a 2020 2020 2020 2020 2270 6c6f 745f  {.        "plot_
+00000300: 785f 7661 6c75 655f 7479 7065 7322 3a20  x_value_types": 
+00000310: 5b0a 2020 2020 2020 2020 2020 2020 2266  [.            "f
+00000320: 6576 616c 7322 2c0a 2020 2020 2020 2020  evals",.        
+00000330: 2020 2020 2274 696d 6522 2c0a 2020 2020      "time",.    
+00000340: 2020 2020 2020 2020 2261 6767 7265 6761          "aggrega
+00000350: 7465 6422 0a20 2020 2020 2020 205d 2c0a  ted".        ],.
+00000360: 2020 2020 2020 2020 2270 6c6f 745f 795f          "plot_y_
+00000370: 7661 6c75 655f 7479 7065 7322 3a20 5b0a  value_types": [.
+00000380: 2020 2020 2020 2020 2020 2020 226e 6f72              "nor
+00000390: 6d61 6c69 7a65 6422 2c0a 2020 2020 2020  malized",.      
+000003a0: 2020 2020 2020 2262 6173 656c 696e 6522        "baseline"
+000003b0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+000003c0: 2020 2020 2263 6f6e 6669 6465 6e63 655f      "confidence_
+000003d0: 6c65 7665 6c22 3a20 302e 3935 2c0a 2020  level": 0.95,.  
+000003e0: 2020 2020 2020 2263 6f6d 7061 7265 5f62        "compare_b
+000003f0: 6173 656c 696e 6573 223a 2074 7275 652c  aselines": true,
+00000400: 0a20 2020 2020 2020 2022 636f 6d70 6172  .        "compar
+00000410: 655f 7370 6c69 745f 7469 6d65 7322 3a20  e_split_times": 
+00000420: 7472 7565 0a20 2020 207d 2c0a 2020 2020  true.    },.    
+00000430: 2273 7472 6174 6567 795f 6465 6661 756c  "strategy_defaul
+00000440: 7473 223a 207b 0a20 2020 2020 2020 2022  ts": {.        "
+00000450: 7265 7065 6174 7322 3a20 3130 2c0a 2020  repeats": 10,.  
+00000460: 2020 2020 2020 226d 696e 696d 756d 5f6e        "minimum_n
+00000470: 756d 6265 725f 6f66 5f65 7661 6c75 6174  umber_of_evaluat
+00000480: 696f 6e73 223a 2032 302c 0a20 2020 2020  ions": 20,.     
+00000490: 2020 2022 7374 6f63 6861 7374 6963 223a     "stochastic":
+000004a0: 2074 7275 652c 0a20 2020 2020 2020 2022   true,.        "
+000004b0: 7265 636f 7264 5f64 6174 6122 3a20 5b0a  record_data": [.
+000004c0: 2020 2020 2020 2020 2020 2020 2274 696d              "tim
+000004d0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+000004e0: 2247 464c 4f50 2f73 220a 2020 2020 2020  "GFLOP/s".      
+000004f0: 2020 5d0a 2020 2020 7d2c 0a20 2020 2022    ].    },.    "
+00000500: 7374 7261 7465 6769 6573 223a 205b 0a20  strategies": [. 
+00000510: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000520: 2020 2020 2022 6e61 6d65 223a 2022 7261       "name": "ra
+00000530: 6e64 6f6d 5f73 616d 706c 655f 3130 5f69  ndom_sample_10_i
+00000540: 7465 7222 2c0a 2020 2020 2020 2020 2020  ter",.          
+00000550: 2020 2273 7472 6174 6567 7922 3a20 2272    "strategy": "r
+00000560: 616e 646f 6d5f 7361 6d70 6c65 222c 0a20  andom_sample",. 
+00000570: 2020 2020 2020 2020 2020 2022 6469 7370             "disp
+00000580: 6c61 795f 6e61 6d65 223a 2022 5261 6e64  lay_name": "Rand
+00000590: 6f6d 2073 616d 706c 696e 6720 3130 2069  om sampling 10 i
+000005a0: 7465 7273 222c 0a20 2020 2020 2020 2020  ters",.         
+000005b0: 2020 2022 7265 7065 6174 7322 3a20 330a     "repeats": 3.
+000005c0: 2020 2020 2020 2020 7d0a 2020 2020 5d0a          }.    ].
+000005d0: 7d                                       }
```

### Comparing `autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8631944444444444%*

 * *Differences: {"'GPUs'": "['mock_GPU']",*

 * * "'kernels'": "['mocktest_kernel_convolution']",*

 * * "'kernels_path'": "'../mockfiles'",*

 * * "'name'": "'Test import runs'",*

 * * "'strategies'": "{0: {'name': 'ktt_profile_searcher', 'strategy': 'profile_searcher', "*

 * *                 "'display_name': 'KTT Profile Searcher', delete: ['repeats']}}",*

 * * "'strategy_defaults'": "{'repeats': 2, 'iterations': 32}"}*

```diff
@@ -1,22 +1,22 @@
 {
     "GPUs": [
-        "RTX_2080_Ti"
+        "mock_GPU"
     ],
     "bruteforced_caches_path": "../../../../cached_data_used/cachefiles",
     "cutoff_percentile": 0.99,
     "cutoff_percentile_start": 0.7,
     "cutoff_type": "fevals",
     "folder_id": "test_output_file_writer",
     "kernels": [
-        "convolution"
+        "mocktest_kernel_convolution"
     ],
-    "kernels_path": "cached_data_used/bogus_kernels_path",
+    "kernels_path": "../mockfiles",
     "minimization": true,
-    "name": "Test output file writer",
+    "name": "Test import runs",
     "objective_performance_keys": [
         "time"
     ],
     "objective_time_keys": [
         "compilation",
         "benchmark",
         "framework",
@@ -34,25 +34,25 @@
             "normalized",
             "baseline"
         ]
     },
     "resolution": 1000.0,
     "strategies": [
         {
-            "display_name": "Random sampling 100 iters",
-            "name": "random_sample_100_iter",
-            "repeats": 5,
-            "strategy": "random_sample"
+            "display_name": "KTT Profile Searcher",
+            "name": "ktt_profile_searcher",
+            "strategy": "profile_searcher"
         }
     ],
     "strategy_defaults": {
+        "iterations": 32,
         "minimum_number_of_evaluations": 20,
         "record_data": [
             "time",
             "GFLOP/s"
         ],
-        "repeats": 100,
+        "repeats": 2,
         "stochastic": true
     },
     "version": "0.1.2",
     "visualization_caches_path": "../../../../cached_data_used/visualizations"
 }
```

### Comparing `autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/test_run_experiment.py` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/test_run_experiment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Integration test for running and fetching an experiment from cache."""
 
 import json
 from importlib.resources import files
 from pathlib import Path
+from shutil import copyfile
 
 import numpy as np
 import pytest
 from jsonschema import validate
 
 from autotuning_methodology.curves import StochasticOptimizationAlgorithm
 from autotuning_methodology.experiments import (
@@ -25,16 +26,25 @@
 mockfiles_path_source = mockfiles_path_root / "mock_gpu.json"
 mockfiles_path = mockfiles_path_root
 experiment_filepath_test = mockfiles_path / "test.json"
 assert experiment_filepath_test.exists()
 kernel_id = "mocktest_kernel_convolution"
 cached_visualization_path = package_path / Path(f"cached_data_used/visualizations/test_run_experiment/{kernel_id}")
 cached_visualization_file = cached_visualization_path / "mock_GPU_random_sample_10_iter.npz"
+cached_visualization_imported_path = package_path / Path(
+    f"cached_data_used/visualizations/test_output_file_writer/{kernel_id}"
+)
+cached_visualization_imported_file = cached_visualization_imported_path / "mock_GPU_ktt_profile_searcher.npz"
 normal_cachefiles_path = package_path / Path(f"cached_data_used/cachefiles/{kernel_id}")
 normal_cachefile_destination = normal_cachefiles_path / "mock_gpu.json"
+experiment_import_filepath_test = mockfiles_path / "test_import_runs.json"
+assert experiment_import_filepath_test.exists()
+import_runs_source_path = mockfiles_path / "import_runs"
+import_runs_path = package_path / Path("cached_data_used/import_runs")
+import_runs_filepaths: list[Path] = list()
 
 
 def _remove_dir(path: Path):
     """Utility function for removing a directory and the contained files."""
     assert path.exists()
     for sub in path.iterdir():
         sub.unlink()
@@ -46,24 +56,42 @@
     assert mockfiles_path_source.exists()
     normal_cachefiles_path.mkdir(parents=True, exist_ok=True)
     assert normal_cachefiles_path.exists()
     normal_cachefile_destination.write_text(mockfiles_path_source.read_text())
     assert normal_cachefile_destination.exists()
     # cached_visualization_path.mkdir(parents=True, exist_ok=True)
     # assert cached_visualization_path.exists()
+    # copy the import run test files to the import run folder
+    assert import_runs_source_path.exists()
+    import_runs_path.mkdir(parents=True, exist_ok=True)
+    assert import_runs_path.exists()
+    for import_run_file in import_runs_source_path.iterdir():
+        if not import_run_file.is_file():
+            continue
+        assert import_run_file.exists()
+        destination = Path(import_runs_path / import_run_file.name).resolve()
+        import_runs_filepaths.append(Path(copyfile(str(import_run_file), str(destination))))
+        assert destination == import_runs_filepaths[-1].resolve()
+        assert destination.exists() and destination.is_file()
 
 
 def teardown_module():
     """Teardown of the tests, removes files where necessary."""
     if normal_cachefile_destination.exists():
         normal_cachefile_destination.unlink()
     _remove_dir(normal_cachefiles_path)
     if cached_visualization_file.exists():
         cached_visualization_file.unlink()
     _remove_dir(cached_visualization_path)
+    if cached_visualization_imported_file.exists():
+        cached_visualization_imported_file.unlink()
+    _remove_dir(cached_visualization_imported_path)
+    # delete the import run test files from the import run folder
+    for import_run_file in import_runs_filepaths:
+        import_run_file.unlink()
 
 
 def test_CLI_input():
     """Test bad and good CLI inputs."""
     # improper input 1
     with pytest.raises(SystemExit) as e:
         dummy_args = ["-dummy_arg=option"]
@@ -116,14 +144,25 @@
     assert normal_cachefile_destination.exists()
     assert cached_visualization_path.exists()
     assert cached_visualization_file.exists()
     (experiment, strategies, results_descriptions) = execute_experiment(str(experiment_filepath_test), profiling=False)
     validate_experiment_results(experiment, strategies, results_descriptions)
 
 
+def test_import_run_experiment():
+    """Import runs from an experiment."""
+    assert import_runs_path.exists()
+    (experiment, strategies, results_descriptions) = execute_experiment(
+        str(experiment_import_filepath_test), profiling=False
+    )
+    assert cached_visualization_imported_path.exists()
+    assert cached_visualization_imported_file.exists()
+    validate_experiment_results(experiment, strategies, results_descriptions)
+
+
 @pytest.mark.usefixtures("test_run_experiment")
 def test_curve_instance():
     """Test a Curve instance."""
     # setup the test
     (experiment, strategies, results_descriptions) = execute_experiment(str(experiment_filepath_test), profiling=False)
     kernel_name = experiment["kernels"][0]
     gpu_name = experiment["GPUs"][0]
```

### Comparing `autotuning_methodology-0.1.0b1/tests/autotuning_methodology/integration/test_visualization.py` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/test_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     normal_cachefiles_path,
 )
 
 from autotuning_methodology.visualize_experiments import Visualize
 
 # setup file paths
 experiment_title = f"{kernel_id}_on_mock_GPU"
-plot_path = Path("generated_plots")
+plot_path = Path("generated_plots/test_run_experiment")
 plot_path_fevals = plot_path / f"{experiment_title}_fevals.png"
 plot_path_time = plot_path / f"{experiment_title}_time.png"
 plot_path_aggregated = plot_path / "aggregated.png"
 plot_path_split_times_fevals = plot_path / f"{experiment_title}_split_times_fevals.png"
 plot_path_split_times_time = plot_path / f"{experiment_title}_split_times_time.png"
 plot_path_split_times_bar = plot_path / f"{experiment_title}_split_times_bar.png"
 plot_path_baselines_comparison = plot_path / f"{experiment_title}_baselines.png"
@@ -56,14 +56,15 @@
     _remove_dir(normal_cachefiles_path)
     if cached_visualization_file.exists():
         cached_visualization_file.unlink()
     _remove_dir(cached_visualization_path)
     if plot_path.exists():
         for plot_filepath in plot_filepaths:
             plot_filepath.unlink(missing_ok=True)
+        plot_path.rmdir()
 
 
 def test_visualize_experiment():
     """Visualize a dummy experiment."""
     assert normal_cachefile_destination.exists()
     if cached_visualization_file.exists():
         cached_visualization_file.unlink()
```

### Comparing `autotuning_methodology-0.1.0b1/tests/autotuning_methodology/release/test_toml_file.py` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/release/test_toml_file.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/tests/autotuning_methodology/unit/test_curves.py` & `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/unit/test_curves.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-0.1.0b1/PKG-INFO` & `autotuning_methodology-1.0.0b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: autotuning_methodology
-Version: 0.1.0b1
+Version: 1.0.0b1
 Summary: Software package easing implementation of the guidelines of the 2023 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'.
 Keywords: autotuning,auto-tuning,methodology,scientific
 Author-email: Floris-Jan Willemsen <fjwillemsen97@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy >= 1.22.4
+Requires-Dist: scipy >= 1.10.1
 Requires-Dist: scikit-learn >= 1.0.2
 Requires-Dist: matplotlib >= 3.7.1
 Requires-Dist: yappi >= 1.4.0
 Requires-Dist: progressbar2 >= 4.2.0
 Requires-Dist: jsonschema >= 4.17.3
 Requires-Dist: nonconformist >= 2.1.0
-Requires-Dist: kernel_tuner >= 0.4.5
+Requires-Dist: kernel_tuner >= 1.0.0b5
 Requires-Dist: pylint >=2.14.4 ; extra == "dev"
 Requires-Dist: black >= 23.3.0 ; extra == "dev"
 Requires-Dist: sphinx >= 6.2.1 ; extra == "docs"
 Requires-Dist: sphinx_rtd_theme >= 1.2.0 ; extra == "docs"
 Requires-Dist: sphinx-pyproject >= 0.1.0 ; extra == "docs"
 Requires-Dist: ruff >= 0.0.263 ; extra == "test"
 Requires-Dist: pep440 >= 0.1.2 ; extra == "test"
@@ -37,70 +40,85 @@
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 
 # Autotuning Methodology Software Package
 
 <p align="center">
-  <img width="25%" src="https://fjwillemsen.github.io/autotuning_methodology/_static/logo_autotuning_methodology.svg" />
+  <img width="25%" src="https://autotuningassociation.github.io/autotuning_methodology/_static/logo_autotuning_methodology.svg" />
 </p>
 
-[![Build Status](https://github.com/fjwillemsen/autotuning_methodology/actions/workflows/build-test-python-package.yml/badge.svg)](https://github.com/fjwillemsen/autotuning_methodology/actions/workflows/build-test-python-package.yml)
-[![Docs](https://img.shields.io/github/actions/workflow/status/fjwillemsen/autotuning_methodology/publish-documentation.yml?label=docs)](https://fjwillemsen.github.io/autotuning_methodology/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 ![PyPI - License](https://img.shields.io/pypi/l/autotuning_methodology)
+[![Build Status](https://github.com/autotuningassociation/autotuning_methodology/actions/workflows/build-test-python-package.yml/badge.svg)](https://github.com/autotuningassociation/autotuning_methodology/actions/workflows/build-test-python-package.yml)
+[![Docs](https://img.shields.io/github/actions/workflow/status/autotuningassociation/autotuning_methodology/publish-documentation.yml?label=docs)](https://autotuningassociation.github.io/autotuning_methodology/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/autotuning_methodology)](https://pypi.org/project/autotuning_methodology/)
+![PyPI - Status](https://img.shields.io/pypi/status/autotuning_methodology)
 
-
+ 
 This repository contains the software package accompanying the paper "A Methodology for Comparing Auto-Tuning Optimization Algorithms". 
 It makes the guidelines in the methodology easy to apply: simply specify the  `.json` file, run `autotuning_visualize [path_to_json]` and wait for the results!
 
 ## Installation
-The package can be installed by cloning this repository and running `pip install .`. Python >= 3.9 is supported.  
+The package can be installed with `pip install autotuning_methodology`. 
+Alternatively, it can be installed by cloning this repository and running `pip install .` in the root of the cloned project. 
+Python >= 3.9 is supported. 
 
 ## Notable features
 - Official software by the authors of the methodology-defining paper. 
 - Supports [BAT benchmark suite](https://github.com/NTNU-HPC-Lab/BAT) and [Kernel Tuner](https://github.com/KernelTuner/kernel_tuner).
 - Split executer and visualizer to allow running the algorithms on a cluster and visualize locally. 
 - Caching built-in to avoid duplicate executions.  
 - Planned support for T1 input and T4 output files.
-- Notebook / interactive window mode; in this case, plots are shown in the notebook / window instead of written to a folder. 
+- Notebook / interactive window mode; if enabled, plots are shown in the notebook / window instead of written to a folder. 
 
 <img width="674" alt="example run in interactive window" src="https://user-images.githubusercontent.com/6725103/232880006-70a05b0e-a4e4-4cc7-bea9-473959c474c2.png">
 <img width="483" alt="example run in interactive window 2" src="https://user-images.githubusercontent.com/6725103/232881244-d432ea8e-801a-44b1-9acb-b98cc1b740ac.png">
 
 ## Usage
 
 ### Entry points
 There are two entry points defined: `autotuning_experiment` and `autotuning_visualize`. Both take one argument: the path to an experiment file (see below). 
 
 ### Input files
 To get started, all you need is an experiments file. This is a `json` file that describes the details of your comparison: which algorithms to use, which programs to tune on which devices, the graphs to output and so on. 
-You can find the API and an example `experiments.json` in the [documentation](). 
+You can find the API and an example `experiments.json` in the [documentation](https://autotuningassociation.github.io/autotuning_methodology/modules.html). 
 
 ### File references
 As we are dealing with input and output files, file references matter. 
 When calling the entrypoints, we are already providing the path to an experiments file. 
 File references in experiments files are relative to the location of the experiment file itself. 
 File references in tuning scripts are relative to the location of the tuning script itself. Tuning scripts need to have the global literals `file_path_results` and `file_path_metadata` for this package to know where to get the results. 
 Plots outputted by this package are placed in a folder called `generated_plots` relative to the current working directory. 
 
 
+## Pipeline
+The below schematics show the pipeline implemented by this tool as described in the paper. 
+
+<!-- <img width="100%" alt="flowchart performance curve generation" src="https://autotuningassociation.github.io/autotuning_methodology/_static/flowchart_performance_curve_generation.svg"> -->
+![flowchart performance curve generation](docs/source/flowchart_performance_curve_generation.png)
+The first flowchart shows the tranformation of raw, stochastic optimization algorithm data to a performance curve. 
+
+<!-- <img width="100%" alt="flowchart output generation" src="docs/source/flowchart_output_generation.svg"> -->
+![flowchart output generation](docs/source/flowchart_output_generation.png)
+The second flowchart shows the adaption of performance curves of various optimization algorithms and search spaces to the desired output.
+
+
 ## Contributing
 
 ### Setup
 If you're looking to contribute to this package: welcome!
 Start out by installing with `pip install -e .[dev]` (this installs the package in editable mode alongside the development dependencies). 
 During development, unit and integration tests can be ran with `pytest`. 
 [Black](https://pypi.org/project/black/) is used as a formatter, and [Ruff](https://pypi.org/project/ruff/) is used as a linter to check the formatting, import sorting et cetera. 
 When using Visual Studio Code, use the `settings.json` found in `.vscode` to automatically have the correct linting, formatting and sorting during development. 
 In addition, install the extensions recommended by us by searching for `@recommended:workspace` in the extensions tab for a better development experience. 
 
 ### Documentation
-The documentation can be found [here](https://fjwillemsen.github.io/autotuning_methodology/). 
+The documentation can be found [here](https://autotuningassociation.github.io/autotuning_methodology/). 
 Locally, the documentation can be build with `make clean html` from the `docs` folder, but the package must have been installed in editable mode with `pip install -e .`. 
 Upon pushing to main or publishing a version, this documentation will be built and published to the GitHub Pages. 
 The Docstring format used is Google. Type hints are to be included in the function signature and therefor omitted from the docstring. In Visual Studio Code, the `autoDocstring` extension can be used to automatically infer docstrings. When referrring to functions and parameters in the docstring outside of their definition, use double backquotes to be compatible with both MarkDown and ReStructuredText, e.g.: *"skip_draws_check: skips checking that each value in ``draws`` is in the ``dist``."*.
 
 ### Tests
 Before contributing a pull request, please run `nox` and ensure it has no errors. This will test against all Python versions explicitely supported by this package, and will check whether the correct formatting has been applied.
 Upon submitting a pull request or pushing to main, these same checks will be ran remotely via GitHub Actions.
```

