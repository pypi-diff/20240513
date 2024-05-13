# Comparing `tmp/geoips-1.12.2.tar.gz` & `tmp/geoips-1.12.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoips-1.12.2.tar", max compression
+gzip compressed data, was "geoips-1.12.2a0.tar", max compression
```

## Comparing `geoips-1.12.2.tar` & `geoips-1.12.2a0.tar`

### file list

```diff
@@ -1,546 +1,540 @@
--rw-r--r--   0        0        0     1589 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/bandit.yaml
--rw-r--r--   0        0        0     1606 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/black.yaml
--rw-r--r--   0        0        0     3534 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/build-html-docs.yaml
--rw-r--r--   0        0        0     3456 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/build-pdf-docs.yaml
--rw-r--r--   0        0        0     5464 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/deploy-ghpages-docs.yaml
--rw-r--r--   0        0        0     1744 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/flake8.yaml
--rw-r--r--   0        0        0      819 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/package-and-publish.yaml
--rw-r--r--   0        0        0     4892 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/pytest-short.yaml
--rw-r--r--   0        0        0     2041 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/release-note-update.yaml
--rw-r--r--   0        0        0     3173 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows/test-interfaces.yaml
--rw-r--r--   0        0        0     1083 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows_archived/docker-build-test-push.yaml
--rw-r--r--   0        0        0      559 2024-05-13 19:37:27.234266 geoips-1.12.2/.github/workflows_archived/validate-pull-request.yaml
--rw-r--r--   0        0        0     1968 2024-05-13 19:37:27.234266 geoips-1.12.2/LICENSE
--rw-r--r--   0        0        0     3226 2024-05-13 19:37:27.234266 geoips-1.12.2/README.md
--rw-r--r--   0        0        0    12093 2024-05-13 19:37:27.238266 geoips-1.12.2/docs/source/_templates/conf_PKG.py
--rw-r--r--   0        0        0     1141 2024-05-13 19:37:27.354267 geoips-1.12.2/docs/source/yaml/20200918.195020.goes-16.Visible_latitude_longitude.tc2020al20teddy.nc.yaml
--rw-r--r--   0        0        0     1131 2024-05-13 19:37:27.354267 geoips-1.12.2/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1147 2024-05-13 19:37:27.354267 geoips-1.12.2/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_WV_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1188 2024-05-13 19:37:27.354267 geoips-1.12.2/docs/source/yaml/abi_test.yaml
--rw-r--r--   0        0        0     1596 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/__init__.py
--rw-r--r--   0        0        0      755 2024-05-13 19:37:31.914289 geoips-1.12.2/geoips/_version.py
--rw-r--r--   0        0        0     9234 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/cli.py
--rw-r--r--   0        0        0      684 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/commandline/__init__.py
--rw-r--r--   0        0        0    39617 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/commandline/args.py
--rw-r--r--   0        0        0     2199 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/commandline/create_sector_image.py
--rw-r--r--   0        0        0     3111 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/commandline/list_available_plugins.py
--rw-r--r--   0        0        0     9585 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/commandline/log_setup.py
--rw-r--r--   0        0        0     4002 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/commandline/run_procflow.py
--rw-r--r--   0        0        0     1118 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/commandline/update_tc_tracks_database.py
--rw-r--r--   0        0        0    41424 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/create_plugin_registries.py
--rw-r--r--   0        0        0      691 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/data_manipulations/__init__.py
--rw-r--r--   0        0        0     2128 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/data_manipulations/conversions.py
--rw-r--r--   0        0        0    17008 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/data_manipulations/corrections.py
--rw-r--r--   0        0        0     1654 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/data_manipulations/info.py
--rw-r--r--   0        0        0     9017 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/data_manipulations/merge.py
--rw-r--r--   0        0        0      669 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/dev/__init__.py
--rw-r--r--   0        0        0    17285 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/dev/output_config.py
--rw-r--r--   0        0        0     9114 2024-05-13 19:37:27.354267 geoips-1.12.2/geoips/dev/product.py
--rw-r--r--   0        0        0     1015 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/errors.py
--rw-r--r--   0        0        0      682 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/filenames/__init__.py
--rwxr-xr-x   0        0        0     9580 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/filenames/base_paths.py
--rw-r--r--   0        0        0     2907 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/filenames/duplicate_files.py
--rw-r--r--   0        0        0    13701 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/geoips_utils.py
--rw-r--r--   0        0        0      677 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/image_utils/__init__.py
--rw-r--r--   0        0        0    11301 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/image_utils/colormap_utils.py
--rw-r--r--   0        0        0    21379 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/image_utils/maps.py
--rw-r--r--   0        0        0    25463 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/image_utils/mpl_utils.py
--rw-r--r--   0        0        0     4855 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/__init__.py
--rw-r--r--   0        0        0    34873 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/base.py
--rw-r--r--   0        0        0      689 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/__init__.py
--rw-r--r--   0        0        0     1874 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/algorithms.py
--rw-r--r--   0        0        0     1459 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/colormappers.py
--rw-r--r--   0        0        0     1437 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/coverage_checkers.py
--rw-r--r--   0        0        0     2753 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/filename_formatters.py
--rw-r--r--   0        0        0     1173 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/interpolators.py
--rw-r--r--   0        0        0    44070 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/output_checkers.py
--rw-r--r--   0        0        0     3334 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/output_formatters.py
--rw-r--r--   0        0        0     1424 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/procflows.py
--rw-r--r--   0        0        0     1173 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/readers.py
--rw-r--r--   0        0        0     1353 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/sector_adjusters.py
--rw-r--r--   0        0        0     1292 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/sector_metadata_generators.py
--rw-r--r--   0        0        0     1324 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/sector_spec_generators.py
--rw-r--r--   0        0        0     1013 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/module_based/title_formatters.py
--rw-r--r--   0        0        0      687 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/yaml_based/__init__.py
--rw-r--r--   0        0        0      935 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/yaml_based/feature_annotators.py
--rw-r--r--   0        0        0      941 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/yaml_based/gridline_annotators.py
--rw-r--r--   0        0        0      933 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/yaml_based/product_defaults.py
--rw-r--r--   0        0        0     8403 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/yaml_based/products.py
--rw-r--r--   0        0        0     3870 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/interfaces/yaml_based/sectors.py
--rw-r--r--   0        0        0     9534 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugin_registry.py
--rw-r--r--   0        0        0      673 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/__init__.py
--rw-r--r--   0        0        0      688 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/__init__.py
--rw-r--r--   0        0        0     2154 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/RGB_Default.py
--rw-r--r--   0        0        0      683 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/__init__.py
--rw-r--r--   0        0        0      689 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/__init__.py
--rw-r--r--   0        0        0     2123 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/pmw_37pct.py
--rw-r--r--   0        0        0     2081 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/pmw_89pct.py
--rw-r--r--   0        0        0     2581 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/pmw_color37.py
--rw-r--r--   0        0        0     2621 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/pmw_color89.py
--rw-r--r--   0        0        0      687 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/sfc_winds/__init__.py
--rw-r--r--   0        0        0     4150 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/sfc_winds/windbarbs.py
--rw-r--r--   0        0        0     6821 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/single_channel.py
--rw-r--r--   0        0        0     3505 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/visir/Night_Vis.py
--rw-r--r--   0        0        0     2414 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/visir/Night_Vis_GeoIPS1.py
--rw-r--r--   0        0        0     3665 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/visir/Night_Vis_IR.py
--rw-r--r--   0        0        0     3463 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/visir/Night_Vis_IR_GeoIPS1.py
--rw-r--r--   0        0        0      688 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/algorithms/visir/__init__.py
--rw-r--r--   0        0        0      685 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/__init__.py
--rw-r--r--   0        0        0     1581 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/cmap_rgb.py
--rw-r--r--   0        0        0     5880 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/matplotlib_linear_norm.py
--rw-r--r--   0        0        0      723 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/__init__.py
--rw-r--r--   0        0        0     3353 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_150H.py
--rw-r--r--   0        0        0     3429 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H.py
--rw-r--r--   0        0        0     3428 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Legacy.py
--rw-r--r--   0        0        0     3390 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Physical.py
--rw-r--r--   0        0        0     2984 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_37pct.py
--rw-r--r--   0        0        0     3327 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H.py
--rw-r--r--   0        0        0     3326 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89HW.py
--rw-r--r--   0        0        0     3365 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Legacy.py
--rw-r--r--   0        0        0     3356 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Physical.py
--rw-r--r--   0        0        0     3488 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89pct.py
--rw-r--r--   0        0        0     3069 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_Rain.py
--rw-r--r--   0        0        0      706 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/tpw/__init__.py
--rw-r--r--   0        0        0     2518 2024-05-13 19:37:27.358266 geoips-1.12.2/geoips/plugins/modules/colormappers/tpw/tpw_pwat.py
--rw-r--r--   0        0        0     3811 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/colormappers/visir/IR_BD.py
--rw-r--r--   0        0        0     3592 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/colormappers/visir/Infrared.py
--rw-r--r--   0        0        0     3559 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/colormappers/visir/WV.py
--rw-r--r--   0        0        0      698 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/colormappers/visir/__init__.py
--rw-r--r--   0        0        0      695 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/colormappers/winds/__init__.py
--rw-r--r--   0        0        0     3806 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/colormappers/winds/wind_radii_transitions.py
--rw-r--r--   0        0        0      690 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/coverage_checkers/__init__.py
--rw-r--r--   0        0        0     4301 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/coverage_checkers/center_radius.py
--rw-r--r--   0        0        0     2565 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/coverage_checkers/center_radius_rgba.py
--rw-r--r--   0        0        0     1545 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/coverage_checkers/masked_arrays.py
--rw-r--r--   0        0        0     1527 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/coverage_checkers/numpy_arrays_nan.py
--rw-r--r--   0        0        0     1540 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/coverage_checkers/rgba.py
--rw-r--r--   0        0        0     1761 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/coverage_checkers/windbarbs.py
--rw-r--r--   0        0        0      692 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/__init__.py
--rw-r--r--   0        0        0     1976 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/basic_fname.py
--rw-r--r--   0        0        0     7481 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/geoips_fname.py
--rw-r--r--   0        0        0     4224 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/geoips_netcdf_fname.py
--rw-r--r--   0        0        0     2052 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/geotiff_fname.py
--rw-r--r--   0        0        0     3107 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/metadata_default_fname.py
--rw-r--r--   0        0        0     2951 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/tc_clean_fname.py
--rw-r--r--   0        0        0    14732 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/tc_fname.py
--rw-r--r--   0        0        0     1972 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/text_winds_day_fname.py
--rw-r--r--   0        0        0     3811 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/text_winds_full_fname.py
--rw-r--r--   0        0        0     4231 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/text_winds_tc_fname.py
--rw-r--r--   0        0        0      706 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/utils/__init__.py
--rw-r--r--   0        0        0     8530 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/filename_formatters/utils/tc_file_naming.py
--rw-r--r--   0        0        0      686 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/__init__.py
--rw-r--r--   0        0        0      697 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/pyresample_wrappers/__init__.py
--rw-r--r--   0        0        0     4539 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_gauss.py
--rw-r--r--   0        0        0     4979 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_nearest.py
--rw-r--r--   0        0        0      698 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/scipy_wrappers/__init__.py
--rw-r--r--   0        0        0     2972 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/scipy_wrappers/interp_grid.py
--rw-r--r--   0        0        0      692 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/utils/__init__.py
--rwxr-xr-x   0        0        0    39645 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/utils/boxdefinitions.py
--rw-r--r--   0        0        0     5166 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/utils/interp_pyresample.py
--rw-r--r--   0        0        0     5440 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/interpolators/utils/interp_scipy.py
--rw-r--r--   0        0        0     5679 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_checkers/geotiff.py
--rw-r--r--   0        0        0     8331 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_checkers/image.py
--rw-r--r--   0        0        0    11161 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_checkers/netcdf.py
--rw-r--r--   0        0        0     5952 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_checkers/text.py
--rw-r--r--   0        0        0      689 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/__init__.py
--rw-r--r--   0        0        0     3986 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/full_disk_image.py
--rw-r--r--   0        0        0     3988 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/geotiff_standard.py
--rw-r--r--   0        0        0     2027 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/histogram_netcdf.py
--rw-r--r--   0        0        0     6729 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/imagery_annotated.py
--rw-r--r--   0        0        0     2899 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/imagery_clean.py
--rw-r--r--   0        0        0    12540 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/imagery_windbarbs.py
--rw-r--r--   0        0        0     1630 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/imagery_windbarbs_clean.py
--rw-r--r--   0        0        0     5804 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/metadata_default.py
--rw-r--r--   0        0        0     7877 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/metadata_tc.py
--rw-r--r--   0        0        0     1409 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/netcdf_geoips.py
--rw-r--r--   0        0        0     4888 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/netcdf_xarray.py
--rw-r--r--   0        0        0     7831 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/text_winds.py
--rw-r--r--   0        0        0     2870 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/output_formatters/unprojected_image.py
--rw-r--r--   0        0        0      681 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/procflows/__init__.py
--rw-r--r--   0        0        0    83615 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/procflows/config_based.py
--rw-r--r--   0        0        0    90032 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/procflows/single_source.py
--rw-r--r--   0        0        0      680 2024-05-13 19:37:27.362266 geoips-1.12.2/geoips/plugins/modules/readers/__init__.py
--rw-r--r--   0        0        0     6447 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/abi_l2_netcdf.py
--rw-r--r--   0        0        0    42928 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/abi_netcdf.py
--rw-r--r--   0        0        0    64102 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/ahi_hsd.py
--rw-r--r--   0        0        0    30640 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/ami_netcdf.py
--rw-r--r--   0        0        0    15706 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/amsr2_netcdf.py
--rw-r--r--   0        0        0     4922 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/amsr2_remss_winds_netcdf.py
--rw-r--r--   0        0        0    10502 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/amsub_hdf.py
--rw-r--r--   0        0        0    19598 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/amsub_mirs.py
--rw-r--r--   0        0        0    15023 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/ascat_uhr_netcdf.py
--rw-r--r--   0        0        0    11734 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/atms_hdf5.py
--rw-r--r--   0        0        0    10268 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/ewsg_netcdf.py
--rw-r--r--   0        0        0     3105 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/geoips_netcdf.py
--rw-r--r--   0        0        0     9760 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/gmi_hdf5.py
--rw-r--r--   0        0        0     7409 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/imerg_hdf5.py
--rw-r--r--   0        0        0     4466 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/mimic_netcdf.py
--rw-r--r--   0        0        0    34756 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/modis_hdf4.py
--rw-r--r--   0        0        0     7592 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/saphir_hdf5.py
--rw-r--r--   0        0        0    11762 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/sar_winds_netcdf.py
--rw-r--r--   0        0        0    10864 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/scat_knmi_winds_netcdf.py
--rw-r--r--   0        0        0    10367 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/scat_noaa_winds_netcdf.py
--rwxr-xr-x   0        0        0    30729 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/seviri_hrit.py
--rw-r--r--   0        0        0     5176 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/sfc_winds_text.py
--rw-r--r--   0        0        0     4813 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/smap_remss_winds_netcdf.py
--rw-r--r--   0        0        0    10319 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/smos_winds_netcdf.py
--rw-r--r--   0        0        0    23045 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/ssmi_binary.py
--rw-r--r--   0        0        0    48302 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/ssmis_binary.py
--rw-r--r--   0        0        0      685 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/utils/__init__.py
--rw-r--r--   0        0        0    25000 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/utils/geostationary_geolocation.py
--rw-r--r--   0        0        0    39669 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/utils/hrit_reader.py
--rw-r--r--   0        0        0     5143 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/utils/remss_reader.py
--rwxr-xr-x   0        0        0    30523 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/viirs_netcdf.py
--rw-r--r--   0        0        0     7650 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/wfabba_ascii.py
--rw-r--r--   0        0        0    20795 2024-05-13 19:37:27.366267 geoips-1.12.2/geoips/plugins/modules/readers/windsat_idr37_binary.py
--rw-r--r--   0        0        0     4256 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/readers/windsat_remss_winds_netcdf.py
--rw-r--r--   0        0        0      690 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/sector_metadata_generators/__init__.py
--rw-r--r--   0        0        0    18201 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/sector_metadata_generators/bdeck_parser.py
--rw-r--r--   0        0        0     6041 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/sector_metadata_generators/tc_sector_file_parser.py
--rw-r--r--   0        0        0      695 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/sector_spec_generators/__init__.py
--rw-r--r--   0        0        0     3073 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/sector_spec_generators/center_coordinates.py
--rw-r--r--   0        0        0      689 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/title_formatters/__init__.py
--rw-r--r--   0        0        0     2009 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/title_formatters/static_standard.py
--rw-r--r--   0        0        0     2830 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/title_formatters/tc_copyright.py
--rw-r--r--   0        0        0     3061 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/modules/title_formatters/tc_standard.py
--rwxr-xr-x   0        0        0     2977 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/txt/ascii_palettes/tpw_cimss.txt
--rw-r--r--   0        0        0     3353 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/txt/ascii_palettes/tpw_purple.txt
--rwxr-xr-x   0        0        0     1083 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/txt/ascii_palettes/tpw_pwat.txt
--rw-r--r--   0        0        0      459 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/feature_annotators/default.yaml
--rw-r--r--   0        0        0      553 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/feature_annotators/tc_pmw.yaml
--rw-r--r--   0        0        0      478 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/feature_annotators/tc_visir.yaml
--rw-r--r--   0        0        0      551 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/feature_annotators/tc_windspeed.yaml
--rw-r--r--   0        0        0      437 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/gridline_annotators/default.yaml
--rw-r--r--   0        0        0      438 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/gridline_annotators/north_pole.yaml
--rw-r--r--   0        0        0      473 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/gridline_annotators/tc_0p25degree.yaml
--rw-r--r--   0        0        0      463 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/gridline_annotators/tc_pmw.yaml
--rw-r--r--   0        0        0      460 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/gridline_annotators/tc_visir.yaml
--rw-r--r--   0        0        0      474 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/gridline_annotators/tc_visir_3200km.yaml
--rw-r--r--   0        0        0      460 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/gridline_annotators/tc_windspeed.yaml
--rw-r--r--   0        0        0      457 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/RGB-Default.yaml
--rw-r--r--   0        0        0     1033 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/Uncorrected-Channel.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/150H.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/150V.yaml
--rw-r--r--   0        0        0      550 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/150VNearest.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/157V.yaml
--rw-r--r--   0        0        0      550 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/157VNearest.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/165H.yaml
--rw-r--r--   0        0        0      550 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/165HNearest.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/166H.yaml
--rw-r--r--   0        0        0      550 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/166HNearest.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/166V.yaml
--rw-r--r--   0        0        0      550 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/166VNearest.yaml
--rw-r--r--   0        0        0      559 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-1H.yaml
--rw-r--r--   0        0        0      554 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-1HNearest.yaml
--rw-r--r--   0        0        0      559 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-3H.yaml
--rw-r--r--   0        0        0      554 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-3HNearest.yaml
--rw-r--r--   0        0        0      559 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-7H.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183H.yaml
--rw-r--r--   0        0        0      550 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183HNearest.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/190V.yaml
--rw-r--r--   0        0        0      550 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/190VNearest.yaml
--rw-r--r--   0        0        0      552 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/19H.yaml
--rw-r--r--   0        0        0      547 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/19HNearest.yaml
--rw-r--r--   0        0        0      552 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/19V.yaml
--rw-r--r--   0        0        0      543 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/19VNearest.yaml
--rw-r--r--   0        0        0      573 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H-Legacy.yaml
--rw-r--r--   0        0        0      568 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H-LegacyNearest.yaml
--rw-r--r--   0        0        0      579 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H-Physical.yaml
--rw-r--r--   0        0        0      574 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H-PhysicalNearest.yaml
--rw-r--r--   0        0        0      552 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H.yaml
--rw-r--r--   0        0        0      547 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37HNearest.yaml
--rw-r--r--   0        0        0      552 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37V.yaml
--rw-r--r--   0        0        0      547 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37VNearest.yaml
--rw-r--r--   0        0        0      553 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37pct.yaml
--rw-r--r--   0        0        0      548 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37pctNearest.yaml
--rw-r--r--   0        0        0      467 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/color37.yaml
--rw-r--r--   0        0        0      462 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/color37Nearest.yaml
--rw-r--r--   0        0        0      573 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H-Legacy.yaml
--rw-r--r--   0        0        0      568 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H-LegacyNearest.yaml
--rw-r--r--   0        0        0      579 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H-Physical.yaml
--rw-r--r--   0        0        0      574 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H-PhysicalNearest.yaml
--rw-r--r--   0        0        0      552 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H.yaml
--rw-r--r--   0        0        0      547 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89HNearest.yaml
--rw-r--r--   0        0        0      563 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89HW.yaml
--rw-r--r--   0        0        0      558 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89HWNearest.yaml
--rw-r--r--   0        0        0      552 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89V.yaml
--rw-r--r--   0        0        0      547 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89VNearest.yaml
--rw-r--r--   0        0        0      557 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89pct.yaml
--rw-r--r--   0        0        0      552 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89pctNearest.yaml
--rw-r--r--   0        0        0      467 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/color89.yaml
--rw-r--r--   0        0        0      462 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/color89Nearest.yaml
--rw-r--r--   0        0        0      560 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/rain_rate/Rain.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/rain_rate/RainNearest.yaml
--rw-r--r--   0        0        0      290 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/sectored.yaml
--rw-r--r--   0        0        0     1103 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/incident-angle.yaml
--rw-r--r--   0        0        0      945 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/nrcs.yaml
--rw-r--r--   0        0        0      604 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/wind-ambiguities.yaml
--rw-r--r--   0        0        0      590 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/windbarbs.yaml
--rw-r--r--   0        0        0      613 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/windspeed.yaml
--rw-r--r--   0        0        0      786 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/tpw/TPW-CIMSS.yaml
--rw-r--r--   0        0        0      791 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/tpw/TPW-PURPLE.yaml
--rw-r--r--   0        0        0      519 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/tpw/TPW-PWAT.yaml
--rw-r--r--   0        0        0      267 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/unmodified.yaml
--rw-r--r--   0        0        0      296 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/unsectored.yaml
--rw-r--r--   0        0        0      598 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/IR-BD.yaml
--rw-r--r--   0        0        0      722 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Infrared-Gray.yaml
--rw-r--r--   0        0        0      607 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Infrared.yaml
--rw-r--r--   0        0        0      662 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Night-Vis-GeoIPS1.yaml
--rw-r--r--   0        0        0      759 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Night-Vis.yaml
--rw-r--r--   0        0        0     1053 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Visible.yaml
--rw-r--r--   0        0        0      599 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/WV-Lower.yaml
--rw-r--r--   0        0        0      599 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/WV-Upper.yaml
--rw-r--r--   0        0        0      587 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/WV.yaml
--rw-r--r--   0        0        0     2429 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/products/abi.yaml
--rw-r--r--   0        0        0     3827 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/products/ahi.yaml
--rw-r--r--   0        0        0     2481 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/products/ami.yaml
--rw-r--r--   0        0        0     4992 2024-05-13 19:37:27.370267 geoips-1.12.2/geoips/plugins/yaml/products/amsr-e.yaml
--rw-r--r--   0        0        0     7947 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/amsr2.yaml
--rw-r--r--   0        0        0     2844 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/amsu-b.yaml
--rw-r--r--   0        0        0     2244 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/ascat.yaml
--rw-r--r--   0        0        0     2280 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/ascatuhr.yaml
--rw-r--r--   0        0        0     1709 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/atms.yaml
--rw-r--r--   0        0        0    10713 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/gmi.yaml
--rw-r--r--   0        0        0     1070 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/gvar.yaml
--rw-r--r--   0        0        0     1167 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/hscat.yaml
--rw-r--r--   0        0        0      587 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/imerg.yaml
--rw-r--r--   0        0        0     2928 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/mhs.yaml
--rw-r--r--   0        0        0      824 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/mimic.yaml
--rw-r--r--   0        0        0     2186 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/modis.yaml
--rw-r--r--   0        0        0     1040 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/oscat.yaml
--rw-r--r--   0        0        0     1330 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/saphir.yaml
--rw-r--r--   0        0        0     1345 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/sar-spd.yaml
--rw-r--r--   0        0        0     2249 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/seviri.yaml
--rw-r--r--   0        0        0      881 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/smap-spd.yaml
--rw-r--r--   0        0        0      881 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/smos-spd.yaml
--rw-r--r--   0        0        0     8612 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/ssmi.yaml
--rw-r--r--   0        0        0    11093 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/ssmis.yaml
--rw-r--r--   0        0        0     8555 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/tmi.yaml
--rw-r--r--   0        0        0     2477 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/viirs.yaml
--rw-r--r--   0        0        0     3935 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/products/windsat.yaml
--rw-r--r--   0        0        0      400 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_1024x1024/tc_1km_1024x1024.yaml
--rw-r--r--   0        0        0      398 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_1024x1024/tc_2km_1024x1024.yaml
--rw-r--r--   0        0        0      398 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_1400x1400/tc_1km_1400x1400.yaml
--rw-r--r--   0        0        0      400 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_1400x1400/tc_2km_1400x1400.yaml
--rw-r--r--   0        0        0      398 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_1600x1600/tc_2km_1600x1600.yaml
--rw-r--r--   0        0        0      398 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_1600x1600/tc_4km_1600x1600.yaml
--rw-r--r--   0        0        0      395 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_256x256/tc_4km_256x256.yaml
--rw-r--r--   0        0        0      390 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_512x512/tc_2km_512x512.yaml
--rw-r--r--   0        0        0      392 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_512x512/tc_4km_512x512.yaml
--rw-r--r--   0        0        0      390 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_800x800/tc_2km_800x800.yaml
--rw-r--r--   0        0        0      390 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_800x800/tc_4km_800x800.yaml
--rw-r--r--   0        0        0      398 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_0p1km_3200x3200.yaml
--rw-r--r--   0        0        0      398 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_1km_2500x2500.yaml
--rw-r--r--   0        0        0      398 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_1km_3200x3200.yaml
--rw-r--r--   0        0        0      391 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_web_2km_template.yaml
--rw-r--r--   0        0        0      338 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_50km_barbs_template.yaml
--rw-r--r--   0        0        0      417 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_high_barbs_template.yaml
--rw-r--r--   0        0        0      341 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_low_barbs_template.yaml
--rw-r--r--   0        0        0      409 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_web_ascatuhr_barbs_template.yaml
--rw-r--r--   0        0        0      397 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_web_halfkm_template.yaml
--rw-r--r--   0        0        0      391 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_web_qkm_template.yaml
--rw-r--r--   0        0        0      340 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/dynamic/tc_web_template.yaml
--rw-r--r--   0        0        0      486 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/abu_dhabi.yaml
--rw-r--r--   0        0        0      454 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/africa.yaml
--rw-r--r--   0        0        0      463 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/african_horn.yaml
--rw-r--r--   0        0        0      463 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/alaska.yaml
--rw-r--r--   0        0        0      448 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/asia.yaml
--rw-r--r--   0        0        0      474 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/australia.yaml
--rw-r--r--   0        0        0      463 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/beijing.yaml
--rw-r--r--   0        0        0      460 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/brazil.yaml
--rw-r--r--   0        0        0      451 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/cairo.yaml
--rw-r--r--   0        0        0      457 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/canada.yaml
--rw-r--r--   0        0        0      454 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/caribbean.yaml
--rw-r--r--   0        0        0      479 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/central_america.yaml
--rw-r--r--   0        0        0      565 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/conus.yaml
--rw-r--r--   0        0        0      443 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/delhi.yaml
--rw-r--r--   0        0        0      474 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/denver.yaml
--rw-r--r--   0        0        0      461 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/e_pacific.yaml
--rw-r--r--   0        0        0      458 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/europe.yaml
--rw-r--r--   0        0        0      531 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/ewsg.yaml
--rw-r--r--   0        0        0      451 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/france.yaml
--rw-r--r--   0        0        0      562 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/geokompsat.yaml
--rw-r--r--   0        0        0      516 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/global.yaml
--rw-r--r--   0        0        0      554 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/goes_east.yaml
--rw-r--r--   0        0        0      555 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/goes_west.yaml
--rw-r--r--   0        0        0      549 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/himawari.yaml
--rw-r--r--   0        0        0      461 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/indian_basin.yaml
--rw-r--r--   0        0        0      526 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/japan.yaml
--rw-r--r--   0        0        0      474 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/mediterranean.yaml
--rw-r--r--   0        0        0      477 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/melbourne.yaml
--rw-r--r--   0        0        0      491 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/meteosat_africa.yaml
--rw-r--r--   0        0        0      491 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/meteosat_europe.yaml
--rw-r--r--   0        0        0      518 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/meteosat_indian_ocean.yaml
--rw-r--r--   0        0        0      472 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/mexico_city.yaml
--rw-r--r--   0        0        0      472 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/middle_east.yaml
--rw-r--r--   0        0        0      466 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/ne_asia.yaml
--rw-r--r--   0        0        0      457 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/north_pole.yaml
--rw-r--r--   0        0        0      451 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/paris.yaml
--rw-r--r--   0        0        0      496 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/rio_de_janeiro.yaml
--rw-r--r--   0        0        0      446 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/russia.yaml
--rw-r--r--   0        0        0      491 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/saskatchewan.yaml
--rw-r--r--   0        0        0      463 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/se_asia.yaml
--rw-r--r--   0        0        0      514 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/south_america.yaml
--rw-r--r--   0        0        0      454 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/south_pole.yaml
--rw-r--r--   0        0        0      492 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/vancouver.yaml
--rw-r--r--   0        0        0      457 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/victoria.yaml
--rw-r--r--   0        0        0      462 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/w_atlantic.yaml
--rw-r--r--   0        0        0      456 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/plugins/yaml/sectors/static/w_pacific.yaml
--rw-r--r--   0        0        0      119 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/bases/docstring.yaml
--rw-r--r--   0        0        0      121 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/bases/family.yaml
--rw-r--r--   0        0        0      118 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/bases/interface.yaml
--rw-r--r--   0        0        0       96 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/bases/name.yaml
--rw-r--r--   0        0        0      119 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/bases/product_defaults.yaml
--rw-r--r--   0        0        0      322 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/bases/top.yaml
--rw-r--r--   0        0        0      274 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/bases/valid_identifier.yaml
--rw-r--r--   0        0        0     1215 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/feature_annotators/cartopy.yaml
--rw-r--r--   0        0        0     1811 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/gridline_annotators/cartopy.yaml
--rw-r--r--   0        0        0      209 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/product_defaults/algorithm.yaml
--rw-r--r--   0        0        0      245 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/product_defaults/algorithm_colormapper.yaml
--rw-r--r--   0        0        0      284 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/product_defaults/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      327 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/product_defaults/bases/algorithm.yaml
--rw-r--r--   0        0        0     1364 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/product_defaults/bases/colormapper.yaml
--rw-r--r--   0        0        0      328 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/product_defaults/bases/coverage_checker.yaml
--rw-r--r--   0        0        0      320 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/product_defaults/bases/interpolator.yaml
--rw-r--r--   0        0        0      195 2024-05-13 19:37:27.374266 geoips-1.12.2/geoips/schema/product_defaults/bases/unvalidated.yaml
--rw-r--r--   0        0        0      833 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/bases/windbarb_plotter.yaml
--rw-r--r--   0        0        0      218 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/interpolator.yaml
--rw-r--r--   0        0        0      248 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/interpolator_algorithm.yaml
--rw-r--r--   0        0        0      284 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0      228 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/sectored_xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      640 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/specs/algorithm.yaml
--rw-r--r--   0        0        0      730 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/specs/algorithm_colormapper.yaml
--rw-r--r--   0        0        0      824 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/specs/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      652 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/specs/interpolator.yaml
--rw-r--r--   0        0        0      734 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/specs/interpolator_algorithm.yaml
--rw-r--r--   0        0        0      824 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/specs/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0       98 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/specs/xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      169 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/unmodified.yaml
--rw-r--r--   0        0        0      237 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/unsectored_xarray_dict_area_to_output_format.yaml
--rw-r--r--   0        0        0      232 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/unsectored_xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      210 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/product_defaults/xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      354 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/algorithm.yaml
--rw-r--r--   0        0        0      390 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/algorithm_colormapper.yaml
--rw-r--r--   0        0        0      429 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      634 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/bases/product.yaml
--rw-r--r--   0        0        0      363 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/interpolator.yaml
--rw-r--r--   0        0        0      393 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/interpolator_algorithm.yaml
--rw-r--r--   0        0        0      429 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0      220 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/list.yaml
--rw-r--r--   0        0        0      243 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/sectored_xarray_dict_area_to_output_format.yaml
--rw-r--r--   0        0        0      233 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/sectored_xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      191 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/single.yaml
--rw-r--r--   0        0        0      179 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/unmodified.yaml
--rw-r--r--   0        0        0      247 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/unsectored_xarray_dict_area_to_output_format.yaml
--rw-r--r--   0        0        0      237 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/unsectored_xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      215 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/products/xarray_dict_to_output_format.yaml
--rw-r--r--   0        0        0      369 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/generated.yaml
--rw-r--r--   0        0        0      217 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/metadata_families/atmosriver.yaml
--rw-r--r--   0        0        0      213 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/metadata_families/pyrocb.yaml
--rw-r--r--   0        0        0      316 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/metadata_families/static.yaml
--rw-r--r--   0        0        0      271 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/metadata_families/stitched.yaml
--rw-r--r--   0        0        0      451 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/metadata_families/tc.yaml
--rw-r--r--   0        0        0      244 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/metadata_families/volcano.yaml
--rw-r--r--   0        0        0      770 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/specs/area_definition.yaml
--rw-r--r--   0        0        0      746 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/specs/center.yaml
--rw-r--r--   0        0        0     2016 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/schema/sectors/static.yaml
--rw-r--r--   0        0        0      685 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/sector_utils/__init__.py
--rw-r--r--   0        0        0    11134 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/sector_utils/estimate_area_extent.py
--rw-r--r--   0        0        0    14003 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/sector_utils/overpass_predictor.py
--rw-r--r--   0        0        0     3880 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/sector_utils/projections.py
--rw-r--r--   0        0        0    11052 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/sector_utils/tc_tracks.py
--rw-r--r--   0        0        0    15280 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/sector_utils/tc_tracks_database.py
--rw-r--r--   0        0        0    26958 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/sector_utils/utils.py
--rw-r--r--   0        0        0     6731 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/sector_utils/yaml_utils.py
--rw-r--r--   0        0        0      682 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/utils/__init__.py
--rw-r--r--   0        0        0     5100 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/utils/composite.py
--rw-r--r--   0        0        0     1486 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/utils/context_managers.py
--rw-r--r--   0        0        0     2582 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/utils/decorators.py
--rw-r--r--   0        0        0     3569 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/utils/memusg.py
--rw-r--r--   0        0        0      685 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/xarray_utils/__init__.py
--rw-r--r--   0        0        0    35356 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/xarray_utils/data.py
--rw-r--r--   0        0        0     4759 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/xarray_utils/time.py
--rw-r--r--   0        0        0     1264 2024-05-13 19:37:27.378267 geoips-1.12.2/geoips/xarray_utils/xr_to_dtree.py
--rw-r--r--   0        0        0     6888 2024-05-13 19:37:31.914289 geoips-1.12.2/pyproject.toml
--rw-r--r--   0        0        0     1348 2024-05-13 19:37:27.378267 geoips-1.12.2/setup/download_test_data.py
--rw-r--r--   0        0        0     1184 2024-05-13 19:37:27.426267 geoips-1.12.2/tests/outputs/abi.tc.IR-BD.imagery_annotated/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1190 2024-05-13 19:37:27.430267 geoips-1.12.2/tests/outputs/abi.tc.Infrared.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Infrared_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1188 2024-05-13 19:37:27.442267 geoips-1.12.2/tests/outputs/abi.tc.Visible.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Visible_110kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1245 2024-05-13 19:37:27.518267 geoips-1.12.2/tests/outputs/amsr2.tc.89H-Physical.imagery_annotated/20200518_073601_IO012020_amsr2_gcom-w1_89H-Physical_140kts_100p00_res1p0-cr300.png.yaml
--rw-r--r--   0        0        0     1667 2024-05-13 19:37:27.522267 geoips-1.12.2/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgInfrared-Gray.png.yaml
--rw-r--r--   0        0        0     1661 2024-05-13 19:37:27.530267 geoips-1.12.2/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgVisible.png.yaml
--rw-r--r--   0        0        0     1668 2024-05-13 19:37:27.538267 geoips-1.12.2/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgInfrared-Gray.png.yaml
--rw-r--r--   0        0        0     1662 2024-05-13 19:37:27.546267 geoips-1.12.2/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgVisible.png.yaml
--rw-r--r--   0        0        0     1243 2024-05-13 19:37:27.546267 geoips-1.12.2/tests/outputs/amsr2_ocean.tc.windspeed.imagery_clean/20200518_073601_IO012020_amsr2_gcom-w1_windspeed_140kts_85p45_1p0-clean.png.yaml
--rw-r--r--   0        0        0     1136 2024-05-13 19:37:27.550267 geoips-1.12.2/tests/outputs/amsub_mirs.tc.183-3H.imagery_annotated/20210419_235400_WP022021_amsu-b_metop-a_183-3H_115kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1234 2024-05-13 19:37:27.554268 geoips-1.12.2/tests/outputs/ascat_knmi.tc.windbarbs.imagery_windbarbs_clean/20210421_014248_WP022021_ascat_metop-c_windbarbs_120kts_78p20_0p5-clean.png.yaml
--rw-r--r--   0        0        0     1222 2024-05-13 19:37:27.558267 geoips-1.12.2/tests/outputs/ascat_low_knmi.tc.windbarbs.imagery_windbarbs/20210421_014156_WP022021_ascat_metop-c_windbarbs_120kts_35p17_1p0.png.yaml
--rw-r--r--   0        0        0     1556 2024-05-13 19:37:27.562267 geoips-1.12.2/tests/outputs/ascat_noaa_25km.tc.windbarbs.imagery_windbarbs/20230524_235304_WP022023_ascat_metop-c_windbarbs_135kts_39p90_0p7.png.yaml
--rw-r--r--   0        0        0     1569 2024-05-13 19:37:27.566268 geoips-1.12.2/tests/outputs/ascat_noaa_50km.tc.wind-ambiguities.imagery_windbarbs/20230524_235200_WP022023_ascat_metop-c_wind-ambiguities_135kts_50p08_1p1.png.yaml
--rw-r--r--   0        0        0     1226 2024-05-13 19:37:27.574267 geoips-1.12.2/tests/outputs/ascat_uhr.tc.wind-ambiguities.imagery_windbarbs/20210421_014200_WP022021_ascatuhr_metop-c_wind-ambiguities_120kts_100p00_0p1.png.yaml
--rw-r--r--   0        0        0     1382 2024-05-13 19:37:27.606268 geoips-1.12.2/tests/outputs/gmi.tc.89pct.imagery_clean/20200917_171519_AL202020_gmi_GPM_89pct_115kts_78p16_res1p0-cr300-clean.png.yaml
--rw-r--r--   0        0        0     1211 2024-05-13 19:37:27.610268 geoips-1.12.2/tests/outputs/hy2.tc.windspeed.imagery_annotated/20211202_084039_WP272021_hscat_hy-2b_windspeed_95kts_97p06_1p0.png.yaml
--rw-r--r--   0        0        0     1131 2024-05-13 19:37:27.618268 geoips-1.12.2/tests/outputs/mimic_fine.tc.TPW-PWAT.imagery_annotated/20210419_230000_WP022021_mimic_tpw_TPW-PWAT_115kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     1220 2024-05-13 19:37:27.626268 geoips-1.12.2/tests/outputs/oscat_knmi.tc.windbarbs.imagery_windbarbs/20210209_025351_SH192021_oscat_scatsat-1_windbarbs_135kts_75p10_1p0.png.yaml
--rw-r--r--   0        0        0     1162 2024-05-13 19:37:27.626268 geoips-1.12.2/tests/outputs/saphir.tc.183-3HNearest.imagery_annotated/20210209_003103_SH192021_saphir_meghatropiques_183-3HNearest_135kts_88p76_1p0.png.yaml
--rw-r--r--   0        0        0     1144 2024-05-13 19:37:27.630268 geoips-1.12.2/tests/outputs/sar.tc.nrcs.imagery_annotated/20181025_203206_WP312018_sar-spd_sentinel-1_nrcs_130kts_58p51_res1p0-cr300.png.yaml
--rw-r--r--   0        0        0    54649 2024-05-13 19:37:27.642268 geoips-1.12.2/tests/outputs/smos.tc.sectored.text_winds/smos-spd_surface_winds_esa_smos_tc2020sh16gabekile_202002161242.txt
--rw-r--r--   0        0        0     1222 2024-05-13 19:37:27.642268 geoips-1.12.2/tests/outputs/ssmi.tc.37pct.imagery_clean/20200519_090000_IO012020_ssmi_F15_37pct_110kts_50p65_1p0-clean.png.yaml
--rw-r--r--   0        0        0     1347 2024-05-13 19:37:27.654268 geoips-1.12.2/tests/outputs/viirsday.tc.Night-Vis-IR.imagery_annotated/20210209_074210_SH192021_viirs_noaa-20_Night-Vis-IR_130kts_100p00_1p0.png.yaml
--rw-r--r--   0        0        0     6905 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/commandline/test_log_setup.py
--rw-r--r--   0        0        0      690 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/bad/invalid_interfaces.yaml
--rw-r--r--   0        0        0      677 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/bad/missing_lowest_keys.yaml
--rw-r--r--   0        0        0      662 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/bad/missing_plugin_types.yaml
--rw-r--r--   0        0        0     8382 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/data_fusion.yaml
--rw-r--r--   0        0        0   224173 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/geoips.yaml
--rw-r--r--   0        0        0     8892 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/geoips_clavrx.yaml
--rw-r--r--   0        0        0     3166 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/geoips_plugin_example.yaml
--rw-r--r--   0        0        0     5822 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/overcast_package.yaml
--rw-r--r--   0        0        0     1877 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/recenter_tc.yaml
--rw-r--r--   0        0        0     1997 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/template_basic_plugin.yaml
--rw-r--r--   0        0        0      626 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/template_fusion_plugin.yaml
--rw-r--r--   0        0        0    10936 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugin_registries/test_plugin_registries.py
--rw-r--r--   0        0        0     2815 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugins/modules/output_checkers/test_output_checkers.py
--rw-r--r--   0        0        0     1529 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugins/yaml/sectors/test_sectors.py
--rw-r--r--   0        0        0     1717 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/plugins/yaml/test_all_yaml_plugins.py
--rw-r--r--   0        0        0       21 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/bases/docstring.yaml
--rw-r--r--   0        0        0       91 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/bases/valid_identifier.yaml
--rw-r--r--   0        0        0     2966 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/feature_annotators/cartopy.yaml
--rw-r--r--   0        0        0     1467 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/gridline_annotators/cartopy.yaml
--rw-r--r--   0        0        0     2028 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/algorithm_colormapper.yaml
--rw-r--r--   0        0        0     2855 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      317 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/bases/algorithm.yaml
--rw-r--r--   0        0        0     1346 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/bases/colormapper.yaml
--rw-r--r--   0        0        0      317 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/bases/coverage_checker.yaml
--rw-r--r--   0        0        0      317 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/bases/interpolator.yaml
--rw-r--r--   0        0        0      663 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm.yaml
--rw-r--r--   0        0        0     1502 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0     1798 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/products/bases/product.yaml
--rw-r--r--   0        0        0      385 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/bad/products/single.yaml
--rw-r--r--   0        0        0       46 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/good/bases/valid_identifier.yaml
--rw-r--r--   0        0        0      996 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/good/feature_annotators/cartopy.yaml
--rw-r--r--   0        0        0      288 2024-05-13 19:37:27.666268 geoips-1.12.2/tests/unit_tests/schema/good/gridline_annotators/cartopy.yaml
--rw-r--r--   0        0        0      283 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/product_defaults/algorithm_colormapper.yaml
--rw-r--r--   0        0        0      384 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/product_defaults/algorithm_interpolator_colormapper.yaml
--rw-r--r--   0        0        0      174 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/product_defaults/bases/algorithm.yaml
--rw-r--r--   0        0        0      523 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/product_defaults/bases/colormapper.yaml
--rw-r--r--   0        0        0      174 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/product_defaults/bases/coverage_checker.yaml
--rw-r--r--   0        0        0      174 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/product_defaults/bases/interpolator.yaml
--rw-r--r--   0        0        0      290 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/product_defaults/interpolator_algorithm.yaml
--rw-r--r--   0        0        0      384 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/product_defaults/interpolator_algorithm_colormapper.yaml
--rw-r--r--   0        0        0      529 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/products/bases/product.yaml
--rw-r--r--   0        0        0     1182 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/products/single.yaml
--rw-r--r--   0        0        0      460 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/good/sectors/static.yaml
--rw-r--r--   0        0        0     3650 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/schema/test_yaml_schema.py
--rw-r--r--   0        0        0     2094 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/utils/context_managers.py
--rw-r--r--   0        0        0     4560 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/xarray_utils/data.py
--rw-r--r--   0        0        0     1867 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests/xarray_utils/test_dtree.py
--rw-r--r--   0        0        0     2828 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/unit_tests_long/plugins/modules/readers/test_readers.py
--rwxr-xr-x   0        0        0     9980 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/utils/test_interfaces.py
--rw-r--r--   0        0        0     1263 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/yaml_configs/abi_test.yaml
--rw-r--r--   0        0        0     1500 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/yaml_configs/abi_test_low_memory.yaml
--rw-r--r--   0        0        0     4833 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/yaml_configs/amsr2_no_compare_full.yaml
--rw-r--r--   0        0        0     1731 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/yaml_configs/amsr2_test.yaml
--rw-r--r--   0        0        0     1813 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/yaml_configs/amsr2_test_low_memory.yaml
--rw-r--r--   0        0        0     1485 2024-05-13 19:37:27.670268 geoips-1.12.2/tests/yaml_configs/amsr2_test_no_compare.yaml
--rw-r--r--   0        0        0     5454 1970-01-01 00:00:00.000000 geoips-1.12.2/PKG-INFO
+-rw-r--r--   0        0        0     1558 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/bandit.yaml
+-rw-r--r--   0        0        0     1613 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/black.yaml
+-rw-r--r--   0        0        0     2992 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/build-html-docs.yaml
+-rw-r--r--   0        0        0     2304 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/changelog-templates-unchanged.yaml
+-rw-r--r--   0        0        0     1775 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/flake8.yaml
+-rw-r--r--   0        0        0      814 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/package-and-publish.yaml
+-rw-r--r--   0        0        0     4598 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/pytest-short.yaml
+-rw-r--r--   0        0        0     2036 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/release-note-update.yaml
+-rw-r--r--   0        0        0     3131 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows/test-interfaces.yaml
+-rw-r--r--   0        0        0     1083 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows_archived/docker-build-test-push.yaml
+-rw-r--r--   0        0        0      559 2024-04-23 23:27:47.593713 geoips-1.12.2a0/.github/workflows_archived/validate-pull-request.yaml
+-rw-r--r--   0        0        0     1968 2024-04-23 23:27:47.593713 geoips-1.12.2a0/LICENSE
+-rw-r--r--   0        0        0     3226 2024-04-23 23:27:47.593713 geoips-1.12.2a0/README.md
+-rw-r--r--   0        0        0    12048 2024-04-23 23:27:47.601713 geoips-1.12.2a0/docs/source/_templates/conf_PKG.py
+-rw-r--r--   0        0        0     1141 2024-04-23 23:27:47.713714 geoips-1.12.2a0/docs/source/yaml/20200918.195020.goes-16.Visible_latitude_longitude.tc2020al20teddy.nc.yaml
+-rw-r--r--   0        0        0     1131 2024-04-23 23:27:47.713714 geoips-1.12.2a0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1147 2024-04-23 23:27:47.713714 geoips-1.12.2a0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_WV_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1188 2024-04-23 23:27:47.713714 geoips-1.12.2a0/docs/source/yaml/abi_test.yaml
+-rw-r--r--   0        0        0     1596 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/__init__.py
+-rw-r--r--   0        0        0      761 2024-04-23 23:27:59.649849 geoips-1.12.2a0/geoips/_version.py
+-rw-r--r--   0        0        0     9234 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/cli.py
+-rw-r--r--   0        0        0      684 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/__init__.py
+-rw-r--r--   0        0        0    39007 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/args.py
+-rw-r--r--   0        0        0     2199 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/create_sector_image.py
+-rw-r--r--   0        0        0     3111 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/list_available_plugins.py
+-rw-r--r--   0        0        0     9271 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/log_setup.py
+-rw-r--r--   0        0        0     4007 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/run_procflow.py
+-rwxr-xr-x   0        0        0     8764 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/test_interfaces.py
+-rw-r--r--   0        0        0     1118 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/commandline/update_tc_tracks_database.py
+-rw-r--r--   0        0        0    40772 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/create_plugin_registries.py
+-rw-r--r--   0        0        0      691 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/__init__.py
+-rw-r--r--   0        0        0     2128 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/conversions.py
+-rw-r--r--   0        0        0    17008 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/corrections.py
+-rw-r--r--   0        0        0     1654 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/info.py
+-rw-r--r--   0        0        0     9017 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/data_manipulations/merge.py
+-rw-r--r--   0        0        0      669 2024-04-23 23:27:47.713714 geoips-1.12.2a0/geoips/dev/__init__.py
+-rw-r--r--   0        0        0    17285 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/dev/output_config.py
+-rw-r--r--   0        0        0     9114 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/dev/product.py
+-rw-r--r--   0        0        0     1129 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/errors.py
+-rw-r--r--   0        0        0      682 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/filenames/__init__.py
+-rwxr-xr-x   0        0        0    10039 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/filenames/base_paths.py
+-rw-r--r--   0        0        0     2907 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/filenames/duplicate_files.py
+-rw-r--r--   0        0        0    15385 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/geoips_utils.py
+-rw-r--r--   0        0        0      677 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/image_utils/__init__.py
+-rw-r--r--   0        0        0    11301 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/image_utils/colormap_utils.py
+-rw-r--r--   0        0        0    21379 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/image_utils/maps.py
+-rw-r--r--   0        0        0    25463 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/image_utils/mpl_utils.py
+-rw-r--r--   0        0        0     3787 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/__init__.py
+-rw-r--r--   0        0        0    35733 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/base.py
+-rw-r--r--   0        0        0      689 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/algorithms.py
+-rw-r--r--   0        0        0     1459 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/colormappers.py
+-rw-r--r--   0        0        0     1437 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/coverage_checkers.py
+-rw-r--r--   0        0        0     2753 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/filename_formatters.py
+-rw-r--r--   0        0        0     1173 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/interpolators.py
+-rw-r--r--   0        0        0    43982 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/output_checkers.py
+-rw-r--r--   0        0        0     3334 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/output_formatters.py
+-rw-r--r--   0        0        0     1424 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/procflows.py
+-rw-r--r--   0        0        0     1173 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/readers.py
+-rw-r--r--   0        0        0     1353 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/sector_adjusters.py
+-rw-r--r--   0        0        0     1292 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/sector_metadata_generators.py
+-rw-r--r--   0        0        0     1324 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/sector_spec_generators.py
+-rw-r--r--   0        0        0     1013 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/module_based/title_formatters.py
+-rw-r--r--   0        0        0      687 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/feature_annotators.py
+-rw-r--r--   0        0        0      941 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/gridline_annotators.py
+-rw-r--r--   0        0        0      933 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/product_defaults.py
+-rw-r--r--   0        0        0     7564 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/products.py
+-rw-r--r--   0        0        0     3746 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/interfaces/yaml_based/sectors.py
+-rw-r--r--   0        0        0     9534 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugin_registry.py
+-rw-r--r--   0        0        0      673 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/__init__.py
+-rw-r--r--   0        0        0      683 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/__init__.py
+-rw-r--r--   0        0        0     2123 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_37pct.py
+-rw-r--r--   0        0        0     2081 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_89pct.py
+-rw-r--r--   0        0        0     2581 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color37.py
+-rw-r--r--   0        0        0     2621 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color89.py
+-rw-r--r--   0        0        0      687 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/sfc_winds/__init__.py
+-rw-r--r--   0        0        0     4150 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/sfc_winds/windbarbs.py
+-rw-r--r--   0        0        0     6821 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/single_channel.py
+-rw-r--r--   0        0        0     3505 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis.py
+-rw-r--r--   0        0        0     2414 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_GeoIPS1.py
+-rw-r--r--   0        0        0     3665 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR.py
+-rw-r--r--   0        0        0     3463 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR_GeoIPS1.py
+-rw-r--r--   0        0        0      688 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/__init__.py
+-rw-r--r--   0        0        0     1581 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/cmap_rgb.py
+-rw-r--r--   0        0        0     5880 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/matplotlib_linear_norm.py
+-rw-r--r--   0        0        0      723 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/__init__.py
+-rw-r--r--   0        0        0     3353 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_150H.py
+-rw-r--r--   0        0        0     3429 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H.py
+-rw-r--r--   0        0        0     3428 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Legacy.py
+-rw-r--r--   0        0        0     3390 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Physical.py
+-rw-r--r--   0        0        0     2984 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37pct.py
+-rw-r--r--   0        0        0     3327 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H.py
+-rw-r--r--   0        0        0     3326 2024-04-23 23:27:47.717714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89HW.py
+-rw-r--r--   0        0        0     3365 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Legacy.py
+-rw-r--r--   0        0        0     3356 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Physical.py
+-rw-r--r--   0        0        0     3488 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89pct.py
+-rw-r--r--   0        0        0     3069 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_Rain.py
+-rw-r--r--   0        0        0      706 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/tpw/__init__.py
+-rw-r--r--   0        0        0     2518 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/tpw/tpw_pwat.py
+-rw-r--r--   0        0        0     3811 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/IR_BD.py
+-rw-r--r--   0        0        0     3592 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/Infrared.py
+-rw-r--r--   0        0        0     3557 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/WV.py
+-rw-r--r--   0        0        0      698 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/winds/__init__.py
+-rw-r--r--   0        0        0     3806 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/colormappers/winds/wind_radii_transitions.py
+-rw-r--r--   0        0        0      690 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/__init__.py
+-rw-r--r--   0        0        0     4301 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/center_radius.py
+-rw-r--r--   0        0        0     2565 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/center_radius_rgba.py
+-rw-r--r--   0        0        0     1545 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/masked_arrays.py
+-rw-r--r--   0        0        0     1527 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/numpy_arrays_nan.py
+-rw-r--r--   0        0        0     1540 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/rgba.py
+-rw-r--r--   0        0        0     1761 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/windbarbs.py
+-rw-r--r--   0        0        0      692 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/__init__.py
+-rw-r--r--   0        0        0     1976 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/basic_fname.py
+-rw-r--r--   0        0        0     7459 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geoips_fname.py
+-rw-r--r--   0        0        0     4224 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geoips_netcdf_fname.py
+-rw-r--r--   0        0        0     2052 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geotiff_fname.py
+-rw-r--r--   0        0        0     3107 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/metadata_default_fname.py
+-rw-r--r--   0        0        0     2951 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/tc_clean_fname.py
+-rw-r--r--   0        0        0    14732 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/tc_fname.py
+-rw-r--r--   0        0        0     1972 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_day_fname.py
+-rw-r--r--   0        0        0     3811 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_full_fname.py
+-rw-r--r--   0        0        0     4231 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_tc_fname.py
+-rw-r--r--   0        0        0      706 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/utils/__init__.py
+-rw-r--r--   0        0        0     8187 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/utils/tc_file_naming.py
+-rw-r--r--   0        0        0      686 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/__init__.py
+-rw-r--r--   0        0        0      697 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/__init__.py
+-rw-r--r--   0        0        0     4411 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_gauss.py
+-rw-r--r--   0        0        0     4822 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_nearest.py
+-rw-r--r--   0        0        0      698 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/scipy_wrappers/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/scipy_wrappers/interp_grid.py
+-rw-r--r--   0        0        0      692 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/__init__.py
+-rwxr-xr-x   0        0        0    39645 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/boxdefinitions.py
+-rw-r--r--   0        0        0     4693 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/interp_pyresample.py
+-rw-r--r--   0        0        0     5097 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/interp_scipy.py
+-rw-r--r--   0        0        0     5679 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_checkers/geotiff.py
+-rw-r--r--   0        0        0     8331 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_checkers/image.py
+-rw-r--r--   0        0        0    11161 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_checkers/netcdf.py
+-rw-r--r--   0        0        0     5952 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_checkers/text.py
+-rw-r--r--   0        0        0      689 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/__init__.py
+-rw-r--r--   0        0        0     3986 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/full_disk_image.py
+-rw-r--r--   0        0        0     3988 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/geotiff_standard.py
+-rw-r--r--   0        0        0     6729 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_annotated.py
+-rw-r--r--   0        0        0     2899 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_clean.py
+-rw-r--r--   0        0        0    12540 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_windbarbs.py
+-rw-r--r--   0        0        0     1630 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_windbarbs_clean.py
+-rw-r--r--   0        0        0     5804 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/metadata_default.py
+-rw-r--r--   0        0        0     7877 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/metadata_tc.py
+-rw-r--r--   0        0        0     1409 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/netcdf_geoips.py
+-rw-r--r--   0        0        0     4888 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/netcdf_xarray.py
+-rw-r--r--   0        0        0     7831 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/text_winds.py
+-rw-r--r--   0        0        0     2870 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/output_formatters/unprojected_image.py
+-rw-r--r--   0        0        0      681 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/procflows/__init__.py
+-rw-r--r--   0        0        0    79206 2024-04-23 23:27:47.721714 geoips-1.12.2a0/geoips/plugins/modules/procflows/config_based.py
+-rw-r--r--   0        0        0    79114 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/procflows/single_source.py
+-rw-r--r--   0        0        0      680 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/__init__.py
+-rw-r--r--   0        0        0     6447 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/abi_l2_netcdf.py
+-rw-r--r--   0        0        0    42928 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/abi_netcdf.py
+-rw-r--r--   0        0        0    63750 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ahi_hsd.py
+-rw-r--r--   0        0        0    15704 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/amsr2_netcdf.py
+-rw-r--r--   0        0        0     4886 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/amsr2_remss_winds_netcdf.py
+-rw-r--r--   0        0        0    10502 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/amsub_hdf.py
+-rw-r--r--   0        0        0    19598 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/amsub_mirs.py
+-rw-r--r--   0        0        0    15023 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ascat_uhr_netcdf.py
+-rw-r--r--   0        0        0    11734 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/atms_hdf5.py
+-rw-r--r--   0        0        0    10268 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ewsg_netcdf.py
+-rw-r--r--   0        0        0     3105 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/geoips_netcdf.py
+-rw-r--r--   0        0        0     9758 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/gmi_hdf5.py
+-rw-r--r--   0        0        0     7409 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/imerg_hdf5.py
+-rw-r--r--   0        0        0     4466 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/mimic_netcdf.py
+-rw-r--r--   0        0        0    34756 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/modis_hdf4.py
+-rw-r--r--   0        0        0     7592 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/saphir_hdf5.py
+-rw-r--r--   0        0        0    11767 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/sar_winds_netcdf.py
+-rw-r--r--   0        0        0    10592 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/scat_knmi_winds_netcdf.py
+-rw-r--r--   0        0        0    10365 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/scat_noaa_winds_netcdf.py
+-rwxr-xr-x   0        0        0    30729 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/seviri_hrit.py
+-rw-r--r--   0        0        0     5176 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/sfc_winds_text.py
+-rw-r--r--   0        0        0     4811 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/smap_remss_winds_netcdf.py
+-rw-r--r--   0        0        0    10319 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/smos_winds_netcdf.py
+-rw-r--r--   0        0        0    23045 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ssmi_binary.py
+-rw-r--r--   0        0        0    48302 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/ssmis_binary.py
+-rw-r--r--   0        0        0      685 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/utils/__init__.py
+-rw-r--r--   0        0        0    24657 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/utils/geostationary_geolocation.py
+-rw-r--r--   0        0        0    39075 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/utils/hrit_reader.py
+-rw-r--r--   0        0        0     4800 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/utils/remss_reader.py
+-rwxr-xr-x   0        0        0    26859 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/viirs_netcdf.py
+-rw-r--r--   0        0        0     7650 2024-04-23 23:27:47.725714 geoips-1.12.2a0/geoips/plugins/modules/readers/wfabba_ascii.py
+-rw-r--r--   0        0        0    20795 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/readers/windsat_idr37_binary.py
+-rw-r--r--   0        0        0     4256 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/readers/windsat_remss_winds_netcdf.py
+-rw-r--r--   0        0        0      690 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/__init__.py
+-rw-r--r--   0        0        0    18201 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/bdeck_parser.py
+-rw-r--r--   0        0        0     6041 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/tc_sector_file_parser.py
+-rw-r--r--   0        0        0      695 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_spec_generators/__init__.py
+-rw-r--r--   0        0        0     3073 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/sector_spec_generators/center_coordinates.py
+-rw-r--r--   0        0        0      689 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/title_formatters/__init__.py
+-rw-r--r--   0        0        0     2009 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/title_formatters/static_standard.py
+-rw-r--r--   0        0        0     2830 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/title_formatters/tc_copyright.py
+-rw-r--r--   0        0        0     3061 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/modules/title_formatters/tc_standard.py
+-rwxr-xr-x   0        0        0     2977 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_cimss.txt
+-rw-r--r--   0        0        0     3353 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_purple.txt
+-rwxr-xr-x   0        0        0     1083 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_pwat.txt
+-rw-r--r--   0        0        0      459 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/default.yaml
+-rw-r--r--   0        0        0      553 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_pmw.yaml
+-rw-r--r--   0        0        0      478 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_visir.yaml
+-rw-r--r--   0        0        0      551 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_windspeed.yaml
+-rw-r--r--   0        0        0      437 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/default.yaml
+-rw-r--r--   0        0        0      438 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/north_pole.yaml
+-rw-r--r--   0        0        0      473 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_0p25degree.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_pmw.yaml
+-rw-r--r--   0        0        0      460 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_visir.yaml
+-rw-r--r--   0        0        0      474 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_visir_3200km.yaml
+-rw-r--r--   0        0        0      460 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/gridline_annotators/tc_windspeed.yaml
+-rw-r--r--   0        0        0     1033 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/Uncorrected-Channel.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150H.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150V.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150VNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/157V.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/157VNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/165H.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/165HNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166H.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166HNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166V.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166VNearest.yaml
+-rw-r--r--   0        0        0      559 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-1H.yaml
+-rw-r--r--   0        0        0      554 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-1HNearest.yaml
+-rw-r--r--   0        0        0      559 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-3H.yaml
+-rw-r--r--   0        0        0      554 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-3HNearest.yaml
+-rw-r--r--   0        0        0      559 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-7H.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183H.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183HNearest.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/190V.yaml
+-rw-r--r--   0        0        0      550 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/190VNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19H.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19HNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19V.yaml
+-rw-r--r--   0        0        0      543 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19VNearest.yaml
+-rw-r--r--   0        0        0      573 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Legacy.yaml
+-rw-r--r--   0        0        0      568 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-LegacyNearest.yaml
+-rw-r--r--   0        0        0      579 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Physical.yaml
+-rw-r--r--   0        0        0      574 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-PhysicalNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37HNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37V.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37VNearest.yaml
+-rw-r--r--   0        0        0      553 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37pct.yaml
+-rw-r--r--   0        0        0      548 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37pctNearest.yaml
+-rw-r--r--   0        0        0      467 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/color37.yaml
+-rw-r--r--   0        0        0      462 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/color37Nearest.yaml
+-rw-r--r--   0        0        0      573 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Legacy.yaml
+-rw-r--r--   0        0        0      568 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-LegacyNearest.yaml
+-rw-r--r--   0        0        0      579 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Physical.yaml
+-rw-r--r--   0        0        0      574 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-PhysicalNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HNearest.yaml
+-rw-r--r--   0        0        0      563 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HW.yaml
+-rw-r--r--   0        0        0      558 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HWNearest.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89V.yaml
+-rw-r--r--   0        0        0      547 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89VNearest.yaml
+-rw-r--r--   0        0        0      557 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89pct.yaml
+-rw-r--r--   0        0        0      552 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89pctNearest.yaml
+-rw-r--r--   0        0        0      467 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/color89.yaml
+-rw-r--r--   0        0        0      462 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/color89Nearest.yaml
+-rw-r--r--   0        0        0      560 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/rain_rate/Rain.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/rain_rate/RainNearest.yaml
+-rw-r--r--   0        0        0      290 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sectored.yaml
+-rw-r--r--   0        0        0     1103 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/incident-angle.yaml
+-rw-r--r--   0        0        0      945 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/nrcs.yaml
+-rw-r--r--   0        0        0      604 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/wind-ambiguities.yaml
+-rw-r--r--   0        0        0      590 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/windbarbs.yaml
+-rw-r--r--   0        0        0      613 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/windspeed.yaml
+-rw-r--r--   0        0        0      786 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-CIMSS.yaml
+-rw-r--r--   0        0        0      791 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-PURPLE.yaml
+-rw-r--r--   0        0        0      519 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-PWAT.yaml
+-rw-r--r--   0        0        0      267 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/unmodified.yaml
+-rw-r--r--   0        0        0      296 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/unsectored.yaml
+-rw-r--r--   0        0        0      598 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/IR-BD.yaml
+-rw-r--r--   0        0        0      722 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Infrared-Gray.yaml
+-rw-r--r--   0        0        0      607 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Infrared.yaml
+-rw-r--r--   0        0        0      662 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-GeoIPS1.yaml
+-rw-r--r--   0        0        0      483 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-IR-GeoIPS1.yaml
+-rw-r--r--   0        0        0      459 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-IR.yaml
+-rw-r--r--   0        0        0      759 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis.yaml
+-rw-r--r--   0        0        0     1053 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Visible.yaml
+-rw-r--r--   0        0        0      599 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV-Lower.yaml
+-rw-r--r--   0        0        0      599 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV-Upper.yaml
+-rw-r--r--   0        0        0      587 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV.yaml
+-rw-r--r--   0        0        0     2429 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/products/abi.yaml
+-rw-r--r--   0        0        0     3827 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/products/ahi.yaml
+-rw-r--r--   0        0        0     4992 2024-04-23 23:27:47.729714 geoips-1.12.2a0/geoips/plugins/yaml/products/amsr-e.yaml
+-rw-r--r--   0        0        0     7947 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/amsr2.yaml
+-rw-r--r--   0        0        0     2844 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/amsu-b.yaml
+-rw-r--r--   0        0        0     2244 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/ascat.yaml
+-rw-r--r--   0        0        0     2280 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/ascatuhr.yaml
+-rw-r--r--   0        0        0     1709 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/atms.yaml
+-rw-r--r--   0        0        0    10713 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/gmi.yaml
+-rw-r--r--   0        0        0     1070 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/gvar.yaml
+-rw-r--r--   0        0        0     1167 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/hscat.yaml
+-rw-r--r--   0        0        0      587 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/imerg.yaml
+-rw-r--r--   0        0        0     2928 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/mhs.yaml
+-rw-r--r--   0        0        0      824 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/mimic.yaml
+-rw-r--r--   0        0        0     2186 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/modis.yaml
+-rw-r--r--   0        0        0     1040 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/oscat.yaml
+-rw-r--r--   0        0        0     1330 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/saphir.yaml
+-rw-r--r--   0        0        0     1345 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/sar-spd.yaml
+-rw-r--r--   0        0        0     2249 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/seviri.yaml
+-rw-r--r--   0        0        0      881 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/smap-spd.yaml
+-rw-r--r--   0        0        0      881 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/smos-spd.yaml
+-rw-r--r--   0        0        0     8612 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/ssmi.yaml
+-rw-r--r--   0        0        0    11093 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/ssmis.yaml
+-rw-r--r--   0        0        0     8555 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/tmi.yaml
+-rw-r--r--   0        0        0     2349 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/viirs.yaml
+-rw-r--r--   0        0        0     3935 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/products/windsat.yaml
+-rw-r--r--   0        0        0      400 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1024x1024/tc_1km_1024x1024.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1024x1024/tc_2km_1024x1024.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1400x1400/tc_1km_1400x1400.yaml
+-rw-r--r--   0        0        0      400 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1400x1400/tc_2km_1400x1400.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1600x1600/tc_2km_1600x1600.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_1600x1600/tc_4km_1600x1600.yaml
+-rw-r--r--   0        0        0      395 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_256x256/tc_4km_256x256.yaml
+-rw-r--r--   0        0        0      390 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_512x512/tc_2km_512x512.yaml
+-rw-r--r--   0        0        0      392 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_512x512/tc_4km_512x512.yaml
+-rw-r--r--   0        0        0      390 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_800x800/tc_2km_800x800.yaml
+-rw-r--r--   0        0        0      390 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_800x800/tc_4km_800x800.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_0p1km_3200x3200.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_1km_2500x2500.yaml
+-rw-r--r--   0        0        0      398 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_huge/tc_1km_3200x3200.yaml
+-rw-r--r--   0        0        0      391 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_2km_template.yaml
+-rw-r--r--   0        0        0      338 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_50km_barbs_template.yaml
+-rw-r--r--   0        0        0      417 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_high_barbs_template.yaml
+-rw-r--r--   0        0        0      341 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascat_low_barbs_template.yaml
+-rw-r--r--   0        0        0      409 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_ascatuhr_barbs_template.yaml
+-rw-r--r--   0        0        0      397 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_halfkm_template.yaml
+-rw-r--r--   0        0        0      391 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_qkm_template.yaml
+-rw-r--r--   0        0        0      340 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/dynamic/tc_web_template.yaml
+-rw-r--r--   0        0        0      486 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/abu_dhabi.yaml
+-rw-r--r--   0        0        0      454 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/africa.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/african_horn.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/alaska.yaml
+-rw-r--r--   0        0        0      448 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/asia.yaml
+-rw-r--r--   0        0        0      474 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/australia.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/beijing.yaml
+-rw-r--r--   0        0        0      460 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/brazil.yaml
+-rw-r--r--   0        0        0      451 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/cairo.yaml
+-rw-r--r--   0        0        0      457 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/canada.yaml
+-rw-r--r--   0        0        0      454 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/caribbean.yaml
+-rw-r--r--   0        0        0      479 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/central_america.yaml
+-rw-r--r--   0        0        0      565 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/conus.yaml
+-rw-r--r--   0        0        0      443 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/delhi.yaml
+-rw-r--r--   0        0        0      474 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/denver.yaml
+-rw-r--r--   0        0        0      461 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/e_pacific.yaml
+-rw-r--r--   0        0        0      458 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/europe.yaml
+-rw-r--r--   0        0        0      531 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/ewsg.yaml
+-rw-r--r--   0        0        0      451 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/france.yaml
+-rw-r--r--   0        0        0      516 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/global.yaml
+-rw-r--r--   0        0        0      554 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/goes_east.yaml
+-rw-r--r--   0        0        0      555 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/goes_west.yaml
+-rw-r--r--   0        0        0      549 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/himawari.yaml
+-rw-r--r--   0        0        0      461 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/indian_basin.yaml
+-rw-r--r--   0        0        0      526 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/japan.yaml
+-rw-r--r--   0        0        0      474 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/mediterranean.yaml
+-rw-r--r--   0        0        0      477 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/melbourne.yaml
+-rw-r--r--   0        0        0      491 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/meteosat_africa.yaml
+-rw-r--r--   0        0        0      491 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/meteosat_europe.yaml
+-rw-r--r--   0        0        0      518 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/meteosat_indian_ocean.yaml
+-rw-r--r--   0        0        0      472 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/mexico_city.yaml
+-rw-r--r--   0        0        0      472 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/middle_east.yaml
+-rw-r--r--   0        0        0      466 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/ne_asia.yaml
+-rw-r--r--   0        0        0      457 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/north_pole.yaml
+-rw-r--r--   0        0        0      451 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/paris.yaml
+-rw-r--r--   0        0        0      496 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/rio_de_janeiro.yaml
+-rw-r--r--   0        0        0      446 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/russia.yaml
+-rw-r--r--   0        0        0      491 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/saskatchewan.yaml
+-rw-r--r--   0        0        0      463 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/se_asia.yaml
+-rw-r--r--   0        0        0      514 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/south_america.yaml
+-rw-r--r--   0        0        0      454 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/south_pole.yaml
+-rw-r--r--   0        0        0      492 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/vancouver.yaml
+-rw-r--r--   0        0        0      457 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/victoria.yaml
+-rw-r--r--   0        0        0      462 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/w_atlantic.yaml
+-rw-r--r--   0        0        0      456 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/w_pacific.yaml
+-rw-r--r--   0        0        0      119 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/docstring.yaml
+-rw-r--r--   0        0        0      121 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/family.yaml
+-rw-r--r--   0        0        0      118 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/interface.yaml
+-rw-r--r--   0        0        0       96 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/name.yaml
+-rw-r--r--   0        0        0      119 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/product_defaults.yaml
+-rw-r--r--   0        0        0      322 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/top.yaml
+-rw-r--r--   0        0        0      274 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/bases/valid_identifier.yaml
+-rw-r--r--   0        0        0     1215 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/feature_annotators/cartopy.yaml
+-rw-r--r--   0        0        0     1811 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/gridline_annotators/cartopy.yaml
+-rw-r--r--   0        0        0      209 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/algorithm.yaml
+-rw-r--r--   0        0        0      245 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      284 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      327 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/algorithm.yaml
+-rw-r--r--   0        0        0     1364 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/colormapper.yaml
+-rw-r--r--   0        0        0      328 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/coverage_checker.yaml
+-rw-r--r--   0        0        0      320 2024-04-23 23:27:47.733714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/interpolator.yaml
+-rw-r--r--   0        0        0      195 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/unvalidated.yaml
+-rw-r--r--   0        0        0      833 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/bases/windbarb_plotter.yaml
+-rw-r--r--   0        0        0      218 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/interpolator.yaml
+-rw-r--r--   0        0        0      248 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0      284 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      228 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/sectored_xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      640 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm.yaml
+-rw-r--r--   0        0        0      730 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      824 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      652 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator.yaml
+-rw-r--r--   0        0        0      734 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0      824 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0       98 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/specs/xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      169 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/unmodified.yaml
+-rw-r--r--   0        0        0      237 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/unsectored_xarray_dict_area_to_output_format.yaml
+-rw-r--r--   0        0        0      232 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/unsectored_xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      210 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/product_defaults/xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      354 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/algorithm.yaml
+-rw-r--r--   0        0        0      390 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      429 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      634 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/bases/product.yaml
+-rw-r--r--   0        0        0      363 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/interpolator.yaml
+-rw-r--r--   0        0        0      393 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0      429 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      220 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/list.yaml
+-rw-r--r--   0        0        0      243 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/sectored_xarray_dict_area_to_output_format.yaml
+-rw-r--r--   0        0        0      233 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/sectored_xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      191 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/single.yaml
+-rw-r--r--   0        0        0      179 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/unmodified.yaml
+-rw-r--r--   0        0        0      247 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/unsectored_xarray_dict_area_to_output_format.yaml
+-rw-r--r--   0        0        0      237 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/unsectored_xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      215 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/products/xarray_dict_to_output_format.yaml
+-rw-r--r--   0        0        0      369 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/generated.yaml
+-rw-r--r--   0        0        0      217 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/atmosriver.yaml
+-rw-r--r--   0        0        0      213 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/pyrocb.yaml
+-rw-r--r--   0        0        0      316 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/static.yaml
+-rw-r--r--   0        0        0      271 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/stitched.yaml
+-rw-r--r--   0        0        0      451 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/tc.yaml
+-rw-r--r--   0        0        0      244 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/metadata_families/volcano.yaml
+-rw-r--r--   0        0        0      770 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/specs/area_definition.yaml
+-rw-r--r--   0        0        0      746 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/specs/center.yaml
+-rw-r--r--   0        0        0     2016 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/schema/sectors/static.yaml
+-rw-r--r--   0        0        0      685 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/__init__.py
+-rw-r--r--   0        0        0    11134 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/estimate_area_extent.py
+-rw-r--r--   0        0        0    12241 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/overpass_predictor.py
+-rw-r--r--   0        0        0     3880 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/projections.py
+-rw-r--r--   0        0        0    11052 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/tc_tracks.py
+-rw-r--r--   0        0        0    15280 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/tc_tracks_database.py
+-rw-r--r--   0        0        0    26958 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/utils.py
+-rw-r--r--   0        0        0     6731 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/sector_utils/yaml_utils.py
+-rw-r--r--   0        0        0      682 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/utils/__init__.py
+-rw-r--r--   0        0        0      838 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/utils/context_managers.py
+-rw-r--r--   0        0        0     2582 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/utils/decorators.py
+-rw-r--r--   0        0        0     3569 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/utils/memusg.py
+-rw-r--r--   0        0        0      685 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/xarray_utils/__init__.py
+-rw-r--r--   0        0        0    33275 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/xarray_utils/data.py
+-rw-r--r--   0        0        0     4421 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/xarray_utils/time.py
+-rw-r--r--   0        0        0     1111 2024-04-23 23:27:47.737714 geoips-1.12.2a0/geoips/xarray_utils/xr_to_dtree.py
+-rw-r--r--   0        0        0     6837 2024-04-23 23:27:59.645849 geoips-1.12.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1062 2024-04-23 23:27:47.737714 geoips-1.12.2a0/setup/download_test_data.py
+-rw-r--r--   0        0        0     1184 2024-04-23 23:27:47.793715 geoips-1.12.2a0/tests/outputs/abi.tc.IR-BD.imagery_annotated/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1190 2024-04-23 23:27:47.797715 geoips-1.12.2a0/tests/outputs/abi.tc.Infrared.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Infrared_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1188 2024-04-23 23:27:47.809715 geoips-1.12.2a0/tests/outputs/abi.tc.Visible.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Visible_110kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1245 2024-04-23 23:27:47.845716 geoips-1.12.2a0/tests/outputs/amsr2.tc.89H-Physical.imagery_annotated/20200518_073601_IO012020_amsr2_gcom-w1_89H-Physical_140kts_100p00_res1p0-cr300.png.yaml
+-rw-r--r--   0        0        0     1667 2024-04-23 23:27:47.849716 geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgInfrared-Gray.png.yaml
+-rw-r--r--   0        0        0     1661 2024-04-23 23:27:47.857716 geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgVisible.png.yaml
+-rw-r--r--   0        0        0     1668 2024-04-23 23:27:47.865716 geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgInfrared-Gray.png.yaml
+-rw-r--r--   0        0        0     1662 2024-04-23 23:27:47.873716 geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgVisible.png.yaml
+-rw-r--r--   0        0        0     1243 2024-04-23 23:27:47.873716 geoips-1.12.2a0/tests/outputs/amsr2_ocean.tc.windspeed.imagery_clean/20200518_073601_IO012020_amsr2_gcom-w1_windspeed_140kts_85p45_1p0-clean.png.yaml
+-rw-r--r--   0        0        0     1136 2024-04-23 23:27:47.877716 geoips-1.12.2a0/tests/outputs/amsub_mirs.tc.183-3H.imagery_annotated/20210419_235400_WP022021_amsu-b_metop-a_183-3H_115kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1234 2024-04-23 23:27:47.881716 geoips-1.12.2a0/tests/outputs/ascat_knmi.tc.windbarbs.imagery_windbarbs_clean/20210421_014248_WP022021_ascat_metop-c_windbarbs_120kts_78p20_0p5-clean.png.yaml
+-rw-r--r--   0        0        0     1222 2024-04-23 23:27:47.885716 geoips-1.12.2a0/tests/outputs/ascat_low_knmi.tc.windbarbs.imagery_windbarbs/20210421_014156_WP022021_ascat_metop-c_windbarbs_120kts_35p17_1p0.png.yaml
+-rw-r--r--   0        0        0     1556 2024-04-23 23:27:47.889716 geoips-1.12.2a0/tests/outputs/ascat_noaa_25km.tc.windbarbs.imagery_windbarbs/20230524_235304_WP022023_ascat_metop-c_windbarbs_135kts_39p90_0p7.png.yaml
+-rw-r--r--   0        0        0     1569 2024-04-23 23:27:47.893716 geoips-1.12.2a0/tests/outputs/ascat_noaa_50km.tc.wind-ambiguities.imagery_windbarbs/20230524_235200_WP022023_ascat_metop-c_wind-ambiguities_135kts_50p08_1p1.png.yaml
+-rw-r--r--   0        0        0     1226 2024-04-23 23:27:47.901716 geoips-1.12.2a0/tests/outputs/ascat_uhr.tc.wind-ambiguities.imagery_windbarbs/20210421_014200_WP022021_ascatuhr_metop-c_wind-ambiguities_120kts_100p00_0p1.png.yaml
+-rw-r--r--   0        0        0     1382 2024-04-23 23:27:47.933717 geoips-1.12.2a0/tests/outputs/gmi.tc.89pct.imagery_clean/20200917_171519_AL202020_gmi_GPM_89pct_115kts_78p16_res1p0-cr300-clean.png.yaml
+-rw-r--r--   0        0        0     1211 2024-04-23 23:27:47.937717 geoips-1.12.2a0/tests/outputs/hy2.tc.windspeed.imagery_annotated/20211202_084039_WP272021_hscat_hy-2b_windspeed_95kts_97p06_1p0.png.yaml
+-rw-r--r--   0        0        0     1131 2024-04-23 23:27:47.945717 geoips-1.12.2a0/tests/outputs/mimic_fine.tc.TPW-PWAT.imagery_annotated/20210419_230000_WP022021_mimic_tpw_TPW-PWAT_115kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     1220 2024-04-23 23:27:47.953717 geoips-1.12.2a0/tests/outputs/oscat_knmi.tc.windbarbs.imagery_windbarbs/20210209_025351_SH192021_oscat_scatsat-1_windbarbs_135kts_75p10_1p0.png.yaml
+-rw-r--r--   0        0        0     1162 2024-04-23 23:27:47.953717 geoips-1.12.2a0/tests/outputs/saphir.tc.183-3HNearest.imagery_annotated/20210209_003103_SH192021_saphir_meghatropiques_183-3HNearest_135kts_88p76_1p0.png.yaml
+-rw-r--r--   0        0        0     1144 2024-04-23 23:27:47.957717 geoips-1.12.2a0/tests/outputs/sar.tc.nrcs.imagery_annotated/20181025_203206_WP312018_sar-spd_sentinel-1_nrcs_130kts_58p51_res1p0-cr300.png.yaml
+-rw-r--r--   0        0        0    54649 2024-04-23 23:27:47.969717 geoips-1.12.2a0/tests/outputs/smos.tc.sectored.text_winds/smos-spd_surface_winds_esa_smos_tc2020sh16gabekile_202002161242.txt
+-rw-r--r--   0        0        0     1222 2024-04-23 23:27:47.969717 geoips-1.12.2a0/tests/outputs/ssmi.tc.37pct.imagery_clean/20200519_090000_IO012020_ssmi_F15_37pct_110kts_50p65_1p0-clean.png.yaml
+-rw-r--r--   0        0        0     1347 2024-04-23 23:27:47.977717 geoips-1.12.2a0/tests/outputs/viirsday.tc.Night-Vis-IR.imagery_annotated/20210209_074210_SH192021_viirs_noaa-20_Night-Vis-IR_130kts_100p00_1p0.png.yaml
+-rw-r--r--   0        0        0     6257 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/commandline/test_log_setup.py
+-rw-r--r--   0        0        0      690 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/invalid_interfaces.yaml
+-rw-r--r--   0        0        0      677 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/missing_lowest_keys.yaml
+-rw-r--r--   0        0        0      662 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/missing_plugin_types.yaml
+-rw-r--r--   0        0        0     8382 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/data_fusion.yaml
+-rw-r--r--   0        0        0   224173 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips.yaml
+-rw-r--r--   0        0        0     8892 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips_clavrx.yaml
+-rw-r--r--   0        0        0     3166 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips_plugin_example.yaml
+-rw-r--r--   0        0        0     5822 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/overcast_package.yaml
+-rw-r--r--   0        0        0     1877 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/recenter_tc.yaml
+-rw-r--r--   0        0        0     1997 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/template_basic_plugin.yaml
+-rw-r--r--   0        0        0      626 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/template_fusion_plugin.yaml
+-rw-r--r--   0        0        0    10936 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugin_registries/test_plugin_registries.py
+-rw-r--r--   0        0        0     2815 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugins/modules/output_checkers/test_output_checkers.py
+-rw-r--r--   0        0        0     1529 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugins/yaml/sectors/test_sectors.py
+-rw-r--r--   0        0        0     1717 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/plugins/yaml/test_all_yaml_plugins.py
+-rw-r--r--   0        0        0       21 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/bases/docstring.yaml
+-rw-r--r--   0        0        0       91 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/bases/valid_identifier.yaml
+-rw-r--r--   0        0        0     2966 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/feature_annotators/cartopy.yaml
+-rw-r--r--   0        0        0     1467 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/gridline_annotators/cartopy.yaml
+-rw-r--r--   0        0        0     2028 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0     2855 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      317 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/algorithm.yaml
+-rw-r--r--   0        0        0     1346 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/colormapper.yaml
+-rw-r--r--   0        0        0      317 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/coverage_checker.yaml
+-rw-r--r--   0        0        0      317 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/interpolator.yaml
+-rw-r--r--   0        0        0      663 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0     1502 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0     1798 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/products/bases/product.yaml
+-rw-r--r--   0        0        0      385 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/bad/products/single.yaml
+-rw-r--r--   0        0        0       46 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/bases/valid_identifier.yaml
+-rw-r--r--   0        0        0      996 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/feature_annotators/cartopy.yaml
+-rw-r--r--   0        0        0      288 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/gridline_annotators/cartopy.yaml
+-rw-r--r--   0        0        0      283 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      384 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/algorithm_interpolator_colormapper.yaml
+-rw-r--r--   0        0        0      174 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/algorithm.yaml
+-rw-r--r--   0        0        0      523 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/colormapper.yaml
+-rw-r--r--   0        0        0      174 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/coverage_checker.yaml
+-rw-r--r--   0        0        0      174 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/interpolator.yaml
+-rw-r--r--   0        0        0      290 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/interpolator_algorithm.yaml
+-rw-r--r--   0        0        0      384 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/interpolator_algorithm_colormapper.yaml
+-rw-r--r--   0        0        0      529 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/products/bases/product.yaml
+-rw-r--r--   0        0        0     1182 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/products/single.yaml
+-rw-r--r--   0        0        0      460 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/good/sectors/static.yaml
+-rw-r--r--   0        0        0     3650 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/schema/test_yaml_schema.py
+-rw-r--r--   0        0        0     1446 2024-04-23 23:27:47.993717 geoips-1.12.2a0/tests/unit_tests/utils/context_managers.py
+-rw-r--r--   0        0        0     3912 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/unit_tests/xarray_utils/data.py
+-rw-r--r--   0        0        0     1867 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/unit_tests/xarray_utils/test_dtree.py
+-rw-r--r--   0        0        0     2533 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/unit_tests_long/plugins/modules/readers/test_readers.py
+-rw-r--r--   0        0        0     1263 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/abi_test.yaml
+-rw-r--r--   0        0        0     1500 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/abi_test_low_memory.yaml
+-rw-r--r--   0        0        0     4833 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/amsr2_no_compare_full.yaml
+-rw-r--r--   0        0        0     1731 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/amsr2_test.yaml
+-rw-r--r--   0        0        0     1813 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/amsr2_test_low_memory.yaml
+-rw-r--r--   0        0        0     1485 2024-04-23 23:27:47.997717 geoips-1.12.2a0/tests/yaml_configs/amsr2_test_no_compare.yaml
+-rw-r--r--   0        0        0     5436 1970-01-01 00:00:00.000000 geoips-1.12.2a0/PKG-INFO
```

### Comparing `geoips-1.12.2/.github/workflows/bandit.yaml` & `geoips-1.12.2a0/.github/workflows/black.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Bandit Pull Request
+name: Black Pull Request
 
 defaults:
   run:
     shell: bash
 
 on:
   # Triggers the workflow when pull request created and updated
@@ -10,45 +10,46 @@
     # Sequence of patterns matched against refs/heads
     branches:
       - main
   # Allows run of this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
-  check_code_bandit:
+  check_code_black:
     runs-on: ${{ vars.RUNNER }}
     steps:
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: "pypy-3.10"
           check-latest: true
+      - name: Checkout plugin current branch
+        uses: actions/checkout@master
       - name: Update pip
         run: pip install --upgrade pip
-      - name: Install bandit
-        run: pip install bandit
+      - name: Install black
+        run: pip install black
       - name: Checkout plugin current branch
         uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-          path: geoips_plugin_repo
-      - name: Checkout geoips default branch
+      - name: Checkout geoips active branch
         uses: actions/checkout@v3
         with:
-          fetch-depth: 0
           repository: ${{ vars.ORGANIZATION }}/geoips
-          ref: ${{ vars.DEFAULT_BRANCH }}
+          ref: ${{ vars.GEOIPS_ACTIVE_BRANCH }}
           token: ${{ secrets.GEOIPS_TOKEN }}
-          path: geoips_default_branch
-      - name: Run code check script bandit
+          path: geoips_dev_utils
+          sparse-checkout: |
+            tests/utils
+            .config
+      - name: Run code check script black
         shell: bash -l {0}
         run: |
-          echo "::group::bandit_analysis"
-          echo "BANDIT analysis of code"
-          ./geoips_default_branch/tests/utils/check_code.sh bandit ./geoips_plugin_repo
+          echo "::group::black_analysis"
+          echo "BLACK analysis of code"
+          ./geoips_dev_utils/tests/utils/check_code.sh black .
           ret=$?
           echo "Return code: ${ret}"
           echo "::endgroup::"
           if [[ "${ret}" != *"0"* ]]; then
-            echo "::error::due to bandit violations, return code ${ret}"
+            echo "::error::due to black violations, return code ${ret}"
             exit 1
           fi
```

### Comparing `geoips-1.12.2/.github/workflows/black.yaml` & `geoips-1.12.2a0/.github/workflows/test-interfaces.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,90 @@
-name: Black Pull Request
+name: Test Code Interfaces on Pull Request
 
 defaults:
   run:
     shell: bash
 
+env:
+  CONDA_ENV: github_actions_test_interfaces
+
+# Can not use variables in the list of branches,
+# GitHub Actions will not recognize, and workflow will not run.
 on:
   # Triggers the workflow when pull request created and updated
-  pull_request:
-    # Sequence of patterns matched against refs/heads
-    branches:
-      - main
+  # pull_request:
+  #   branches:
+  #     - main
   # Allows run of this workflow manually from the Actions tab
+  # Must be merged to default before it will be available to manually run.
   workflow_dispatch:
 
+# conda command to install all the required libraries for installing geoips
+# and geoips dependencies
+#   openblas required for scipy
+#   gcc/gxx required for akima/recenter_tc
+# conda create -y -n github_actions -c conda-forge gcc gxx openblas
 jobs:
-  check_code_black:
+  run_code_interfaces:
     runs-on: ${{ vars.RUNNER }}
     steps:
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v4 # v4is the latest for setup-python
         with:
-          python-version: "pypy-3.10"
+          python-version: "pypy-3.10"  # I believe 3.10 is the latest for actions
           check-latest: true
       - name: Update pip
         run: pip install --upgrade pip
-      - name: Install black
-        run: pip install black
-      - name: Checkout plugin current branch
-        uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-          path: geoips_plugin_repo
-      - name: Checkout geoips default branch
-        uses: actions/checkout@v3
+      - name: Checkout geoips default branch for dev utils
+        uses: actions/checkout@v3 # v3 is the latest for checkout
         with:
           fetch-depth: 0
           repository: ${{ vars.ORGANIZATION }}/geoips
           ref: ${{ vars.DEFAULT_BRANCH }}
           token: ${{ secrets.GEOIPS_TOKEN }}
-          path: geoips_default_branch
-      - name: Run code check script black
-        shell: bash -l {0}
+          path: geoips_dev_utils
+      - name: pip install geoips_dev_utils[test]
+        run: |
+          echo "which pip"
+          which pip
+          echo "pip uninstall -y geoips"
+          pip uninstall -y geoips
+          echo "pip install $PWD/geoips_dev_utils[test]"
+          pip install $PWD/geoips_dev_utils[test]
+          ret=$?
+          echo "${ret}"
+      - name: Checkout current repo default branch
+        uses: actions/checkout@v3 # v3 is the latest for checkout
+        with:
+          fetch-depth: 0
+          path: geoips_plugin_repo
+      - name: pip install geoips plugin repo
+        run: |
+          echo "which pip"
+          which pip
+          curr_repo=`echo "$GITHUB_REPOSITORY" | sed "s,$GITHUB_REPOSITORY_OWNER/,,"`
+          echo "pip uninstall -y $curr_repo"
+          pip uninstall -y $curr_repo
+          echo "pip install -v $PWD/geoips_plugin_repo"
+          pip install -v $PWD/geoips_plugin_repo
+          ret=$?
+          echo "${ret}"
+      - name: create_plugin_registries
+        run: |
+          echo "which create_plugin_registries"
+          which create_plugin_registries
+          echo "create_plugin_registries"
+          create_plugin_registries
+          ret=$?
+          echo "${ret}"
+      - name: Run code check script interfaces
         run: |
-          echo "::group::black_analysis"
-          echo "BLACK analysis of code"
-          black --version
-          ./geoips_default_branch/tests/utils/check_code.sh black ./geoips_plugin_repo
+          $PWD/geoips_dev_utils/tests/utils/check_code.sh interfaces $PWD/geoips_plugin_repo
           ret=$?
-          echo "Return code: ${ret}"
+          echo "::group::interface_analysis"
+          echo "INTERFACES analysis of code"
+          echo "${ret}"
           echo "::endgroup::"
-          if [[ "${ret}" != *"0"* ]]; then
-            echo "::error::due to black violations, return code ${ret}"
+          if [[ "${ret##*:}" != *"0"* ]]; then
+            echo "::error::due to interface violations ${ret##*:}"
             exit 1
           fi
```

### Comparing `geoips-1.12.2/.github/workflows/deploy-ghpages-docs.yaml` & `geoips-1.12.2a0/.github/workflows/pytest-short.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,136 +1,120 @@
-name: Build and deploy docs
+name: Pytest Short Unit Tests Pull Request
 
 defaults:
   run:
     shell: bash
 
-env:
-  CONDA_ENV: build_deploy_docs-${{ github.run_id }}-${{ github.run_attempt }}
-
+# Can not use variables in the list of branches,
+# GitHub Actions will not recognize, and workflow will not run.
 on:
+  # Triggers the workflow when pull request created and updated
+  # pull_request:
+  #   branches:
+  #     - main
   # Allows run of this workflow manually from the Actions tab
-  # Must be merged to dev before it will be available to manually run.
+  # Must be merged to default before it will be available to manually run.
   workflow_dispatch:
-  # Run on each published release
-  release:
-    types: [published]
 
+# conda command to install all the required libraries for installing geoips
+# and geoips dependencies
+#   openblas required for scipy
+#   gcc/gxx required for akima/recenter_tc
+# conda create -y -n github_actions -c conda-forge gcc gxx openblas
 jobs:
-  deploy_ghpages:
+  run_short_unit_tests:
     runs-on: ${{ vars.RUNNER }}
     steps:
       - name: Setup Python
         uses: actions/setup-python@v4 # v4is the latest for setup-python
         with:
           python-version: "pypy-3.10"  # I believe 3.10 is the latest for actions
           check-latest: true
       - name: Update pip
         run: pip install --upgrade pip
-      - name: Checkout geoips repo default branch
+      - name: Checkout geoips default branch
         uses: actions/checkout@v3 # v3 is the latest for checkout
         with:
           fetch-depth: 0
           repository: ${{ vars.ORGANIZATION }}/geoips
           ref: ${{ vars.DEFAULT_BRANCH }}
           token: ${{ secrets.GEOIPS_TOKEN }}
-          path: geoips_default_branch
-      - name: pip install geoips_default_branch[doc]
+          path: geoips_dev_utils
+      - name: pip install geoips_dev_utils[test]
         run: |
+          echo "which pip"
           which pip
+          echo "pip uninstall -y geoips"
           pip uninstall -y geoips
-          pip install $PWD/geoips_default_branch[doc]
+          echo "pip install $PWD/geoips_dev_utils[test]"
+          pip install $PWD/geoips_dev_utils[test]
           ret=$?
           echo "${ret}"
-          python -c "import geoips; print(geoips.__version__)"
-      - name: Checkout current repo current branch
+      - name: Checkout current repo default branch
         uses: actions/checkout@v3 # v3 is the latest for checkout
         with:
           fetch-depth: 0
           path: geoips_plugin_repo
       - name: pip install geoips plugin repo
         run: |
+          echo "which pip"
           which pip
           curr_repo=`echo "$GITHUB_REPOSITORY" | sed "s,$GITHUB_REPOSITORY_OWNER/,,"`
-          # Do not re-install if this is the geoips repo
-          if [[ "$curr_repo" != "geoips" ]]; then
-              pip uninstall -y $curr_repo
-              pip install -v $PWD/geoips_plugin_repo
-              ret=$?
-              echo "${ret}"
-              python -c "import $curr_repo; print($curr_repo.__version__)"
-          fi
+          echo "pip uninstall -y $curr_repo"
+          pip uninstall -y $curr_repo
+          echo "pip install -v $PWD/geoips_plugin_repo"
+          pip install -v $PWD/geoips_plugin_repo
+          ret=$?
+          echo "${ret}"
       - name: create_plugin_registries
         run: |
-          echo "create plugin registries"
+          echo "which create_plugin_registries"
           which create_plugin_registries
+          echo "create_plugin_registries"
           create_plugin_registries
           ret=$?
           echo "${ret}"
-      - name: Run build docs
+      - name: Run plugin repo pytest unit tests
         run: |
-          which pip
-          echo "Build html and pdf docs"
-          # Ie, get 'recenter_tc' out of 'NRLMMD-GEOIPS/recenter_tc'
+          echo "::group::pytest_unit_test"
+          echo "Pytest short unit tests of code ${PWD}/geoips_plugin_repo"
+          echo "which pytest"
+          which pytest
           curr_repo=`echo "$GITHUB_REPOSITORY" | sed "s,$GITHUB_REPOSITORY_OWNER/,,"`
-          # Call build_docs.sh from the geoips default branch
-          # Pass in
-          #   the path to the current plugin repo,
-          #   the name of the current repo,
-          #   "html_pdf" to indicate producing both html and pdf output, and
-          #   the path to the docs template directory in the geoips default branch.
-          ./geoips_default_branch/docs/build_docs.sh ./geoips_plugin_repo $curr_repo html_pdf ./geoips_default_branch/docs
-          ret=$?
-          if [[ "${ret##*:}" != *"0"* ]]; then
-            echo "::error::Building html and pdf docs ${ret##*:}"
-            exit 1
+          if [[ -d $PWD/geoips_plugin_repo/tests/unit_tests ]]; then
+            # If we are testing a different plugin repo, use the dev version
+            # of check_code.sh
+            echo "pytest -q $PWD/geoips_plugin_repo/tests/unit_tests"
+            pytest -q $PWD/geoips_plugin_repo/tests/unit_tests
+            ret=$?
+            echo "Return code: ${ret}"
+            echo "::endgroup::"
+            if [[ "${ret}" != *"0"* ]]; then
+              echo "::error::due to plugin repo pytest errors, return code ${ret}"
+              exit 1
+            fi
+          else
+            echo "No pytests found for plugin repo"
           fi
-      - name: Run deploy docs
+      - name: Run geoips repo pytest unit tests
         run: |
-          which pip
-          echo "Deploy docs to github pages"
-          # GITHUB_REPOSITORY, GITHUB_REPOSITORY_OWNER, and GITHUB_SERVER_URL are all
-          # standard github variables defined for every github actions run.
-          # Ie, get 'recenter_tc' out of 'NRLMMD-GEOIPS/recenter_tc'
+          echo "::group::pytest_unit_test"
+          echo "Pytest short unit tests of code ${PWD}/geoips_dev_utils"
+          echo "which pytest"
+          which pytest
           curr_repo=`echo "$GITHUB_REPOSITORY" | sed "s,$GITHUB_REPOSITORY_OWNER/,,"`
-          # ie, https://github.com/NRLMMD-GEOIPS
-          GEOIPS_REPO_URL="$GITHUB_SERVER_URL/$GITHUB_REPOSITORY_OWNER"
-          # Remove ghpages_repo dir if it exists.
-          # deploy_pages.sh will not run if ghpages_repo exists.
-          if [[ -d ./ghpages_repo ]]; then
-              echo "::group::remove_ghpages_before"
-              echo "Remove ghpages_repo before deploy"
-              echo "rm -rfv ./ghpages_repo"
-              rm -rfv ./ghpages_repo
-              echo "::endgroup::"
-              rmret=$?
-              if [[ "${rmret##*:}" != *"0"* ]]; then
-                echo "::error::Removing ./ghpages_repo before deploy ${rmret##*:}"
-                exit 1
-              fi
-          fi
-          # Use the deploy_pages.sh script from the geoips default branch.
-          # Pass in the
-          #   current plugin repo path,
-          #   the geoips repo url, and
-          #   a path to a new directory for the ghpages checkout/push
-          #   the name of the current repository
-          ./geoips_default_branch/docs/deploy_pages.sh ./geoips_plugin_repo $GEOIPS_REPO_URL ./ghpages_repo $curr_repo
-          ret=$?
-          if [[ "${ret##*:}" != *"0"* ]]; then
-            echo "::error::Deploying docs to GitHub pages ${ret##*:}"
-            exit 1
-          fi
-          # Remove ghpages_repo dir after running deploy_pages.sh.
-          # deploy_pages.sh will not run if ghpages_repo exists.
-          if [[ -d ./ghpages_repo ]]; then
-              echo "::group::remove_ghpages_after"
-              echo "Remove ghpages_repo after deploy"
-              echo "rm -rfv ./ghpages_repo"
-              rm -rfv ./ghpages_repo
-              echo "::endgroup::"
-              rmret=$?
-              if [[ "${rmret##*:}" != *"0"* ]]; then
-                echo "::error::Removing ./ghpages_repo after deploy ${rmret##*:}"
-                exit 1
-              fi
+          # If we are testing a plugin repo (not geoips), then we will run pytest
+          # on the current code. If this is the geoips repo, then we already tested
+          # above.
+          if [[ "$curr_repo" != "geoips" ]]; then
+            echo "pytest -q $PWD/geoips_dev_utils/tests/unit_tests"
+            pytest -q $PWD/geoips_dev_utils/tests/unit_tests
+            ret=$?
+            echo "Return code: ${ret}"
+            echo "::endgroup::"
+            if [[ "${ret}" != *"0"* ]]; then
+              echo "::error::due to geoips repo pytest errors, return code ${ret}"
+              exit 1
+            fi
+          else
+            echo "Do not run unit tests twice for geoips repo."
           fi
```

### Comparing `geoips-1.12.2/.github/workflows/flake8.yaml` & `geoips-1.12.2a0/.github/workflows/flake8.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -11,48 +11,49 @@
     branches:
       - main
   # Allows run of this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
   check_code_flake8:
-    runs-on: ${{ vars.RUNNER }}
+    runs-on: ubuntu-latest
     steps:
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: "pypy-3.10"
+          python-version: "pypy-3.9"
           check-latest: true
+      - name: Checkout plugin current branch
+        uses: actions/checkout@v3
       - name: Update pip
         run: pip install --upgrade pip
       - name: Install flake8
         run: pip install flake8
       - name: Install flake8-docstrings
         run: pip install flake8-docstrings
       - name: Install flake8-rst-docstrings
         run: pip install flake8-rst-docstrings
       - name: Checkout plugin current branch
         uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-          path: geoips_plugin_repo
-      - name: Checkout geoips default branch
+      - name: Checkout geoips active branch
         uses: actions/checkout@v3
         with:
-          fetch-depth: 0
-          repository: ${{ vars.ORGANIZATION }}/geoips
-          ref: ${{ vars.DEFAULT_BRANCH }}
+          repository: NRLMMD-GEOIPS/geoips
+          ref: ${{ vars.GEOIPS_ACTIVE_BRANCH }}
           token: ${{ secrets.GEOIPS_TOKEN }}
-          path: geoips_default_branch
+          path: geoips_dev_utils
+          sparse-checkout: |
+            tests/utils
+            .config
       - name: Run code check script flake8
         shell: bash -l {0}
         run: |
           echo "::group::flake8_analysis"
           echo "FLAKE8 analysis of code"
-          ./geoips_default_branch/tests/utils/check_code.sh flake8 .
+          ./geoips_dev_utils/tests/utils/check_code.sh flake8 .
           ret=$?
           echo "Return code: ${ret}"
           echo "::endgroup::"
           if [[ "${ret}" != *"0"* ]]; then
             echo "::error::due to flake8 violations, return code ${ret}"
             exit 1
           fi
```

### Comparing `geoips-1.12.2/.github/workflows/package-and-publish.yaml` & `geoips-1.12.2a0/.github/workflows/package-and-publish.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   workflow_dispatch:
   release:
     types: [published]
 
 jobs:
   deploysdist:
     name: "Deploy to Pypi"
-    runs-on: ${{ vars.RUNNER }}
+    runs-on: ubuntu-latest
 
     steps:
       - name: Checkout source
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
           fetch-tags: true
```

### Comparing `geoips-1.12.2/.github/workflows/release-note-update.yaml` & `geoips-1.12.2a0/.github/workflows/release-note-update.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     branches:
       - main
   # Allows run of this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
   release_v_change_detection:
-    runs-on: ${{ vars.RUNNER }}
+    runs-on: ubuntu-latest
     steps:
       - name: Checkout geoips repo default branch
         uses: actions/checkout@v3 # v3 is the latest for checkout
         with:
           fetch-depth: 0
           repository: ${{ vars.ORGANIZATION }}/geoips
           ref: ${{ vars.DEFAULT_BRANCH }}
```

### Comparing `geoips-1.12.2/.github/workflows/test-interfaces.yaml` & `geoips-1.12.2a0/.github/workflows/build-html-docs.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,85 @@
-name: Test Code Interfaces on Pull Request
+name: Build Sphinx html docs
 
 defaults:
   run:
     shell: bash
 
-env:
-  CONDA_ENV: test-interfaces-${{ github.run_id }}-${{ github.run_attempt }}
-
 # Can not use variables in the list of branches,
 # GitHub Actions will not recognize, and workflow will not run.
 on:
   # Triggers the workflow when pull request created and updated
-  pull_request:
-    branches:
-      - main
+  # pull_request:
+  #   branches:
+  #     - main
   # Allows run of this workflow manually from the Actions tab
-  # Must be merged to default before it will be available to manually run.
+  # Must be merged before it will be available to manually run.
   workflow_dispatch:
 
-# conda command to install all the required libraries for installing geoips
-# and geoips dependencies
-#   openblas required for scipy
-#   gcc/gxx required for akima/recenter_tc
-# conda create -y -n github_actions -c conda-forge gcc gxx openblas
 jobs:
-  run_code_interfaces:
+  build_sphinx_html:
     runs-on: ${{ vars.RUNNER }}
     steps:
       - name: Setup Python
         uses: actions/setup-python@v4 # v4is the latest for setup-python
         with:
           python-version: "pypy-3.10"  # I believe 3.10 is the latest for actions
           check-latest: true
       - name: Update pip
         run: pip install --upgrade pip
-      - name: Checkout geoips repo default branch
+      - name: Checkout geoips active branch for dev utils
         uses: actions/checkout@v3 # v3 is the latest for checkout
         with:
           fetch-depth: 0
           repository: ${{ vars.ORGANIZATION }}/geoips
-          ref: ${{ vars.DEFAULT_BRANCH }}
+          ref: ${{ vars.GEOIPS_ACTIVE_BRANCH }}
           token: ${{ secrets.GEOIPS_TOKEN }}
-          path: geoips_default_branch
-      - name: pip install geoips_default_branch[test]
+          path: geoips_dev_utils
+      - name: pip install -e geoips_dev_utils[test]
         run: |
           echo "which pip"
           which pip
-          echo "pip uninstall -y geoips"
-          pip uninstall -y geoips
-          echo "pip install $PWD/geoips_default_branch[test]"
-          pip install $PWD/geoips_default_branch[test]
+          echo "pip install -e $PWD/geoips_dev_utils[doc]"
+          pip install -e $PWD/geoips_dev_utils[doc]
           ret=$?
           echo "${ret}"
       - name: Checkout current repo default branch
         uses: actions/checkout@v3 # v3 is the latest for checkout
         with:
           fetch-depth: 0
           path: geoips_plugin_repo
-      - name: pip install geoips plugin repo
+      - name: pip install -e geoips plugin repo
         run: |
           echo "which pip"
           which pip
-          curr_repo=`echo "$GITHUB_REPOSITORY" | sed "s,$GITHUB_REPOSITORY_OWNER/,,"`
-          echo "pip uninstall -y $curr_repo"
-          pip uninstall -y $curr_repo
-          echo "pip install -v $PWD/geoips_plugin_repo"
-          pip install -v $PWD/geoips_plugin_repo
+          echo "pip uninstall -y geoips"
+          pip uninstall -y geoips
+          echo "pip install -e $PWD/geoips_plugin_repo"
+          pip install -e $PWD/geoips_plugin_repo
           ret=$?
           echo "${ret}"
       - name: create_plugin_registries
         run: |
           echo "which create_plugin_registries"
           which create_plugin_registries
           echo "create_plugin_registries"
           create_plugin_registries
           ret=$?
           echo "${ret}"
-      - name: Run code check script interfaces
+      - name: Run build html
         run: |
-          $PWD/geoips_default_branch/tests/utils/check_code.sh interfaces $PWD/geoips_plugin_repo
+          echo "Build html docs"
+          echo "$GITHUB_REPOSITORY"
+          echo "${GITHUB_REPOSITORY}"
+          echo "${{ github.repository }}"
+          echo "$GITHUB_REPOSITORY_OWNER"
+          echo "${GITHUB_REPOSITORY_OWNER}"
+          echo "${{ github.repository_owner }}"
+          # Ie, get 'recenter_tc' out of 'NRLMMD-GEOIPS/recenter_tc'
+          curr_repo=`echo "$GITHUB_REPOSITORY" | sed "s,$GITHUB_REPOSITORY_OWNER/,,"`
+          echo "./geoips_dev_utils/docs/build_docs.sh ./geoips_dev_utils $curr_repo"
+          ./geoips_dev_utils/docs/build_docs.sh ./geoips_dev_utils $curr_repo
           ret=$?
-          echo "::group::interface_analysis"
-          echo "INTERFACES analysis of code"
-          echo "${ret}"
-          echo "::endgroup::"
           if [[ "${ret##*:}" != *"0"* ]]; then
-            echo "::error::due to interface violations ${ret##*:}"
+            echo "::error::Building html docs ${ret##*:}"
             exit 1
           fi
```

### Comparing `geoips-1.12.2/.github/workflows_archived/docker-build-test-push.yaml` & `geoips-1.12.2a0/.github/workflows_archived/docker-build-test-push.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/.github/workflows_archived/validate-pull-request.yaml` & `geoips-1.12.2a0/.github/workflows_archived/validate-pull-request.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/LICENSE` & `geoips-1.12.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/README.md` & `geoips-1.12.2a0/README.md`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/docs/source/_templates/conf_PKG.py` & `geoips-1.12.2a0/docs/source/_templates/conf_PKG.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 # html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-html_last_updated_fmt = "%b %d, %Y %H:%M:%S"
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
 # html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
 # html_sidebars = {}
@@ -245,18 +245,18 @@
 # Latex additional files to include to format header footer for PDF.
 latex_additional_files = ["fancyhf.sty"]
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
-    "pointsize": "10pt",
+    "pointsize": "12pt",
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
-    "preamble": r"\usepackage{fancyhf}\usepackage{enumitem}\setlistdepth{99}",
+    "preamble": r"\usepackage{fancyhf}",
     # Latex figure (float) alignment
     "figure_align": "H",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
```

### Comparing `geoips-1.12.2/docs/source/yaml/20200918.195020.goes-16.Visible_latitude_longitude.tc2020al20teddy.nc.yaml` & `geoips-1.12.2a0/docs/source/yaml/20200918.195020.goes-16.Visible_latitude_longitude.tc2020al20teddy.nc.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_WV_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/docs/source/yaml/20200918_195020_AL202020_abi_goes-16_WV_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/docs/source/yaml/abi_test.yaml` & `geoips-1.12.2a0/docs/source/yaml/abi_test.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/__init__.py` & `geoips-1.12.2a0/geoips/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/_version.py` & `geoips-1.12.2a0/geoips/_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 # DO NOT EDIT
 # managed by poetry-dynamic-versioning
-__version__ = "1.12.2"
-__version_tuple__ = (1, 12, 2)
+__version__ = "1.12.2a0"
+__version_tuple__ = (1, 12, "2a0")
```

### Comparing `geoips-1.12.2/geoips/cli.py` & `geoips-1.12.2a0/geoips/cli.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/commandline/__init__.py` & `geoips-1.12.2a0/geoips/commandline/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/commandline/args.py` & `geoips-1.12.2a0/geoips/commandline/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,16 +256,15 @@
         )
 
     if arglist is None or "logging_level" in arglist:
         parser.add_argument(
             "-l",
             "--logging_level",
             choices=["INTERACTIVE", "INFO", "DEBUG", "WARNING", "ERROR", "CRITICAL"],
-            # Will default to $GEOIPS_LOGGING_LEVEL if set, else INTERACTIVE
-            default=getenv("GEOIPS_LOGGING_LEVEL"),
+            default="INTERACTIVE",
             help="""Specify logging config level for GeoIPS commands.""",
             type=str.upper,
         )
 
     sect_group = parser.add_argument_group(
         title="Sector Requests: General arguments for sectors"
     )
@@ -504,14 +503,24 @@
                             output products to compare with current outputs.
                             This should be formatted as a json dictionary string, with
                             YAML output config output_types as keys, and full directory
                             comparison output path as values.  Special key "all" will
                             pertain to all output types.""",
         )
 
+    if arglist is None or "compare_outputs_module" in arglist:
+        comp_group.add_argument(
+            "--compare_outputs_module",
+            nargs="?",
+            default="compare_outputs",
+            help="""Specify module to use for comparing outputs.
+                            Defaults to geoips.compare_outputs
+                            internally if not specified.""",
+        )
+
     procflow_group = parser.add_argument_group(
         title="Processing workflow specifications"
     )
     if arglist is None or "procflow" in arglist:
         procflow_group.add_argument(
             "--procflow",
             default=None,
@@ -883,35 +892,15 @@
                     database writer will be located in
                     geoips*.plugins.modules.postgres_database.
                         mywriter_name.mywriter_name,
                     The writer_name string should be the reader module name
                     (no .py)""",
         )
         prod_db_group.add_argument(
-            "--product_db_writer_kwargs",
-            default=None,
-            type=jloads,
-            help="""Provide the product db writer kwargs for the plugin passed under the
-                    product_db_writer flag. Should be formatted as a json dictionary
-                    string. Only provide one json dict str to this flag.""",
-        )
-        prod_db_group.add_argument(
             "--product_db_writer_override",
             nargs="?",
             default={},
             type=jloads,
             help="""Specify product database writer that should be used for each
                     available sector should be formatted as a json dictionary
                     string.""",
         )
-
-    composite_group = parser.add_argument_group(title="Image composite kwargs")
-    if arglist is None or "composite_output_kwargs_override" in arglist:
-        composite_group.add_argument(
-            "--composite_output_kwargs_override",
-            nargs="?",
-            default={},
-            type=jloads,
-            help="""Specify product composite kwargs that should be used for each
-                    available sector output. Should be formatted as a json dictionary
-                    string.""",
-        )
```

### Comparing `geoips-1.12.2/geoips/commandline/create_sector_image.py` & `geoips-1.12.2a0/geoips/commandline/create_sector_image.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/commandline/list_available_plugins.py` & `geoips-1.12.2a0/geoips/commandline/list_available_plugins.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/commandline/log_setup.py` & `geoips-1.12.2a0/geoips/commandline/log_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,15 @@
     # Even though only strings should be passed here, we are going to allow any type of
     # object to be passed for the time being. Best not to overthink the situation and
     # just cast for the time being.
     messages = filter(lambda s: len(str(s)) > 0, messages)
 
     for message in messages:
         # wrap the message to a specified length
-        wrapped_messages += wrap(
-            message, width=74, break_long_words=False, break_on_hyphens=False
-        )
+        wrapped_messages += wrap(message, width=74, break_long_words=False)
     try:
         max_message_len = min(74, max([len(wmessage) for wmessage in wrapped_messages]))
     except ValueError as e:
         raise ValueError(
             "No proper messages were provided for logging.\n"
             + "Make sure the messages are not all empty strings."
         ) from e
@@ -178,42 +176,37 @@
             self._logToRoot_funcs[level_num] = logToRoot
         return self._logToRoot_funcs[level_num]
 
 
 add_logging_level = LogLevelAdder()
 
 
-def setup_logging(logging_level=None, verbose=True):
+def setup_logging(logging_level="INTERACTIVE", verbose=True):
     """Get a new logger instance for GeoIPS.
 
     Get a new logger instance for GeoIPS. This will set the logger's logging level, its
     formatter, and add a `StreamHandler` pointing to `sys.stdout`.
 
     This is most often used at the top-level of an applcation to set up the root logger
     for the application (e.g. in a command line script). Once configured, the root
     logger's properties will be inherited by lower-level logger instances. So, to use
     the same logging configuration in submodules, simply instantiate a new logger
     instance via `LOG = logging.getLogger(__name__)` and it will behave the same as the
     root logger.
 
     Parameters
     ----------
-    logging_level : str, default=None
+    logging_level : str, default="INTERACTIVE"
         Sets the minimum log level for which log output will be written to stdout.
-        If None, will default to "INTERACTIVE".  This allows using env var
-        GEOIPS_LOGGING_LEVEL to override default (applied in run_procflow).
     verbose : bool, default=True
         Determines which log formatter will be used. If `True`, a longer format will be
         used, providing more information, but also cluttering the screen. If `False`, a
         shorter format will be used.
     """
     log = logging.getLogger()
-    # If logging_level was not specified, default to INTERACTIVE here.
-    if not logging_level:
-        logging_level = "INTERACTIVE"
     log.setLevel(getattr(logging, logging_level))
     fmt = logging.Formatter(
         "%(asctime)s %(module)12s.py:%(lineno)-4d %(levelname)7s: %(message)s",
         "%d_%H%M%S",
     )
     if not verbose:
         fmt = logging.Formatter("%(asctime)s: %(message)s", "%d_%H%M%S")
```

### Comparing `geoips-1.12.2/geoips/commandline/run_procflow.py` & `geoips-1.12.2a0/geoips/commandline/run_procflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         get_command_line_args_func = get_command_line_args
     # arglist=None allows all possible arguments.
     ARGS = get_command_line_args_func(
         arglist=None, description="Run data file processing"
     )
 
     COMMAND_LINE_ARGS = ARGS.__dict__
-    if COMMAND_LINE_ARGS.get("logging_level"):
+    if "logging_level" in COMMAND_LINE_ARGS.keys():
         LOG = setup_logging(logging_level=COMMAND_LINE_ARGS["logging_level"])
     else:
         LOG = setup_logging()
     LOG.info("RETRIEVED COMMAND LINE ARGUMENTS")
     LOG.interactive("\n\n\nStarting %s procflow...\n\n", COMMAND_LINE_ARGS["procflow"])
     import sys
```

### Comparing `geoips-1.12.2/geoips/commandline/update_tc_tracks_database.py` & `geoips-1.12.2a0/geoips/commandline/update_tc_tracks_database.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/create_plugin_registries.py` & `geoips-1.12.2a0/geoips/create_plugin_registries.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,21 +500,15 @@
         reporting them all at once, to facilitate rapidly identifying and
         resolving errors.
     """
     plugin = yaml.safe_load(open(filepath, mode="r"))
     plugin["relpath"] = relpath
     plugin["package"] = package
 
-    try:
-        interface_name = plugin["interface"]
-    except KeyError:
-        raise PluginRegistryError(
-            f"""No 'interface' level in '{filepath}'.
-                Ensure all required metadata is included."""
-        )
+    interface_name = plugin["interface"]
     interface_module = getattr(geoips.interfaces, f"{interface_name}")
 
     if interface_name not in plugins.keys():
         plugins[interface_name] = {}
 
     error_message = ""
     # If the current family is "list", make sure we loop through the list,
@@ -861,21 +855,14 @@
         "-s",
         "--save_type",
         type=str.lower,
         default="json",
         choices=["json", "yaml"],
         help="Format to write registries to. This will also be the file extension.",
     )
-    parser.add_argument(
-        "-p",
-        "--package_name",
-        type=str.lower,
-        default=None,
-        help="Package name to create registries for. If not specified, run on all.",
-    )
     return parser
 
 
 def main():
     """Generate all available plugins from all installed GeoIPS packages.
 
     After all plugins have been generated, they are written to registered_plugins.yaml
@@ -887,25 +874,19 @@
     args: list
         List of strings representing the arguments provided via command line.
     """
     parser = get_parser()
 
     ARGS = parser.parse_args()
     save_type = ARGS.save_type
-    package_name = ARGS.package_name
 
     LOG = setup_logging(logging_level="INTERACTIVE")
     # Note: Python 3.9 appears to return duplicates when installed with setuptools.
     # These are filtered within the create_plugin_registries function.
     plugin_packages = get_entry_point_group("geoips.plugin_packages")
-    if package_name:
-        for plugin_package in plugin_packages:
-            if plugin_package.name == package_name:
-                use_plugin_package = plugin_package
-        plugin_packages = [use_plugin_package]
     LOG.debug(plugin_packages)
     create_plugin_registries(plugin_packages, save_type)
     sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `geoips-1.12.2/geoips/data_manipulations/__init__.py` & `geoips-1.12.2a0/geoips/data_manipulations/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/data_manipulations/conversions.py` & `geoips-1.12.2a0/geoips/data_manipulations/conversions.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/data_manipulations/corrections.py` & `geoips-1.12.2a0/geoips/data_manipulations/corrections.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/data_manipulations/info.py` & `geoips-1.12.2a0/geoips/data_manipulations/info.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/data_manipulations/merge.py` & `geoips-1.12.2a0/geoips/data_manipulations/merge.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/dev/__init__.py` & `geoips-1.12.2a0/geoips/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/dev/output_config.py` & `geoips-1.12.2a0/geoips/dev/output_config.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/dev/product.py` & `geoips-1.12.2a0/geoips/dev/product.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/errors.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,26 +6,8 @@
 # # # This program is free software: you can redistribute it and/or modify it under
 # # # the terms of the NRLMMD License included with this program. This program is
 # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
-"""GeoIPS error module."""
-
-
-class PluginError(Exception):
-    """Exception to be raised when there is an error in a GeoIPS plugin."""
-
-    pass
-
-
-class PluginRegistryError(Exception):
-    """Exception to be raised when there is an error in a plugin registry."""
-
-    pass
-
-
-class CoverageError(Exception):
-    """Raise exception on data coverage error."""
-
-    pass
+"""Geoips interpolators utils init file."""
```

### Comparing `geoips-1.12.2/geoips/filenames/__init__.py` & `geoips-1.12.2a0/geoips/filenames/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/filenames/base_paths.py` & `geoips-1.12.2a0/geoips/filenames/base_paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,27 +176,32 @@
     PATHS["LOCALSCRATCH"] = getenv("LOCALSCRATCH").rstrip("/")
 
 if not getenv("SHAREDSCRATCH"):
     PATHS["SHAREDSCRATCH"] = PATHS["SCRATCH"]
 else:
     PATHS["SHAREDSCRATCH"] = getenv("SHAREDSCRATCH").rstrip("/")
 
-if not getenv("GEOIPS_ANCILDAT"):
-    PATHS["GEOIPS_ANCILDAT"] = pathjoin(PATHS["GEOIPS_OUTDIRS"], "ancildat")
-elif getenv("GEOIPS_ANCILDAT"):
-    PATHS["GEOIPS_ANCILDAT"] = getenv("GEOIPS_ANCILDAT").rstrip("/")
-# Separating the auto-generated files from the source files allows for
+# This is the default ANCILDATDIR specified in $GEOIPS/geoips/geoalgs/Makefile
+# These MUST match or geoalgs won't find ancildat files
+# (ANCILDATDIR gets built into fortran routines).
+# Used to be $GEOIPS/geoips/geoalgs/dat, but decided it shouldn't be relative to
+# source by default...
+# Also note I added GEOALGSAUTOGENDATA - these were going directly in ancildat
+# previously, which can get rather crowded with TCs and other dynamic sectors.
+# Also, separating the auto-generated files from the source files allows for
 # individual users to read from the shared ancildat, and write to their own
 # auto-generated location
-if not getenv("GEOIPS_ANCILDAT_AUTOGEN"):
-    PATHS["GEOIPS_ANCILDAT_AUTOGEN"] = pathjoin(
-        PATHS["GEOIPS_OUTDIRS"], "ancildat_autogen"
-    )
-elif getenv("GEOIPS_ANCILDAT_AUTOGEN"):
-    PATHS["GEOIPS_ANCILDAT_AUTOGEN"] = getenv("GEOIPS_ANCILDAT_AUTOGEN").rstrip("/")
+if not getenv("ANCILDATDIR"):
+    PATHS["ANCILDATDIR"] = pathjoin(PATHS["GEOIPS_OUTDIRS"], "ancildat")
+    PATHS["ANCILDATEXTERNAL"] = pathjoin(PATHS["GEOIPS_OUTDIRS"], "ancildat_external")
+    PATHS["ANCILDATAUTOGEN"] = pathjoin(PATHS["GEOIPS_OUTDIRS"], "ancildat_autogen")
+else:
+    PATHS["ANCILDATDIR"] = getenv("ANCILDATDIR").rstrip("/")
+    PATHS["ANCILDATEXTERNAL"] = pathjoin(getenv("ANCILDATDIR"), "external")
+    PATHS["ANCILDATAUTOGEN"] = pathjoin(getenv("ANCILDATDIR"), "autogen")
 
 if not getenv("LOGDIR"):
     PATHS["LOGDIR"] = pathjoin(PATHS["GEOIPS_OUTDIRS"], "logs")
 else:
     PATHS["LOGDIR"] = getenv("LOGDIR").rstrip("/")
 
 if not getenv("GEOIPSDATA"):
```

### Comparing `geoips-1.12.2/geoips/filenames/duplicate_files.py` & `geoips-1.12.2a0/geoips/filenames/duplicate_files.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/geoips_utils.py` & `geoips-1.12.2a0/geoips/geoips_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,34 +11,24 @@
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 """General high level utilities for geoips processing."""
 
 import os
 from copy import deepcopy
 import sys
-import inspect
 
 # import yaml
 import logging
 from importlib import metadata, resources
 
-from geoips.errors import PluginRegistryError
+from geoips.errors import EntryPointError, PluginRegistryError
 
 LOG = logging.getLogger(__name__)
 
-
-def remove_unsupported_kwargs(module, requested_kwargs):
-    """Remove unsupported keyword arguments."""
-    module_args = set(inspect.signature(module).parameters.keys())
-    unsupported = list(set(requested_kwargs.keys()).difference(module_args))
-    if "kwargs" not in module_args:
-        for key in unsupported:
-            LOG.warning("REMOVING UNSUPPORTED %s key %s", module, key)
-            requested_kwargs.pop(key)
-    return requested_kwargs
+NAMESPACE_PREFIX = "geoips"
 
 
 def get_entry_point_group(group):
     """Get entry point group."""
     # NOTE: When there is a .egg-info directory in the plugin package top
     # level (ie, from setuptools pip install -e), it seems to return that
     # package twice in this list.  For now, just use the full list with
@@ -117,14 +107,97 @@
                         registered_plugins["yaml_based"][interface],
                     )
         except TypeError:
             raise PluginRegistryError(f"Failed reading {pkg_plug_path}.")
     return yaml_plugins
 
 
+def find_entry_point(namespace, name, default=None):
+    """Find object matching 'name' using GEOIPS entry point namespace 'namespace'.
+
+    Automatically add 'geoips' prefix to namespace for disambiguation.
+
+    This is used in geoips.interfaces.base.get_plugin when "name" exists.
+    In that case, default is passed in as the full path, and is likely just
+    returned as the full path.  So the entry points in here probably are not
+    actually used, but the function is still required.
+
+    Parameters
+    ----------
+    namespace : str
+        Entry point namespace (e.g. 'readers')
+    name : str
+        Entry point name (e.g. 'amsr2_netcdf')
+    default : entry point, optional
+        Default value if no match is found.  If this is not set (i.e. None),
+        then no match will result in an exception
+    """
+    ep_namespace = ".".join([NAMESPACE_PREFIX, namespace])
+    for ep in get_entry_point_group(ep_namespace):
+        if ep.name == name:
+            resolved_ep = ep.load()
+            break
+    else:
+        resolved_ep = None
+    if resolved_ep is not None:
+        return resolved_ep
+    else:
+        if default is not None:
+            return default
+        else:
+            raise EntryPointError(
+                f"Failed to find object matching {name} in namespace {ep_namespace}"
+            )
+
+
+def get_all_entry_points(namespace):
+    """Return all entry points in GEOIPS entry point namespace 'namespace'.
+
+    Automatically add 'geoips' prefix to namespace for disambiguation.
+
+    Parameters
+    ----------
+    namespace :str
+        Entry point namespace (e.g. 'readers')
+    """
+    ep_namespace = ".".join([NAMESPACE_PREFIX, namespace])
+    retlist = []
+    # Do not use a list comprehension here so we can raise exceptions
+    # containing the actual package that errored.
+    try:
+        for ep in get_entry_point_group(ep_namespace):
+            try:
+                retlist += [ep.load()]
+            except Exception as resp:
+                raise EntryPointError(
+                    f"{resp}:"
+                    f"\nAn error occurred while loading entry point "
+                    f"'{ep.name}={ep.value}' entry point."
+                    f"\nTry checking to ensure init file exists in package subdir "
+                    f"\n(ALL directories containing python files MUST have init file)"
+                ) from resp
+    except KeyError:
+        retlist = []
+    return retlist
+
+
+def list_entry_points(namespace):
+    """List names of objects in GEOIPS entry point namespace 'namespace'.
+
+    Automatically add 'geoips' prefix to namespace for disambiguation.
+
+    Parameters
+    ----------
+    namespace :str
+        Entry point namespace (e.g. 'readers')
+    """
+    ep_namespace = ".".join([NAMESPACE_PREFIX, namespace])
+    return [ep.name for ep in get_entry_point_group(ep_namespace)]
+
+
 def copy_standard_metadata(orig_xarray, dest_xarray, extra_attrs=None, force=True):
     """Copy standard metadata from orig_xarray to dest_xarray.
 
     Parameters
     ----------
     orig_xarray : xarray.Dataset
         Original xarray to copy attributes from
@@ -344,43 +417,24 @@
         "data_provider",
         "start_datetime",
         "end_datetime",
     ]
     return required_xarray_attrs
 
 
-def merge_nested_dicts(dest, src, in_place=True, replace=False):
+def merge_nested_dicts(dest, src, in_place=True):
     """Perform an in-place merge of src into dest.
 
     Performs an in-place merge of src into dest while preserving any values that already
     exist in dest.
     """
     if not in_place:
         final_dest = deepcopy(dest)
     else:
         final_dest = dest
-
-    # NOTE: this is a top-level field, where if you set
-    # product_spec_override:
-    #   replace: true
-    # It will automatically replace ALL fields found in
-    # the original product spec and also found in the
-    # override with what is specified in the override
-    # in its entirety, without merging.  This is not
-    # terribly useful overall - we probably want this
-    # sort of capability in the end, but more flexible
-    # and able to be applied to only specific fields,
-    # etc.  This is a brute force method to at least
-    # allow overriding entire fields.
-    if replace:
-        for key in final_dest:
-            if key in src:
-                final_dest[key] = src[key]
-        return final_dest
-
     try:
         final_dest.update(src | final_dest)
     except (AttributeError, TypeError):
         return
     try:
         for key, val in final_dest.items():
             try:
```

### Comparing `geoips-1.12.2/geoips/image_utils/__init__.py` & `geoips-1.12.2a0/geoips/image_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/image_utils/colormap_utils.py` & `geoips-1.12.2a0/geoips/image_utils/colormap_utils.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/image_utils/maps.py` & `geoips-1.12.2a0/geoips/image_utils/maps.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/image_utils/mpl_utils.py` & `geoips-1.12.2a0/geoips/image_utils/mpl_utils.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/base.py` & `geoips-1.12.2a0/geoips/interfaces/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,33 @@
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 """Base classes for interfaces, plugins, and plugin validation machinery."""
 
 import yaml
 import inspect
 import logging
-from os.path import splitext
+from os.path import exists, splitext
 
 from importlib.resources import files
 from importlib import util
 from pathlib import Path
 import jsonschema
 import referencing
 from referencing import jsonschema as refjs
 from jsonschema.exceptions import ValidationError, SchemaError
 
-from geoips.errors import PluginError, PluginRegistryError
+from geoips.errors import EntryPointError, PluginError, PluginRegistryError
+
+from geoips.geoips_utils import (
+    find_entry_point,
+    # get_all_entry_points,
+    # load_all_yaml_plugins,
+)
+
+# from geoips.interfaces import product_defaults
 
 LOG = logging.getLogger(__name__)
 
 
 JSONSCHEMA_DRAFT = "202012"
 SCHEMA_PATH = files("geoips") / "schema"
 
@@ -700,32 +708,41 @@
 
         Raises
         ------
         PluginError
           If the specified plugin isn't found within the interface.
         """
         # Find the plugin module
-        # Convert the module into an object
-        registered_module_plugins = self.registered_module_based_plugins
-        if name not in registered_module_plugins[self.name]:
+        try:
+            if exists(name):
+                # This is used! For output checkers at least.
+                module = find_entry_point(self.name, name)
+            else:
+                registered_module_plugins = self.registered_module_based_plugins
+                package = registered_module_plugins[self.name][name]["package"]
+                relpath = registered_module_plugins[self.name][name]["relpath"]
+                module_path = splitext(relpath.replace("/", "."))[0]
+                module_path = f"{package}.{module_path}"
+                abspath = files(package) / relpath
+                spec = util.spec_from_file_location(module_path, abspath)
+                module = util.module_from_spec(spec)
+                spec.loader.exec_module(module)
+            # module = find_entry_point(self.name, name)
+        except EntryPointError as resp:
             raise PluginError(
-                f"Plugin '{name}', "
-                f"from interface '{self.name}' "
-                f"appears to not exist."
-                f"\nCreate plugin, then call create_plugin_registries?"
-            )
-
-        package = registered_module_plugins[self.name][name]["package"]
-        relpath = registered_module_plugins[self.name][name]["relpath"]
-        module_path = splitext(relpath.replace("/", "."))[0]
-        module_path = f"{package}.{module_path}"
-        abspath = files(package) / relpath
-        spec = util.spec_from_file_location(module_path, abspath)
-        module = util.module_from_spec(spec)
-        spec.loader.exec_module(module)
+                f"{resp}:\nPlugin '{name}' not found for '{self.name}' interface. "
+                f"\nCheck 'pyproject.toml' for typos, "
+                f"\nthat path in pyproject.toml matches path to '{name}' module, "
+                f"\ncheck top level attributes on module '{name}' "
+                f"(interface, family, name), "
+                f"\n and check that you are attempting to use the correct plugin name "
+                f"\n(ie, check in product YAMLs or command line that you are"
+                f" attempting to access the correct plugin name)"
+            ) from resp
+        # Convert the module into an object
         return self._plugin_module_to_obj(name, module)
 
     def get_plugins(self):
         """Get a list of plugins for this interface."""
         plugins = []
         # All plugin interfaces are explicitly imported in
         # geoips/interfaces/__init__.py
```

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/__init__.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/algorithms.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/algorithms.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/colormappers.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/colormappers.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/coverage_checkers.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/coverage_checkers.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/filename_formatters.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/filename_formatters.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/interpolators.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/interpolators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/output_checkers.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/output_checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from geoips.interfaces.base import (
     BaseModuleInterface,
     BaseModulePlugin,
     ValidationError,
 )
 import logging
+from geoips.errors import PluginError
 
 # import subprocess
 from geoips.commandline.log_setup import log_with_emphasis
 import gzip
 from glob import glob
 from os.path import exists, splitext, basename, dirname, isdir, join
 from os import makedirs, getenv
@@ -252,30 +253,26 @@
         with open(fname_rm, "w") as fobj:
             # Now loop through each missing product to write them to the file
             for missingproduct in missingproducts:
                 missingproduct_basename = basename(missingproduct)
                 for compare_product in compare_products:
                     # Pull the file that is actually used for comparison from
                     # the compare_products dictionary.
-                    file_for_comparison = compare_products[compare_product][
-                        "file_for_comparison"
-                    ]
-                    file_for_comparison_basename = basename(file_for_comparison)
+                    file_for_comparison_basename = basename(
+                        compare_products[compare_product]["file_for_comparison"]
+                    )
                     # If the basename of the current missing product matches the
                     # basename of the file for comparison, then write out the
                     # command to remove the actual stored comparison file from
                     # the test repo.
                     if missingproduct_basename == file_for_comparison_basename:
                         comparison_filename = compare_products[compare_product][
                             "stored_comparison"
                         ]
-                        fobj.write(f"  rm -v {comparison_filename}\n")
-                        LOG.interactive(f"    TEST OUTPUT: {comparison_filename}")
-                    else:
-                        LOG.interactive(f"    TEST OUTPUT: {file_for_comparison}")
+                        fobj.write(f"rm -v {comparison_filename}\n")
         # This is just for testing purposes - write out copy commands to
         # copy the missing product into a test location for easy review.
         with open(fname_missingprodcptest, "w") as fobj:
             fobj.write(f"mkdir {test_path}\n")
             for missingproduct in missingproducts:
                 # For display purposes - tifs are easier to view
                 test_basename = basename(missingproduct).replace(".jif", ".tif")
@@ -349,16 +346,15 @@
         test_path = join(diffdir, "MISSINGCOMPARE")
         with open(fname_cp, "w") as fobj:
             for missingcomp in missingcomps:
                 # We are passing the missingcomp directly to the diff dir
                 # We have no knowledge if these should be gzipped or not,
                 # so they are just copied as is.  Developers must manually
                 # gzip before commiting if desired.
-                fobj.write(f"  cp -v {missingcomp} {comparison_path}\n")
-                LOG.interactive(f"    CURR OUTPUT: {missingcomp}")
+                fobj.write(f"cp -v {missingcomp} {comparison_path}\n")
         with open(fname_missingcompcptest, "w") as fobj:
             fobj.write(f"mkdir {test_path}\n")
             for missingcomp in missingcomps:
                 # For display purposes - tifs are easier to view
                 test_basename = basename(missingcomp).replace(".jif", ".tif")
                 test_filename = join(test_path, test_basename)
                 fobj.write(f"cp -v {missingcomp} {test_filename}\n")
@@ -1017,18 +1013,23 @@
                 checker_name = output_checker.module.name
                 break
         if not checker_found:
             raise TypeError("There isn't an output checker built for this data type.")
         return checker_name
 
     def get_plugin(self, name):
-        """Return the output checker plugin corresponding to checker_name."""
-        plug = super().get_plugin(name)
-        if self.valid_plugin(plug):
-            return plug
+        """Get the output checker plugin corresponding to checker_name and return it."""
+        try:
+            plug = super().get_plugin(name)
+            if self.valid_plugin(plug):
+                return plug
+        except PluginError:
+            plug = super().get_plugin(self.identify_checker(name))
+            if self.valid_plugin(plug):
+                return plug
 
     def valid_plugin(self, plugin):
         """Check the validity of the supplied output_checker plugin."""
         if (
             not hasattr(plugin.module, "outputs_match")
             or not hasattr(plugin.module, "correct_file_format")
             or not hasattr(plugin.module, "call")
```

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/output_formatters.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/output_formatters.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/procflows.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/procflows.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/readers.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/readers.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/sector_adjusters.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/sector_adjusters.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/sector_metadata_generators.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/sector_metadata_generators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/sector_spec_generators.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/sector_spec_generators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/module_based/title_formatters.py` & `geoips-1.12.2a0/geoips/interfaces/module_based/title_formatters.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/yaml_based/__init__.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/yaml_based/feature_annotators.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/feature_annotators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/yaml_based/gridline_annotators.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/gridline_annotators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/yaml_based/product_defaults.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/product_defaults.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/interfaces/yaml_based/products.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/products.py`

 * *Files 12% similar despite different names*

```diff
@@ -125,32 +125,16 @@
             override_args = {}
             # If available, use the current product's override values
             if name in product_spec_override:
                 override_args = product_spec_override[name]
             # Otherwise, if "all" specified, use those override values
             elif "all" in product_spec_override:
                 override_args = product_spec_override["all"]
-            replace_arg = False
-            # NOTE: this is a top-level field, where if you set
-            # product_spec_override:
-            #   spec:
-            #     replace: true
-            # It will automatically replace ALL fields found in
-            # the original product spec and also found in the
-            # override with what is specified in the override
-            # in its entirety, without merging.  This is not
-            # terribly useful overall - we probably want this
-            # sort of capability in the end, but more flexible
-            # and able to be applied to only specific fields,
-            # etc.  This is a brute force method to at least
-            # allow overriding entire fields.
-            if product_spec_override.get("replace"):
-                replace_arg = True
             prod_plugin["spec"] = merge_nested_dicts(
-                prod_plugin["spec"], override_args, in_place=False, replace=replace_arg
+                prod_plugin["spec"], override_args, in_place=False
             )
 
         return prod_plugin
 
     def get_plugins(self):
         """Retrieve a plugin by name."""
         plugins = []
```

### Comparing `geoips-1.12.2/geoips/interfaces/yaml_based/sectors.py` & `geoips-1.12.2a0/geoips/interfaces/yaml_based/sectors.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,31 +74,28 @@
             ad = load_area(abspath, "spec")
         # elif self.family.startswith("center"):
         #     ad = center_to_area_definition(self)
         # elif self.family.startswith("corners"):
         #     ad = corners_to_area_definition(self)
         return ad
 
-    def create_test_plot(self, fname, return_fig_ax_map=False):
+    def create_test_plot(self, fname):
         """Create a test PNG image for this sector."""
         from geoips.image_utils.mpl_utils import create_figure_and_main_ax_and_mapobj
         from cartopy import feature as cfeature
 
         fig, ax, mapobj = create_figure_and_main_ax_and_mapobj(
             self.area_definition.shape[1],
             self.area_definition.shape[0],
             self.area_definition,
             noborder=True,
         )
         ax.add_feature(cfeature.COASTLINE)
         ax.add_feature(cfeature.BORDERS)
-        if fname is not None:
-            fig.savefig(fname)
-        if return_fig_ax_map:
-            return fig, ax, mapobj
+        fig.savefig(fname)
 
 
 class SectorsInterface(BaseYamlInterface):
     """Interface for sector plugins."""
 
     name = "sectors"
     plugin_class = SectorPluginBase
```

### Comparing `geoips-1.12.2/geoips/plugin_registry.py` & `geoips-1.12.2a0/geoips/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/__init__.py` & `geoips-1.12.2a0/geoips/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/RGB_Default.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_GeoIPS1.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,54 +6,70 @@
 # # # This program is free software: you can redistribute it and/or modify it under
 # # # the terms of the NRLMMD License included with this program. This program is
 # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
-"""Data manipulation steps for "Night_Vis_IR" product.
+"""Data manipulation steps for "Night_Vis" product, GeoIPS 1 Version.
 
-This algorithm expects two VIIRS channels (DNBRad and M16BT) for a RGB image
+This algorithm expects one VIIRS channel (DNBRad) for a single channel image.
 """
 import logging
+from geoips.data_manipulations.corrections import mask_day
+from geoips.data_manipulations.corrections import apply_data_range, apply_gamma
 
 LOG = logging.getLogger(__name__)
 
 interface = "algorithms"
 family = "list_numpy_to_numpy"
-name = "RGB_Default"
+name = "Night_Vis_GeoIPS1"
 
 
-def call(arrays):
-    """Apply default RGB algorithm.
+def call(arrays, min_outbounds="crop", max_outbounds="crop", max_night_zen=90):
+    """Night Vis product algorithm data manipulation steps, GeoIPS 1 version.
 
-    Plots RGB with the red gun being the first variable specified in the
-    product YAML, green second, and blue third.
-
-    Note this is currently entirely unused, and is included here for
-    reference/completeness.  Eventually we may want to fully support
-    this generalized RGB default algorithm, where you can pass in
-    ranges, channel combinations, etc for RGB output, but for now it
-    will ONLY plot arrays 0, 1, 2 as red, green, blue respectively,
-    with no adjustments/combinations.
+    This algorithm expects DNBRad in reflectance, and returns the adjusted
+    array.
 
     Parameters
     ----------
     arrays : list of numpy.ndarray
         * list of numpy.ndarray or numpy.MaskedArray of channel data,
             in order of sensor "channels" list
+        * Degrees Kelvin
 
     Returns
     -------
     numpy.ndarray
-        numpy.ndarray or numpy.MaskedArray of qualitative RGBA image output
+        numpy.ndarray or numpy.MaskedArray of adjusted DNB output.
+
+    Notes
+    -----
+    It will generate a product in daytime if we do not apply the daytime check.
+    For now, it is for both day/night.
+
+    We will decide whether this product is only for nighttime.
+    If so, a daytime check will be required.
+
+    We may focus only on nighttime product with moonlight after additional
+    validation (TBD).
     """
-    red = arrays[0]  # Red gun: First listed variable
-    grn = arrays[1]  # Green gun: Second listed variable
-    blu = arrays[2]  # Blue gun: Third listed variable
+    data = arrays[0]
+    sun_zenith = arrays[1]
+
+    data = mask_day(data, sun_zenith, max_night_zen)
 
-    from geoips.image_utils.mpl_utils import alpha_from_masked_arrays, rgba_from_arrays
+    data_range1 = [5.0e-10, 2.5e-8]
 
-    alp = alpha_from_masked_arrays([red, grn, blu])
-    rgba = rgba_from_arrays(red, grn, blu, alp)
+    data = apply_data_range(
+        data,
+        min_val=data_range1[0],
+        max_val=data_range1[1],
+        min_outbounds=min_outbounds,
+        max_outbounds=max_outbounds,
+        norm=True,
+        inverse=False,
+    )
+    data = apply_gamma(data, 2.0)
 
-    return rgba
+    return data
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/pmw_37pct.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_37pct.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/pmw_89pct.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_89pct.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/pmw_color37.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color37.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/pmw_tb/pmw_color89.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/pmw_tb/pmw_color89.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/sfc_winds/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/sfc_winds/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/sfc_winds/windbarbs.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/sfc_winds/windbarbs.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/single_channel.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/single_channel.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/visir/Night_Vis.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/visir/Night_Vis_GeoIPS1.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR_GeoIPS1.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,70 +6,107 @@
 # # # This program is free software: you can redistribute it and/or modify it under
 # # # the terms of the NRLMMD License included with this program. This program is
 # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
-"""Data manipulation steps for "Night_Vis" product, GeoIPS 1 Version.
+"""Data manipulation steps for "Night_Vis_IR" product, GeoIPS 1 Version.
 
-This algorithm expects one VIIRS channel (DNBRad) for a single channel image.
+This algorithm expects two VIIRS channels (DNBRad and M16BT) for a RGB image
 """
 import logging
 from geoips.data_manipulations.corrections import mask_day
-from geoips.data_manipulations.corrections import apply_data_range, apply_gamma
 
 LOG = logging.getLogger(__name__)
 
 interface = "algorithms"
 family = "list_numpy_to_numpy"
-name = "Night_Vis_GeoIPS1"
+name = "Night_Vis_IR_GeoIPS1"
 
 
-def call(arrays, min_outbounds="crop", max_outbounds="crop", max_night_zen=90):
-    """Night Vis product algorithm data manipulation steps, GeoIPS 1 version.
+def call(arrays, max_night_zen=90):
+    """Night Vis IR RGB product algorithm data manipulation steps.
 
-    This algorithm expects DNBRad in reflectance, and returns the adjusted
-    array.
+    This algorithm expects DNBRad in reflectance and M16BT
+    Brightness Temperatures in units of degrees Kelvin,
+    and returns red green and blue gun arrays.
 
     Parameters
     ----------
     arrays : list of numpy.ndarray
         * list of numpy.ndarray or numpy.MaskedArray of channel data,
             in order of sensor "channels" list
         * Degrees Kelvin
 
     Returns
     -------
     numpy.ndarray
-        numpy.ndarray or numpy.MaskedArray of adjusted DNB output.
+        numpy.ndarray or numpy.MaskedArray of qualitative RGBA image output
 
     Notes
     -----
     It will generate a product in daytime if we do not apply the daytime check.
     For now, it is for both day/night.
 
     We will decide whether this product is only for nighttime.
     If so, a daytime check will be required.
 
     We may focus only on nighttime product with moonlight after additional
     validation (TBD).
     """
-    data = arrays[0]
-    sun_zenith = arrays[1]
-
-    data = mask_day(data, sun_zenith, max_night_zen)
-
-    data_range1 = [5.0e-10, 2.5e-8]
+    ch1 = arrays[0]  # Red gun: DNBRad
+    ch2 = arrays[0]  # Green gun: DNBRad
+    ch3 = arrays[1]  # Blue gun: M16BT (200-300K)
+    sun_zenith = arrays[2]
+
+    ch1 = mask_day(ch1, sun_zenith, max_night_zen)
+    ch2 = mask_day(ch2, sun_zenith, max_night_zen)
+    ch3 = mask_day(ch3, sun_zenith, max_night_zen)
+
+    data_range1 = [0, 2.5e-8]
+    data_range2 = [200, 300]
+
+    from geoips.data_manipulations.corrections import apply_data_range, apply_gamma
+
+    red = ch1
+    red = apply_data_range(
+        red,
+        min_val=data_range1[0],
+        max_val=data_range1[1],
+        min_outbounds="crop",
+        max_outbounds="crop",
+        norm=True,
+        inverse=False,
+    )  # need inverse option?
+    red = apply_gamma(red, 2.0)
 
-    data = apply_data_range(
-        data,
+    grn = ch2
+    grn = apply_data_range(
+        grn,
         min_val=data_range1[0],
         max_val=data_range1[1],
-        min_outbounds=min_outbounds,
-        max_outbounds=max_outbounds,
+        min_outbounds="crop",
+        max_outbounds="crop",
         norm=True,
         inverse=False,
     )
-    data = apply_gamma(data, 2.0)
+    grn = apply_gamma(grn, 2.0)
+
+    blu = ch3
+    blu = apply_data_range(
+        blu,
+        min_val=data_range2[0],
+        max_val=data_range2[1],
+        min_outbounds="crop",
+        max_outbounds="crop",
+        norm=True,
+        inverse=True,
+    )  # create image of deep clouds in blueish color
+    blu = apply_gamma(blu, 1.2)
+
+    from geoips.image_utils.mpl_utils import alpha_from_masked_arrays, rgba_from_arrays
+
+    alp = alpha_from_masked_arrays([red, grn, blu])
+    rgba = rgba_from_arrays(red, grn, blu, alp)
 
-    return data
+    return rgba
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/visir/Night_Vis_IR.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/Night_Vis_IR.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/algorithms/visir/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/algorithms/visir/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/cmap_rgb.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/cmap_rgb.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/matplotlib_linear_norm.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/matplotlib_linear_norm.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_150H.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_150H.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Legacy.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Legacy.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Physical.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37H_Physical.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_37pct.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_37pct.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89HW.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89HW.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Legacy.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Legacy.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Physical.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89H_Physical.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_89pct.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_89pct.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/pmw_tb/cmap_Rain.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/pmw_tb/cmap_Rain.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/tpw/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/tpw/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/tpw/tpw_pwat.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/tpw/tpw_pwat.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/visir/IR_BD.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/IR_BD.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/visir/Infrared.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/Infrared.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/visir/WV.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/WV.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         (-40, -35),
         (-35, -30),
         (-30, -20),
         (-20, -10),
         (-10, -0.1),
         (-0.1, max_tb),
     ]
-    # LOG.info("inside util= ", max_tb)
+    LOG.info("inside util= ", max_tb)
 
     # matching TerraScan Color scheme: noaa_bd_151
     transition_colors = [
         ("#800000", "#800000"),
         ("#820200", "#FFB266"),
         ("#FFB266", "#FFFF7B"),
         ("#FFFF80", "#66FFB2"),
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/visir/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/visir/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/winds/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/winds/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/colormappers/winds/wind_radii_transitions.py` & `geoips-1.12.2a0/geoips/plugins/modules/colormappers/winds/wind_radii_transitions.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/coverage_checkers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/coverage_checkers/center_radius.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/center_radius.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/coverage_checkers/center_radius_rgba.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/center_radius_rgba.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/coverage_checkers/masked_arrays.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/masked_arrays.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/coverage_checkers/numpy_arrays_nan.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/numpy_arrays_nan.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/coverage_checkers/rgba.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/rgba.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/coverage_checkers/windbarbs.py` & `geoips-1.12.2a0/geoips/plugins/modules/coverage_checkers/windbarbs.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/basic_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/basic_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/geoips_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geoips_fname.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     coverage=None,
     output_type="png",
     output_type_dir=None,
     product_dir=None,
     product_subdir=None,
     source_dir=None,
     basedir=gpaths["ANNOTATED_IMAGERY_PATH"],
-    output_dict=None,
 ):
     """Create GeoIPS standard filenames, sector-based subdirs.
 
     This uses the sector specification (continent, country, area, subarea,
     state, city), product name, source name, and platform name
     to generate a full unique path, as well as additional attributes to
     create a fully unique file name.
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/geoips_netcdf_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geoips_netcdf_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/geotiff_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/geotiff_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/metadata_default_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/metadata_default_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/tc_clean_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/tc_clean_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/tc_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/tc_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/text_winds_day_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_day_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/text_winds_full_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_full_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/text_winds_tc_fname.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/text_winds_tc_fname.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/utils/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/filename_formatters/utils/tc_file_naming.py` & `geoips-1.12.2a0/geoips/plugins/modules/filename_formatters/utils/tc_file_naming.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 from glob import glob
 from os.path import basename as pathbasename
 from os.path import join as pathjoin
 from geoips.interfaces import products
 
 LOG = logging.getLogger(__name__)
 
-# interface = None indicates to the GeoIPS interfaces that this is not a valid
-# plugin, and this module will not be added to the GeoIPS plugin registry.
-# This allows including python modules within the geoips/plugins directory
-# that provide helper or utility functions to the geoips plugins, but are
-# not full GeoIPS plugins on their own.
 interface = None
 
 
 def get_storm_subdir(
     basin_path, base_tc_stormname, tc_stormnum, output_dict, sector_info
 ):
     """Get the TC storm subdirectory."""
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/pyresample_wrappers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_gauss.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_gauss.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import xarray
 
 from geoips.plugins.modules.interpolators.utils.interp_pyresample import (
     interp_kd_tree,
     get_data_box_definition,
 )
-from geoips.geoips_utils import copy_standard_metadata, remove_unsupported_kwargs
+from geoips.geoips_utils import copy_standard_metadata
 
 LOG = logging.getLogger(__name__)
 
 interface = "interpolators"
 family = "2d"
 name = "interp_gauss"
 
@@ -33,15 +33,14 @@
     area_def,
     input_xarray,
     output_xarray,
     varlist,
     array_num=None,
     sigmaval=None,
     drop_nan=False,
-    **kwargs,
 ):
     """Pyresample interp_kd_tree gaussian interpolation GeoIPS plugin."""
     LOG.info(
         "Interpolating using standard scifile register method: "
         "kd_tree gauss sigmaval %s",
         sigmaval,
     )
@@ -93,23 +92,21 @@
     data_box_definition = get_data_box_definition(input_xarray.source_name, lons, lats)
 
     # Set s default value of igmaval as 10000
 
     if sigmaval is None:
         sigmaval = 10000
 
-    kd_kwargs = remove_unsupported_kwargs(interp_kd_tree, kwargs)
     interp_data = interp_kd_tree(
         vars_to_interp,
         area_def,
         data_box_definition,
         input_xarray.interpolation_radius_of_influence,
         interp_type="gauss",
         sigmas=sigmaval,
-        **kd_kwargs,
     )
     if output_xarray is None:
         output_xarray = xarray.Dataset()
     if "latitude" not in output_xarray.variables.keys():
         interp_lons, interp_lats = area_def.get_lonlats()
         output_xarray["latitude"] = xarray.DataArray(interp_lats)
         output_xarray["longitude"] = xarray.DataArray(interp_lons)
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_nearest.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/pyresample_wrappers/interp_nearest.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import xarray
 
 from geoips.plugins.modules.interpolators.utils.interp_pyresample import (
     interp_kd_tree,
     get_data_box_definition,
 )
 from geoips.data_manipulations.info import percent_unmasked
-from geoips.geoips_utils import copy_standard_metadata, remove_unsupported_kwargs
+from geoips.geoips_utils import copy_standard_metadata
 
 LOG = logging.getLogger(__name__)
 
 interface = "interpolators"
 family = "2d"
 name = "interp_nearest"
 
@@ -45,15 +45,15 @@
         LOG.info("    USING AREA_DEF X ROI of %s", roi)
     if area_def.pixel_size_y > roi:
         roi = area_def.pixel_size_y
         LOG.info("    USING AREA_DEF Y ROI of %s", roi)
     return roi
 
 
-def call(area_def, input_xarray, output_xarray, varlist, array_num=None, **kwargs):
+def call(area_def, input_xarray, output_xarray, varlist, array_num=None):
     """Pyresample interp_kd_tree nearest neighbor GeoIPS plugin."""
     LOG.info(
         "Interpolating nearest using standard scifile register method: kd_tree nearest"
     )
 
     roi = get_final_roi(input_xarray, area_def)
 
@@ -86,22 +86,16 @@
         lats = input_xarray["latitude"].to_masked_array()
         for varname in varlist:
             vars_to_interp += [input_xarray[varname].to_masked_array()]
 
     # Use standard scifile / pyresample registration
     data_box_definition = get_data_box_definition(input_xarray.source_name, lons, lats)
 
-    kd_kwargs = remove_unsupported_kwargs(interp_kd_tree, kwargs)
     interp_data = interp_kd_tree(
-        vars_to_interp,
-        area_def,
-        data_box_definition,
-        float(roi),
-        interp_type="nearest",
-        **kd_kwargs,
+        vars_to_interp, area_def, data_box_definition, float(roi), interp_type="nearest"
     )
 
     for arr, orig, varname in zip(interp_data, vars_to_interp, varlist):
         LOG.info("%s min/max before: %s to %s", varname, orig.min(), orig.max())
         LOG.info("%s min/max after:  %s to %s", varname, arr.min(), arr.max())
         LOG.info("%s Percent unmasked before %s", varname, percent_unmasked(orig))
         LOG.info("%s Percent unmasked after  %s", varname, percent_unmasked(arr))
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/scipy_wrappers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/scipy_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/scipy_wrappers/interp_grid.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/scipy_wrappers/interp_grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,16 +41,16 @@
             lats = input_xarray["latitude"].to_masked_array()
             var_to_interp = input_xarray[varname].to_masked_array()
 
         min_gridlon = area_def.area_extent_ll[0]
         max_gridlon = area_def.area_extent_ll[2]
         min_gridlat = area_def.area_extent_ll[1]
         max_gridlat = area_def.area_extent_ll[3]
-        numx_grid = area_def.width
-        numy_grid = area_def.height
+        numx_grid = area_def.pixel_size_x
+        numy_grid = area_def.pixel_size_y
 
         interp_datas += [
             interp_griddata(
                 var_to_interp,
                 lons,
                 lats,
                 min_gridlon,
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/utils/__init__.py` & `geoips-1.12.2a0/geoips/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 # # # This program is free software: you can redistribute it and/or modify it under
 # # # the terms of the NRLMMD License included with this program. This program is
 # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
-"""Geoips interpolators utils init file."""
+"""Geoips utilities init file."""
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/utils/boxdefinitions.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/boxdefinitions.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/utils/interp_pyresample.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/interp_pyresample.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,14 @@
 import logging
 
 import numpy
 from pyresample import kd_tree
 
 LOG = logging.getLogger(__name__)
 
-# interface = None indicates to the GeoIPS interfaces that this is not a valid
-# plugin, and this module will not be added to the GeoIPS plugin registry.
-# This allows including python modules within the geoips/plugins directory
-# that provide helper or utility functions to the geoips plugins, but are
-# not full GeoIPS plugins on their own.
 interface = None
 
 
 def get_data_box_definition(source_name, lons, lats):
     """Obtain pyresample geometry definitions.
 
     For use with pyresample based reprojections
@@ -100,25 +95,21 @@
     sigmas : int, default=None
         Used for interp_type 'gauss' - multiplication factor for sigmas option:
             * sigmas = [sigmas]*len(list_of_arrays)
     """
     dstacked_arrays = numpy.ma.dstack(list_of_arrays)
 
     if interp_type == "nearest":
-        kw_args = {}
-        kw_args["fill_value"] = None
-        kw_args["radius_of_influence"] = radius_of_influence
-        if nprocs is not None:
-            kw_args["nprocs"] = nprocs
         LOG.info("Using interp_type %s", interp_type)
         dstacked_arrays = kd_tree.resample_nearest(
             data_box_definition,
             dstacked_arrays,
             area_definition,
-            **kw_args,
+            radius_of_influence=radius_of_influence,
+            fill_value=None,
         )
     elif interp_type == "gauss":
         kw_args = {}
         kw_args["sigmas"] = [4000] * len(list_of_arrays)
         kw_args["fill_value"] = None
         kw_args["radius_of_influence"] = radius_of_influence
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/interpolators/utils/interp_scipy.py` & `geoips-1.12.2a0/geoips/plugins/modules/interpolators/utils/interp_scipy.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 
 # from matplotlib import cm, colors
 import scipy
 import numpy
 
 LOG = logging.getLogger(__name__)
 
-# interface = None indicates to the GeoIPS interfaces that this is not a valid
-# plugin, and this module will not be added to the GeoIPS plugin registry.
-# This allows including python modules within the geoips/plugins directory
-# that provide helper or utility functions to the geoips plugins, but are
-# not full GeoIPS plugins on their own.
 interface = None
 
 
 def interp_gaussian_kde(data_lons, data_lats, target_lons, target_lats, vw_method=None):
     """
     Interpolate a given array of non-uniform data using scipy.stats.gaussian_kde.
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_checkers/geotiff.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_checkers/geotiff.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_checkers/image.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_checkers/image.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_checkers/netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_checkers/netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_checkers/text.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_checkers/text.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/full_disk_image.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/full_disk_image.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/geotiff_standard.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/geotiff_standard.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/histogram_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/netcdf_geoips.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,58 +6,36 @@
 # # # This program is free software: you can redistribute it and/or modify it under
 # # # the terms of the NRLMMD License included with this program. This program is
 # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
-"""Produce histogram from the given dataset with specified bin size."""
+"""Geoips style NetCDF output format."""
 import logging
-import numpy
 
 LOG = logging.getLogger(__name__)
 
 interface = "output_formatters"
 family = "xarray_data"
-name = "histogram_json"
+name = "netcdf_geoips"
 
 
-def call(
-    xarray_obj, product_names, output_fnames, min_val=None, max_val=None, num_bins=501
-):
-    """Produce histogram.
-
-    Parameters
-    ----------
-    xarray_obj: xarray Dataset
-
-    Returns
-    -------
-    xarray.Dataset
-        Resulting histogram
-    """
+def call(xarray_obj, product_names, output_fnames):
+    """Write GeoIPS style NetCDF to disk."""
     import xarray
 
     prod_xarray = xarray.Dataset()
 
     from geoips.geoips_utils import copy_standard_metadata
 
     copy_standard_metadata(xarray_obj, prod_xarray)
     for product_name in product_names:
         prod_xarray[product_name] = xarray_obj[product_name]
 
-        if product_name == "latitude" or product_name == "longitude":
-            continue
-        xda = xarray_obj[product_name]
-        hist = numpy.histogram(xda, numpy.linspace(min_val, max_val, num_bins + 1))
-        prod_xarray[f"{product_name}_histogram"] = xarray.DataArray(
-            hist[0], dims=("dim_2")
-        )
-        prod_xarray["bins"] = xarray.DataArray(hist[1], dims=("dim_3"))
-
     from geoips.plugins.modules.output_formatters.netcdf_xarray import (
         write_xarray_netcdf,
     )
 
     for ncdf_fname in output_fnames:
         write_xarray_netcdf(prod_xarray, ncdf_fname)
     return output_fnames
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/imagery_annotated.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_annotated.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/imagery_clean.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_clean.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/imagery_windbarbs.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_windbarbs.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/imagery_windbarbs_clean.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/imagery_windbarbs_clean.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/metadata_default.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/metadata_default.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/metadata_tc.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/metadata_tc.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/netcdf_xarray.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/netcdf_xarray.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/text_winds.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/text_winds.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/output_formatters/unprojected_image.py` & `geoips-1.12.2a0/geoips/plugins/modules/output_formatters/unprojected_image.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/procflows/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/procflows/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/procflows/config_based.py` & `geoips-1.12.2a0/geoips/plugins/modules/procflows/config_based.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,15 @@
 from geoips.utils.memusg import print_mem_usage
 from geoips.geoips_utils import output_process_times
 from geoips.dev.product import (
     get_covg_from_product,
     get_covg_args_from_product,
     get_required_variables,
 )
-from geoips.xarray_utils.data import (
-    sector_xarrays,
-    combine_preproc_xarrays_with_alg_xarray,
-)
+from geoips.xarray_utils.data import sector_xarrays
 from geoips.filenames.duplicate_files import remove_duplicates
 from geoips.geoips_utils import replace_geoips_paths
 from geoips.utils.context_managers import import_optional_dependencies
 
 with import_optional_dependencies(loglevel="info"):
     """Attempt to import a package and print to LOG.info if the import fails."""
     from geoips_db.utils.database_writes import (
@@ -63,16 +60,14 @@
     pad_area_definition,
     add_filename_extra_field,
     get_area_defs_from_command_line_args,
     plot_data,
     combine_filename_extra_fields,
     get_alg_xarray,
     verify_area_def,
-    remove_unsupported_kwargs,
-    get_unique_dataset_key,
 )
 
 # Moved to top-level errors module, fixing issue #67
 from geoips.errors import CoverageError
 
 PMW_NUM_PIXELS_X = 1400
 PMW_NUM_PIXELS_Y = 1400
@@ -222,15 +217,14 @@
         "Getting background xarray dataset for product '%s'", prod_plugin.name
     )
     if "interpolator" in prod_plugin["spec"]:
         interp_plugin = interpolators.get_plugin(
             prod_plugin["spec"]["interpolator"]["plugin"]["name"]
         )
         interp_args = prod_plugin["spec"]["interpolator"]["plugin"]["arguments"]
-        interp_args = remove_unsupported_kwargs(interp_plugin, interp_args)
 
     alg_xarray = None
 
     # If this is a preprocessed data file with the final product in it,
     # just pull the final product. Must take out METADATA dataset!
     if (
         len(set(sect_xarrays.keys()).difference({"METADATA"})) == 1
@@ -383,31 +377,36 @@
     """
     compare_path = None
     if command_line_args is not None and command_line_args["compare_path"] is not None:
         compare_path = command_line_args["compare_path"]
 
     # If this config has a compare_path specified, replace variables appropriately
     if "compare_path" in output_dict or compare_path is not None:
+        if "compare_outputs_module" in output_dict:
+            compare_outputs_module = output_dict["compare_outputs_module"]
+        else:
+            compare_outputs_module = "compare_outputs"
 
         if compare_path is None:
             compare_path = output_dict["compare_path"]
 
         cpath = (
             compare_path.replace("<product>", product_name)
             .replace("<procflow>", "config_based")
             .replace("<output>", output_type)
         )
     # If there is no comparison specified, identify as "no_comparison"
     else:
         cpath = "no_comparison"
+        compare_outputs_module = "no_compare_outputs_module"
 
-    return cpath
+    return cpath, compare_outputs_module
 
 
-def initialize_final_products(final_products, cpath):
+def initialize_final_products(final_products, cpath, cmodule):
     """Initialize the final_products dictionary with cpath dict key if needed.
 
     Parameters
     ----------
     final_products : dict
         Dictionary of final products, with keys of final required "compare_path"
         Products with no compare_path specified are stored with the key
@@ -422,14 +421,15 @@
         final_products[cpath]['files'] = <list_of_files_in_given_cpath>
     """
     if cpath not in final_products:
         final_products[cpath] = {}
         # This is where we store all the files
         final_products[cpath]["files"] = []
         final_products[cpath]["database writes"] = []
+        final_products[cpath]["compare_outputs_module"] = cmodule
 
     return final_products
 
 
 def process_unsectored_data_outputs(
     final_products,
     available_outputs_dict,
@@ -488,22 +488,23 @@
                 if output_dict["requested_sector_type"] == sector_type:
                     # Now we will produce all of the individual products for the given
                     # output_type/sector_type
                     for product_name in output_dict["product_names"]:
                         # This grabs the compare_path that was requested in the YAML
                         # config, and replaces all instances of <product> with
                         # product_name and all instances of <output> with output_type
-                        cpath = set_comparison_path(
+                        cpath, cmodule = set_comparison_path(
                             output_dict, product_name, output_type, command_line_args
                         )
                         # This adds "cpath" to the final_products dictionary, if
                         # necessary
                         final_products = initialize_final_products(
-                            final_products, cpath
+                            final_products, cpath, cmodule
                         )
+                        final_products[cpath]["compare_outputs_module"] = cmodule
 
                         # This actually produces all the required output files for the
                         # current produsct
                         prod_plugin = products.get_plugin(
                             xobjs["METADATA"].source_name,
                             product_name,
                             output_dict.get("product_spec_override"),
@@ -950,20 +951,14 @@
 
     if command_line_args.get("product_db_writer_override"):
         for sector, database_writer in command_line_args[
             "product_db_writer_override"
         ].items():
             config_dict["available_sectors"][sector] = database_writer
 
-    if command_line_args.get("composite_output_kwargs_override"):
-        for sector_output, kwargs in command_line_args[
-            "composite_output_kwargs_override"
-        ].items():
-            config_dict["outputs"][sector_output]["composite_kwargs"] = kwargs
-
     if bg_files is not None:
         LOG.interactive(
             "Reading background datasets using reader '%s'...", bg_reader_plugin.name
         )
         bg_xobjs = bg_reader_plugin(bg_files, metadata_only=True, **bg_reader_kwargs)
         prod_plugin = products.get_plugin(
             bg_xobjs["METADATA"].source_name,
@@ -1372,21 +1367,24 @@
                             area_def,
                             curr_variables,
                             config_dict["available_sectors"][sector_type][
                                 "adjust_variables"
                             ],
                         )
 
-                cpath = set_comparison_path(
+                cpath, cmodule = set_comparison_path(
                     config_dict["available_sectors"][sector_type],
                     product_name="archer",
                     output_type="archer",
                     command_line_args=command_line_args,
                 )
-                final_products = initialize_final_products(final_products, cpath)
+                final_products = initialize_final_products(
+                    final_products, cpath, cmodule
+                )
+                final_products[cpath]["compare_outputs_module"] = cmodule
                 final_products[cpath]["files"] += adadj_fnames
 
                 LOG.info(
                     "\n\n\n\nAFTER ADJUSTMENT area definition: %s\n\n\n\n", area_def
                 )
 
             print_mem_usage("MEMUSG", verbose=False)
@@ -1519,18 +1517,21 @@
                     if not set(product_variables).issubset(all_vars):
                         LOG.interactive(
                             "SKIPPING product %s missing variables %s",
                             product_name,
                             set(product_variables).difference(all_vars),
                         )
                         continue
-                    cpath = set_comparison_path(
+                    cpath, cmodule = set_comparison_path(
                         output_dict, product_name, output_type, command_line_args
                     )
-                    final_products = initialize_final_products(final_products, cpath)
+                    final_products = initialize_final_products(
+                        final_products, cpath, cmodule
+                    )
+                    final_products[cpath]["compare_outputs_module"] = cmodule
 
                     # Produce sectored data output
                     LOG.interactive(
                         "Processing sectored data products for product '%s'",
                         prod_plugin.name,
                     )
                     curr_output_products = process_sectored_data_output(
@@ -1567,34 +1568,20 @@
                         # If we're saving out intermediate data file, write out
                         # pad_area_def.
                         if product_name not in pad_alg_xarrays:
                             pad_alg_xarrays[product_name] = get_alg_xarray(
                                 pad_sect_xarrays,
                                 pad_area_def,
                                 prod_plugin,
-                                processed_xarrays=pad_alg_xarrays,
                                 resector=presector_data,
                                 resampled_read=resampled_read,
                                 variable_names=product_variables,
                                 window_start_time=window_start_time,
                                 window_end_time=window_end_time,
                             )
-                        else:
-                            LOG.info(
-                                "  product %s already in pad_alg_xarrays", product_name
-                            )
-                            LOG.info(
-                                "  pad_alg_xarrays datasets: %s",
-                                list(pad_alg_xarrays.keys()),
-                            )
-                            LOG.info(
-                                "  pad_alg_xarrays[%s] datasets: %s",
-                                product_name,
-                                list(pad_alg_xarrays[product_name].variables.keys()),
-                            )
                         alg_xarray = pad_alg_xarrays[product_name]
                     elif area_def.sector_type in ["reader_defined", "self_register"]:
                         alg_xarray = get_alg_xarray(
                             pad_sect_xarrays,
                             pad_area_def,
                             prod_plugin,
                             resector=False,
@@ -1607,39 +1594,20 @@
                         # If we're writing out an image, cut it down to the desired
                         # size.
                         if product_name not in alg_xarrays:
                             alg_xarrays[product_name] = get_alg_xarray(
                                 sect_xarrays,
                                 area_def,
                                 prod_plugin,
-                                processed_xarrays=alg_xarrays,
                                 resector=presector_data,
                                 resampled_read=resampled_read,
                                 variable_names=product_variables,
                                 window_start_time=window_start_time,
                                 window_end_time=window_end_time,
                             )
-                            # This is a unique identifier so we can re-use variables
-                            # and product arrays appropriately.
-                            area_def_key = get_unique_dataset_key(
-                                area_def, alg_xarrays[product_name]
-                            )
-                            alg_xarrays[area_def_key] = alg_xarrays[product_name]
-                        else:
-                            LOG.info(
-                                "  product %s already in alg_xarrays", product_name
-                            )
-                            LOG.info(
-                                "  alg_xarrays datasets: %s", list(alg_xarrays.keys())
-                            )
-                            LOG.info(
-                                "  alg_xarrays[%s] datasets: %s",
-                                product_name,
-                                list(alg_xarrays[product_name].variables.keys()),
-                            )
                         alg_xarray = alg_xarrays[product_name]
 
                     covg_plugin = get_covg_from_product(
                         prod_plugin,
                         covg_field="image_production_coverage_checker",
                     )
                     covg_args = get_covg_args_from_product(
@@ -1713,65 +1681,14 @@
                     if covg < minimum_coverage and fname_covg < minimum_coverage:
                         LOG.interactive(
                             "Insufficient coverage %s / %s for data products, SKIPPING",
                             covg,
                             fname_covg,
                         )
                         continue
-                    composite_kwargs = output_dict.get("composite_kwargs", {})
-                    if composite_kwargs.get("composite_products"):
-                        from geoips.utils.composite import find_preproc_alg_files
-
-                        # Required kwargs for generating composite
-                        comp_settings = output_dict["composite_kwargs"]
-                        reader = readers.get_plugin(
-                            comp_settings["composite_input_file_reader"]
-                        )
-                        comp_file_format = comp_settings["composite_input_file_format"]
-                        composite_window = comp_settings["composite_window"]
-
-                        # Optional kwargs for generating composite
-                        db_query_plugin = comp_settings.get("database_query_module")
-                        db_kwargs = config_dict["available_sectors"][sector_type].get(
-                            "product_database_writer_kwargs", {}
-                        )
-                        db_schemas = db_kwargs.get("schema_name")
-                        db_tables = db_kwargs.get("table_name")
-
-                        preproc_files = find_preproc_alg_files(
-                            product_time=alg_xarray.start_datetime,
-                            composite_window=composite_window,
-                            sector_name=area_def.area_id,
-                            product=product_name,
-                            sensor=alg_xarray.source_name,
-                            platform=alg_xarray.platform_name,
-                            file_format=comp_file_format,
-                            product_db=product_db,
-                            db_query_plugin=db_query_plugin,
-                            db_schemas=db_schemas,
-                            db_tables=db_tables,
-                        )
-                        if preproc_files:
-                            pre_proc = reader(preproc_files)
-                            if (
-                                "rgb"
-                                in prod_plugin["spec"]["colormapper"]["plugin"]["name"]
-                            ):
-                                rgb_var = prod_plugin.name
-                            else:
-                                rgb_var = None
-                            alg_xarray = combine_preproc_xarrays_with_alg_xarray(
-                                pre_proc, alg_xarray, rgb_var=rgb_var
-                            )
-                            comp_covg = covg_plugin(
-                                alg_xarray, covg_varname, area_def, **covg_args
-                            )
-                            LOG.info("Composite coverage: %s", comp_covg)
-                        else:
-                            LOG.info("No files to create composite!")
 
                     plot_data_kwargs = get_output_formatter_kwargs(
                         output_dict,
                         alg_xarray,
                         area_def,
                         sector_type,
                         bg_files,
@@ -1838,16 +1755,15 @@
     retval = 0
     failed_compares = {}
     for cpath in final_products:
         if cpath != "no_comparison":
             from geoips.interfaces.module_based.output_checkers import output_checkers
 
             for output_product in final_products[cpath]["files"]:
-                plugin_name = output_checkers.identify_checker(output_product)
-                output_checker = output_checkers.get_plugin(plugin_name)
+                output_checker = output_checkers.get_plugin(output_product)
                 kwargs = {}
                 if output_checker.name in output_checker_kwargs:
                     kwargs = output_checker_kwargs[output_checker.name]
                 curr_retval = output_checker(
                     output_checker,
                     cpath,
                     [output_product],
@@ -1878,15 +1794,15 @@
             successful_comparison_dirs = successful_comparison_dirs + 1
         for filename in final_products[cpath]["files"]:
             LOG.interactive(
                 "    \u001b[34mCONFIGSUCCESS\033[0m %s",
                 replace_geoips_paths(filename, curly_braces=True),
             )
             if filename in final_products[cpath]["database writes"]:
-                LOG.interactive("    DATABASESUCCESS %s", filename)
+                LOG.info("    DATABASESUCCESS %s", filename)
         LOG.info("\n")
 
     for removed_product in removed_products:
         LOG.interactive("    DELETEDPRODUCT %s", removed_product)
         if product_db:
             LOG.info("    FLAGGING as deleted in product database")
             flag_product_as_deleted(removed_product, area_defs)
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/procflows/single_source.py` & `geoips-1.12.2a0/geoips/plugins/modules/procflows/single_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -201,587 +201,24 @@
             "metadata_filename_formatter": metadata_filename_formatter,
             "metadata_filename_formatter_kwargs": metadata_filename_formatter_kwargs,
             "product_name": prod_plugin.name,
         }
     return output_fnames, metadata_fnames
 
 
-def add_attrs_from_area_def(final_xarray, source_xarray, area_def):
-    """Add attributes from an area_def."""
-    # MLS I think this should actually just be final_xarray and final_xarray,
-    # no source_xarray!  We might be losing information...
-    # Ensure we have the "adjustment"id" in the filename appropriately
-    if "adjustment_id" in area_def.sector_info:
-        final_xarray = add_filename_extra_field(
-            source_xarray, "adjustment_id", area_def.sector_info["adjustment_id"]
-        )
-    return final_xarray
-
-
-def resector_xarrays(
-    resector, sect_xarrays, area_def, variables, window_start_time, window_end_time
-):
-    """Resector xarrays if requested."""
-    # If the initial sectoring was to a padded area definition, must sector to final
-    # area_def here.
-    # Allow specifying whether it needs to be resectored or not via kwargs.
-    if resector:
-        LOG.interactive("Resectoring xarrays without padding...")
-        curr_sect_xarrays = sector_xarrays(
-            sect_xarrays,
-            area_def,
-            varlist=variables,
-            hours_before_sector_time=6,
-            hours_after_sector_time=9,
-            drop=True,
-            window_start_time=window_start_time,
-            window_end_time=window_end_time,
-        )
-        # hours_before_sector_time=6, hours_after_sector_time=6, drop=True)
-    else:
-        curr_sect_xarrays = sect_xarrays
-    return curr_sect_xarrays
-
-
-def get_interp_plugin_from_product(prod_plugin):
-    """Get the interpolator plugin from the product spec.
-
-    Reassign interp_plugin based on CURRENT sect_xarray
-    Allow re-defining interpolation for different datasets.
-    """
-    interp_plugin = None
-    if "interpolator" in prod_plugin["spec"]:
-        interp_plugin = interpolators.get_plugin(
-            prod_plugin["spec"]["interpolator"]["plugin"]["name"]
-        )
-        interp_args = prod_plugin["spec"]["interpolator"]["plugin"]["arguments"]
-        interp_args = remove_unsupported_kwargs(interp_plugin, interp_args)
-    return interp_plugin, interp_args
-
-
-def apply_interp_first(
-    variables,
-    curr_sect_xarrays,
-    prod_plugin,
-    datasets_for_vars,
-    resampled_read,
-    area_def,
-    processed_xarrays,
-):
-    """Apply interpolation first.
-
-    For product types that involve interpolation before algorithm.
-    """
-    # Default to empty xarray.Dataset() - will be populated within loop with
-    # appropriate regridded variables.
-    interp_xarray = xarray.Dataset()
-    for varname in variables:
-        LOG.info("TRYING variable %s", varname)
-        for key, sect_xarray in curr_sect_xarrays.items():
-            LOG.info("    TRYING dataset %s for variable %s", key, varname)
-
-            if varname not in sect_xarray.variables:
-                continue
-
-            # Determine which interpolator to use based on the product definition.
-            interp_plugin, interp_args = get_interp_plugin_from_product(prod_plugin)
-
-            # Check if a specific dataset was specified for the current variable,
-            # and ensure we are pulling the variable from the correct dataset.
-            if not use_variable_from_current_dataset(
-                varname,
-                key,
-                variables,
-                sect_xarray,
-                interp_xarray,
-                resampled_read,
-                datasets_for_vars,
-            ):
-                continue
-
-            # Potential efficiency hit with to_masked_array for dask arrays, etc
-            # LOG.info('Min/max %s %s / %s, dataset %s',
-            #          varname,
-            #          sect_xarray[varname].to_masked_array().min(),
-            #          sect_xarray[varname].to_masked_array().max(),
-            #          key)
-
-            # It is much faster to interpolate all variables at once than
-            # one at a time. Since we can assume "variables" is all of the
-            # requested variables, just interpolate them all the first time
-            # through, and add logic to NOT reinterpolate variables if they've
-            # already been interpolated.
-            # For reference, with 11 variables, it was 1 min 13s
-            # to interpolate individually, 22s in one call.
-            interp_args["varlist"] = variables
-            if "time_dim" in sect_xarray.dims:
-                # This is for a particularly formatted dataset, that includes
-                # separate arrays for different times (ABI fire product).
-                # We need to be careful this does not break for some other
-                # dataset that includes a differently formatted "time"
-                # dimension.
-                tdims = len(sect_xarray.time_dim)
-
-                interp_list = []
-                for i in range(tdims):
-                    interp_list.append(
-                        perform_interpolation(
-                            interp_plugin,
-                            area_def,
-                            sect_xarray.isel(time_dim=i),
-                            xarray.Dataset(),
-                            interp_args,
-                            processed_xarrays,
-                        )
-                    )
-
-                interp_xarray[varname] = xarray.concat(interp_list, dim="dim_2")[
-                    varname
-                ]
-            else:
-                interp_xarray = perform_interpolation(
-                    interp_plugin,
-                    area_def,
-                    sect_xarray,
-                    interp_xarray,
-                    interp_args,
-                    processed_xarrays,
-                )
-
-            # Potential efficiency hit with to_masked_array for dask arrays, etc
-            # LOG.info('Min/max interp %s %s / %s',
-            #          varname,
-            #          interp_xarray[varname].to_masked_array().min(),
-            #          interp_xarray[varname].to_masked_array().max())
-    return interp_xarray
-
-
-def use_variable_from_current_dataset(
-    varname,
-    key,
-    variables,
-    sect_xarray,
-    interp_xarray,
-    resampled_read,
-    datasets_for_vars,
-):
-    """Use the variable from the current dataset.
-
-    If a specific dataset was requested for the current variable, and
-    this dataset was NOT requested via a resampled_read (in which case
-    the native datasets won't exist, only the resampled dataset),
-    then use the appropriately requested dataset.
-    """
-    if varname in datasets_for_vars and not resampled_read:
-        if key in datasets_for_vars[varname]:
-            LOG.info(
-                "        USING %s varname from dataset %s, as specified in "
-                "product_input YAML config",
-                varname,
-                key,
-            )
-        else:
-            LOG.info(
-                "        WAITING dataset %s not requested for variable %s in "
-                "product_input YAML config",
-                key,
-                varname,
-            )
-            return False
-    # If we've already interpolated this variable, check if it is needed
-    # before interpolating again
-    elif interp_xarray is not None and varname in list(interp_xarray.keys()):
-        # If all of the required variables are in the current dataset, use this
-        # version
-        if set(variables).issubset(set(sect_xarray.variables.keys())):
-            LOG.info(
-                "        REPLACING %s with current dataset %s, all required "
-                "variables in current dataset",
-                varname,
-                key,
-            )
-        # Otherwise, skip re-interpolating to avoid unecessary computation
-        else:
-            LOG.warning(
-                "        SKIPPING %s, encountered multiple versions, skipping "
-                "subsequent dataset %s",
-                varname,
-                key,
-            )
-            return False
-    else:
-        LOG.info(
-            "        USING %s varname from dataset %s - first availalbe, and "
-            "not specified in YAML",
-            varname,
-            key,
-        )
-    return True
-
-
-def get_alg_and_interp_plugins(prod_plugin):
-    """Get algorithm and interpolator plugins from prod_plugin definition."""
-    # Only attempt to set algorithm function if algorithm requested in product type
-    try:
-        alg_args = prod_plugin["spec"]["algorithm"]["plugin"]["arguments"]
-        alg_plugin = algorithms.get_plugin(
-            prod_plugin["spec"]["algorithm"]["plugin"]["name"]
-        )
-    except KeyError:
-        alg_args = None
-        alg_plugin = None
-
-    try:
-        interp_args = prod_plugin["spec"]["interpolator"]["plugin"]["arguments"]
-        interp_plugin = interpolators.get_plugin(
-            prod_plugin["spec"]["interpolator"]["plugin"]["name"]
-        )
-        interp_args = remove_unsupported_kwargs(interp_plugin, interp_args)
-    except KeyError:
-        interp_args = None
-        interp_plugin = None
-    return alg_plugin, alg_args, interp_plugin, interp_args
-
-
-def apply_alg_after_interp(
-    interp_xarray,
-    area_def,
-    alg_plugin,
-    alg_args,
-    prod_plugin,
-    variables,
-    processed_xarrays,
-):
-    """Apply algorithm after interpolation.
-
-    MLS need to add ability here to pull from processed_xarrays if algorithm
-    was already applied.
-    """
-    if processed_xarrays and prod_plugin.name in processed_xarrays:
-        return processed_xarrays[prod_plugin.name]
-    # Specify the call signature and return value for different algorithm types:
-    if prod_plugin.family in ["interpolator"]:
-        # Note "interp" product type will NOT have a single variable named
-        # "product_name", just the individual interpolated variables.
-        interp_xarray = interp_xarray
-    elif alg_plugin.family in ["xarray_to_numpy"]:
-        # xarray_to_numpy will return a single array, which can be set to the
-        # "product_name" variable.
-        LOG.interactive(
-            "  Applying '%s' family algorithm '%s' to data...",
-            alg_plugin.family,
-            alg_plugin.name,
-        )
-        interp_xarray[prod_plugin.name] = xarray.DataArray(
-            alg_plugin(interp_xarray, **alg_args)
-        )
-    elif alg_plugin.family in ["xarray_to_xarray"]:
-        # xarray_to_xarray algorithm type will return the full xarray object -
-        # assume variable names have been set appropriately within the
-        # algorithm.  This could be another good use of the
-        # "alt_varname_for_covg" kwarg in the coverage checks - if we want to
-        # just use a specific variable for the coverage checks rather than the
-        # "product_name" variable.
-        LOG.interactive(
-            "  Applying '%s' family algorithm '%s' to data...",
-            alg_plugin.family,
-            alg_plugin.name,
-        )
-        interp_xarray = alg_plugin(
-            interp_xarray, variables, prod_plugin.name, **alg_args
-        )
-    elif alg_plugin.family in [
-        "single_channel",
-        "channel_combination",
-        "list_numpy_to_numpy",
-        "rgb",
-    ]:
-        # Assume ANYTHING else takes in a list of numpy arrays, and returns a
-        # single numpy array.
-        # Perhaps we should be explicit here...
-        LOG.interactive(
-            "  Applying '%s' family algorithm '%s' to data...",
-            alg_plugin.family,
-            alg_plugin.name,
-        )
-        interp_xarray[prod_plugin.name] = xarray.DataArray(
-            alg_plugin(
-                [interp_xarray[varname].to_masked_array() for varname in variables],
-                **alg_args,
-            )
-        )
-    else:
-        raise TypeError(
-            f"UNSUPPORTED algorithm family '{alg_plugin.family}' or product family "
-            f"'{prod_plugin.family}', please add to the single_source procflow's "
-            "'get_alg_xarray' function appropriately"
-        )
-    return interp_xarray
-
-
-def apply_alg_first(
-    alg_plugin,
-    alg_args,
-    prod_plugin,
-    curr_sect_xarrays,
-    sect_xarrays,
-    variables,
-    variable_names,
-    area_def,
-):
-    """Apply algorithm appropriately based on algorithm family.
-
-    MLS
-    Inexplicably some of these use curr_sect_xarrays, and some use sect_xarrays.
-    Also, some use variables and some use variable_names.
-    I am guessing there is no reason for the difference, but maintaining the
-    original functionality for now.
-    """
-    alg_xarray = xarray.Dataset()
-    alg_xarray.attrs = sect_xarrays["METADATA"].attrs.copy()
-    if alg_plugin.family in ["xarray_to_numpy"]:
-        # Why does this one use sect_xarrays and not curr_sect_xarrays?
-        # And it uses variable_names, not variables.
-        alg_xarray = apply_alg_xarray_to_numpy(
-            alg_xarray, alg_plugin, alg_args, prod_plugin, sect_xarrays, variable_names
-        )
-    elif alg_plugin.family in ["xarray_dict_area_def_to_numpy"]:
-        # Why does this one use sect_xarrays and not curr_sect_xarrays?
-        alg_xarray = apply_alg_xarray_dict_area_def_to_numpy(
-            alg_xarray, alg_plugin, alg_args, prod_plugin, sect_xarrays, area_def
-        )
-    elif alg_plugin.family in ["xarray_dict_to_xarray"]:
-        # This one uses sect_xarrays
-        alg_xarray = apply_alg_xarray_dict_to_xarray(alg_plugin, alg_args, sect_xarrays)
-    elif alg_plugin.family in ["xarray_to_xarray"]:
-        # This one uses variables, not variable_names
-        alg_xarray = apply_alg_xarray_to_xarray(
-            alg_plugin, alg_args, prod_plugin, sect_xarrays, variables
-        )
-    elif alg_plugin.family in ["list_numpy_to_numpy"]:
-        # Why does this one use curr_sect_xarrays and not sect_xarrays?
-        # And variables, not variable_names ?
-        alg_xarray = apply_alg_list_numpy_to_numpy(
-            alg_xarray,
-            alg_plugin,
-            alg_args,
-            prod_plugin,
-            curr_sect_xarrays,
-            variables,
-        )
-    return alg_xarray
-
-
-def apply_interp_after_alg(
-    alg_xarray, interp_plugin, interp_args, prod_plugin, area_def, processed_xarrays
-):
-    """Apply interpolation after algorithm."""
-    # No interpolation required
-    if prod_plugin.family in ["algorithm", "algorithm_colormapper"]:
-        final_xarray = alg_xarray
-    # If required, interpolate the result prior to returning
-    elif prod_plugin.family == "algorithm_interpolator_colormapper":
-        interp_args["varlist"] = [prod_plugin.name]
-        final_xarray = perform_interpolation(
-            interp_plugin,
-            area_def,
-            alg_xarray,
-            alg_xarray,
-            interp_args,
-            processed_xarrays,
-        )
-    return final_xarray
-
-
-def apply_alg_xarray_to_xarray(
-    alg_plugin, alg_args, prod_plugin, sect_xarrays, variable_names
-):
-    """Apply xarray_to_xarray algorithm."""
-    input_alg_xarray = None
-    for varname in variable_names:
-        LOG.info("TRYING variable %s for non-interpolated algorithms", varname)
-        for curr_sect_xarray in sect_xarrays.values():
-            if varname in curr_sect_xarray:
-                if input_alg_xarray is None:
-                    LOG.info(
-                        "    USING sectored xarray %s for non-interpolated "
-                        "algorithms",
-                        curr_sect_xarray,
-                    )
-                    input_alg_xarray = curr_sect_xarray
-                else:
-                    LOG.info(
-                        "    SKIPPING For non-interpolated data processing, "
-                        "all native variables must be the same resolution! "
-                        "Skipping variable %s, shape %s, input_alg_xarrays: %s",
-                        varname,
-                        curr_sect_xarray[varname].shape,
-                        input_alg_xarray,
-                    )
-    if input_alg_xarray is None:
-        raise ValueError(
-            "No required variables in any xarrays for 'xarray_to_xarray' "
-            "algorithm type"
-        )
-    LOG.interactive(
-        "  Applying '%s' family algorithm '%s' to data...",
-        alg_plugin.family,
-        alg_plugin.name,
-    )
-    alg_xarray = alg_plugin(
-        input_alg_xarray, variable_names, prod_plugin.name, **alg_args
-    )
-    return alg_xarray
-
-
-def apply_alg_xarray_dict_to_xarray(alg_plugin, alg_args, sect_xarrays):
-    """Apply xarray_dict_to_xarray algorithm."""
-    # Format the call signature for passing a dictionary of xarrays,
-    # plus area_def, and return a single numpy array
-    LOG.interactive(
-        "  Applying '%s' family algorithm '%s' to data...",
-        alg_plugin.family,
-        alg_plugin.name,
-    )
-    alg_xarray = alg_plugin(sect_xarrays, **alg_args)
-    return alg_xarray
-
-
-def apply_alg_xarray_dict_area_def_to_numpy(
-    alg_xarray, alg_plugin, alg_args, prod_plugin, sect_xarrays, area_def
-):
-    """Apply xarray_dict_area_def_to_numpy algorithm."""
-    # Format the call signature for passing a dictionary of xarrays,
-    # plus area_def, and return a single numpy array
-    LOG.interactive(
-        "  Applying '%s' family algorithm '%s' to data...",
-        alg_plugin.family,
-        alg_plugin.name,
-    )
-    alg_xarray[prod_plugin.name] = xarray.DataArray(
-        alg_plugin(sect_xarrays, area_def, **alg_args)
-    )
-    return alg_xarray
-
-
-def apply_alg_xarray_to_numpy(
-    alg_xarray, alg_plugin, alg_args, prod_plugin, sect_xarrays, variable_names
-):
-    """Apply xarray_to_numpy algorithm."""
-    # Format the call signature for passing a dictionary of xarrays,
-    # plus area_def, and return a single numpy array
-    for dsname in sect_xarrays.keys():
-        if set(variable_names).issubset(set(sect_xarrays[dsname].variables.keys())):
-            LOG.interactive(
-                "  Applying '%s' family algorithm '%s' to data...",
-                alg_plugin.family,
-                alg_plugin.name,
-            )
-            alg_xarray[prod_plugin.name] = xarray.DataArray(
-                alg_plugin(sect_xarrays[dsname], **alg_args)
-            )
-    return alg_xarray
-
-
-def apply_alg_list_numpy_to_numpy(
-    alg_xarray, alg_plugin, alg_args, prod_plugin, sect_xarrays, variables
-):
-    """Apply list_numpy_to_numpy algorithm."""
-    # Need to pull all the required variables out of the various xarray datasets
-    # and add them to numpy list.
-    # Then assign the resulting numpy array to the "product_name" DataArray
-    # within the xarray Dataset
-    numpys = []
-    for varname in variables:
-        for curr_sect_xarray in sect_xarrays.values():
-            if varname in list(curr_sect_xarray.variables.keys()):
-                numpys += [curr_sect_xarray[varname].to_masked_array()]
-                alg_xarray = curr_sect_xarray
-    LOG.interactive(
-        "  Applying '%s' family algorithm '%s' to data...",
-        alg_plugin.family,
-        alg_plugin.name,
-    )
-    alg_xarray[prod_plugin.name] = xarray.DataArray(alg_plugin(numpys, **alg_args))
-    return alg_xarray
-
-
-def perform_interpolation(
-    interp_plugin, area_def, sect_xarray, interp_xarray, interp_args, processed_xarrays
-):
-    """Perform standard interpolation."""
-    interp_args, interp_xarray = select_variables_to_interp(
-        interp_args, area_def, sect_xarray, interp_xarray, processed_xarrays
-    )
-    LOG.interactive(
-        "  Interpolating data with interpolator '%s' args '%s'...",
-        interp_plugin.name,
-        interp_args,
-    )
-    # Only attempt to interpolate if there are required variables left.
-    if interp_args["varlist"]:
-        interp_xarray = interp_plugin(
-            area_def, sect_xarray, interp_xarray, **interp_args
-        )
-    else:
-        LOG.info("No variables to interpolate, returning interp_xarray unchanged.")
-    return interp_xarray
-
-
-def get_unique_dataset_key(area_def, xobj):
-    """Get a unique id for xarray dataset."""
-    standard_attrs = (
-        f"{xobj.attrs['start_datetime']}_"
-        f"{xobj.attrs['end_datetime']}_"
-        f"{xobj.attrs['platform_name']}_"
-        f"{xobj.attrs['source_name']}"
-    )
-    return f"{area_def.area_id}_{hash(area_def)}_{standard_attrs}"
-
-
-def select_variables_to_interp(
-    interp_args, area_def, source_xarray, interp_xarray, processed_xarrays
-):
-    """Select interpolation variables."""
-    curr_available_vars = set(list(source_xarray.variables.keys()))
-    already_interped_vars = set(list(interp_xarray.variables.keys()))
-    all_requested_vars = set(interp_args["varlist"])
-    curr_requested_vars = curr_available_vars.intersection(all_requested_vars)
-    interp_vars = curr_requested_vars.difference(already_interped_vars)
-    final_interp_vars = list(interp_vars)
-    # This is a unique identifier so we can re-use variables
-    # and product arrays appropriately.
-    area_def_key = get_unique_dataset_key(area_def, source_xarray)
-    if processed_xarrays and area_def_key in processed_xarrays:
-        LOG.info(
-            "  Area def '%s' in processed_xarrays, "
-            "with variables '%s', using existing array, "
-            "in place of interp_xarray '%s'.",
-            area_def_key,
-            list(processed_xarrays[area_def_key].variables.keys()),
-            interp_xarray,
-        )
-        # Just add to this existing array
-        interp_xarray = processed_xarrays[area_def_key]
-        final_interp_vars = []
-        for varname in interp_vars:
-            if varname not in processed_xarrays[area_def_key].variables.keys():
-                final_interp_vars += [varname]
-    interp_args["varlist"] = final_interp_vars
-    return interp_args, interp_xarray
-
-
 def remove_unsupported_kwargs(module, requested_kwargs):
     """Remove unsupported keyword arguments."""
-    module_args = set(inspect.signature(module).parameters.keys())
-    unsupported = list(set(requested_kwargs.keys()).difference(module_args))
-    if "kwargs" not in module_args:
-        for key in unsupported:
-            LOG.warning("REMOVING UNSUPPORTED %s key %s", module, key)
-            requested_kwargs.pop(key)
+    unsupported = list(
+        set(requested_kwargs.keys()).difference(
+            set(inspect.signature(module).parameters.keys())
+        )
+    )
+    for key in unsupported:
+        LOG.warning("REMOVING UNSUPPORTED %s key %s", module, key)
+        requested_kwargs.pop(key)
     return requested_kwargs
 
 
 def add_filename_extra_field(xarray_obj, field_name, field_value):
     """Add filename extra field."""
     if "filename_extra_fields" not in xarray_obj.attrs:
         xarray_obj.attrs["filename_extra_fields"] = {}
@@ -1064,15 +501,14 @@
     alg_xarray used for filename formats, etc.
     If included, fused_xarray_dict used for output format call
     """
     # If keyword argument is allowed for output function, include it
     output_kwargs["output_dict"] = output_dict
     output_formatter = get_output_formatter(output_dict)
     output_plugin = output_formatters.get_plugin(output_formatter)
-    output_kwargs = remove_unsupported_kwargs(output_plugin, output_kwargs)
     exclude_platforms = prod_plugin["spec"].get("exclude_platforms")
     include_platforms = prod_plugin["spec"].get("include_platforms")
     if exclude_platforms and alg_xarray.platform_name in exclude_platforms:
         LOG.interactive(
             "SKIPPING Platform %s not requested for product '%s'"
             "Excluded platforms: '%s'...",
             alg_xarray.platform_name,
@@ -1111,15 +547,14 @@
             output_plugin.family,
             output_plugin.name,
         )
         output_products = output_plugin(
             xarray_obj=alg_xarray,
             product_names=[prod_plugin.name, "latitude", "longitude"],
             output_fnames=list(output_fnames.keys()),
-            **output_kwargs,
         )
         if output_products != list(output_fnames.keys()):
             raise ValueError("Did not produce expected products")
     else:
         mpl_colors_info = None
         if "colormapper" in prod_plugin["spec"]:
             cmap_plugin = colormappers.get_plugin(
@@ -1323,30 +758,22 @@
             "area_definition" in xobjs[self_register_dataset].attrs
             and xobjs[self_register_dataset].attrs["area_definition"] is not None
         ):
             area_def = xobjs[self_register_dataset].attrs["area_definition"]
         else:
             import pyresample
 
-            orig_lons = xobjs[self_register_dataset]["longitude"]
-            lons = pyresample.utils.wrap_longitudes(orig_lons)
             area_def = pyresample.geometry.SwathDefinition(
-                lons=lons,
+                lons=xobjs[self_register_dataset]["longitude"],
                 lats=xobjs[self_register_dataset]["latitude"],
             )
             min_lat = xobjs[self_register_dataset]["latitude"].min()
             max_lat = xobjs[self_register_dataset]["latitude"].max()
             min_lon = xobjs[self_register_dataset]["longitude"].min()
             max_lon = xobjs[self_register_dataset]["longitude"].max()
-            if max_lon > 180 and min_lon < 180:
-                min_lon = lons.where(lons > 0).min()
-                max_lon = lons.where(lons < 0).max()
-            else:
-                min_lon = lons.min()
-                max_lon = lons.max()
             area_def.area_extent_ll = [min_lon, min_lat, max_lon, max_lat]
             if (
                 "interpolation_radius_of_influence"
                 in xobjs[self_register_dataset].attrs
             ):
                 area_def.pixel_size_x = xobjs[self_register_dataset].attrs[
                     "interpolation_radius_of_influence"
@@ -1434,15 +861,14 @@
     return list(area_defs)
 
 
 def get_alg_xarray(
     sect_xarrays,
     area_def,
     prod_plugin,
-    processed_xarrays=None,
     resector=True,
     resampled_read=False,
     variable_names=None,
     window_start_time=None,
     window_end_time=None,
 ):
     """Get alg xarray.
@@ -1480,128 +906,368 @@
     else:
         # If variable_names are passed, actually use them
         # Previously was only being used for checking existence of variables in
         # sectored xarray.
         variables = variable_names
 
     LOG.interactive("Applying algorithms and interpolation...")
-
     datasets_for_vars = get_requested_datasets_for_variables(prod_plugin)
 
-    # Get the algorithm and interpolator plugins we need to use, based
-    # on the contents of prod_plugin.
-    alg_plugin, alg_args, interp_plugin, interp_args = get_alg_and_interp_plugins(
-        prod_plugin
-    )
+    # Only attempt to set algorithm function if algorithm requested in product type
+    try:
+        alg_args = prod_plugin["spec"]["algorithm"]["plugin"]["arguments"]
+        alg_plugin = algorithms.get_plugin(
+            prod_plugin["spec"]["algorithm"]["plugin"]["name"]
+        )
+    except KeyError:
+        alg_args = None
+        alg_plugin = None
 
-    # Re-sector the xarrays if requested.
-    curr_sect_xarrays = resector_xarrays(
-        resector, sect_xarrays, area_def, variables, window_start_time, window_end_time
-    )
+    try:
+        interp_args = prod_plugin["spec"]["interpolator"]["plugin"]["arguments"]
+        interp_plugin = interpolators.get_plugin(
+            prod_plugin["spec"]["interpolator"]["plugin"]["name"]
+        )
+    except KeyError:
+        interp_args = None
+        interp_plugin = None
+
+    # If the initial sectoring was to a padded area definition, must sector to final
+    # area_def here.
+    # Allow specifying whether it needs to be resectored or not via kwargs.
+    if resector:
+        LOG.interactive("Resectoring xarrays without padding...")
+        curr_sect_xarrays = sector_xarrays(
+            sect_xarrays,
+            area_def,
+            varlist=variables,
+            hours_before_sector_time=6,
+            hours_after_sector_time=9,
+            drop=True,
+            window_start_time=window_start_time,
+            window_end_time=window_end_time,
+        )
+        # hours_before_sector_time=6, hours_after_sector_time=6, drop=True)
+    else:
+        curr_sect_xarrays = sect_xarrays
 
     LOG.info("get_alg_xarray required variables: %s", variables)
     LOG.info("get_alg_xarray requested datasets for variables: %s", datasets_for_vars)
 
     # If we want to run the algorithm prior to interpolation, apply the algorithm here,
     # and return either the unprojected result or interpolated result appropriately.
     if prod_plugin.family in [
         "algorithm_colormapper",
         "algorithm_interpolator_colormapper",
         "algorithm",
     ]:
-        # All of these apply the algorithm first, so go ahead and
-        # apply the algorithm.
-        # Some use variables and some use variable_names... So pass both.
-        # Some use curr_sect_xarrays and some use sect_xarrays... So pass both.
-        # MLS I'm guessing this random selection is not right.
-        alg_xarray = apply_alg_first(
-            alg_plugin,
-            alg_args,
-            prod_plugin,
-            curr_sect_xarrays,
-            sect_xarrays,
-            variables,
-            variable_names,
-            area_def,
-        )
+        alg_xarray = xarray.Dataset()
+        alg_xarray.attrs = sect_xarrays["METADATA"].attrs.copy()
+        if alg_plugin.family in ["xarray_to_numpy"]:
+            # Format the call signature for passing a dictionary of xarrays,
+            # plus area_def, and return a single numpy array
+            for dsname in sect_xarrays.keys():
+                if set(variable_names).issubset(
+                    set(sect_xarrays[dsname].variables.keys())
+                ):
+                    LOG.interactive(
+                        "  Applying '%s' family algorithm '%s' to data...",
+                        alg_plugin.family,
+                        alg_plugin.name,
+                    )
+                    alg_xarray[prod_plugin.name] = xarray.DataArray(
+                        alg_plugin(sect_xarrays[dsname], **alg_args)
+                    )
+        elif alg_plugin.family in ["xarray_dict_area_def_to_numpy"]:
+            # Format the call signature for passing a dictionary of xarrays,
+            # plus area_def, and return a single numpy array
+            LOG.interactive(
+                "  Applying '%s' family algorithm '%s' to data...",
+                alg_plugin.family,
+                alg_plugin.name,
+            )
+            alg_xarray[prod_plugin.name] = xarray.DataArray(
+                alg_plugin(sect_xarrays, area_def, **alg_args)
+            )
+        elif alg_plugin.family in ["xarray_dict_to_xarray"]:
+            # Format the call signature for passing a dictionary of xarrays,
+            # plus area_def, and return a single numpy array
+            LOG.interactive(
+                "  Applying '%s' family algorithm '%s' to data...",
+                alg_plugin.family,
+                alg_plugin.name,
+            )
+            alg_xarray = alg_plugin(sect_xarrays, **alg_args)
+        elif alg_plugin.family in ["xarray_to_xarray"]:
+            input_alg_xarray = None
+            for varname in variables:
+                LOG.info("TRYING variable %s for non-interpolated algorithms", varname)
+                for curr_sect_xarray in curr_sect_xarrays:
+                    if varname in curr_sect_xarray:
+                        if input_alg_xarray is None:
+                            LOG.info(
+                                "    USING sectored xarray %s for non-interpolated "
+                                "algorithms",
+                                curr_sect_xarray,
+                            )
+                            input_alg_xarray = curr_sect_xarray
+                        else:
+                            LOG.info(
+                                "    SKIPPING For non-interpolated data processing, "
+                                "all native variables must be the same resolution! "
+                                "Skipping variable %s, shape %s, input_alg_xarrays: %s",
+                                varname,
+                                curr_sect_xarrays[varname].shape,
+                                input_alg_xarray,
+                            )
+            if input_alg_xarray is None:
+                raise ValueError(
+                    "No required variables in any xarrays for 'xarray_to_xarray' "
+                    "algorithm type"
+                )
+            LOG.interactive(
+                "  Applying '%s' family algorithm '%s' to data...",
+                alg_plugin.family,
+                alg_plugin.name,
+            )
+            alg_xarray = alg_plugin(
+                input_alg_xarray, variables, prod_plugin.name, **alg_args
+            )
+        elif alg_plugin.family in ["list_numpy_to_numpy"]:
+            # Need to pull all the required variables out of the various xarray datasets
+            # and add them to numpy list.
+            # Then assign the resulting numpy array to the "product_name" DataArray
+            # within the xarray Dataset
+            numpys = []
+            for varname in variables:
+                for curr_sect_xarray in curr_sect_xarrays.values():
+                    if varname in list(curr_sect_xarray.variables.keys()):
+                        numpys += [curr_sect_xarray[varname].to_masked_array()]
+                        alg_xarray = curr_sect_xarray
+            LOG.interactive(
+                "  Applying '%s' family algorithm '%s' to data...",
+                alg_plugin.family,
+                alg_plugin.name,
+            )
+            alg_xarray[prod_plugin.name] = xarray.DataArray(
+                alg_plugin(numpys, **alg_args)
+            )
 
-        # Now apply the intepolator after applying the algorithm.
-        final_xarray = apply_interp_after_alg(
-            alg_xarray,
-            interp_plugin,
-            interp_args,
-            prod_plugin,
-            area_def,
-            processed_xarrays,
-        )
+        # No interpolation required
+        if prod_plugin.family in ["algorithm", "algorithm_colormapper"]:
+            final_xarray = alg_xarray
+        # If required, interpolate the result prior to returning
+        elif prod_plugin.family == "algorithm_interpolator_colormapper":
+            interp_args["varlist"] = [prod_plugin.name]
+            LOG.interactive(
+                "  Interpolating data with interpolator '%s'...", interp_plugin.name
+            )
+            final_xarray = interp_plugin(area_def, alg_xarray, None, **interp_args)
 
-        # MLS This appears to update alg_xarray, not final_xarray, with the
-        # area_def information.  So this might not be right..
-        final_xarray = add_attrs_from_area_def(final_xarray, alg_xarray, area_def)
+        # Ensure we have the "adjustment"id" in the filename appropriately
+        if "adjustment_id" in area_def.sector_info:
+            final_xarray = add_filename_extra_field(
+                alg_xarray, "adjustment_id", area_def.sector_info["adjustment_id"]
+            )
         # return here - we are done for either alg_cmap or alg_interp_cmap type
         return final_xarray
 
     # NOTE if algorithm specified first in product_type, we will not get to this point!
     # Returned from above if statement
 
-    # For products that first require interpolator, start with interpolator.
-    # These appear to consistently use curr_sect_xarrays and variables.
-    # Don't re-interpolate if a variable is found in processed_xarrays.
-    interp_xarray = apply_interp_first(
-        variables,
-        curr_sect_xarrays,
-        prod_plugin,
-        datasets_for_vars,
-        resampled_read,
-        area_def,
-        processed_xarrays,
-    )
+    # Default to empty xarray.Dataset() - will be populated within loop with
+    # appropriate regridded variables.
+    interp_xarray = xarray.Dataset()
+
+    for varname in variables:
+        LOG.info("TRYING variable %s", varname)
+        for key, sect_xarray in curr_sect_xarrays.items():
+            LOG.info("    TRYING dataset %s for variable %s", key, varname)
+
+            if varname not in sect_xarray.variables:
+                continue
+
+            # Reassign interp_plugin based on CURRENT sect_xarray
+            # Allow re-defining interpolation for different datasets.
+            interp_plugin = None
+            if "interpolator" in prod_plugin["spec"]:
+                interp_plugin = interpolators.get_plugin(
+                    prod_plugin["spec"]["interpolator"]["plugin"]["name"]
+                )
+                interp_args = prod_plugin["spec"]["interpolator"]["plugin"]["arguments"]
+
+            # If a specific dataset was requested for the current variable, and
+            # this dataset was NOT requested via a resampled_read (in which case
+            # the native datasets won't exist, only the resampled dataset),
+            # then use the appropriately requested dataset.
+            if varname in datasets_for_vars and not resampled_read:
+                if key in datasets_for_vars[varname]:
+                    LOG.info(
+                        "        USING %s varname from dataset %s, as specified in "
+                        "product_input YAML config",
+                        varname,
+                        key,
+                    )
+                else:
+                    LOG.info(
+                        "        WAITING dataset %s not requested for variable %s in "
+                        "product_input YAML config",
+                        key,
+                        varname,
+                    )
+                    continue
+            # If we've already interpolated this variable, check if it is needed
+            # before interpolating again
+            elif interp_xarray is not None and varname in list(interp_xarray.keys()):
+                # If all of the required variables are in the current dataset, use this
+                # version
+                if set(variables).issubset(set(sect_xarray.variables.keys())):
+                    LOG.info(
+                        "        REPLACING %s with current dataset %s, all required "
+                        "variables in current dataset",
+                        varname,
+                        key,
+                    )
+                # Otherwise, skip re-interpolating to avoid unecessary computation
+                else:
+                    LOG.warning(
+                        "        SKIPPING %s, encountered multiple versions, skipping "
+                        "subsequent dataset %s",
+                        varname,
+                        key,
+                    )
+                    continue
+            else:
+                LOG.info(
+                    "        USING %s varname from dataset %s - first availalbe, and "
+                    "not specified in YAML",
+                    varname,
+                    key,
+                )
+
+            # Potential efficiency hit with to_masked_array for dask arrays, etc
+            # LOG.info('Min/max %s %s / %s, dataset %s',
+            #          varname,
+            #          sect_xarray[varname].to_masked_array().min(),
+            #          sect_xarray[varname].to_masked_array().max(),
+            #          key)
+
+            # apply the requested interpolation routine.
+            interp_args["varlist"] = [varname]
+            if "time_dim" in sect_xarray.dims:
+                # This is for a particularly formatted dataset, that includes
+                # separate arrays for different times (ABI fire product).
+                # We need to be careful this does not break for some other
+                # dataset that includes a differently formatted "time"
+                # dimension.
+                tdims = len(sect_xarray.time_dim)
+                LOG.interactive(
+                    "  Interpolating data with interpolator '%s'...", interp_plugin.name
+                )
+                interp_list = [
+                    interp_plugin(
+                        area_def,
+                        sect_xarray.isel(time_dim=i),
+                        xarray.Dataset(),
+                        **interp_args,
+                    )
+                    for i in range(tdims)
+                ]
+                interp_xarray[varname] = xarray.concat(interp_list, dim="dim_2")[
+                    varname
+                ]
+            else:
+                LOG.interactive(
+                    "  Interpolating data with interpolator '%s'...", interp_plugin.name
+                )
+                interp_xarray = interp_plugin(
+                    area_def, sect_xarray, interp_xarray, **interp_args
+                )
+
+            # Potential efficiency hit with to_masked_array for dask arrays, etc
+            # LOG.info('Min/max interp %s %s / %s',
+            #          varname,
+            #          interp_xarray[varname].to_masked_array().min(),
+            #          interp_xarray[varname].to_masked_array().max())
 
     # Make sure we have all the appropriate attributes attached to the current
     # interp_xarray.
     # Use force=False so if attributes were set above, we do not overwrite them.
-    # MLS This was originally using sect_xarray, which would have just been
-    # the last sect_xarray when looping through the datasets.  Not sure that
-    # is what we wanted. Also not sure how much this is going to change outputs.
-    copy_standard_metadata(sect_xarrays["METADATA"], interp_xarray, force=False)
-
-    # Now apply the algorithm after interpolating. Don't reapply if it is
-    # found in processed_xarrays.
-    interp_xarray = apply_alg_after_interp(
-        interp_xarray,
-        area_def,
-        alg_plugin,
-        alg_args,
-        prod_plugin,
-        variables,
-        processed_xarrays,
-    )
+    copy_standard_metadata(sect_xarray, interp_xarray, force=False)
+
+    # Specify the call signature and return value for different algorithm types:
+    if prod_plugin.family in ["interpolator"]:
+        # Note "interp" product type will NOT have a single variable named
+        # "product_name", just the individual interpolated variables.
+        interp_xarray = interp_xarray
+    elif alg_plugin.family in ["xarray_to_numpy"]:
+        # xarray_to_numpy will return a single array, which can be set to the
+        # "product_name" variable.
+        LOG.interactive(
+            "  Applying '%s' family algorithm '%s' to data...",
+            alg_plugin.family,
+            alg_plugin.name,
+        )
+        interp_xarray[prod_plugin.name] = xarray.DataArray(
+            alg_plugin(interp_xarray, **alg_args)
+        )
+    elif alg_plugin.family in ["xarray_to_xarray"]:
+        # xarray_to_xarray algorithm type will return the full xarray object -
+        # assume variable names have been set appropriately within the
+        # algorithm.  This could be another good use of the
+        # "alt_varname_for_covg" kwarg in the coverage checks - if we want to
+        # just use a specific variable for the coverage checks rather than the
+        # "product_name" variable.
+        LOG.interactive(
+            "  Applying '%s' family algorithm '%s' to data...",
+            alg_plugin.family,
+            alg_plugin.name,
+        )
+        interp_xarray = alg_plugin(
+            interp_xarray, variables, prod_plugin.name, **alg_args
+        )
+    elif alg_plugin.family in [
+        "single_channel",
+        "channel_combination",
+        "list_numpy_to_numpy",
+        "rgb",
+    ]:
+        # Assume ANYTHING else takes in a list of numpy arrays, and returns a
+        # single numpy array.
+        # Perhaps we should be explicit here...
+        LOG.interactive(
+            "  Applying '%s' family algorithm '%s' to data...",
+            alg_plugin.family,
+            alg_plugin.name,
+        )
+        interp_xarray[prod_plugin.name] = xarray.DataArray(
+            alg_plugin(
+                [interp_xarray[varname].to_masked_array() for varname in variables],
+                **alg_args,
+            )
+        )
+    else:
+        raise TypeError(
+            f"UNSUPPORTED algorithm family '{alg_plugin.family}' or product family "
+            f"'{prod_plugin.family}', please add to the single_source procflow's "
+            "'get_alg_xarray' function appropriately"
+        )
 
     # Make sure we have all the appropriate attributes attached to the current
     # interp_xarray.
     # Use force=False so if attributes were set above, we do not overwrite them.
-    # MLS This was originally using sect_xarray, which would have just been
-    # the last sect_xarray when looping through the datasets.  Not sure that
-    # is what we wanted. Also not sure how much this is going to change outputs.
-    copy_standard_metadata(sect_xarrays["METADATA"], interp_xarray, force=False)
+    copy_standard_metadata(sect_xarray, interp_xarray, force=False)
     # Attach final product_name to the interp_xarray as well (the end goal of
-    # this routine).
-    if (
-        interp_xarray.attrs.get("product_name")
-        and interp_xarray.attrs["product_name"] != prod_plugin.name
-    ):
-        # Only include product_names if there is more than one product_name
-        if "product_names" not in interp_xarray.attrs:
-            interp_xarray.attrs["product_names"] = [prod_plugin.name]
-        else:
-            interp_xarray.attrs["product_names"].append(prod_plugin.name)
+    # this routine)
     interp_xarray.attrs["product_name"] = prod_plugin.name
-    # MLS This one uses interp_xarray and interp_xarray...
-    # The other one I think passed the wrong ones.
-    interp_xarray = add_attrs_from_area_def(interp_xarray, interp_xarray, area_def)
+    # Add appropriate attributes to alg_xarray
+    if "adjustment_id" in area_def.sector_info:
+        interp_xarray = add_filename_extra_field(
+            interp_xarray, "adjustment_id", area_def.sector_info["adjustment_id"]
+        )
 
     return interp_xarray
 
 
 def verify_area_def(
     area_defs,
     check_area_def,
@@ -1740,33 +1406,33 @@
     ]  # output_formatters.imagery_annotated
     reader_name = command_line_args["reader_name"]  # ssmis_binary
     reader_kwargs = command_line_args.get("reader_kwargs")
     if not reader_kwargs:
         reader_kwargs = {}
     compare_path = command_line_args["compare_path"]
     output_file_list_fname = command_line_args["output_file_list_fname"]
+    # compare_outputs_module = command_line_args["compare_outputs_module"]
     sector_adjuster = command_line_args["sector_adjuster"]
     sector_adjuster_kwargs = command_line_args["sector_adjuster_kwargs"]
     self_register_source = command_line_args["self_register_source"]
     self_register_dataset = command_line_args["self_register_dataset"]
     reader_defined_area_def = command_line_args["reader_defined_area_def"]
     sectored_read = command_line_args["sectored_read"]
     resampled_read = command_line_args["resampled_read"]
     product_db = command_line_args["product_db"]
     product_db_writer = command_line_args["product_db_writer"]
-    product_db_writer_kwargs = command_line_args["product_db_writer_kwargs"]
     presector_data = not command_line_args["no_presectoring"]
     output_checker_kwargs = command_line_args["output_checker_kwargs"]
 
     if product_db:
-        from geoips_db.interfaces import databases
+        from geoips_db.interfaces.databases import get_plugin
 
-        db_writer = databases.get_plugin(product_db_writer)
-        if not getenv("GEOIPS_DB_USER") or not getenv("GEOIPS_DB_PASS"):
-            raise ValueError("Need to set both $GEOIPS_DB_USER and $GEOIPS_DB_PASS")
+        db_writer = get_plugin(product_db_writer)
+        if not getenv("G2DB_USER") or not getenv("G2DB_PASS"):
+            raise ValueError("Need to set both $G2DB_USER and $G2DB_PASS")
 
     # Load plugins
     reader_plugin = readers.get_plugin(reader_name)
 
     print_mem_usage("MEMUSG", verbose=False)
 
     num_jobs = 0
@@ -2191,26 +1857,22 @@
                 for fprod, fname_fmt in curr_products.items():
                     additional_attrs = {
                         "coverage": covg,
                         "product": product_name,
                         "fileType": fprod.split(".")[-1],
                     }
                     product_added = db_writer(
-                        fprod,
-                        area_def=area_def,
-                        xarray_obj=alg_xarray,
-                        additional_attrs=additional_attrs,
-                        **product_db_writer_kwargs,
+                        fprod, area_def, alg_xarray, additional_attrs=additional_attrs
                     )
                     database_writes += [product_added]
 
             process_datetimes[area_def.area_id]["end"] = datetime.utcnow()
             num_jobs += 1
         else:
-            LOG.interactive(
+            LOG.info(
                 'SKIPPING No coverage or required variables "%s" for %s %s',
                 variables,
                 xobjs["METADATA"].source_name,
                 area_def.name,
             )
 
     LOG.interactive(
@@ -2235,16 +1897,15 @@
             fobj.writelines(["\n"])
 
     retval = 0
     if compare_path:
         from geoips.interfaces.module_based.output_checkers import output_checkers
 
         for output_product in final_products:
-            plugin_name = output_checkers.identify_checker(output_product)
-            output_checker = output_checkers.get_plugin(plugin_name)
+            output_checker = output_checkers.get_plugin(output_product)
             kwargs = {}
             if output_checker.name in output_checker_kwargs:
                 kwargs = output_checker_kwargs[output_checker.name]
             retval += output_checker(
                 output_checker,
                 compare_path.replace("<product>", product_name)
                 .replace("<procflow>", "single_source")
@@ -2259,15 +1920,15 @@
     )
     for output_product in final_products:
         LOG.interactive(
             "    \u001b[34mSINGLESOURCESUCCESS\033[0m %s",
             replace_geoips_paths(output_product, curly_braces=True),
         )
         if output_product in database_writes:
-            LOG.interactive("    DATABASESUCCESS %s", output_product)
+            LOG.info("    DATABASESUCCESS %s", output_product)
     for removed_product in removed_products:
         LOG.interactive("    DELETEDPRODUCT %s", removed_product)
 
     print_mem_usage("MEMUSG", verbose=True)
     LOG.interactive("READER_NAME: %s", reader_name)
     LOG.interactive("PRODUCT_NAME: %s", product_name)
     LOG.interactive("NUM_PRODUCTS: %s", len(final_products))
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/abi_l2_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/abi_l2_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/abi_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/abi_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/ahi_hsd.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ahi_hsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1303,21 +1303,14 @@
     print_mem_usage("MEMUSG", verbose=False)
 
     # Remove lines and samples arrays.  Not needed.
     for res in gvars.keys():
         try:
             gvars[res].pop("Lines")
             gvars[res].pop("Samples")
-            for varname, var in gvars[res].items():
-                gvars[res][varname] = np.ma.array(
-                    var, mask=gvars[res]["satellite_zenith_angle"].mask
-                )
-                gvars[res][varname] = np.ma.masked_where(
-                    gvars[res]["satellite_zenith_angle"] > 85, gvars[res][varname]
-                )
         except KeyError:
             pass
     for ds in datavars.keys():
         if not datavars[ds]:
             datavars.pop(ds)
         else:
             for varname in datavars[ds].keys():
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/amsr2_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/amsr2_netcdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,8 +400,8 @@
     tmp_xr = call(filelist)
 
     return tmp_xr
 
 
 def get_test_parameters():
     """Generate a data key for unit testing."""
-    return [{"data_key": "Brightness_Temperature_10_GHzH", "data_var": "tb10h"}]
+    return {"data_key": "Brightness_Temperature_10_GHzH", "data_var": "tb10h"}
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/amsr2_remss_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/amsr2_remss_winds_netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,13 @@
     tmp_xr = call(filelist)
 
     return tmp_xr
 
 
 def get_test_parameters():
     """Generate data key for unit testing."""
-    return [
-        {
-            "data_key": "WINDSPEED_1",
-            "data_var": "wind_speed_kts",
-            "lon_bounds": [],
-            "lat_bounds": [],
-        }
-    ]
+    return {
+        "data_key": "WINDSPEED_1",
+        "data_var": "wind_speed_kts",
+        "lon_bounds": [],
+        "lat_bounds": [],
+    }
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/amsub_hdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/amsub_hdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/amsub_mirs.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/amsub_mirs.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/ascat_uhr_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ascat_uhr_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/atms_hdf5.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/atms_hdf5.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/ewsg_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ewsg_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/geoips_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/geoips_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/gmi_hdf5.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/gmi_hdf5.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,8 +279,8 @@
     if len(filelist) == 0:
         raise NameError("No files found")
     return tmp_xr
 
 
 def get_test_parameters():
     """Yeilds data key for unit testing."""
-    return [{"data_key": "GMI", "data_var": "V10"}]
+    return {"data_key": "GMI", "data_var": "V10"}
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/imerg_hdf5.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/imerg_hdf5.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/mimic_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/mimic_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/modis_hdf4.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/modis_hdf4.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/saphir_hdf5.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/saphir_hdf5.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/sar_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/sar_winds_netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,16 +165,17 @@
     wind_xarray.attrs["source_file_names"] = [basename(fname)]
     wind_xarray.attrs["sample_distance_km"] = "unknown"
 
     LOG.info("Read data from %s", fname)
 
     if (
         hasattr(wind_xarray, "source")
-        and ("SAR" in wind_xarray.source or "SAR" in wind_xarray.title)
+        and "SAR" in wind_xarray.source
         and hasattr(wind_xarray, "title")
+        and "SAR" in wind_xarray.title
     ):
         wind_xarrays = []
         columns = None
         for fname in fnames:
             LOG.info("    Reading file %s", fname)
             wind_xarray = xarray.open_dataset(str(fname))
             LOG.info(
@@ -299,8 +300,8 @@
     if len(filelist) == 0:
         raise NameError("No files found")
     return tmp_xr
 
 
 def get_test_parameters():
     """Generate test data key for unit testing."""
-    return [{"data_key": "WINDSPEED", "data_var": "wind_speed_kts"}]
+    return {"data_key": "WINDSPEED", "data_var": "wind_speed_kts"}
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/scat_knmi_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/scat_knmi_winds_netcdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 """Read derived surface winds from KNMI scatterometer netcdf data."""
 
 import logging
 from os.path import basename
 from copy import deepcopy
 from glob import glob
-import numpy
 
 LOG = logging.getLogger(__name__)
 
 MS_TO_KTS = 1.94384
 DEG_TO_KM = 111.321
 
 interface = "readers"
@@ -88,14 +87,15 @@
     wind_xarray.wind_dir_deg_met.attrs["valid_max"] = 360
 
     # Set lat/lons/time appropriately
     wind_xarray = wind_xarray.rename(
         {"lat": "latitude", "lon": "longitude", "time": "time"}
     )
     import xarray
+    import numpy
 
     RAIN_FLAG_BIT = 9
     if hasattr(xarray, "ufuncs"):
         # ufuncs no longer available as of xarray v2022.06 (at least)
         wind_xarray["rain_flag"] = xarray.ufuncs.logical_and(
             wind_xarray["wvc_quality_flag"], (1 << RAIN_FLAG_BIT)
         )
@@ -165,18 +165,14 @@
     ingested = []
     for fname in fnames:
         try:
             wind_xarray = xarray.open_dataset(str(fname))
         except ValueError:
             # <=2023.08 versions of xarray would filter bad dates
             # current versions >=2023.9 raise Value Errors now
-            # Note: This is important for oscat, but not for any other sensors.
-            # This persists in versions as new as 2024.02.0 and I don't expect
-            # that it will be "fixed" because oscat's times are non-conforming
-            # with the CF standard.
             wind_xarray = xarray.open_dataset(str(fname), decode_times=False)
             # filters out negative dates, converting them to NaT
             wind_xarray = fix_datetime(wind_xarray)
 
         LOG.info("Read data from %s", fname)
 
         if (
@@ -268,8 +264,8 @@
     if len(filelist) == 0:
         raise NameError("No files found")
     return tmp_xr
 
 
 def get_test_parameters():
     """Generate test data key for unit testing."""
-    return [{"data_key": "WINDSPEED", "data_var": "wind_speed_kts"}]
+    return {"data_key": "WINDSPEED", "data_var": "wind_speed_kts"}
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/scat_noaa_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/scat_noaa_winds_netcdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,8 +265,8 @@
     if len(filelist) == 0:
         raise NameError("No files found")
     return tmp_xr
 
 
 def get_test_parameters():
     """Generate test data key for unit testing."""
-    return [{"data_key": "WINDSPEED", "data_var": "wind_speed_kts"}]
+    return {"data_key": "WINDSPEED", "data_var": "wind_speed_kts"}
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/seviri_hrit.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/seviri_hrit.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/sfc_winds_text.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/sfc_winds_text.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/smap_remss_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/smap_remss_winds_netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,8 +130,8 @@
     if len(filelist) == 0:
         raise NameError("No files found")
     return tmp_xr
 
 
 def get_test_parameters():
     """Generate test data key for unit testing."""
-    return [{"data_key": "WINDSPEED_1", "data_var": "wind_speed_kts"}]
+    return {"data_key": "WINDSPEED_1", "data_var": "wind_speed_kts"}
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/smos_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/smos_winds_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/ssmi_binary.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ssmi_binary.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/ssmis_binary.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/ssmis_binary.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/utils/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/utils/geostationary_geolocation.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/utils/geostationary_geolocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 
 from geoips.errors import CoverageError
 from geoips.filenames.base_paths import PATHS as gpaths
 from geoips.utils.context_managers import import_optional_dependencies
 
 LOG = logging.getLogger(__name__)
 
-# interface = None indicates to the GeoIPS interfaces that this is not a valid
-# plugin, and this module will not be added to the GeoIPS plugin registry.
-# This allows including python modules within the geoips/plugins directory
-# that provide helper or utility functions to the geoips plugins, but are
-# not full GeoIPS plugins on their own.
 interface = None
 
 with import_optional_dependencies(loglevel="info"):
     """Attempt to import a package and print to LOG.info if the import fails."""
     import numexpr as ne
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/utils/hrit_reader.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/utils/hrit_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,33 +18,19 @@
 import logging
 import shutil
 import operator
 from functools import reduce
 from copy import copy
 from struct import unpack
 from datetime import datetime, timedelta
-
-from geoips.utils.context_managers import import_optional_dependencies
-
-with import_optional_dependencies(loglevel="interactive"):
-    """Attempt to import xRITDecompress from pyPublicDecompWT.
-
-    Needed to decompress xRIT data types.
-    """
-    from pyPublicDecompWT import xRITDecompress
-
+from pyPublicDecompWT import xRITDecompress
 import numpy as np
 
 log = logging.getLogger(__name__)
 
-# interface = None indicates to the GeoIPS interfaces that this is not a valid
-# plugin, and this module will not be added to the GeoIPS plugin registry.
-# This allows including python modules within the geoips/plugins directory
-# that provide helper or utility functions to the geoips plugins, but are
-# not full GeoIPS plugins on their own.
 interface = None
 
 
 class HritDtype(object):
     """HRIT data type."""
 
     types = {
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/utils/remss_reader.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/utils/remss_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,14 @@
 import logging
 
 LOG = logging.getLogger(__name__)
 
 MS_TO_KTS = 1.94384
 DEG_TO_KM = 111.321
 
-# interface = None indicates to the GeoIPS interfaces that this is not a valid
-# plugin, and this module will not be added to the GeoIPS plugin registry.
-# This allows including python modules within the geoips/plugins directory
-# that provide helper or utility functions to the geoips plugins, but are
-# not full GeoIPS plugins on their own.
 interface = None
 
 
 def read_remss_data(wind_xarray, data_type):
     """
     Reformat SMAP or WindSat xarray object appropriately.
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/viirs_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/viirs_netcdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,22 +57,18 @@
 """
 # Python Standard Libraries
 import logging
 import os
 
 # Installed Libraries
 import numpy
-import pandas as pd
 import xarray as xr
 
 from geoips.utils.context_managers import import_optional_dependencies
 
-# GeoIPS Libraries
-from geoips.plugins.modules.readers.utils.geostationary_geolocation import get_indexes
-
 # If this reader is not installed on the system, don't fail altogether, just skip this
 # import. This reader will not work if the import fails, and the package will have to be
 # installed to process data of this type.
 LOG = logging.getLogger(__name__)
 
 with import_optional_dependencies(loglevel="info"):
     """Attempt to import a package and print to LOG.info if the import fails."""
@@ -209,34 +205,14 @@
 #    Run plan:  fname has a list of VIIRS files (3 *02* or *03* files)
 
 interface = "readers"
 family = "standard"
 name = "viirs_netcdf"
 
 
-def _get_geolocation_metadata(orig_shape, fnames, xarray):
-    """
-    Gather all of the metadata used in creating geolocation data for input file.
-
-    This is split out so we can easily create a chash of the data for creation
-    of a unique filename. This allows us to avoid recalculation of angles that
-    have already been calculated.
-    """
-    geomet = {}
-    geomet["platform_name"] = "viirs"
-    geomet["scene"] = "stitched_granules"
-    # Just getting the nadir resolution in kilometers.  Must extract from a string.
-    geomet["res_km"] = xarray.attrs["resolution_km"]
-    geomet["roi_factor"] = 5  # roi = res * roi_factor, was 10
-    geomet["num_lines"] = orig_shape[0]
-    geomet["num_samples"] = orig_shape[1]
-    geomet["fnames"] = fnames
-    return geomet
-
-
 def required_chan(chans, varnames):
     """Return True if required channel."""
     if chans is None:
         return True
     for varname in varnames:
         if varname in chans:
             return True
@@ -287,29 +263,18 @@
     # array of False the size of nparr
     if nparr_mask.shape != nparr.shape:
         nparr_mask = numpy.zeros(nparr.shape).astype(bool)
     # If we haven't merged nparr_mask into dataset_masks[data_type] yet, do it now
     if dataset_masks[data_type] is False:
         dataset_masks[data_type] = nparr_mask
     elif dataset_masks[data_type].shape != merged_array.shape:
-        # This was previously only being applied to "BT_CHANNELS", which
-        # caused the unprojected test scripts to fail (due to incorrect
-        # shape of the final mask array).  Removing that check so ALL
-        # variables are vstacked.
         dataset_masks[data_type] = numpy.vstack([dataset_masks[data_type], nparr_mask])
 
 
-def call(
-    fnames,
-    metadata_only=False,
-    chans=None,
-    area_def=None,
-    self_register=False,
-    resample=False,
-):
+def call(fnames, metadata_only=False, chans=None, area_def=None, self_register=False):
     """Read VIIRS netcdf data products.
 
     Parameters
     ----------
     fnames : list
         * List of strings, full paths to files
     metadata_only : bool, default=False
@@ -652,80 +617,18 @@
                         nparr.mask,
                     )
                     for attrname in ncvar.ncattrs():
                         xarrays[geo_target_data_type][xvarname].attrs[attrname] = (
                             ncvar.getncattr(attrname)
                         )
 
-        xarrays[data_type].attrs["resolution_km"] = (
-            float(ncdf_file.LongName[-4:-1]) / 1000.0
-        )
-
         # close the files
 
         ncdf_file.close()
 
-    # Geolocation resampling
-    if resample and area_def:
-        adname = area_def.area_id
-        new_shape = area_def.shape
-
-        LOG.info("")
-        LOG.info("Getting geolocation information for {}.".format(adname))
-
-        for dtype in xarrays.keys():
-            if "latitude" not in xarrays[dtype].variables:
-                LOG.info(
-                    "No data read for dataset %s, removing from xarray list", dtype
-                )
-                continue
-            fldk_lats = xarrays[dtype]["latitude"]
-            fldk_lons = xarrays[dtype]["longitude"]
-            # Get just the metadata we need
-            geo_metadata = _get_geolocation_metadata(
-                fldk_lats.shape, fnames, xarrays[dtype]
-            )
-            lines, samples = get_indexes(geo_metadata, fldk_lats, fldk_lons, area_def)
-
-            index_mask = lines != -999
-
-            new_dim0 = "dim_{:d}".format(new_shape[0])
-            new_dim1 = "dim_{:d}".format(new_shape[1])
-
-            # Resample the mask
-            old_dataset_masks = dataset_masks[dtype]
-            dataset_masks[dtype] = numpy.full(new_shape, True)
-            dataset_masks[dtype][index_mask] = old_dataset_masks[
-                lines[index_mask], samples[index_mask]
-            ]
-
-            for varname in xarrays[dtype].variables.keys():
-                new_var = numpy.full(new_shape, -999.1)
-                new_var[index_mask] = xarrays[dtype][varname].values[
-                    lines[index_mask], samples[index_mask]
-                ]
-                if varname not in list(xvarnames.values()) + ["latitude", "longitude"]:
-                    # Set values <= -999.9 to NaN so they also get interpolated.
-                    new_var[numpy.where(new_var <= -999.9)] = numpy.nan
-                    # Interpolate missing data.
-                    out_var = numpy.array(pd.DataFrame(new_var).interpolate())
-                    # Reset the mask so these values get shown.
-                    skip_mask = numpy.where(
-                        numpy.isnan(new_var) & ~numpy.isnan(out_var)
-                    )
-                    dataset_masks[dtype][skip_mask] = False
-                else:
-                    out_var = new_var
-                xarrays[dtype][varname] = xr.DataArray(
-                    out_var, dims=[new_dim0, new_dim1]
-                )
-
-        LOG.interactive("Done with geolocation for {}".format(adname))
-        LOG.info("")
-
     # Clean up the final xarray dictionary
     xarray_returns = {}
     for dtype in xarrays.keys():
         if "latitude" not in xarrays[dtype].variables:
             LOG.info("No data read for dataset %s, removing from xarray list", dtype)
             continue
         for varname in xarrays[dtype].variables.keys():
@@ -757,13 +660,17 @@
         xarray_returns[dtype] = xarrays[dtype]
 
     # Force masking of latitude/longitude fill values, otherwise causes issues
     # when sectoring
     # fill_value = -999.9
     for dtype in xarray_returns:
         bad_llmask = xarray_returns[dtype]["latitude"] == -999.9
-        for var in xarray_returns[dtype].variables.keys():
-            xarray_returns[dtype][var] = xarray_returns[dtype][var].where(~bad_llmask)
+        xarray_returns[dtype]["latitude"] = xarray_returns[dtype]["latitude"].where(
+            ~bad_llmask
+        )
+        xarray_returns[dtype]["longitude"] = xarray_returns[dtype]["longitude"].where(
+            ~bad_llmask
+        )
 
     xarray_returns["METADATA"] = list(xarray_returns.values())[0][[]]
 
     return xarray_returns
```

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/wfabba_ascii.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/wfabba_ascii.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/windsat_idr37_binary.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/windsat_idr37_binary.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/readers/windsat_remss_winds_netcdf.py` & `geoips-1.12.2a0/geoips/plugins/modules/readers/windsat_remss_winds_netcdf.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/sector_metadata_generators/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/sector_metadata_generators/bdeck_parser.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/bdeck_parser.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/sector_metadata_generators/tc_sector_file_parser.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_metadata_generators/tc_sector_file_parser.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/sector_spec_generators/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_spec_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/sector_spec_generators/center_coordinates.py` & `geoips-1.12.2a0/geoips/plugins/modules/sector_spec_generators/center_coordinates.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/title_formatters/__init__.py` & `geoips-1.12.2a0/geoips/plugins/modules/title_formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/title_formatters/static_standard.py` & `geoips-1.12.2a0/geoips/plugins/modules/title_formatters/static_standard.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/title_formatters/tc_copyright.py` & `geoips-1.12.2a0/geoips/plugins/modules/title_formatters/tc_copyright.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/modules/title_formatters/tc_standard.py` & `geoips-1.12.2a0/geoips/plugins/modules/title_formatters/tc_standard.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/txt/ascii_palettes/tpw_cimss.txt` & `geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_cimss.txt`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/txt/ascii_palettes/tpw_purple.txt` & `geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_purple.txt`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/txt/ascii_palettes/tpw_pwat.txt` & `geoips-1.12.2a0/geoips/plugins/txt/ascii_palettes/tpw_pwat.txt`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/feature_annotators/tc_pmw.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_pmw.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/feature_annotators/tc_windspeed.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/feature_annotators/tc_windspeed.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/Uncorrected-Channel.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/Uncorrected-Channel.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/150H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/150V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/150VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/150VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/157V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/157V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/157VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/157VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/165H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/165H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/165HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/165HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/166H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/166HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/166V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/166VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/166VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-1H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-1H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-1HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-1HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-3H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-3H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-3HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-3HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183-7H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183-7H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/183HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/183HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/190V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/190V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_150/190VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_150/190VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/19H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/19HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/19V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/19VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/19VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H-Legacy.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Legacy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H-LegacyNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-LegacyNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H-Physical.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-Physical.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H-PhysicalNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H-PhysicalNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37pct.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37pct.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_37/37pctNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_37/37pctNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H-Legacy.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Legacy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H-LegacyNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-LegacyNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H-Physical.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-Physical.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H-PhysicalNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H-PhysicalNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89H.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89H.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89HNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89HW.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HW.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89HWNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89HWNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89V.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89V.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89VNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89VNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89pct.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89pct.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/pmw_89/89pctNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/pmw_89/89pctNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/rain_rate/Rain.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/rain_rate/Rain.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/rain_rate/RainNearest.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/rain_rate/RainNearest.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/incident-angle.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/incident-angle.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/nrcs.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/nrcs.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/wind-ambiguities.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/wind-ambiguities.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/windbarbs.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/windbarbs.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/sfc_winds/windspeed.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/sfc_winds/windspeed.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/tpw/TPW-CIMSS.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-CIMSS.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/tpw/TPW-PURPLE.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-PURPLE.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/tpw/TPW-PWAT.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/tpw/TPW-PWAT.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/IR-BD.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/IR-BD.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Infrared-Gray.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Infrared-Gray.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Infrared.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Infrared.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Night-Vis-GeoIPS1.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis-GeoIPS1.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Night-Vis.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Night-Vis.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/Visible.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/Visible.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/WV-Lower.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV-Lower.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/WV-Upper.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV-Upper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/product_defaults/visir/WV.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/product_defaults/visir/WV.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/abi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/abi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/ahi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ahi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/ami.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/seviri.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 interface: products
 family: list
-name: ami
+name: seviri
 docstring: |
-  The AMI products configuration, which produces Infrared products, Vertical Velocity products, and the Visible IR products
+  The seviri product_inputs configuration, which produces Infrared, Vertical Velocity, and Visible products.
 spec:
   products:
     - name: Infrared
-      source_names: [ami]
+      source_names: [seviri]
       docstring: |
-        The Infrared product_defaults configuration for the Geokompsat AMI product.
+        The Infrared product_defaults configuration for seviri products.
       product_defaults: Infrared
       spec:
-        variables: ["IR112BT"]
+        variables: ["B09BT"]
     - name: Infrared-Gray
-      source_names: [ami]
+      source_names: [seviri]
       docstring: |
-        The Infrared-Gray product_defaults configuration for Geokompsat AMI product.
+        The Infrared-Gray product_defaults configuration for seviri products.
       product_defaults: Infrared-Gray
       spec:
-        variables: ["IR112BT"]
+        variables: ["B09BT"]
     - name: IR-BD
-      source_names: [ami]
+      source_names: [seviri]
       docstring: |
-        The IR-BD product_defaults configuration for Geokompsat AMI product.
+        The IR-BD product_defaults configuration for seviri products.
       product_defaults: IR-BD
       spec:
-        variables: ["IR112BT"]
-    - name: WV
-      source_names: [ami]
-      docstring: |
-        The WV product_defaults configuration for Geokompsat AMI product.
-      product_defaults: WV
-      spec:
-        variables: ["WV069BT"] # B09 abi, 6.9um Mid-level WV; B09 ahi 6.9410 Mid-level WV; B27 modis 6.535-6.895um
+        variables: ["B09BT"]
     - name: WV-Lower
-      source_names: [ami]
+      source_names: [seviri]
       docstring: |
-        The WV-Lower product_defaults configuration for Geokompsat AMI product.
+        The WV-Lower product_defaults configuration for seviri products.
       product_defaults: WV-Lower
       spec:
-        variables: ["WV073BT"] # B10 abi, 7.3um Lower-level WV; B10 ahi 7.3467um Lower-level WV; B28 modis, B06 seviri IR7.3
+        variables: ["B06BT"] # B10 abi, 7.3um Lower-level WV; B10 ahi 7.3467um Lower-level WV; B28 modis, B06 seviri IR7.3
     - name: WV-Upper
-      source_names: [ami]
+      source_names: [seviri]
       docstring: |
-        The WV-Upper product_defaults configuration for Geokompsat AMI product.
+        The WV-Upper product_defaults configuration for seviri products.
       product_defaults: WV-Upper
       spec:
-        variables: ["WV063BT"] # B08 abi, 6.2um Upper-level WV; B08 ahi 6.2429um Upper-level WV; B05 seviri IR6.2
+        variables: ["B05BT"] # B08 abi, 6.2um Upper-level WV; B08 ahi 6.2429um Upper-level WV; B05 seviri IR6.2
     - name: Visible
-      source_names: [ami]
+      source_names: [seviri]
       docstring: |
-        The Visible product_defaults for Geokompsat AMI product.
+        The Visible product_defaults configuration for seviri products.
       product_defaults: Visible
       spec:
-        variables: ["VI006Ref"] # RED: B03 0.64um ahi (hi  res) and B02 0.64um abi (hi), B01 0.635um seviri
+        variables: ["B01Ref", "solar_zenith_angle"] # RED: B03 0.64um ahi (hi  res) and B02 0.64um abi (hi),  B01 0.635um seviri
         # BLU: B01 0.47um ahi (med res) and B01 0.47um abi (med), no seviri equiv
         # GRN: B02 0.51um ahi (med res) no abi grn band,          no seviri equiv
         # VEG: B04 0.86um ahi (med res) and B03 0.86um abi (med), B02 0.81um seviri
         colormapper:
           plugin:
             name: matplotlib_linear_norm
             arguments:
-              cbar_label: "Reflectance, AMI B03 0.64um Red Band"
+              cbar_label: "Reflectance, SEVIRI B01 0.635um red band"
+        # cbar_label: "Reflectance, SEVIRI B02 0.81um Veggie Band"
```

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/amsr-e.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/amsr-e.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/amsr2.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/amsr2.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/amsu-b.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/amsu-b.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/ascat.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ascat.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/ascatuhr.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ascatuhr.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/atms.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/atms.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/gmi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/gmi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/gvar.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/gvar.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/hscat.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/hscat.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/imerg.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/imerg.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/mhs.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/mhs.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/mimic.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/mimic.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/modis.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/modis.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/oscat.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/oscat.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/saphir.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/saphir.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/sar-spd.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/sar-spd.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/smap-spd.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/smap-spd.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/smos-spd.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/smos-spd.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/ssmi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ssmi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/ssmis.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/ssmis.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/tmi.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/tmi.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/viirs.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/viirs.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -39,31 +39,25 @@
         The Night-Vis-GeoIPS1 product_defaults configuration for viirs products.
       product_defaults: Night-Vis-GeoIPS1
       spec:
         variables: ["DNBRad", "DNB:solar_zenith_angle"]
     - name: Night-Vis-IR
       source_names: [viirs]
       docstring: |
-        The Night-Vis-IR product configuration for viirs products.
-      product_defaults: RGB-Default
+        The Night-Vis-IR product_defaults configuration for viirs products.
+      product_defaults: Night-Vis-IR
       spec:
         variables: ["DNBRad", "M16BT"]
-        algorithm:
-            plugin:
-                name: Night_Vis_IR
     - name: Night-Vis-IR-GeoIPS1
       source_names: [viirs]
       docstring: |
-        The Night-Vis-IR-GeoIPS1 product configuration for viirs products.
-      product_defaults: RGB-Default
+        The Night-Vis-IR-GeoIPS1 product_defaults configuration for viirs products.
+      product_defaults: Night-Vis-IR-GeoIPS1
       spec:
         variables: ["DNBRad", "M16BT", "DNB:solar_zenith_angle"]
-        algorithm:
-            plugin:
-                name: Night_Vis_IR_GeoIPS1
     - name: Visible
       source_names: [viirs]
       docstring: |
         The Visible product_defaults configuration for viirs products.
       product_defaults: Visible
       spec:
         variables: ["M05Ref"] # Ocean Color Aerosol: VIIRS M05 0.673um
```

### Comparing `geoips-1.12.2/geoips/plugins/yaml/products/windsat.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/products/windsat.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/sectors/static/conus.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/conus.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/sectors/static/ewsg.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/ewsg.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/sectors/static/geokompsat.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/himawari.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 interface: sectors
 family: area_definition_static
-name: geokompsat
-docstring: "Full disk sector for GEO-KOMPSAT"
+name: himawari
+docstring: "Full disk sector for Himawari"
 metadata:
   region:
     continent: Global
     country: x
-    area: GEO-KOMPSAT
+    area: Himawari
     subarea: x
     state: x
     city: x
 spec:
-  area_id: geokompsat
-  description: GEO-KOMPSAT Coverage
+  area_id: himawari
+  description: Himawari Coverage
   projection:
     a: 6371228.0
     lat_0: 0
-    lon_0: 128.2
+    lon_0: 140.7
     proj: eqc
     units: m
   resolution:
     - 10000
     - 10000
   shape:
     height: 2000
```

### Comparing `geoips-1.12.2/geoips/plugins/yaml/sectors/static/global.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/global.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/sectors/static/goes_east.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/goes_east.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/sectors/static/goes_west.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/goes_west.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/sectors/static/himawari.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/japan.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 interface: sectors
 family: area_definition_static
-name: himawari
-docstring: "Full disk sector for Himawari"
+name: japan
+docstring: "Full disk sector for Himawari-8"
 metadata:
   region:
-    continent: Global
-    country: x
-    area: Himawari
+    continent: Asia
+    country: Japan
+    area: x
     subarea: x
     state: x
     city: x
 spec:
-  area_id: himawari
-  description: Himawari Coverage
+  area_id: japan
+  description: Japan
   projection:
     a: 6371228.0
-    lat_0: 0
-    lon_0: 140.7
+    lat_0: 37.0
+    lon_0: 138.25
     proj: eqc
     units: m
   resolution:
-    - 10000
-    - 10000
+    - 1000
+    - 1000
   shape:
     height: 2000
     width: 2000
   area_extent:
-    lower_left_xy: [-10000000, -10000000]
-    upper_right_xy: [10000000, 10000000]
+    lower_left_xy: [-1000000, -1000000]
+    upper_right_xy: [1000000, 1000000]
```

### Comparing `geoips-1.12.2/geoips/plugins/yaml/sectors/static/meteosat_indian_ocean.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/meteosat_indian_ocean.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/plugins/yaml/sectors/static/south_america.yaml` & `geoips-1.12.2a0/geoips/plugins/yaml/sectors/static/south_america.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/feature_annotators/cartopy.yaml` & `geoips-1.12.2a0/geoips/schema/feature_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/gridline_annotators/cartopy.yaml` & `geoips-1.12.2a0/geoips/schema/gridline_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/product_defaults/bases/colormapper.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/bases/colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/product_defaults/bases/windbarb_plotter.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/bases/windbarb_plotter.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/product_defaults/specs/algorithm.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/product_defaults/specs/algorithm_colormapper.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/product_defaults/specs/algorithm_interpolator_colormapper.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/algorithm_interpolator_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/product_defaults/specs/interpolator.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/product_defaults/specs/interpolator_algorithm.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator_algorithm.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/product_defaults/specs/interpolator_algorithm_colormapper.yaml` & `geoips-1.12.2a0/geoips/schema/product_defaults/specs/interpolator_algorithm_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/products/bases/product.yaml` & `geoips-1.12.2a0/geoips/schema/products/bases/product.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/sectors/specs/area_definition.yaml` & `geoips-1.12.2a0/geoips/schema/sectors/specs/area_definition.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/sectors/specs/center.yaml` & `geoips-1.12.2a0/geoips/schema/sectors/specs/center.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/schema/sectors/static.yaml` & `geoips-1.12.2a0/geoips/schema/sectors/static.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/sector_utils/__init__.py` & `geoips-1.12.2a0/geoips/sector_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/sector_utils/estimate_area_extent.py` & `geoips-1.12.2a0/geoips/sector_utils/estimate_area_extent.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/sector_utils/overpass_predictor.py` & `geoips-1.12.2a0/geoips/sector_utils/overpass_predictor.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 """Overpass predictor, based on Two Line Element files."""
 
 # Standard libraries
 from datetime import timedelta
 import math
-from numpy import linspace
 
 # Installed libraries
 import ephem
 from pyresample import spherical_geometry
 
 from logging import getLogger
 
@@ -209,79 +208,21 @@
     )
     earth_radius_km = 6730.0
     cpa_km = ptsatdeg.distance(ptsecdeg) * earth_radius_km
     opass_info["closest pass approach (km)"] = cpa_km
     return opass_info
 
 
-def create_sector_observers(ll_lon, ll_lat, ur_lon, ur_lat, spacing=50):
-    """Create multiple prediction points for large sectors.
-
-    Parameters
-    ----------
-    ll_lon : float
-        Lower left longitude of sector.
-    ll_lat : float
-        Lower left latitude of sector.
-    ur_lon : float
-        Upper right longtitude of sector.
-    ur_lat : float
-        Upper right latitude of sector.
-    spacing : int, optional
-        Spacing between latitude/longitude observer points (degrees), by default 50
-
-    Returns
-    -------
-    list
-        List of observer points for sector.
-    """
-    if ur_lon < ll_lon:
-        # Check if sector crosses dateline.
-        # Convert lons to 0 - 360 just to make things easier.
-        ur_lon = 360 + ur_lon
-    # Find how wide and tall the sector is
-    lon_delta = abs((ur_lon - spacing) - (ll_lon - spacing))
-    lat_delta = abs((ur_lat - spacing) - (ll_lat - spacing))
-    # Determine how many observers we'd expect for this sector.
-    n_lat_points = round(round(lat_delta) / spacing)
-    n_lon_points = round(round(lon_delta) / spacing)
-    # Create list of latitude observer points.
-    # Only try to create multiple observers if the expected
-    # number of observers is greater than one.
-    if n_lat_points > 1:
-        check_lats = linspace(ll_lat + spacing / 2, ur_lat - spacing / 2, n_lat_points)
-    else:
-        check_lats = [(ur_lat + ll_lat) / 2]
-    # Create list of longitude observer points.
-    # Only try to create multiple observers if the expected
-    # number of observers is greater than one.
-    if n_lon_points > 1:
-        check_lons = linspace(ll_lon + spacing / 2, ur_lon - spacing / 2, n_lon_points)
-        # Convert back to -180 - 180
-        check_lons[check_lons > 180] -= 360
-    else:
-        center_lon = (ur_lon + ll_lon) / 2
-        if center_lon > 180:
-            # Convert lons back to -180 - 180
-            center_lon -= 360
-        check_lons = [center_lon]
-    check_points = []
-    for clat in check_lats:
-        for clon in check_lons:
-            check_points.append([clat, clon])
-    return check_points
-
-
 def predict_satellite_overpass(
     tlefile,
     satellite_name,
     satellite_tle,
     area_def,
     start_datetime,
-    observer_spacing=50,
+    check_midpoints=False,
 ):
     """Estimate next satellite overpass information with ephem.
 
     Parameters
     ----------
     tlefile : str
         file path of TLE
@@ -289,75 +230,82 @@
         name of satellite
     satellite_tle : dict
         dictionary holding satellite tle line1 and line2 data
     area_def : pyresample AreaDefinition
         area definition
     start_datetime :datetime.datetime
         start time to find the next available overpass
-    observer_spacing : float
-        Spacing (degrees) between observer points in sector. If domain exceeds the
-        specified spacing, multiple observer are automatically added across the sector.
+    check_midpoints :bool
+        check mid points of area definition for additional overpassses
 
     Returns
     -------
     dict
         dictionary holding next overpass information
     """
     tle = ephem.readtle(tlefile, satellite_tle["line1"], satellite_tle["line2"])
     ll_lon, ll_lat, ur_lon, ur_lat = area_def.area_extent_ll
-    observers = create_sector_observers(
-        ll_lon, ll_lat, ur_lon, ur_lat, spacing=observer_spacing
-    )
-    total_observers = len(observers)
+    center_lon = (ll_lon + ur_lon) / 2.0
+    center_lat = (ll_lat + ur_lat) / 2.0
+    observers = [(center_lat, center_lon)]
+    if check_midpoints:
+        mid_lon_upper = (center_lon + ur_lon) / 2.0
+        mid_lon_lower = (center_lon + ll_lon) / 2.0
+        mid_lat_upper = (center_lat + ur_lat) / 2.0
+        mid_lat_lower = (center_lat + ll_lat) / 2.0
+        observers.append((mid_lat_upper, center_lon))
+        observers.append((mid_lat_lower, center_lon))
+        observers.append((center_lat, mid_lon_upper))
+        observers.append((center_lat, mid_lon_lower))
     overpasses = {}
-    LOG.info(
-        "Running %s overpass predictor for %s. Total observers: %s",
-        satellite_name,
-        area_def.area_id,
-        total_observers,
-    )
+    rise_times = []
+    valid_overpasses = 0
     for i, observer in enumerate(observers):
         observer_lat, observer_lon = observer
         opass_info = calculate_overpass(
             tle, observer_lat, observer_lon, start_datetime, satellite_name
         )
         if isinstance(opass_info, type(None)):
             # Either something went wrong in the predictor, or found a
             # geostationary satellite that does not overpass the sector, ever!
+            overpasses = None
             continue
-        opass_key = "_".join(
-            [
-                satellite_name,
-                area_def.area_id,
-                opass_info["max altitude time"].strftime("%Y%m%dT%H%MZ"),
-            ]
-        )
-        if opass_key not in overpasses:
-            overpasses[opass_key] = opass_info
+        if i < 1:
+            # Keep track of center rise set times
+            center_rise = opass_info["rise time"]
+            center_set = opass_info["set time"]
+            valid_overpasses += 1
+            overpasses["pass {0}".format(valid_overpasses)] = opass_info
+        # Only add if overpass does not intersect
+        # with the sector's center observer point
+        max_t = opass_info["max altitude time"]
+        if (max_t < center_rise) or (max_t > center_set):
+            rise_times.append(opass_info["rise time"])
+            valid_overpasses += 1
+            overpasses["pass {0}".format(valid_overpasses)] = opass_info
     return overpasses
 
 
 def predict_overpass_area_def(
-    tlefile, area_definition, satellite_list, start_datetime, observer_spacing=50
+    tlefile, area_definition, satellite_list, start_datetime, check_midpoints=False
 ):
     """Predict satellite overpass for an area_definition.
 
     Parameters
     ----------
     tlefile : str
         file path of TLE
     area_definition : pyresample AreaDefinition
         pyresample area definition
     satellite_list : list
         list of satellites to predict the overpass times
     start_datetime : datetime.datetime
         start time to find the next available overpass
-    observer_spacing : float
-        Spacing (degrees) between observer points in sector. If domain exceeds the
-        specified spacing, multiple observer are automatically added across the sector.
+    check_midpoints : bool
+        check mid points of area definition for additional overpassses
 
     Returns
     -------
     dict
         dictionary holding next satellite overpass estimates
         (sorted by satellite -> overpass info)
     """
@@ -368,28 +316,28 @@
     for satellite, sat_tle in satellite_tle_dict.items():
         next_overpass = predict_satellite_overpass(
             tlefile,
             satellite,
             sat_tle,
             area_definition,
             start_datetime,
-            observer_spacing=observer_spacing,
+            check_midpoints=check_midpoints,
         )
         if next_overpass:
             area_def_overpasses[satellite] = next_overpass
     return area_def_overpasses
 
 
 def predict_overpass_yaml(
     tlefile,
     sectorfile,
     sector_list,
     satellite_list,
     start_datetime,
-    observer_spacing=50,
+    check_midpoints=False,
 ):
     """Predict satellite overpass for sectors from a given yaml sector file.
 
     Parameters
     ----------
     tlefile : str
         file path of TLE
@@ -397,17 +345,16 @@
         file path of sectorfile
     sector_list : list
         list of sectors held within the sectorfile
     satellite_list : list
         list of satellites to predict the overpass times
     start_datetime : datetime.datetime
         start time to find the next available overpass
-    observer_spacing : float
-        Spacing (degrees) between observer points in sector. If domain exceeds the
-        specified spacing, multiple observer are automatically added across the sector.
+    check_midpoints : bool
+        check mid points of area definition for additional overpassses
 
     Returns
     -------
     dict
         dictionary holding next satellite overpass estimates for sectors
         (sorted by sector -> satellite -> overpass info)
     """
@@ -419,11 +366,11 @@
     for yaml_sector in sector_list:
         sector_area_def = create_areadefinition_from_yaml(sectorfile, yaml_sector)
         overpasses = predict_overpass_area_def(
             tlefile,
             sector_area_def,
             satellite_list,
             start_datetime,
-            observer_spacing=observer_spacing,
+            check_midpoints=check_midpoints,
         )
         sector_overpasses[yaml_sector] = overpasses
     return sector_overpasses
```

### Comparing `geoips-1.12.2/geoips/sector_utils/projections.py` & `geoips-1.12.2a0/geoips/sector_utils/projections.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/sector_utils/tc_tracks.py` & `geoips-1.12.2a0/geoips/sector_utils/tc_tracks.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/sector_utils/tc_tracks_database.py` & `geoips-1.12.2a0/geoips/sector_utils/tc_tracks_database.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/sector_utils/utils.py` & `geoips-1.12.2a0/geoips/sector_utils/utils.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/sector_utils/yaml_utils.py` & `geoips-1.12.2a0/geoips/sector_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/utils/__init__.py` & `geoips-1.12.2a0/geoips/xarray_utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 # # # This program is free software: you can redistribute it and/or modify it under
 # # # the terms of the NRLMMD License included with this program. This program is
 # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
-"""Geoips utilities init file."""
+"""Geoips xarray utils init file."""
```

### Comparing `geoips-1.12.2/geoips/utils/decorators.py` & `geoips-1.12.2a0/geoips/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/utils/memusg.py` & `geoips-1.12.2a0/geoips/utils/memusg.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/geoips/xarray_utils/data.py` & `geoips-1.12.2a0/geoips/xarray_utils/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -763,26 +763,19 @@
     Returns
     -------
     dict of xarray.Dataset
         Dictionary of sectored datasets containing requested "varnames",
         sectored spatially and temporally as requested.
     """
     ret_xobjs = {}
-    from geoips.xarray_utils.time import (
-        get_min_from_xarray_time,
-        get_max_from_xarray_time,
-    )
-
     for key, xobj in xobjs.items():
         LOG.info("SECTORING dataset %s area_def %s", key, area_def.name)
         LOG.info(" requested variables %s", set(varlist))
         LOG.info(" dataset variables %s", set(xobj.variables.keys()))
         LOG.info(" dataset data_vars %s", set(xobj.data_vars))
-        LOG.info("  Min time: %s", get_min_from_xarray_time(xobj, "time"))
-        LOG.info("  Max time: %s", get_max_from_xarray_time(xobj, "time"))
         # Compile a list of variables that will be used to sector - the current data
         # variable, and we will add in the appropriate latitude and longitude variables
         # (of the same shape as data), and if it exists the appropriately shaped time
         # array.
         # Use data_vars here - since coordinates (lat/lon/time) get added below
         vars_to_interp = list(set(varlist) & set(xobj.data_vars))
         if not vars_to_interp:
@@ -877,14 +870,16 @@
                 sect_xarray.attrs["start_datetime"] = covg_xarray.start_datetime
                 sect_xarray.attrs["end_datetime"] = covg_xarray.end_datetime
 
         sect_xarray.attrs["area_definition"] = (
             area_def  # add name of this sector to sector attribute
         )
         if hasattr(sect_xarray, "time"):
+            from geoips.xarray_utils.time import get_min_from_xarray_time
+            from geoips.xarray_utils.time import get_max_from_xarray_time
 
             sect_xarray.attrs["start_datetime"] = get_min_from_xarray_time(
                 sect_xarray, "time"
             )
             sect_xarray.attrs["end_datetime"] = get_max_from_xarray_time(
                 sect_xarray, "time"
             )
@@ -899,16 +894,14 @@
             sect_xarray[vars_to_interp[0]].size,
             vars_to_interp[0],
             vars_to_interp,
         )
         sect_xarray.attrs["sectored"] = True
         ret_xobjs[key] = sect_xarray
         ret_xobjs["METADATA"] = sect_xarray[[]]
-        LOG.info("  Min time: %s", get_min_from_xarray_time(sect_xarray, "time"))
-        LOG.info("  Max time: %s", get_max_from_xarray_time(sect_xarray, "time"))
 
     return ret_xobjs
 
 
 def get_sectored_xarrays(
     xobjs, area_def, varlist, get_bg_xarrays=False, check_center=True, drop=False
 ):
@@ -932,53 +925,7 @@
     else:
         LOG.info(
             "SKIPPING BACKGROUNDS, no coverage for %s %s",
             xobjs[0].source_name,
             area_def.name,
         )
     return sect_xarrays
-
-
-def combine_preproc_xarrays_with_alg_xarray(dict_of_xarrays, alg_xarray, rgb_var=None):
-    """Combine preprocessed xarrays with an xarray output from an algorithm.
-
-    The dimensions of the preprocessed xarrays must match the algorithm xarray.
-
-    Parameters
-    ----------
-    dict_of_xarrays : dict
-        Dictionary of xarray objects (e.g. output from geoips_netcdf reader).
-    alg_xarray : xarray dataset
-        xarray dataset returned from algorithm.
-    rgb_var : bool
-        Specify the product name produced by an algorithm that outputs RGB values.
-        If so, there will not be any NaNs to replace and a composite will not be made.
-        This function will first set all 0s to NaN during the merge process,
-        then replace any remaining NaNs back to 0.
-
-    Returns
-    -------
-    xarray.Dataset
-        Combined xarray dataset of input xarrays datasets
-    """
-    # Merge xarray objects from newest to oldest
-    # Otherwise older swaths will be overlaid on newer
-    keys = sorted(dict_of_xarrays)[::-1]
-    # Set merged xarray object to alg_xarray, NaNs in this xarray dataset will
-    # be replaced with increasingly older pre-processed swaths
-    merged = alg_xarray
-    if rgb_var:
-        from numpy import nan
-
-        merged[rgb_var] = merged[rgb_var].where(merged[rgb_var] != 0, nan)
-    for i, key in enumerate(keys):
-        if key == "METADATA":
-            continue
-        preproc = dict_of_xarrays[key]
-        if rgb_var:
-            preproc[rgb_var] = preproc[rgb_var].where(preproc[rgb_var] != 0, nan)
-        # # Replace NaNs in new dataset with composited xarray
-        # merged = new_dset.combine_first(merged)
-        merged = merged.combine_first(preproc)
-    if rgb_var:
-        merged[rgb_var] = merged[rgb_var].fillna(0)
-    return merged
```

### Comparing `geoips-1.12.2/geoips/xarray_utils/time.py` & `geoips-1.12.2a0/geoips/xarray_utils/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,18 +71,14 @@
 
     Returns
     -------
     datetime.datetime
         Python datetime.datetime object representing minimum time of the
         Dataset or DataArray
     """
-    # If requested varname is not even in the xarray object, just
-    # return None rather than failing.
-    if varname not in xarray_obj.variables:
-        return None
     minval = xarray_obj[varname].min().to_dict()["data"]
     # Hack to get around bug in most recent version of numpy
     if minval is None:
         goodinds = np.ma.where(xarray_obj[varname].to_masked_array())
         minval = get_datetime_from_datetime64(
             xarray_obj[varname].to_masked_array()[goodinds].min()
         )
@@ -101,18 +97,14 @@
 
     Returns
     -------
     datetime.datetime
         Python datetime.datetime object representing maximum time of the
         Dataset or DataArray
     """
-    # If requested varname is not even in the xarray object, just
-    # return None rather than failing.
-    if varname not in xarray_obj.variables:
-        return None
     maxval = xarray_obj[varname].max().to_dict()["data"]
     # Hack to get around bug in most recent version of numpy
     if maxval is None:
         goodinds = np.ma.where(xarray_obj[varname].to_masked_array())
         maxval = get_datetime_from_datetime64(
             xarray_obj[varname].to_masked_array()[goodinds].max()
         )
```

### Comparing `geoips-1.12.2/geoips/xarray_utils/xr_to_dtree.py` & `geoips-1.12.2a0/geoips/xarray_utils/xr_to_dtree.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,23 +10,17 @@
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 """Takes in a dictionary of xarrays and converts to xarray datatree."""
 
 
 import logging
+from datatree import DataTree
 
 LOG = logging.getLogger(__name__)
-try:
-    from datatree import DataTree
-except ImportError:
-    LOG.info(
-        "Failed import DataTree in xarray_utils/xr_to_dtree.py. "
-        "If you need it, install it."
-    )
 
 
 def xarray_to_datatree(xarray_dict):
     """Convert a flat (non nested) dictionary of xarrays to DataTree format."""
     tmp_meta = xarray_dict.pop("METADATA")
     xarray_datatree = DataTree(
         name="METADATA", data=tmp_meta, children=DataTree.from_dict(xarray_dict)
```

### Comparing `geoips-1.12.2/pyproject.toml` & `geoips-1.12.2a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # required ones
 name = "geoips"  # geoips package available at the root of the project
-version = "1.12.2"  # 0.0.0 will be auto-updated with poetry dynamic versioning!
+version = "1.12.2a0"  # 0.0.0 will be auto-updated with poetry dynamic versioning!
 description = "Geolocated Information Processing System"
 authors = ["Tom <tom.jerry@colostate.edu>"]
 
 # optional ones
 maintainers = ["Tom <tom.jerry@colostate.edu>"]
 #homepage = "set the url"   // optional
 repository = "https://github.com/NRLMMD-GEOIPS/geoips" #optional
@@ -25,15 +25,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 metadata = false # don't include local-version hash; date doesn't appear by deafult
 style = "pep440" # pep440 is deafult; can rmeove later on; used for : keeping 0.0.8 as the default install until 0.0.9 is out
 #style = "semver"
 #tag-branch = "feature-poetry"
-strict = false
+strict = true
 pattern = "(?x)^((?P<epoch>\\d+)!)?(?P<base>\\d+(\\.\\d+)*)([-._]?((?P<stage>[a-zA-Z]+)[-._]?(?P<revision>\\d+)?))?(\\+(?P<tagged_metadata>.+))?$"
 
 # NOTE: You must CREATE a _version.py file and commit it via git!
 #     That file will have 0.0.0 as the version - which will get updated when
 #     pip installed.
 # FURTHER NOTE: pip install -e will actually NOT update _version.py.
 #     if you must have a valid version in your local editable install (which
@@ -60,28 +60,28 @@
 matplotlib = ">=3.7.0" # Base requirement works, version specific to test outputs
 netcdf4 = "*"          # Base requirement
 numpy = "*"            # Base requirement
 pyresample = "*"       # Base requirement Geospatial image resampling
 # efficiency improvements >= 1.22.3
 pyyaml = "*"           # Base requirement
 scipy = ">1.2"         # Base requirement, requires openblas
-xarray = "<2024.3"           # Base requirement; Pinned to <2024.3 due to bug mentioned in #558
+xarray = "*"           # Base requirement
 astropy = "*"          # Used for accounting leap seconds when converting epoch timestamps
 cartopy = ">=0.22.0"   # No longer requires libgeos
 ephem = "*"            # Required for overpass predictor
 h5py = "*"             # hdf5 readers (GMI)
 isodate = "*"          # Required for overpass predictor
 jsonschema = ">4.18.0" # Provides validation for YAML plugins
 numexpr = "<2.8.5"     # for efficiency improvements
 psutil = "*"           # Required for memory checks
 pyhdf = "*"            # hdf4 readers (MODIS)
 pyaml-env = "*"        # Reading YAML output config files, with paths
 pyorbital = "*"        # required by satpy
 pypublicdecompwt = "*" # Required to read SEVIRI data
-rasterio = "<1.3.10"         # GEOTIFF output; Pinned to <1.3.10 due to the bug mentioned in #...
+rasterio = "*"         # GEOTIFF output
 referencing = "*"
 satpy = "*"            # efficiency improvements >= 0.33.1
 scikit-image = "*"     # Radius based center coverage checks
 
 # Optional dependencies
 # To add a new optional dependency it must be added both here and in one of the "extra"
 # groups below.
@@ -147,10 +147,11 @@
 geoips = "geoips"
 
 [tool.poetry.scripts]
 convert_trackfile_to_yaml = "geoips.commandline.convert_trackfile_to_yaml:main"
 create_sector_image = "geoips.commandline.create_sector_image:main"
 list_available_plugins = "geoips.commandline.list_available_plugins:main"
 run_procflow = "geoips.commandline.run_procflow:main"
+test_interfaces = "geoips.commandline.test_interfaces:main"
 update_tc_tracks_database = "geoips.commandline.update_tc_tracks_database:main"
 xml_to_yaml_sector = "geoips.commandline.xml_to_yaml_sector:main"
 create_plugin_registries = "geoips.create_plugin_registries:main"
```

### Comparing `geoips-1.12.2/tests/outputs/abi.tc.IR-BD.imagery_annotated/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/abi.tc.IR-BD.imagery_annotated/20200918_195020_AL202020_abi_goes-16_IR-BD_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/abi.tc.Infrared.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Infrared_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/abi.tc.Infrared.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Infrared_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/abi.tc.Visible.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Visible_110kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/abi.tc.Visible.imagery_annotated/20200918_195020_AL202020_abi_goes-16_Visible_110kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/amsr2.tc.89H-Physical.imagery_annotated/20200518_073601_IO012020_amsr2_gcom-w1_89H-Physical_140kts_100p00_res1p0-cr300.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc.89H-Physical.imagery_annotated/20200518_073601_IO012020_amsr2_gcom-w1_89H-Physical_140kts_100p00_res1p0-cr300.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgInfrared-Gray.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgInfrared-Gray.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgVisible.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.37pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_37pct_140kts_95p89_res1p0-cr100-bgVisible.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgInfrared-Gray.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Infrared-Gray/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgInfrared-Gray.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgVisible.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2.tc_overlay.89pct.imagery_annotated_over_Visible/20200518_073601_IO012020_amsr2_gcom-w1_89pct_140kts_98p32_res1p0-cr100-bgVisible.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/amsr2_ocean.tc.windspeed.imagery_clean/20200518_073601_IO012020_amsr2_gcom-w1_windspeed_140kts_85p45_1p0-clean.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsr2_ocean.tc.windspeed.imagery_clean/20200518_073601_IO012020_amsr2_gcom-w1_windspeed_140kts_85p45_1p0-clean.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/amsub_mirs.tc.183-3H.imagery_annotated/20210419_235400_WP022021_amsu-b_metop-a_183-3H_115kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/amsub_mirs.tc.183-3H.imagery_annotated/20210419_235400_WP022021_amsu-b_metop-a_183-3H_115kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/ascat_knmi.tc.windbarbs.imagery_windbarbs_clean/20210421_014248_WP022021_ascat_metop-c_windbarbs_120kts_78p20_0p5-clean.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_knmi.tc.windbarbs.imagery_windbarbs_clean/20210421_014248_WP022021_ascat_metop-c_windbarbs_120kts_78p20_0p5-clean.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/ascat_low_knmi.tc.windbarbs.imagery_windbarbs/20210421_014156_WP022021_ascat_metop-c_windbarbs_120kts_35p17_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_low_knmi.tc.windbarbs.imagery_windbarbs/20210421_014156_WP022021_ascat_metop-c_windbarbs_120kts_35p17_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/ascat_noaa_25km.tc.windbarbs.imagery_windbarbs/20230524_235304_WP022023_ascat_metop-c_windbarbs_135kts_39p90_0p7.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_noaa_25km.tc.windbarbs.imagery_windbarbs/20230524_235304_WP022023_ascat_metop-c_windbarbs_135kts_39p90_0p7.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/ascat_noaa_50km.tc.wind-ambiguities.imagery_windbarbs/20230524_235200_WP022023_ascat_metop-c_wind-ambiguities_135kts_50p08_1p1.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_noaa_50km.tc.wind-ambiguities.imagery_windbarbs/20230524_235200_WP022023_ascat_metop-c_wind-ambiguities_135kts_50p08_1p1.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/ascat_uhr.tc.wind-ambiguities.imagery_windbarbs/20210421_014200_WP022021_ascatuhr_metop-c_wind-ambiguities_120kts_100p00_0p1.png.yaml` & `geoips-1.12.2a0/tests/outputs/ascat_uhr.tc.wind-ambiguities.imagery_windbarbs/20210421_014200_WP022021_ascatuhr_metop-c_wind-ambiguities_120kts_100p00_0p1.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/gmi.tc.89pct.imagery_clean/20200917_171519_AL202020_gmi_GPM_89pct_115kts_78p16_res1p0-cr300-clean.png.yaml` & `geoips-1.12.2a0/tests/outputs/gmi.tc.89pct.imagery_clean/20200917_171519_AL202020_gmi_GPM_89pct_115kts_78p16_res1p0-cr300-clean.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/hy2.tc.windspeed.imagery_annotated/20211202_084039_WP272021_hscat_hy-2b_windspeed_95kts_97p06_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/hy2.tc.windspeed.imagery_annotated/20211202_084039_WP272021_hscat_hy-2b_windspeed_95kts_97p06_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/mimic_fine.tc.TPW-PWAT.imagery_annotated/20210419_230000_WP022021_mimic_tpw_TPW-PWAT_115kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/mimic_fine.tc.TPW-PWAT.imagery_annotated/20210419_230000_WP022021_mimic_tpw_TPW-PWAT_115kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/oscat_knmi.tc.windbarbs.imagery_windbarbs/20210209_025351_SH192021_oscat_scatsat-1_windbarbs_135kts_75p10_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/oscat_knmi.tc.windbarbs.imagery_windbarbs/20210209_025351_SH192021_oscat_scatsat-1_windbarbs_135kts_75p10_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/saphir.tc.183-3HNearest.imagery_annotated/20210209_003103_SH192021_saphir_meghatropiques_183-3HNearest_135kts_88p76_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/saphir.tc.183-3HNearest.imagery_annotated/20210209_003103_SH192021_saphir_meghatropiques_183-3HNearest_135kts_88p76_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/sar.tc.nrcs.imagery_annotated/20181025_203206_WP312018_sar-spd_sentinel-1_nrcs_130kts_58p51_res1p0-cr300.png.yaml` & `geoips-1.12.2a0/tests/outputs/sar.tc.nrcs.imagery_annotated/20181025_203206_WP312018_sar-spd_sentinel-1_nrcs_130kts_58p51_res1p0-cr300.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/smos.tc.sectored.text_winds/smos-spd_surface_winds_esa_smos_tc2020sh16gabekile_202002161242.txt` & `geoips-1.12.2a0/tests/outputs/smos.tc.sectored.text_winds/smos-spd_surface_winds_esa_smos_tc2020sh16gabekile_202002161242.txt`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/ssmi.tc.37pct.imagery_clean/20200519_090000_IO012020_ssmi_F15_37pct_110kts_50p65_1p0-clean.png.yaml` & `geoips-1.12.2a0/tests/outputs/ssmi.tc.37pct.imagery_clean/20200519_090000_IO012020_ssmi_F15_37pct_110kts_50p65_1p0-clean.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/outputs/viirsday.tc.Night-Vis-IR.imagery_annotated/20210209_074210_SH192021_viirs_noaa-20_Night-Vis-IR_130kts_100p00_1p0.png.yaml` & `geoips-1.12.2a0/tests/outputs/viirsday.tc.Night-Vis-IR.imagery_annotated/20210209_074210_SH192021_viirs_noaa-20_Night-Vis-IR_130kts_100p00_1p0.png.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/commandline/test_log_setup.py` & `geoips-1.12.2a0/tests/unit_tests/commandline/test_log_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-# # # Distribution Statement A. Approved for public release. Distribution unlimited.
-# # #
-# # # Author:
-# # # Naval Research Laboratory, Marine Meteorology Division
-# # #
-# # # This program is free software: you can redistribute it and/or modify it under
-# # # the terms of the NRLMMD License included with this program. This program is
-# # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
-# # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
-# # # for more details. If you did not receive the license, for more information see:
-# # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
-
 """Unit tests for geoips/commandline/log_setup.py.
 
 Tests the following functions:
 - log_with_emphasis
 - add_log_level (by importing geoips.logging)
 """
```

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/bad/invalid_interfaces.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/invalid_interfaces.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/bad/missing_lowest_keys.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/missing_lowest_keys.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/bad/missing_plugin_types.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/bad/missing_plugin_types.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/data_fusion.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/data_fusion.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/geoips.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/geoips_clavrx.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips_clavrx.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/geoips_plugin_example.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/geoips_plugin_example.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/overcast_package.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/overcast_package.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/recenter_tc.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/recenter_tc.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/template_basic_plugin.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/template_basic_plugin.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/files/good/template_fusion_plugin.yaml` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/files/good/template_fusion_plugin.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugin_registries/test_plugin_registries.py` & `geoips-1.12.2a0/tests/unit_tests/plugin_registries/test_plugin_registries.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugins/modules/output_checkers/test_output_checkers.py` & `geoips-1.12.2a0/tests/unit_tests/plugins/modules/output_checkers/test_output_checkers.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugins/yaml/sectors/test_sectors.py` & `geoips-1.12.2a0/tests/unit_tests/plugins/yaml/sectors/test_sectors.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/plugins/yaml/test_all_yaml_plugins.py` & `geoips-1.12.2a0/tests/unit_tests/plugins/yaml/test_all_yaml_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 product_validator = ProductsPluginValidator()
 
 
 def yield_plugins():
     """Yield plugins."""
     plugin_packages = get_entry_point_group("geoips.plugin_packages")
     for pkg in plugin_packages:
-        fpath = resources.files(pkg.name) / "plugins/yaml"
+        fpath = resources.files("geoips") / "plugins/yaml"
         plugin_files = fpath.rglob("*.yaml")
         for pf in plugin_files:
             yield pf
 
 
 def gen_label(val):
     """Generate the yaml name for pytest ids."""
```

### Comparing `geoips-1.12.2/tests/unit_tests/schema/bad/feature_annotators/cartopy.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/feature_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/bad/gridline_annotators/cartopy.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/gridline_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/algorithm_colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/algorithm_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/algorithm_interpolator_colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/algorithm_interpolator_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/bases/colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/bases/colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm_colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/product_defaults/interpolator_algorithm_colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/bad/products/bases/product.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/bad/products/bases/product.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/good/feature_annotators/cartopy.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/good/feature_annotators/cartopy.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/good/product_defaults/bases/colormapper.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/good/product_defaults/bases/colormapper.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/good/products/bases/product.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/good/products/bases/product.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/good/products/single.yaml` & `geoips-1.12.2a0/tests/unit_tests/schema/good/products/single.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/schema/test_yaml_schema.py` & `geoips-1.12.2a0/tests/unit_tests/schema/test_yaml_schema.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests/xarray_utils/data.py` & `geoips-1.12.2a0/tests/unit_tests/xarray_utils/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-# # # Distribution Statement A. Approved for public release. Distribution unlimited.
-# # #
-# # # Author:
-# # # Naval Research Laboratory, Marine Meteorology Division
-# # #
-# # # This program is free software: you can redistribute it and/or modify it under
-# # # the terms of the NRLMMD License included with this program. This program is
-# # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
-# # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
-# # # for more details. If you did not receive the license, for more information see:
-# # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
-
 """Unit test module for testing functionality of geoips/xarray_utils/data.py."""
 
 from importlib import resources
 import logging
 import pytest
 from pyresample import load_area
```

### Comparing `geoips-1.12.2/tests/unit_tests/xarray_utils/test_dtree.py` & `geoips-1.12.2a0/tests/unit_tests/xarray_utils/test_dtree.py`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/unit_tests_long/plugins/modules/readers/test_readers.py` & `geoips-1.12.2a0/tests/unit_tests_long/plugins/modules/readers/test_readers.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # # # the terms of the NRLMMD License included with this program. This program is
 # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
 # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 """Unit tests on all the readers."""
-import numpy as np
 import pytest
 from geoips.commandline.log_setup import setup_logging
 from geoips.interfaces import readers
 from os import environ
 
 LOG = setup_logging()
 
@@ -29,34 +28,30 @@
         """Yeild test xarray and parameters."""
         test_xr = plugin.module.get_test_files(environ["GEOIPS_TESTDATA_DIR"])
         test_param = plugin.module.get_test_parameters()
         self.verify_xarray(test_xr, test_param)
 
     def verify_xarray(self, inxr, test_parameters):
         """Test every parameter."""
-        for test_parameter in test_parameters:
-            data_key = test_parameter["data_key"]
-            data_var = test_parameter["data_var"]
-            if "mean" in test_parameter:
-                mean = test_parameter["mean"]
-                assert np.isclose(inxr[data_key].variables[data_var].mean(), mean)
-
-            assert inxr
-            assert inxr[data_key]
-            assert inxr[data_key].longitude.max()
-            assert inxr[data_key].longitude.min()
-            assert inxr[data_key].latitude.max()
-            assert inxr[data_key].latitude.min()
-            assert inxr[data_key].variables[data_var].mean()
-            assert inxr["METADATA"].attrs["source_name"]
-            assert inxr["METADATA"].attrs["platform_name"]
-            assert inxr["METADATA"].attrs["data_provider"]
-            assert inxr["METADATA"].attrs["start_datetime"]
-            assert inxr["METADATA"].attrs["end_datetime"]
-            assert inxr["METADATA"].attrs["interpolation_radius_of_influence"]
+        data_key = test_parameters["data_key"]
+        data_var = test_parameters["data_var"]
+
+        assert inxr
+        assert inxr[data_key]
+        assert inxr[data_key].longitude.max()
+        assert inxr[data_key].longitude.min()
+        assert inxr[data_key].latitude.max()
+        assert inxr[data_key].latitude.min()
+        assert getattr(inxr[data_key], data_var).mean()
+        assert inxr["METADATA"].attrs["source_name"]
+        assert inxr["METADATA"].attrs["platform_name"]
+        assert inxr["METADATA"].attrs["data_provider"]
+        assert inxr["METADATA"].attrs["start_datetime"]
+        assert inxr["METADATA"].attrs["end_datetime"]
+        assert inxr["METADATA"].attrs["interpolation_radius_of_influence"]
 
     @pytest.mark.parametrize("reader_name", available_readers)
     def test_reader_plugins(self, reader_name):
         """Unit test every plugin, xfail for ones with no unit tests."""
         reader = readers.get_plugin(reader_name)
         if not hasattr(reader.module, "get_test_files") or not hasattr(
             reader.module, "get_test_parameters"
```

### Comparing `geoips-1.12.2/tests/utils/test_interfaces.py` & `geoips-1.12.2a0/geoips/commandline/test_interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 # # # for more details. If you did not receive the license, for more information see:
 # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/
 
 """Simple test script to run "test_interface" for each interface."""
 from pprint import pformat
 import traceback
 import json
-
-from geoips import interfaces
+from geoips import interfaces, plugin_registry
 from geoips.interfaces.base import BaseInterface
 from geoips.commandline.log_setup import setup_logging
 from geoips.commandline.args import get_argparser, check_command_line_args
-from geoips.utils.context_managers import import_optional_dependencies
 
 FAILED_INTERFACE_HEADER_PRE = "FAILED: issues found within "
 FAILED_INTERFACE_HEADER_POST = "interface:"
 
 FAILED_INTERFACE_HEADER_PRE = "FAILED: issues found within "
 FAILED_INTERFACE_HEADER_POST = "interface:"
 
@@ -76,64 +74,42 @@
 
     out_dicts = {}
 
     # Plugin registry was previously being tested during runtime.
     # We want to avoid catastrophic failure at runtime for a single
     # bad plugin, so ensure these are validated in testing, and allow
     # bad plugins to get through at runtime.
+    plg_reg = plugin_registry.PluginRegistry()
+    try:
+        LOG.interactive("Testing all registries...")
+        plg_reg.validate_all_registries()
+        successful_registries += ["all"]
+    except plugin_registry.PluginRegistryError as resp:
+        failed_registries += ["all"]
+        failed_tracebacks += [
+            f"\n\n\n{FAILED_INTERFACE_HEADER_PRE}\n\n{traceback.format_exc()}"
+        ]
+        failed_errors += [f"\n\n\n{FAILED_INTERFACE_HEADER_PRE}\n\n {str(resp)}"]
 
-    # NOTE: The section below will only be used if the user has pytest installed. We
-    # still should figure out where and when we'd like to validate the plugin
-    # registries. Currently validation of the registires invokes pytest, which is not a
-    # required dependency of GeoIPS. Calls 'plg_reg.validate_all_registries()' and
-    # 'plg_reg.validate_registry(pkg_plugins, reg_path)' are no longer on the plugin
-    # registry class, rather, they can be found under
-    # 'geoips/tests/unit_tests/plugin_registries/test_plugin_registries.py' -->
-    # PluginRegistryValidator
-
-    with import_optional_dependencies(loglevel="interactive"):
-        """Attempt to import the pytest-based PluginRegistryValidator.
-
-        If this import works, validate the registries for testing purposes. See
-        'tests.unit_tests.plugin_registries.test_plugin_registries' for more
-        information.
-        """
-        from tests.unit_tests.plugin_registries.test_plugin_registries import (
-            PluginRegistryValidator,
-        )
-        from geoips.errors import PluginRegistryError
-
-        plg_reg = PluginRegistryValidator()
+    # Now test each registry file individually.
+    for reg_path in plg_reg.registry_files:
+        pkg_plugins = json.load(open(reg_path, "r"))
+        LOG.interactive(f"Testing registry: {reg_path}...")
         try:
-            LOG.interactive("Testing all registries...")
-            plg_reg.validate_all_registries()
-            successful_registries += ["all"]
-        except PluginRegistryError as resp:
-            failed_registries += ["all"]
+            plg_reg.validate_registry(pkg_plugins, reg_path)
+            successful_registries += [reg_path]
+        except plugin_registry.PluginRegistryError as resp:
+            failed_registries += [reg_path]
             failed_tracebacks += [
-                f"\n\n\n{FAILED_INTERFACE_HEADER_PRE}\n\n{traceback.format_exc()}"
+                f"\n\n\n{FAILED_INTERFACE_HEADER_PRE} '{reg_path}'\n\n"
+                f"{traceback.format_exc()}"
+            ]
+            failed_errors += [
+                f"\n\n\n{FAILED_INTERFACE_HEADER_PRE} '{reg_path}'\n\n{str(resp)}"
             ]
-            failed_errors += [f"\n\n\n{FAILED_INTERFACE_HEADER_PRE}\n\n {str(resp)}"]
-
-        # Now test each registry file individually.
-        for reg_path in plg_reg.registry_files:
-            pkg_plugins = json.load(open(reg_path, "r"))
-            LOG.interactive(f"Testing registry: {reg_path}...")
-            try:
-                plg_reg.validate_registry(pkg_plugins, reg_path)
-                successful_registries += [reg_path]
-            except PluginRegistryError as resp:
-                failed_registries += [reg_path]
-                failed_tracebacks += [
-                    f"\n\n\n{FAILED_INTERFACE_HEADER_PRE} '{reg_path}'\n\n"
-                    f"{traceback.format_exc()}"
-                ]
-                failed_errors += [
-                    f"\n\n\n{FAILED_INTERFACE_HEADER_PRE} '{reg_path}'\n\n{str(resp)}"
-                ]
 
     # Loop through all requested interfaces, fully testing all plugins in each.
     # Collect output in lists, so we can fully print everything at the end before
     # raising an exception on error.
     for curr_interface in curr_interfaces:
         # Do not test "BaseInterface"
         if (type(curr_interface) is BaseInterface) or not isinstance(
```

### Comparing `geoips-1.12.2/tests/yaml_configs/abi_test.yaml` & `geoips-1.12.2a0/tests/yaml_configs/abi_test.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/yaml_configs/abi_test_low_memory.yaml` & `geoips-1.12.2a0/tests/yaml_configs/abi_test_low_memory.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/yaml_configs/amsr2_no_compare_full.yaml` & `geoips-1.12.2a0/tests/yaml_configs/amsr2_no_compare_full.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/yaml_configs/amsr2_test.yaml` & `geoips-1.12.2a0/tests/yaml_configs/amsr2_test.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/yaml_configs/amsr2_test_low_memory.yaml` & `geoips-1.12.2a0/tests/yaml_configs/amsr2_test_low_memory.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/tests/yaml_configs/amsr2_test_no_compare.yaml` & `geoips-1.12.2a0/tests/yaml_configs/amsr2_test_no_compare.yaml`

 * *Files identical despite different names*

### Comparing `geoips-1.12.2/PKG-INFO` & `geoips-1.12.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoips
-Version: 1.12.2
+Version: 1.12.2a0
 Summary: Geolocated Information Processing System
 Home-page: https://github.com/NRLMMD-GEOIPS/geoips
 Keywords: GeoIPS,Poetry
 Author: Tom
 Author-email: tom.jerry@colostate.edu
 Maintainer: Tom
 Maintainer-email: tom.jerry@colostate.edu
@@ -45,23 +45,23 @@
 Requires-Dist: pylint ; extra == "lint"
 Requires-Dist: pyorbital
 Requires-Dist: pypublicdecompwt
 Requires-Dist: pyresample
 Requires-Dist: pytest ; extra == "test" or extra == "test"
 Requires-Dist: pytest-cov ; extra == "test" or extra == "test"
 Requires-Dist: pyyaml
-Requires-Dist: rasterio (<1.3.10)
+Requires-Dist: rasterio
 Requires-Dist: referencing
 Requires-Dist: satpy
 Requires-Dist: scikit-image
 Requires-Dist: scipy (>1.2)
 Requires-Dist: sphinx (<7.2) ; extra == "doc"
 Requires-Dist: sphinx-design ; extra == "doc"
 Requires-Dist: sphinxcontrib-autoprogram ; extra == "doc"
-Requires-Dist: xarray (<2024.3)
+Requires-Dist: xarray
 Requires-Dist: xarray-datatree ; extra == "test"
 Project-URL: Repository, https://github.com/NRLMMD-GEOIPS/geoips
 Description-Content-Type: text/markdown
 
     # # # Distribution Statement A. Approved for public release. Distribution unlimited.
     # # #
     # # # Author:
```

