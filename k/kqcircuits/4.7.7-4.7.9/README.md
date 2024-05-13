# Comparing `tmp/kqcircuits-4.7.7.tar.gz` & `tmp/kqcircuits-4.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kqcircuits-4.7.7.tar", last modified: Fri Dec  1 15:15:49 2023, max compression
+gzip compressed data, was "kqcircuits-4.7.9.tar", last modified: Mon Dec 11 15:18:46 2023, max compression
```

## Comparing `kqcircuits-4.7.7.tar` & `kqcircuits-4.7.9.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.225663 kqcircuits-4.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-12-01 15:15:49.225663 kqcircuits-4.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.197663 kqcircuits-4.7.7/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/console_scripts/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.225663 kqcircuits-4.7.7/kqcircuits/
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-01 15:15:49.225663 kqcircuits-4.7.7/kqcircuits/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.205663 kqcircuits-4.7.7/kqcircuits/chips/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/airbridge_crossings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/airbridge_dc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31406 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/crossing_twoface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/daisy_woven.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/dc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11053 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/demo_twoface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/junction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/junction_test2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/lithography_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/lithography_test_twoface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11360 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/quality_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/quality_factor_twoface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/sample_holder_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16609 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/single_xmons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/stripes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/tsv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/chips/xmons_direct_coupling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.205663 kqcircuits-4.7.7/kqcircuits/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/airbridge_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.205663 kqcircuits-4.7.7/kqcircuits/elements/airbridges/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/airbridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/airbridges/airbridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/airbridges/airbridge_multi_face.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/airbridges/airbridge_rectangular.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/capacitive_x_coupler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/chip_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/circular_capacitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/daisy_woven.oas
--rw-r--r--   0 runner    (1001) docker     (127)    30815 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/finger_capacitor_square.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/finger_capacitor_taper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.209663 kqcircuits-4.7.7/kqcircuits/elements/flip_chip_connectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/flip_chip_connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.209663 kqcircuits-4.7.7/kqcircuits/elements/fluxlines/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/fluxlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/fluxlines/fluxline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/fluxlines/fluxline_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/fluxlines/fluxline_straight.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/hanger_resonator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/launcher_dc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.209663 kqcircuits-4.7.7/kqcircuits/elements/markers/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/markers/marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/markers/marker_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/markers/mask_marker_fc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9819 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/meander.py
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/smooth_capacitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    26807 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/spiral_resonator_polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.209663 kqcircuits-4.7.7/kqcircuits/elements/tsvs/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/tsvs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/tsvs/tsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/tsvs/tsv_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/tsvs/tsv_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)    43349 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/waveguide_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar_curved.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar_straight.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar_taper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.209663 kqcircuits-4.7.7/kqcircuits/junctions/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/junctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/junctions/junction.py
--rw-r--r--   0 runner    (1001) docker     (127)    14565 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/junctions/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/junctions/manhattan_single_junction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/junctions/no_squid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/junctions/sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/junctions/squid.py
--rw-r--r--   0 runner    (1001) docker     (127)    19943 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/klayout_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/layer_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.209663 kqcircuits-4.7.7/kqcircuits/layer_config/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/layer_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11929 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/layer_config/default_layer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    41622 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/layer_config/default_layer_props.lyp
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/layer_config/example_layer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.213663 kqcircuits-4.7.7/kqcircuits/masks/
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/masks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/masks/mask_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    30501 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/masks/mask_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    18822 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/masks/mask_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/masks/multi_face_mask_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/pya_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.213663 kqcircuits-4.7.7/kqcircuits/qubits/
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/qubits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/qubits/concentric_transmon.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/qubits/double_pads.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/qubits/double_pads_splines.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/qubits/qubit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/qubits/swissmon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.213663 kqcircuits-4.7.7/kqcircuits/simulations/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/airbridges_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/cross_section_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/empty_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.217663 kqcircuits-4.7.7/kqcircuits/simulations/export/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.217663 kqcircuits-4.7.7/kqcircuits/simulations/export/ansys/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/ansys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18211 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/ansys/ansys_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.217663 kqcircuits-4.7.7/kqcircuits/simulations/export/elmer/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/elmer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25564 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/elmer/elmer_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/export_and_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/export_singularity.py
--rw-r--r--   0 runner    (1001) docker     (127)    15893 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/remote_export_and_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/simulation_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.217663 kqcircuits-4.7.7/kqcircuits/simulations/export/sonnet/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/sonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/sonnet/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9707 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/sonnet/sonnet_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/sonnet/template.son
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.217663 kqcircuits-4.7.7/kqcircuits/simulations/export/xsection/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/xsection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28587 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/export/xsection/xsection_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    55246 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/single_element_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/single_xmons_full_chip_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/waveguides_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/simulations/xmons_direct_coupling_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.217663 kqcircuits-4.7.7/kqcircuits/test_structures/
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/airbridge_dc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/cross_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.217663 kqcircuits-4.7.7/kqcircuits/test_structures/junction_test_pads/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/junction_test_pads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/stripes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/stripes_test_increasing_width.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/test_structures/tsv_test_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.221663 kqcircuits-4.7.7/kqcircuits/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/count_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/coupler_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/deep_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/edit_node_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/export_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18383 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/geometry_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/geometry_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/groundgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/gui_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/import_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    21854 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/layout_to_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    14347 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/library_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/log_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/netlist_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/netlist_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/plugin_startup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/refpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/replace_squids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/kqcircuits/util/symmetric_polygons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:15:49.221663 kqcircuits-4.7.7/kqcircuits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-12-01 15:15:49.000000 kqcircuits-4.7.7/kqcircuits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2023-12-01 15:15:49.000000 kqcircuits-4.7.7/kqcircuits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 15:15:49.000000 kqcircuits-4.7.7/kqcircuits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-01 15:15:49.000000 kqcircuits-4.7.7/kqcircuits.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-01 15:15:49.000000 kqcircuits-4.7.7/kqcircuits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-01 15:15:49.000000 kqcircuits-4.7.7/kqcircuits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-01 15:15:49.225663 kqcircuits-4.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2023-12-01 15:15:35.000000 kqcircuits-4.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.784690 kqcircuits-4.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-12-11 15:18:46.784690 kqcircuits-4.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.756690 kqcircuits-4.7.9/console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/console_scripts/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.784690 kqcircuits-4.7.9/kqcircuits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-11 15:18:46.784690 kqcircuits-4.7.9/kqcircuits/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.764690 kqcircuits-4.7.9/kqcircuits/chips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/airbridge_crossings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/airbridge_dc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31410 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/crossing_twoface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/daisy_woven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/dc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11053 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/demo_twoface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/junction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/junction_test2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/lithography_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/lithography_test_twoface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/quality_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/quality_factor_twoface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/sample_holder_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16609 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/single_xmons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/stripes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/tsv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/chips/xmons_direct_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.768690 kqcircuits-4.7.9/kqcircuits/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/airbridge_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.768690 kqcircuits-4.7.9/kqcircuits/elements/airbridges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/airbridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/airbridges/airbridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/airbridges/airbridge_multi_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/airbridges/airbridge_rectangular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/capacitive_x_coupler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/chip_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/circular_capacitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/daisy_woven.oas
+-rw-r--r--   0 runner    (1001) docker     (127)    30878 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/finger_capacitor_square.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/finger_capacitor_taper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.768690 kqcircuits-4.7.9/kqcircuits/elements/flip_chip_connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/flip_chip_connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.768690 kqcircuits-4.7.9/kqcircuits/elements/fluxlines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/fluxlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/fluxlines/fluxline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/fluxlines/fluxline_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/fluxlines/fluxline_straight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/hanger_resonator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/launcher_dc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.768690 kqcircuits-4.7.9/kqcircuits/elements/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/markers/marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/markers/marker_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/markers/mask_marker_fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9819 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/meander.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/smooth_capacitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26807 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/spiral_resonator_polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.768690 kqcircuits-4.7.9/kqcircuits/elements/tsvs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/tsvs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/tsvs/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/tsvs/tsv_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/tsvs/tsv_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43300 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/waveguide_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar_curved.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar_straight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar_taper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.772690 kqcircuits-4.7.9/kqcircuits/junctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/junctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/junctions/junction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/junctions/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/junctions/manhattan_single_junction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/junctions/no_squid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/junctions/sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/junctions/squid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19943 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/klayout_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/layer_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.772690 kqcircuits-4.7.9/kqcircuits/layer_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/layer_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11929 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/layer_config/default_layer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41622 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/layer_config/default_layer_props.lyp
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/layer_config/example_layer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.772690 kqcircuits-4.7.9/kqcircuits/masks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/masks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/masks/mask_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31281 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/masks/mask_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18822 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/masks/mask_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/masks/multi_face_mask_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/pya_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.772690 kqcircuits-4.7.9/kqcircuits/qubits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/qubits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/qubits/concentric_transmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/qubits/double_pads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/qubits/double_pads_splines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/qubits/qubit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8632 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/qubits/swissmon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.776690 kqcircuits-4.7.9/kqcircuits/simulations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/airbridges_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/cross_section_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/empty_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.776690 kqcircuits-4.7.9/kqcircuits/simulations/export/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.776690 kqcircuits-4.7.9/kqcircuits/simulations/export/ansys/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/ansys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18647 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/ansys/ansys_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.776690 kqcircuits-4.7.9/kqcircuits/simulations/export/elmer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/elmer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35924 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/elmer/elmer_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/export_and_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/export_singularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/remote_export_and_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/simulation_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.776690 kqcircuits-4.7.9/kqcircuits/simulations/export/sonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/sonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/sonnet/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9707 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/sonnet/sonnet_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/sonnet/template.son
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.776690 kqcircuits-4.7.9/kqcircuits/simulations/export/xsection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/xsection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28587 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/export/xsection/xsection_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55246 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/single_element_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/single_xmons_full_chip_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/waveguides_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/simulations/xmons_direct_coupling_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.776690 kqcircuits-4.7.9/kqcircuits/test_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/airbridge_dc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/cross_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.780690 kqcircuits-4.7.9/kqcircuits/test_structures/junction_test_pads/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/junction_test_pads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/stripes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/stripes_test_increasing_width.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/test_structures/tsv_test_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.784690 kqcircuits-4.7.9/kqcircuits/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/count_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/coupler_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/deep_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/edit_node_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/export_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18383 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/geometry_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/geometry_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/groundgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/gui_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/import_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21854 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/layout_to_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/library_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/log_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/netlist_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/netlist_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/plugin_startup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/refpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/replace_squids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/kqcircuits/util/symmetric_polygons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:18:46.784690 kqcircuits-4.7.9/kqcircuits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-12-11 15:18:46.000000 kqcircuits-4.7.9/kqcircuits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2023-12-11 15:18:46.000000 kqcircuits-4.7.9/kqcircuits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 15:18:46.000000 kqcircuits-4.7.9/kqcircuits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-11 15:18:46.000000 kqcircuits-4.7.9/kqcircuits.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-11 15:18:46.000000 kqcircuits-4.7.9/kqcircuits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-11 15:18:46.000000 kqcircuits-4.7.9/kqcircuits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 15:18:46.784690 kqcircuits-4.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2023-12-11 15:18:30.000000 kqcircuits-4.7.9/setup.py
```

### Comparing `kqcircuits-4.7.7/PKG-INFO` & `kqcircuits-4.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kqcircuits
-Version: 4.7.7
+Version: 4.7.9
 Summary: KQCircuits is a KLayout/Python-based superconducting quantum circuit library developed by IQM.
 Home-page: https://iqm-finland.github.io/KQCircuits/
 Author: IQM Finland Oy
 Author-email: kqcircuits@meetiqm.com
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
 Requires-Dist: klayout>=0.28
```

### Comparing `kqcircuits-4.7.7/console_scripts/__init__.py` & `kqcircuits-4.7.9/console_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/console_scripts/run.py` & `kqcircuits-4.7.9/console_scripts/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
         if args.remote:
             remote_host = str(args.export_script)
             remote_export_and_run(remote_host,
                                   args.kqc_remote_tmp_path,
                                   args.detach,
                                   args.poll_interval,
+                                  args.export_path_basename,
                                   args_for_script)
             return
         if args.remote_run_only:
             remote_host = str(args.export_script)
             remote_run_only(remote_host,
                             args.kqc_remote_tmp_path,
                             args.detach,
```

### Comparing `kqcircuits-4.7.7/kqcircuits/__init__.py` & `kqcircuits-4.7.9/kqcircuits/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/_version.py` & `kqcircuits-4.7.9/kqcircuits/_version.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/__init__.py` & `kqcircuits-4.7.9/kqcircuits/chips/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/airbridge_crossings.py` & `kqcircuits-4.7.9/kqcircuits/chips/airbridge_crossings.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/airbridge_dc_test.py` & `kqcircuits-4.7.9/kqcircuits/chips/airbridge_dc_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/chip.py` & `kqcircuits-4.7.9/kqcircuits/chips/chip.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         """
         for i in range(len(self.face_ids)):
             self.merge_layout_layers_on_face(self.face(i))
 
     def produce_structures(self):
         """Produces chip frame and possibly other structures before the ground grid.
 
-        This method is called in build(). Override this method to produce a different set of chip frames.
+        This method is called in post_build(). Override this method to produce a different set of chip frames.
         """
 
         for i, face in enumerate(self.frames_enabled):
             face = int(face)
             frame_box = self.get_box(face)
             frame_parameters = self.pcell_params_by_name(
                 ChipFrame,
@@ -270,17 +270,14 @@
 
         if self.with_gnd_tsvs:
             self._produce_ground_tsvs(face_id=[0, 2])
         if self.with_face1_gnd_tsvs:
             tsv_box = self.get_box(1).enlarged(pya.DVector(-self.edge_from_tsv, -self.edge_from_tsv))
             self._produce_ground_tsvs(face_id=[3, 1], tsv_box=tsv_box)
 
-        if self.with_gnd_bumps:
-            self._produce_ground_bumps()
-
     def get_box(self, face=0):
         """
         Get the chip frame box for the specified face, correctly resolving defaults.
 
         Args:
             face: Integer specifying face, default 0
 
@@ -348,14 +345,16 @@
             self.insert_cell(bump, pya.DTrans(location))
 
         logging.info(f'Found {existing_bump_count} existing bumps and inserted {len(bump_locations)} ground bumps, '
                         + f'totalling {existing_bump_count + len(bump_locations)} bumps.')
 
     def post_build(self):
         self.produce_structures()
+        if self.with_gnd_bumps:
+            self._produce_ground_bumps()
         if self.with_grid:
             self.produce_ground_grid()
         if self.merge_base_metal_gap:
             self.merge_layout_layers()
         self._produce_instance_name_labels()
 
     def _produce_instance_name_labels(self):
```

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/crossing_twoface.py` & `kqcircuits-4.7.9/kqcircuits/chips/crossing_twoface.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/daisy_woven.py` & `kqcircuits-4.7.9/kqcircuits/chips/daisy_woven.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             y_min = min(self.box.p1.y, self.box.p2.y)
             y_max = max(self.box.p1.y, self.box.p2.y)
 
             # shorthand notation
             origin_offset_x = 1e3 * (x_max - x_min) / 2.
             origin_offset_y = 1e3 * (y_max - y_min) / 2.
 
-            chip_region = pya.Region([box.to_itype(self.layout.dbu)])  # this is already the shape of the box
+            chip_region = pya.Region(box.to_itype(self.layout.dbu))  # this is already the shape of the box
 
             # Using a static file, so use static layer indices
             daisy_shapes_base_metal_gap_wo_grid  = daisy_cell.shapes(self.layout.layer(11 + face_id * 30, 1))
             daisy_shapes_underbump_metallization = daisy_cell.shapes(self.layout.layer(32 + face_id * 30, 4))
             daisy_shapes_indium_bump             = daisy_cell.shapes(self.layout.layer(33 + face_id * 30, 4))
 
             protection = pya.Region(
```

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/dc_test.py` & `kqcircuits-4.7.9/kqcircuits/chips/dc_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/demo.py` & `kqcircuits-4.7.9/kqcircuits/chips/demo.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/demo_twoface.py` & `kqcircuits-4.7.9/kqcircuits/chips/demo_twoface.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/empty.py` & `kqcircuits-4.7.9/kqcircuits/chips/empty.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/junction_test.py` & `kqcircuits-4.7.9/kqcircuits/chips/junction_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/junction_test2.py` & `kqcircuits-4.7.9/kqcircuits/chips/junction_test2.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/launchers.py` & `kqcircuits-4.7.9/kqcircuits/chips/launchers.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/lithography_test.py` & `kqcircuits-4.7.9/kqcircuits/chips/lithography_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/lithography_test_twoface.py` & `kqcircuits-4.7.9/kqcircuits/chips/lithography_test_twoface.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/quality_factor.py` & `kqcircuits-4.7.9/kqcircuits/chips/quality_factor.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/quality_factor_twoface.py` & `kqcircuits-4.7.9/kqcircuits/chips/quality_factor_twoface.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/sample_holder_test.py` & `kqcircuits-4.7.9/kqcircuits/chips/sample_holder_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/shaping.py` & `kqcircuits-4.7.9/kqcircuits/chips/shaping.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/simple.py` & `kqcircuits-4.7.9/kqcircuits/chips/simple.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/single_xmons.py` & `kqcircuits-4.7.9/kqcircuits/chips/single_xmons.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/stripes.py` & `kqcircuits-4.7.9/kqcircuits/chips/stripes.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/tsv_test.py` & `kqcircuits-4.7.9/kqcircuits/chips/tsv_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/chips/xmons_direct_coupling.py` & `kqcircuits-4.7.9/kqcircuits/chips/xmons_direct_coupling.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/defaults.py` & `kqcircuits-4.7.9/kqcircuits/defaults.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/__init__.py` & `kqcircuits-4.7.9/kqcircuits/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/airbridge_connection.py` & `kqcircuits-4.7.9/kqcircuits/elements/airbridge_connection.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/airbridges/__init__.py` & `kqcircuits-4.7.9/kqcircuits/elements/airbridges/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/airbridges/airbridge.py` & `kqcircuits-4.7.9/kqcircuits/elements/airbridges/airbridge.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/airbridges/airbridge_multi_face.py` & `kqcircuits-4.7.9/kqcircuits/elements/airbridges/airbridge_multi_face.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/airbridges/airbridge_rectangular.py` & `kqcircuits-4.7.9/kqcircuits/elements/airbridges/airbridge_rectangular.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/capacitive_x_coupler.py` & `kqcircuits-4.7.9/kqcircuits/elements/capacitive_x_coupler.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/chip_frame.py` & `kqcircuits-4.7.9/kqcircuits/elements/chip_frame.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/circular_capacitor.py` & `kqcircuits-4.7.9/kqcircuits/elements/circular_capacitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,25 +59,25 @@
 
         # generate the outer island
         outer_island = self._get_outer_island(self.r_outer, self.outer_island_width, self.swept_angle)
         capacitor_region.append(outer_island)
         capacitor_neg = pya.Region([poly.to_itype(self.layout.dbu) for poly in capacitor_region])
 
         # add the waveguides inside the ground padding
-        capacitor_neg += pya.Region([pya.DPolygon([
+        capacitor_neg += pya.Region(pya.DPolygon([
             pya.DPoint(-x_end, -y_left),
             pya.DPoint(-0, -y_left),
             pya.DPoint(-0, y_left),
             pya.DPoint(-x_end, y_left),
-        ]).to_itype(self.layout.dbu)]) + pya.Region([pya.DPolygon([
+        ]).to_itype(self.layout.dbu)) + pya.Region(pya.DPolygon([
             pya.DPoint(x_end, y_right),
             pya.DPoint(self.r_outer - self.outer_island_width / 2, y_right),
             pya.DPoint(self.r_outer - self.outer_island_width / 2, -y_right),
             pya.DPoint(x_end, -y_right),
-        ]).to_itype(self.layout.dbu)])
+        ]).to_itype(self.layout.dbu))
         capacitor_neg.round_corners(5 / self.layout.dbu, 5 / self.layout.dbu, self.n)
         self._add_waveguides(capacitor_neg, x_end, y_left, y_right)
 
         # define the capacitor in the ground
         ground_region = self._add_ground_region(x_end)
         capacitor_region = ground_region - capacitor_neg
         self.cell.shapes(self.get_layer("base_metal_gap_wo_grid")).insert(capacitor_region)
@@ -117,22 +117,22 @@
 
         return protection_region
 
     def _add_waveguides(self, region, x_end, y_left, y_right):
         x_guide = self.fixed_length / 2 if (self.fixed_length > 0) else x_end
         if x_guide < x_end:
             raise ValueError(f"Circular capacitor parameters not compatible with fixed_length={self.fixed_length}")
-        region += pya.Region([pya.DPolygon([
+        region += pya.Region(pya.DPolygon([
             pya.DPoint(-x_end + self.margin, -y_left),
             pya.DPoint(-x_guide, -y_left),
             pya.DPoint(-x_guide, y_left),
             pya.DPoint(-x_end + self.margin, y_left),
-        ]).to_itype(self.layout.dbu)]) + pya.Region([pya.DPolygon([
+        ]).to_itype(self.layout.dbu)) + pya.Region(pya.DPolygon([
             pya.DPoint(x_end - self.margin, y_right),
             pya.DPoint(x_guide, y_right),
             pya.DPoint(x_guide, -y_right),
             pya.DPoint(x_end - self.margin, -y_right),
-        ]).to_itype(self.layout.dbu)])
+        ]).to_itype(self.layout.dbu))
 
     @classmethod
     def get_sim_ports(cls, simulation):
         return Element.left_and_right_waveguides(simulation)
```

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/daisy_woven.oas` & `kqcircuits-4.7.9/kqcircuits/elements/daisy_woven.oas`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/element.py` & `kqcircuits-4.7.9/kqcircuits/elements/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,24 +278,29 @@
         if inst_name is not None:
             # copies probing refpoints to chip level with unique names using subcell id property
             for ref_name, pos in refpoints_abs.items():
                 new_name = "{}_{}".format(inst_name, ref_name)
                 self.refpoints[new_name] = pos
         return cell_inst, refpoints_abs
 
-    def face(self, face_index=0):
-        """Returns the face dictionary corresponding to self.face_ids[face_index].
+    def _resolve_face(self, face_id):
+        """Returns face_id if the parameter is given as string or self.face_ids[face_id] otherwise.
+        The face_id as a string must be a key in default_faces but does not necessarily need to be in self.face_ids.
+        """
+        return face_id if isinstance(face_id, str) else self.face_ids[face_id]
+
+    def face(self, face_id=0):
+        """Returns the face dictionary corresponding to face_id.
 
         The face dictionary contains key "id" for the face ID and keys for all the available layers in that face.
 
         Args:
-            face_index: index of the face_id in self.face_ids, default=0
-
+            face_id: name or index of the face, default=0
         """
-        return default_faces[self.face_ids[face_index]]
+        return default_faces[self._resolve_face(face_id)]
 
     def pcell_params_by_name(self, cls=None, **parameters):
         """Give PCell parameters as a dictionary.
 
         Arguments:
             cls: Return only parameters present in this class. All by default.
             **parameters: Optionally update with other keyword arguments
@@ -325,15 +330,15 @@
         Args:
             name: name for the port. Will be "decorated" for annotation layer, left as is for port layer. If evaluates
                 to False, it will be replaced with `port`
             pos: pya.DVector or pya.DPoint marking the position of the port in the Element base
             direction: direction of the signal going _to_ the port to determine the location of the "corner" reference
                 point which is used for waveguide direction. If evaluates to False as is the default, no corner point is
                 added.
-            face_id: index of the face id, default=0
+            face_id: name or index of the face, default=0
         """
         text = pya.DText(name, pos.x, pos.y)
         self.cell.shapes(self.get_layer("ports", face_id)).insert(text)
 
         port_name = name if "port" in name else ("port_"+name if name else "port")
         self.refpoints[port_name] = pos
         if direction:
@@ -420,20 +425,17 @@
     def get_layer(self, layer_name, face_id=0):
         """Returns the specified Layer object.
 
         Args:
             layer_name: layer name text
             face_id: Name or index of the face to use, default=0
         """
-        if isinstance(face_id, str):
-            return self.layout.layer(self.face(self.face_ids.index(face_id))[layer_name])
-        elif (face_id == 0) and (layer_name not in self.face(0)):
+        if (face_id == 0) and (layer_name not in self.face(0)):
             return self.layout.layer(default_layers[layer_name])
-        else:
-            return self.layout.layer(self.face(face_id)[layer_name])
+        return self.layout.layer(self.face(face_id)[layer_name])
 
     @staticmethod
     def _create_cell(elem_cls, layout, library=None, **parameters) -> pya.Cell:
         """Create cell for elem_cls in layout.
 
         This is separated from the class method `create` to enable invocation from classes where `create` is shadowed.
 
@@ -518,25 +520,24 @@
         raise ValueError(error_msg)
 
     def add_protection(self, shape, face_id=0):
         """Add ground grid protection shape
 
         Args:
              shape: The shape (Region, DPolygon, etc.) to add to ground_grid_avoidance layer
-             face_id: primary face index of ground_grid_avoidance layer, default=0
+             face_id: Name or index of the primary face of ground_grid_avoidance layer, default=0
         """
-
-        self.cell.shapes(self.get_layer("ground_grid_avoidance", face_id)).insert(shape)
+        face = self._resolve_face(face_id)
+        self.cell.shapes(self.get_layer("ground_grid_avoidance", face)).insert(shape)
         if self.protect_opposite_face:
             for group in self.opposing_face_id_groups:
-                if self.face_ids[face_id] in group:
-                    for other_face_id in group:
-                        if other_face_id != self.face_ids[face_id] and other_face_id in self.face_ids:
-                            self.cell.shapes(self.get_layer("ground_grid_avoidance",
-                                                            self.face_ids.index(other_face_id))).insert(shape)
+                if face in group:
+                    for other_face in group:
+                        if other_face != face:
+                            self.cell.shapes(self.get_layer("ground_grid_avoidance", other_face)).insert(shape)
                     break
 
     def sync_parameters(self, abc):
         """Syncronise the calling class' parameters with a JSON representation.
 
         This is called several times from coerce_parameters_impl() while using the PCell editor GUI. Particularly, each
         time a parameter of abc's sub-class is changed by the user. It figures out which parameter is changed and
```

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/finger_capacitor_square.py` & `kqcircuits-4.7.9/kqcircuits/elements/finger_capacitor_square.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,34 +52,34 @@
         x_left = x_mid + self.finger_width + (self.ground_padding if y_left > y_mid else 0.0)
         x_right = x_mid + self.finger_width + (self.ground_padding if y_right > y_mid else 0.0)
         x_end = x_mid + self.finger_width + self.ground_padding
         x_max = x_end + self.corner_r
 
         region_ground = self.get_ground_region()
 
-        region_taper_right = pya.Region([pya.DPolygon([
+        region_taper_right = pya.Region(pya.DPolygon([
             pya.DPoint(x_mid, y_mid),
             pya.DPoint(x_right, y_mid),
             pya.DPoint(x_right, y_right),
             pya.DPoint(x_max, y_right),
             pya.DPoint(x_max, -y_right),
             pya.DPoint(x_right, -y_right),
             pya.DPoint(x_right, -y_mid),
             pya.DPoint(x_mid, -y_mid)
-        ]).to_itype(self.layout.dbu)])
-        region_taper_left = pya.Region([pya.DPolygon([
+        ]).to_itype(self.layout.dbu))
+        region_taper_left = pya.Region(pya.DPolygon([
             pya.DPoint(-x_mid, y_mid),
             pya.DPoint(-x_left, y_mid),
             pya.DPoint(-x_left, y_left),
             pya.DPoint(-x_max, y_left),
             pya.DPoint(-x_max, -y_left),
             pya.DPoint(-x_left, -y_left),
             pya.DPoint(-x_left, -y_mid),
             pya.DPoint(-x_mid, -y_mid)
-        ]).to_itype(self.layout.dbu)])
+        ]).to_itype(self.layout.dbu))
 
         polys_fingers = []
         for i in range(self.finger_number):
             x = (i % 2) * self.finger_gap_end - x_mid
             y = i * (self.finger_width + self.finger_gap) - y_mid
             polys_fingers.append(pya.DPolygon([
                 pya.DPoint(x + self.finger_length, y + self.finger_width),
@@ -119,28 +119,28 @@
         y_right = (self.a if self.a2 < 0 else self.a2) / 2 + (self.b if self.b2 < 0 else self.b2)
         x_mid = self.finger_area_length() / 2 + self.finger_width
         x_left = x_mid + (self.ground_padding if y_left < y_mid else 0.0)
         x_right = x_mid + (self.ground_padding if y_right < y_mid else 0.0)
         x_end = x_mid + self.ground_padding
         x_max = x_end + self.corner_r
 
-        region_ground = pya.Region([pya.DPolygon([
+        region_ground = pya.Region(pya.DPolygon([
             pya.DPoint(-x_left, -y_mid),
             pya.DPoint(-x_left, -y_left),
             pya.DPoint(-x_max, -y_left),
             pya.DPoint(-x_max, y_left),
             pya.DPoint(-x_left, y_left),
             pya.DPoint(-x_left, y_mid),
             pya.DPoint(x_right, y_mid),
             pya.DPoint(x_right, y_right),
             pya.DPoint(x_max, y_right),
             pya.DPoint(x_max, -y_right),
             pya.DPoint(x_right, -y_right),
             pya.DPoint(x_right, -y_mid),
-        ]).to_itype(self.layout.dbu)])
+        ]).to_itype(self.layout.dbu))
 
         if self.ground_gap_ratio > 0:
             x_conn = self.ground_gap_ratio * self.finger_gap_end / 2
             left_pts = []
             right_pts = []
             for i in range(self.finger_number):
                 sign = 2 * (i % 2) - 1
@@ -148,50 +148,50 @@
                 y0 = i * (self.finger_width + self.finger_gap) - (finger_area_width + self.finger_gap) / 2
                 y1 = y0 + self.finger_width + self.finger_gap
                 y_conn = sign * self.ground_gap_ratio * self.finger_gap / 2
                 left_pts += [pya.DPoint(x - x_conn, y0 - y_conn if i > 0 else -y_mid),
                              pya.DPoint(x - x_conn, y1 + y_conn if i + 1 < self.finger_number else y_mid)]
                 right_pts += [pya.DPoint(x + x_conn, y0 + y_conn if i > 0 else -y_mid),
                               pya.DPoint(x + x_conn, y1 - y_conn if i + 1 < self.finger_number else y_mid)]
-            region_ground -= pya.Region([pya.DPolygon(left_pts + right_pts[::-1]).to_itype(self.layout.dbu)])
+            region_ground -= pya.Region(pya.DPolygon(left_pts + right_pts[::-1]).to_itype(self.layout.dbu))
 
         region_ground.round_corners(self.corner_r / self.layout.dbu, self.corner_r / self.layout.dbu, self.n)
         self.cut_region(region_ground, x_end, max(y_mid, y_left, y_right))
         self.add_waveguides(region_ground, x_end, y_left, y_right)
 
         return region_ground
 
     def finger_area_width(self):
         return self.finger_number * self.finger_width + (self.finger_number - 1) * self.finger_gap
 
     def finger_area_length(self):
         return self.finger_length + self.finger_gap_end
 
     def cut_region(self, region, x_max, y_max):
-        cutter = pya.Region([pya.DPolygon([
+        cutter = pya.Region(pya.DPolygon([
             pya.DPoint(x_max, -y_max),
             pya.DPoint(x_max, y_max),
             pya.DPoint(-x_max, y_max),
             pya.DPoint(-x_max, -y_max)
-        ]).to_itype(self.layout.dbu)])
+        ]).to_itype(self.layout.dbu))
         region &= cutter
 
     def add_waveguides(self, region, x_end, y_left, y_right):
         x_guide = self.fixed_length / 2
         if self.fixed_length != 0 and x_guide < x_end:
             raise ValueError(f"FingerCapacitorSquare parameters not compatible with fixed_length={self.fixed_length}")
         if x_guide > x_end:
-            region += pya.Region([pya.DPolygon([
+            region += pya.Region(pya.DPolygon([
                 pya.DPoint(-x_end, -y_left),
                 pya.DPoint(-x_guide, -y_left),
                 pya.DPoint(-x_guide, y_left),
                 pya.DPoint(-x_end, y_left),
-            ]).to_itype(self.layout.dbu)]) + pya.Region([pya.DPolygon([
+            ]).to_itype(self.layout.dbu)) + pya.Region(pya.DPolygon([
                 pya.DPoint(x_end, y_right),
                 pya.DPoint(x_guide, y_right),
                 pya.DPoint(x_guide, -y_right),
                 pya.DPoint(x_end, -y_right),
-            ]).to_itype(self.layout.dbu)])
+            ]).to_itype(self.layout.dbu))
 
     @classmethod
     def get_sim_ports(cls, simulation):
         return Element.left_and_right_waveguides(simulation)
```

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/finger_capacitor_taper.py` & `kqcircuits-4.7.9/kqcircuits/elements/finger_capacitor_taper.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,32 +46,32 @@
         l = self.finger_length
         g = self.finger_gap
         t = self.taper_length
         total_width = float(n) * (w + g) - g
         a = self.a
         b = self.b
 
-        region_ground = pya.Region([pya.DPolygon([
+        region_ground = pya.Region(pya.DPolygon([
             pya.DPoint((l + g) / 2, total_width * (b / a) + total_width / 2),
             pya.DPoint((l + g) / 2 + t, b + a / 2),
             pya.DPoint((l + g) / 2 + t, -b - a / 2),
             pya.DPoint((l + g) / 2, -total_width * (b / a) - total_width / 2),
             pya.DPoint(-(l + g) / 2, -total_width * (b / a) - total_width / 2),
             pya.DPoint(-(l + g) / 2 - t, -b - a / 2),
             pya.DPoint(-(l + g) / 2 - t, b + a / 2),
             pya.DPoint(-(l + g) / 2, total_width * (b / a) + total_width / 2),
 
-        ]).to_itype(self.layout.dbu)])
+        ]).to_itype(self.layout.dbu))
 
-        region_taper_right = pya.Region([pya.DPolygon([
+        region_taper_right = pya.Region(pya.DPolygon([
             pya.DPoint((l + g) / 2, total_width / 2),
             pya.DPoint((l + g) / 2 + t, a / 2),
             pya.DPoint((l + g) / 2 + t, -a / 2),
             pya.DPoint((l + g) / 2, -total_width / 2)
-        ]).to_itype(self.layout.dbu)])
+        ]).to_itype(self.layout.dbu))
         region_taper_left = region_taper_right.transformed(pya.Trans().M90)
 
         polys_fingers = []
         poly_finger = pya.DPolygon([
             pya.DPoint(l / 2, w),
             pya.DPoint(l / 2, 0),
             pya.DPoint(-l / 2, 0),
@@ -84,20 +84,20 @@
 
         region_fingers = pya.Region([
             poly.to_itype(self.layout.dbu) for poly in polys_fingers
         ])
         region_etch = region_taper_left + region_taper_right + region_fingers
         region_etch.round_corners(self.corner_r / self.layout.dbu, self.corner_r / self.layout.dbu, self.n)
 
-        region_taper_right_small = pya.Region([pya.DPolygon([
+        region_taper_right_small = pya.Region(pya.DPolygon([
             pya.DPoint((l + g) / 2 + self.corner_r, (total_width / 2 - a / 2) * (t - 2 * self.corner_r) / t + a / 2),
             pya.DPoint((l + g) / 2 + t, a / 2),
             pya.DPoint((l + g) / 2 + t, -a / 2),
             pya.DPoint((l + g) / 2 + self.corner_r, -(total_width / 2 - a / 2) * (t - 2 * self.corner_r) / t - a / 2)
-        ]).to_itype(self.layout.dbu)])
+        ]).to_itype(self.layout.dbu))
         region_taper_left_small = region_taper_right_small.transformed(pya.Trans().M90)
 
         region = (region_ground - region_etch) - region_taper_right_small - region_taper_left_small
 
         self.cell.shapes(self.get_layer("base_metal_gap_wo_grid")).insert(region)
 
         # protection
```

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/flip_chip_connectors/__init__.py` & `kqcircuits-4.7.9/kqcircuits/elements/flip_chip_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py` & `kqcircuits-4.7.9/kqcircuits/elements/flip_chip_connectors/flip_chip_connector.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py` & `kqcircuits-4.7.9/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_dc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py` & `kqcircuits-4.7.9/kqcircuits/elements/flip_chip_connectors/flip_chip_connector_rf.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
             length = w + bumps_length
 
             def produce_shape(face, a, b, rotation, trace_rotation):
                 # Base metal gap outline
                 trace_dtrans = pya.DCplxTrans(1, trace_rotation, False, - bumps_length / 2, 0)
                 trace_itrans = trace_dtrans.to_itrans(self.layout.dbu)
                 region = rounded_plate(0, w, length) + trace(0, a + 2 * b, - w / 2).transformed(trace_itrans)
-                logging.info(f'{str(trace_itrans)=}')
 
                 # Ground grid avoidance
                 avoid_region = region.sized(self.margin / self.layout.dbu, self.margin / self.layout.dbu, 2)
 
                 # Subtract circles under bumps
                 for i in range(self.n_center_bumps):
                     region -= rounded_plate((i - (self.n_center_bumps - 1) / 2) * self.inter_bump_distance,
```

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/fluxlines/__init__.py` & `kqcircuits-4.7.9/kqcircuits/elements/fluxlines/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/fluxlines/fluxline.py` & `kqcircuits-4.7.9/kqcircuits/elements/fluxlines/fluxline.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/fluxlines/fluxline_standard.py` & `kqcircuits-4.7.9/kqcircuits/elements/fluxlines/fluxline_standard.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/fluxlines/fluxline_straight.py` & `kqcircuits-4.7.9/kqcircuits/elements/fluxlines/fluxline_straight.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/hanger_resonator.py` & `kqcircuits-4.7.9/kqcircuits/elements/hanger_resonator.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/launcher.py` & `kqcircuits-4.7.9/kqcircuits/elements/launcher.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/launcher_dc.py` & `kqcircuits-4.7.9/kqcircuits/elements/launcher_dc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/markers/__init__.py` & `kqcircuits-4.7.9/kqcircuits/elements/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/markers/marker.py` & `kqcircuits-4.7.9/kqcircuits/elements/markers/marker.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         # center box
         sqr_uni = pya.DBox(
             pya.DPoint(10, 10),
             pya.DPoint(-10, -10),
         )
         insert_to_main_layers(sqr_uni)
 
-        self.inv_corners = pya.Region([protection_box.to_itype(self.layout.dbu)])
+        self.inv_corners = pya.Region(protection_box.to_itype(self.layout.dbu))
         self.inv_corners -= corners
         self.cell.shapes(layer_pads).insert(self.inv_corners - pya.Region(sqr_uni.to_itype(self.layout.dbu)))
 
         # window for airbridge flyover layer
         aflw = pya.DPolygon([
             pya.DPoint(800, 800),
             pya.DPoint(800, 10),
```

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/markers/marker_standard.py` & `kqcircuits-4.7.9/kqcircuits/elements/markers/marker_standard.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/markers/mask_marker_fc.py` & `kqcircuits-4.7.9/kqcircuits/elements/markers/mask_marker_fc.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         # protection for the box
         protection_box = pya.DBox(
             pya.DPoint(200, 350),
             pya.DPoint(-200, -350)
         )
         self.cell.shapes(layer_protection).insert(protection_box)
-        negative_layer = pya.Region([protection_box.to_itype(self.layout.dbu)])
+        negative_layer = pya.Region(protection_box.to_itype(self.layout.dbu))
 
         # crosses
 
         arm_widths = [20, 35, 70]
         arm_lengths = [70, 124, 250]
         offset_width = [30, 43, 85]
         offset_length = [80, 132, 265]
@@ -107,15 +107,15 @@
             insert_to_main_layers(inner_shapes)
             inner_corner_shape = pya.DCplxTrans(1, 0, False,
                                                 pya.DVector(shift)) * self.create_cross(cross_length, cross_width)
             for layer_insert in [layer_pads]:
                 self.cell.shapes(layer_insert).insert(inner_corner_shape)
             negative_offset = pya.DCplxTrans(1, 0, False,
                                              pya.DVector(shift)) * self.create_cross(arm_lengths[i], arm_widths[i])
-            negative_layer -= pya.Region([negative_offset.to_itype(self.layout.dbu)])
+            negative_layer -= pya.Region(negative_offset.to_itype(self.layout.dbu))
 
             inner_shapes_offset = pya.DCplxTrans(1, 0, False,
                                                  pya.DVector(shift)) * self.create_cross(arm_lengths[i], arm_widths[i])
             self.cell.shapes(layer_indium_bump).insert(inner_shapes_offset)
         self.cell.shapes(layer_ubm).insert(negative_layer)
         # marker arrow
         for i in range(self.arrow_number):
```

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/meander.py` & `kqcircuits-4.7.9/kqcircuits/elements/meander.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/smooth_capacitor.py` & `kqcircuits-4.7.9/kqcircuits/elements/smooth_capacitor.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/spiral_resonator_polygon.py` & `kqcircuits-4.7.9/kqcircuits/elements/spiral_resonator_polygon.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/tsvs/__init__.py` & `kqcircuits-4.7.9/kqcircuits/elements/tsvs/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/tsvs/tsv.py` & `kqcircuits-4.7.9/kqcircuits/elements/tsvs/tsv.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/tsvs/tsv_ellipse.py` & `kqcircuits-4.7.9/kqcircuits/elements/tsvs/tsv_ellipse.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/tsvs/tsv_standard.py` & `kqcircuits-4.7.9/kqcircuits/elements/tsvs/tsv_standard.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/waveguide_composite.py` & `kqcircuits-4.7.9/kqcircuits/elements/waveguide_composite.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,15 +535,15 @@
             params['a'], params['b'] = self.a, self.b
 
         fc_cell = self.add_element(element, **params)
 
         self._insert_cell_and_waveguide(ind, fc_cell, before=f'{self.old_id}_port', after=f'{self.new_id}_port')
 
         self.a, self.b = new_a, new_b
-        self.face_ids = [self.new_id] + [a for a in self.face_ids if a != self.new_id]
+        self.face_ids = [self.new_id]
 
         if 'r' in node.params:
             self.r = params['r']
 
     def _add_airbridge(self, ind, **kwargs):
         """Add an airbridge with tapers at both sides and change default a/b if required."""
```

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar.py` & `kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,23 +178,27 @@
         b = elem.b
 
         v = (point_2 - point_1)*(1/point_1.distance(point_2))
         u = pya.DTrans.R270.trans(v)
         shift_start = pya.DTrans(pya.DVector(point_2))
 
         if term_len > 0:
-            poly = pya.DPolygon([u*(a/2 + b), u*(a/2 + b) + v*term_len, u*(-a/2 - b) + v*term_len,
-                                 u*(-a/2 - b)])
+            poly = pya.DPolygon([pya.DPoint(u*(a/2 + b)),
+                                 pya.DPoint(u*(a/2 + b) + v*term_len),
+                                 pya.DPoint(u*(-a/2 - b) + v*term_len),
+                                 pya.DPoint(u*(-a/2 - b))])
             elem.cell.shapes(elem.layout.layer(elem.face(face_index)["base_metal_gap_wo_grid"])).insert(
                 poly.transform(shift_start))
 
         # protection
         term_len += elem.margin
-        poly2 = pya.DPolygon([u*(a/2 + b + elem.margin), u*(a/2 + b + elem.margin) + v*term_len,
-                              u*(-a/2 - b - elem.margin) + v*term_len, u*(-a/2 - b - elem.margin)])
+        poly2 = pya.DPolygon([pya.DPoint(u*(a/2 + b + elem.margin)),
+                              pya.DPoint(u*(a/2 + b + elem.margin) + v*term_len),
+                              pya.DPoint(u*(-a/2 - b - elem.margin) + v*term_len),
+                              pya.DPoint(u*(-a/2 - b - elem.margin))])
         elem.add_protection(poly2.transform(shift_start), face_index)
 
     @staticmethod
     def is_continuous(waveguide_cell, annotation_layer, tolerance):
         """Returns true if the given waveguide is determined to be continuous, false otherwise.
 
         The waveguide is considered continuous if the endpoints of its every segment (except first and last) are close
```

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar_curved.py` & `kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar_curved.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar_splitter.py` & `kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar_splitter.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar_straight.py` & `kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar_straight.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/elements/waveguide_coplanar_taper.py` & `kqcircuits-4.7.9/kqcircuits/elements/waveguide_coplanar_taper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/junctions/__init__.py` & `kqcircuits-4.7.9/kqcircuits/junctions/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/junctions/junction.py` & `kqcircuits-4.7.9/kqcircuits/junctions/junction.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/junctions/manhattan.py` & `kqcircuits-4.7.9/kqcircuits/junctions/manhattan.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/junctions/manhattan_single_junction.py` & `kqcircuits-4.7.9/kqcircuits/junctions/manhattan_single_junction.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/junctions/no_squid.py` & `kqcircuits-4.7.9/kqcircuits/junctions/no_squid.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/junctions/sim.py` & `kqcircuits-4.7.9/kqcircuits/junctions/sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/junctions/squid.py` & `kqcircuits-4.7.9/kqcircuits/junctions/squid.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/klayout_view.py` & `kqcircuits-4.7.9/kqcircuits/klayout_view.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/layer_cluster.py` & `kqcircuits-4.7.9/kqcircuits/layer_cluster.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/layer_config/__init__.py` & `kqcircuits-4.7.9/kqcircuits/layer_config/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/layer_config/default_layer_config.py` & `kqcircuits-4.7.9/kqcircuits/layer_config/default_layer_config.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/layer_config/default_layer_props.lyp` & `kqcircuits-4.7.9/kqcircuits/layer_config/default_layer_props.lyp`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/layer_config/example_layer_config.py` & `kqcircuits-4.7.9/kqcircuits/layer_config/example_layer_config.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/masks/__init__.py` & `kqcircuits-4.7.9/kqcircuits/masks/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/masks/mask_export.py` & `kqcircuits-4.7.9/kqcircuits/masks/mask_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     layout = top_cell.layout()
     layer_info = resolve_default_layer_info(layer_name, mask_layout.face_id)
     layer = layout.layer(layer_info)
     tmp_layer = layout.layer()
 
     if invert:
         wafer = pya.Region(top_cell.begin_shapes_rec(layer)).merged()
-        disc = pya.Region([circle_polygon(mask_layout.wafer_rad).to_itype(layout.dbu)])
+        disc = pya.Region(circle_polygon(mask_layout.wafer_rad).to_itype(layout.dbu))
         layout.copy_layer(layer, tmp_layer)
         layout.clear_layer(layer)
         top_cell.shapes(layer).insert(wafer ^ disc)
 
     if mirror:
         wafer = pya.Region(top_cell.begin_shapes_rec(layer)).merged()
         layout.copy_layer(layer, tmp_layer)
```

### Comparing `kqcircuits-4.7.7/kqcircuits/masks/mask_layout.py` & `kqcircuits-4.7.9/kqcircuits/masks/mask_layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -276,26 +276,35 @@
                     labels_cells[submask_layout] = inst_cell
                     break
 
         # find all unique x and y coords of chips and place them in the corresponding keys in chips_dict
         chips_dict = {}  # {(pos_x, pos_y): chip_name, chip_pos (in submask coordinates), chip_inst, mask_layout}
         xvals = set()
         yvals = set()
+        # To not pollute the space of chip positions, rather than assigning a new row letter and column number
+        # for each unique x- and y-coordinate, round the coordinates to the smallest chip dimensions.
+        # This still guarantees that each chip gets unique chip position label, but rows that are closer
+        # together than the smallest chip height will be assigned the same letter.
+        unit_x = min(bbox.p2.x - bbox.p1.x for _,_,bbox,_,_ in self.added_chips)
+        unit_y = min(bbox.p2.y - bbox.p1.y for _,_,bbox,_,_ in self.added_chips)
         for chip_name, pos, bbox, dtrans, position_label in self.added_chips:
+            pos_x = math.floor(pos.x / unit_x) * unit_x
+            pos_y = math.floor(pos.y / unit_y) * unit_y
             if not position_label:
-                xvals.add(pos.x)
-                yvals.add(pos.y)
-            chips_dict[(pos.x, pos.y)] = chip_name, pos, bbox, dtrans, position_label, self
+                xvals.add(pos_x)
+                yvals.add(pos_y)
+            chips_dict[(pos_x, pos_y)] = chip_name, pos, bbox, dtrans, position_label, self
         for submask_layout, submask_pos in self.submasks:
             for chip_name, pos, bbox, dtrans, position_label in submask_layout.added_chips:
-                pos2 = pos + submask_pos
+                pos_x = math.floor((pos + submask_pos).x / unit_x) * unit_x
+                pos_y = math.floor((pos + submask_pos).y / unit_y) * unit_y
                 if not position_label:
-                    xvals.add(pos2.x)
-                    yvals.add(pos2.y)
-                chips_dict[(pos2.x, pos2.y)] = chip_name, pos, bbox, dtrans, position_label, submask_layout
+                    xvals.add(pos_x)
+                    yvals.add(pos_y)
+                chips_dict[(pos_x, pos_y)] = chip_name, pos, bbox, dtrans, position_label, submask_layout
         # produce the labels such that chips with identical x-coordinate (y-coordinate) have identical number (letter)
         used_position_labels = set()
         for (x, y), (chip_name, _, bbox, dtrans, position_label, mask_layout) in chips_dict.items():
             labels_cell_2 = labels_cells[mask_layout]
             if x not in xvals or y not in yvals:
                 i, j = None, None
             else:
@@ -387,15 +396,15 @@
                 orig = pya.DVector(-h + self._min_x * self.layout.dbu, w)
             elif align == "right":
                 orig = pya.DVector(self._max_x * self.layout.dbu, w)
         if align in ("left", "right"):  # rotate clockwise
             chips_map = zip(*reversed(chips_map))
 
         region_used = pya.Region()
-        allowed_region = pya.Region([circle_polygon(self.wafer_rad - self.edge_clearance).to_itype(self.layout.dbu)]) \
+        allowed_region = pya.Region(circle_polygon(self.wafer_rad - self.edge_clearance).to_itype(self.layout.dbu)) \
             - marker_region \
             - pya.Region(pya.DBox(-self.wafer_rad, self._mask_name_box_bottom_y,
                                   self.wafer_rad, self.wafer_rad).to_itype(self.layout.dbu))
         for (i, row) in enumerate(tqdm(chips_map, desc='Adding chips to mask', bar_format=default_bar_format)):
             for (j, name) in enumerate(row):
                 if name == "---":
                     continue
```

### Comparing `kqcircuits-4.7.7/kqcircuits/masks/mask_set.py` & `kqcircuits-4.7.9/kqcircuits/masks/mask_set.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/masks/multi_face_mask_layout.py` & `kqcircuits-4.7.9/kqcircuits/masks/multi_face_mask_layout.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/pya_resolver.py` & `kqcircuits-4.7.9/kqcircuits/pya_resolver.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/qubits/__init__.py` & `kqcircuits-4.7.9/kqcircuits/qubits/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/qubits/concentric_transmon.py` & `kqcircuits-4.7.9/kqcircuits/qubits/concentric_transmon.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,26 +125,26 @@
     def _make_waveguides(self):
         # Make the waveguides for each coupler with custom impedance and return the region
         waveguides_signal_region = pya.Region()
         waveguides_gap_region = pya.Region()
         # Add the waveguides inside the ground padding
         overlapping_margin = 0.5
         for (c_a, c_b, c_angle) in zip(self.couplers_a, self.couplers_b, self.couplers_angle):
-            waveguide_signal = pya.Region([pya.DPolygon([
+            waveguide_signal = pya.Region(pya.DPolygon([
                 pya.DPoint(self.x_end + overlapping_margin, float(c_a) / 2),
                 pya.DPoint(self.couplers_r, float(c_a) / 2),
                 pya.DPoint(self.couplers_r, -float(c_a) / 2),
                 pya.DPoint(self.x_end + overlapping_margin, -float(c_a) / 2),
-            ]).to_itype(self.layout.dbu)]).transformed(pya.ICplxTrans(1, float(c_angle), False, 0, 0))
-            waveguide_gap = pya.Region([pya.DPolygon([
+            ]).to_itype(self.layout.dbu)).transformed(pya.ICplxTrans(1, float(c_angle), False, 0, 0))
+            waveguide_gap = pya.Region(pya.DPolygon([
                 pya.DPoint(self.x_end, float(c_a) / 2 + float(c_b)),
                 pya.DPoint(self.couplers_r, float(c_a) / 2 + float(c_b)),
                 pya.DPoint(self.couplers_r, -float(c_a) / 2 - float(c_b)),
                 pya.DPoint(self.x_end, -float(c_a) / 2 - float(c_b)),
-            ]).to_itype(self.layout.dbu)]).transformed(pya.ICplxTrans(1, float(c_angle), False, 0, 0))
+            ]).to_itype(self.layout.dbu)).transformed(pya.ICplxTrans(1, float(c_angle), False, 0, 0))
             waveguides_signal_region += waveguide_signal
             waveguides_gap_region += waveguide_gap
         return waveguides_signal_region, waveguides_gap_region
 
     def _add_junction(self, region):
         # Add the junction to the qubit islands
         squid_origin = \
```

### Comparing `kqcircuits-4.7.7/kqcircuits/qubits/double_pads.py` & `kqcircuits-4.7.9/kqcircuits/qubits/double_pads.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     island1_taper_junction_width = Param(pdt.TypeDouble,
                                          "First qubit island tapering width on the junction side", 10, unit="µm")
     island2_taper_width = Param(pdt.TypeDouble, "Second qubit island tapering width on the island side", 10, unit="µm")
     island2_taper_junction_width = Param(pdt.TypeDouble,
                                          "Second qubit island tapering width on the junction side", 10, unit="µm")
 
     island_island_gap = Param(pdt.TypeDouble, "Island to island gap distance", 70, unit="µm")
+    with_squid = Param(pdt.TypeBoolean, "Boolean whether to include the squid", True)
 
     def build(self):
 
         # Qubit base
         ground_gap_points = [
             pya.DPoint(float(self.ground_gap[0]) / 2,  float(self.ground_gap[1]) / 2),
             pya.DPoint(float(self.ground_gap[0]) / 2, -float(self.ground_gap[1]) / 2),
@@ -78,15 +79,17 @@
         # SQUID
         # Create temporary SQUID cell to calculate SQUID height
         temp_squid_cell = self.add_element(Squid, junction_type=self.junction_type)
         temp_squid_ref = self.get_refpoints(temp_squid_cell)
         squid_height = temp_squid_ref["port_common"].distance(pya.DPoint(0, 0))
         # Now actually add SQUID
         squid_transf = pya.DCplxTrans(1, 0, False, pya.DVector(0, self.squid_offset - squid_height / 2))
-        self.produce_squid(squid_transf)
+
+        if self.with_squid:
+            self.produce_squid(squid_transf)
 
         taper_height = (self.island_island_gap - squid_height)/2
 
         # First island
         island1_region = self._build_island1(squid_height, taper_height)
 
         # Second island
```

### Comparing `kqcircuits-4.7.7/kqcircuits/qubits/double_pads_splines.py` & `kqcircuits-4.7.9/kqcircuits/qubits/double_pads_splines.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/qubits/qubit.py` & `kqcircuits-4.7.9/kqcircuits/qubits/qubit.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/qubits/swissmon.py` & `kqcircuits-4.7.9/kqcircuits/qubits/swissmon.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         aw = [ww, wn, we, ws][cpl_nr]
         w = float(self.cpl_width[cpl_nr])
         l = float(self.cpl_length[cpl_nr])
         g = float(self.cpl_gap[cpl_nr]) / 2
 
         # Location for connecting the waveguides to
         port_shape = pya.DBox(-a / 2, 0, a / 2, b)
-        port_region = pya.Region([port_shape.to_itype(self.layout.dbu)])
+        port_region = pya.Region(port_shape.to_itype(self.layout.dbu))
 
         if l > 0:
             # Horseshoe opened to below
             # Refpoint in the top center
             shoe_points = [
                 pya.DPoint(a, 0),
                 pya.DPoint(g + w, 0),
@@ -95,15 +95,15 @@
                 pya.DPoint(-a, 0)
             ]
             shoe = pya.DPolygon(shoe_points)
             shoe.size(b)
             shoe.insert_hole(shoe_points[::-1])
 
             # convert to range and recover CPW port
-            shoe_region = pya.Region([shoe.to_itype(self.layout.dbu)])
+            shoe_region = pya.Region(shoe.to_itype(self.layout.dbu))
             shoe_region.round_corners(self.island_r / self.layout.dbu, self.island_r / self.layout.dbu, self.n)
             shoe_region2 = shoe_region - port_region
 
         # move to the north arm of swiss cross
         ground_width = (2 * g - float(self.gap_width[1]) - 2 * b) / 2
         shift_up = float(self.arm_length[cpl_nr]) + (float(self.gap_width[1]) - 2 * aw) / 2 + ground_width + w + b
         transf = pya.DCplxTrans(1, 0, False, pya.DVector(0, shift_up))
```

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/__init__.py` & `kqcircuits-4.7.9/kqcircuits/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/airbridges_sim.py` & `kqcircuits-4.7.9/kqcircuits/simulations/airbridges_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/cross_section_simulation.py` & `kqcircuits-4.7.9/kqcircuits/simulations/cross_section_simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/empty_simulation.py` & `kqcircuits-4.7.9/kqcircuits/simulations/empty_simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/__init__.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/ansys/__init__.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/ansys/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/ansys/ansys_export.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/ansys/ansys_export.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 def export_ansys_json(simulation: Simulation, path: Path, ansys_tool='hfss',
                       frequency_units="GHz", frequency=5, max_delta_s=0.1, percent_error=1, percent_refinement=30,
                       maximum_passes=12, minimum_passes=1, minimum_converged_passes=1,
                       sweep_enabled=True, sweep_start=0, sweep_end=10, sweep_count=101, sweep_type='interpolating',
                       max_delta_f=0.1, n_modes=2, mesh_size=None, substrate_loss_tangent=0,
                       dielectric_surfaces=None, simulation_flags=None, ansys_project_template=None,
-                      integrate_energies=False):
+                      integrate_energies=False, hfss_capacitance_export=False):
     r"""
     Export Ansys simulation into json and gds files.
 
     Arguments:
         simulation: The simulation to be exported.
         path: Location where to write json and gds files.
         ansys_tool: Determines whether to use HFSS ('hfss') or Q3D Extractor ('q3d').
@@ -93,14 +93,15 @@
                     'tan_delta_surf': 0.001,
                     'th': 2e-9,
                     'eps_r': 10
                 },
         simulation_flags: Optional export processing, given as list of strings
         ansys_project_template: path to the simulation template
         integrate_energies: Calculate energy integrals over each layer and save them into a file
+        hfss_capacitance_export: If True, the capacitance matrices are exported from HFSS simulations
 
     Returns:
          Path to exported json file.
     """
     if simulation is None or not isinstance(simulation, Simulation):
         raise ValueError("Cannot export without simulation")
     if simulation_flags is None:
@@ -127,15 +128,16 @@
             'max_delta_f': max_delta_f,
             'n_modes': n_modes,
         },
         'mesh_size': {} if mesh_size is None else mesh_size,
         'substrate_loss_tangent': substrate_loss_tangent,
         'dielectric_surfaces': dielectric_surfaces,
         'simulation_flags': simulation_flags,
-        'integrate_energies': integrate_energies
+        'integrate_energies': integrate_energies,
+        'hfss_capacitance_export': hfss_capacitance_export
     }
 
     if ansys_project_template is not None:
         json_data['ansys_project_template'] = ansys_project_template
 
     # write .json file
     json_filename = str(path.joinpath(simulation.name + '.json'))
@@ -230,15 +232,16 @@
                  frequency_units="GHz", frequency=5, max_delta_s=0.1, percent_error=1, percent_refinement=30,
                  maximum_passes=12, minimum_passes=1, minimum_converged_passes=1,
                  sweep_enabled=True, sweep_start=0, sweep_end=10, sweep_count=101, sweep_type='interpolating',
                  max_delta_f=0.1, n_modes=2, mesh_size=None, substrate_loss_tangent=0,
                  dielectric_surfaces=None, exit_after_run=False,
                  import_script='import_and_simulate.py', post_process_script='export_batch_results.py',
                  intermediate_processing_command=None, use_rel_path=True, simulation_flags=None,
-                 ansys_project_template=None, integrate_energies=False, skip_errors=False):
+                 ansys_project_template=None, integrate_energies=False, hfss_capacitance_export=False,
+                 skip_errors=False):
     r"""
     Export Ansys simulations by writing necessary scripts and json, gds, and bat files.
 
     Arguments:
         simulations: List of simulations to be exported.
         path: Location where to write export files.
         ansys_tool: Determines whether to use HFSS ('hfss'), Q3D Extractor ('q3d') or HFSS eigenmode ('eigenmode').
@@ -290,14 +293,15 @@
 
                 python scripts/script.py json_filename.json
 
         use_rel_path: Determines if to use relative paths.
         simulation_flags: Optional export processing, given as list of strings. See Simulation Export in docs.
         ansys_project_template: path to the simulation template
         integrate_energies: Calculate energy integrals over each layer and save them into a file
+        hfss_capacitance_export: If True, the capacitance matrices are exported from HFSS simulations
         skip_errors: Skip simulations that cause errors. Default is False.
 
             .. warning::
 
                **Use this carefully**, some of your simulations might not make sense physically and
                you might end up wasting time on bad simulations.
 
@@ -319,15 +323,16 @@
                                             sweep_end=sweep_end, sweep_count=sweep_count, sweep_type=sweep_type,
                                             max_delta_f=max_delta_f, n_modes=n_modes,
                                             mesh_size=mesh_size,
                                             substrate_loss_tangent=substrate_loss_tangent,
                                             dielectric_surfaces=dielectric_surfaces,
                                             simulation_flags=simulation_flags,
                                             ansys_project_template=ansys_project_template,
-                                            integrate_energies=integrate_energies))
+                                            integrate_energies=integrate_energies,
+                                            hfss_capacitance_export=hfss_capacitance_export))
         except (IndexError, ValueError, Exception) as e:  # pylint: disable=broad-except
             if skip_errors:
                 logging.warning(
                     f'Simulation {simulation.name} skipped due to {e.args}. '\
                     'Some of your other simulations might not make sense geometrically. '\
                     'Disable `skip_errors` to see the full traceback.'
                 )
```

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/elmer/__init__.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/elmer/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/export_and_run.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/export_and_run.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/export_singularity.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/export_singularity.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/remote_export_and_run.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/remote_export_and_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,23 +265,26 @@
     return (allowed_simulations, simdir, tmpdir)
 
 
 def remote_export_and_run(ssh_login: str,
                           kqc_remote_tmp_path: str=None,
                           detach_simulation :bool=False,
                           poll_interval: int=None,
+                          export_path_basename: str=None,
                           args=None):
     """
     Exports locally and runs KQC simulations on a remote host. Froced to use no GUI (--quiet, -q option)
 
     Args:
         ssh_login              (str): ssh login info "user@hostname"
         kqc_remote_tmp_path    (str): tmp directory on remote
         detach_simulation     (bool): Detach the remote simulation from terminal, not waiting for it to finish
         poll_interval           (int): Polling interval in seconds when waiting for the remote simulation to finish
+        export_path_basename   (str): Alternative export folder name for the simulation
+                                      If None, the simulation script name will be used
         args                  (list): a list of strings:
                                         - If starts with a letter and ends with ".py"  -> export script
                                         - If starts with "-" or "--"                   -> script option
     """
 
     allowed_simulations, simdir, tmpdir = _allowed_simulations()
 
@@ -302,16 +305,18 @@
                 if arg in allowed_simulations:
                     export_scripts.append(arg_path)
                 else:
                     logging.warning(f"Skipping unkown simulation: {arg}")
             else:
                 logging.warning(f"Skipping unkown argument: {arg}")
 
-
-    export_tmp_paths = [str(Path(tmpdir) / str(script.stem)) for script in export_scripts]
+    if export_path_basename is not None and len(export_scripts) == 1:
+        export_tmp_paths = [str(Path(tmpdir) / str(export_path_basename))]
+    else:
+        export_tmp_paths = [str(Path(tmpdir) / str(script.stem)) for script in export_scripts]
 
     if len(export_scripts) == 0:
         logging.error("No valid simulation script provided in remote_export_and_run")
         sys.exit()
 
     # Export simulation files locally
     for export_path, export_script in zip(export_tmp_paths, export_scripts):
```

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/simulation_export.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/simulation_export.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/sonnet/__init__.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/sonnet/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/sonnet/parser.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/sonnet/parser.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/sonnet/sonnet_export.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/sonnet/sonnet_export.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/sonnet/template.son` & `kqcircuits-4.7.9/kqcircuits/simulations/export/sonnet/template.son`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/util.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/util.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/xsection/__init__.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/xsection/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/export/xsection/xsection_export.py` & `kqcircuits-4.7.9/kqcircuits/simulations/export/xsection/xsection_export.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/port.py` & `kqcircuits-4.7.9/kqcircuits/simulations/port.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/simulation.py` & `kqcircuits-4.7.9/kqcircuits/simulations/simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/single_element_simulation.py` & `kqcircuits-4.7.9/kqcircuits/simulations/single_element_simulation.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/single_xmons_full_chip_sim.py` & `kqcircuits-4.7.9/kqcircuits/simulations/single_xmons_full_chip_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/waveguides_sim.py` & `kqcircuits-4.7.9/kqcircuits/simulations/waveguides_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py` & `kqcircuits-4.7.9/kqcircuits/simulations/xmons_direct_coupling_full_chip_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/simulations/xmons_direct_coupling_sim.py` & `kqcircuits-4.7.9/kqcircuits/simulations/xmons_direct_coupling_sim.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/__init__.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/airbridge_dc.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/airbridge_dc.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/cross_test.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/cross_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/junction_test_pads/__init__.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/junction_test_pads/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/junction_test_pads/junction_test_pads.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/junction_test_pads/junction_test_pads_simple.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/stripes_test.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/stripes_test.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/stripes_test_increasing_width.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/stripes_test_increasing_width.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/test_structure.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/test_structure.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/test_structures/tsv_test_pattern.py` & `kqcircuits-4.7.9/kqcircuits/test_structures/tsv_test_pattern.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/__init__.py` & `kqcircuits-4.7.9/kqcircuits/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/area.py` & `kqcircuits-4.7.9/kqcircuits/util/area.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/count_instances.py` & `kqcircuits-4.7.9/kqcircuits/util/count_instances.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/coupler_lib.py` & `kqcircuits-4.7.9/kqcircuits/util/coupler_lib.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/deep_delete.py` & `kqcircuits-4.7.9/kqcircuits/util/deep_delete.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/dependencies.py` & `kqcircuits-4.7.9/kqcircuits/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/edit_node_plugin.py` & `kqcircuits-4.7.9/kqcircuits/util/edit_node_plugin.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/export_helper.py` & `kqcircuits-4.7.9/kqcircuits/util/export_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/geometry_helper.py` & `kqcircuits-4.7.9/kqcircuits/util/geometry_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/geometry_json_encoder.py` & `kqcircuits-4.7.9/kqcircuits/util/geometry_json_encoder.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/groundgrid.py` & `kqcircuits-4.7.9/kqcircuits/util/groundgrid.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/gui_helper.py` & `kqcircuits-4.7.9/kqcircuits/util/gui_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/import_helper.py` & `kqcircuits-4.7.9/kqcircuits/util/import_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/label.py` & `kqcircuits-4.7.9/kqcircuits/util/label.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/layout_to_code.py` & `kqcircuits-4.7.9/kqcircuits/util/layout_to_code.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/library_helper.py` & `kqcircuits-4.7.9/kqcircuits/util/library_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/log_router.py` & `kqcircuits-4.7.9/kqcircuits/util/log_router.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/merge.py` & `kqcircuits-4.7.9/kqcircuits/util/merge.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/netlist_extraction.py` & `kqcircuits-4.7.9/kqcircuits/util/netlist_extraction.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/netlist_graph.py` & `kqcircuits-4.7.9/kqcircuits/util/netlist_graph.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/parameter_helper.py` & `kqcircuits-4.7.9/kqcircuits/util/parameter_helper.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/parameters.py` & `kqcircuits-4.7.9/kqcircuits/util/parameters.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/plugin_startup.py` & `kqcircuits-4.7.9/kqcircuits/util/plugin_startup.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/refpoints.py` & `kqcircuits-4.7.9/kqcircuits/util/refpoints.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/replace_squids.py` & `kqcircuits-4.7.9/kqcircuits/util/replace_squids.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits/util/symmetric_polygons.py` & `kqcircuits-4.7.9/kqcircuits/util/symmetric_polygons.py`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/kqcircuits.egg-info/PKG-INFO` & `kqcircuits-4.7.9/kqcircuits.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kqcircuits
-Version: 4.7.7
+Version: 4.7.9
 Summary: KQCircuits is a KLayout/Python-based superconducting quantum circuit library developed by IQM.
 Home-page: https://iqm-finland.github.io/KQCircuits/
 Author: IQM Finland Oy
 Author-email: kqcircuits@meetiqm.com
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
 Requires-Dist: klayout>=0.28
```

### Comparing `kqcircuits-4.7.7/kqcircuits.egg-info/SOURCES.txt` & `kqcircuits-4.7.9/kqcircuits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kqcircuits-4.7.7/setup.py` & `kqcircuits-4.7.9/setup.py`

 * *Files identical despite different names*

