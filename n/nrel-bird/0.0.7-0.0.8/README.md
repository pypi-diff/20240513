# Comparing `tmp/nrel_bird-0.0.7.tar.gz` & `tmp/nrel_bird-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrel_bird-0.0.7.tar", last modified: Mon May  6 16:17:08 2024, max compression
+gzip compressed data, was "nrel_bird-0.0.8.tar", last modified: Mon May 13 20:17:43 2024, max compression
```

## Comparing `nrel_bird-0.0.7.tar` & `nrel_bird-0.0.8.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.646859 nrel_bird-0.0.7/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1523 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/LICENSE
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12900 2024-05-06 16:17:08.646532 nrel_bird-0.0.7/PKG-INFO
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12061 2024-05-06 16:15:02.000000 nrel_bird-0.0.7/README.md
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.627315 nrel_bird-0.0.7/bird/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      923 2024-05-06 16:11:12.000000 nrel_bird-0.0.7/bird/__init__.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.628764 nrel_bird-0.0.7/bird/meshing/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12016 2024-05-06 14:57:17.000000 nrel_bird-0.0.7/bird/meshing/_mesh_tools.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4295 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/_stir_tank_reactor.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    17267 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.624994 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.629506 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1308 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      835 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn/input.yaml
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1144 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.629904 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      803 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      550 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.630254 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1164 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      829 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.630598 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1215 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1669 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.630942 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle_projected/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1043 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle_projected/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      834 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle_projected/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.631440 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1216 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.631773 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1044 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      840 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.632279 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1125 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1163 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.632642 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1217 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.632996 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2769 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3943 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.633339 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2815 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3943 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.633696 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2524 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3797 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.634031 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1690 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.634361 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1969 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2572 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.634969 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2247 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3176 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.635376 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2247 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3176 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.635782 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2524 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3797 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.636198 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2273 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1938 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.636616 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1288 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.637041 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1289 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.637525 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1249 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.637957 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1249 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.638360 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1722 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.638789 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1722 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.639162 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1287 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.639570 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1287 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/topology.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     7158 2024-05-06 16:11:12.000000 nrel_bird-0.0.7/bird/meshing/block_rect_mesh.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.625291 nrel_bird-0.0.7/bird/meshing/block_rect_mesh_templates/
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.639782 nrel_bird-0.0.7/bird/meshing/block_rect_mesh_templates/loopReactor/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      535 2024-05-06 16:11:12.000000 nrel_bird-0.0.7/bird/meshing/block_rect_mesh_templates/loopReactor/input.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.640003 nrel_bird-0.0.7/bird/meshing/block_rect_mesh_templates/sub_blocks/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      541 2024-05-06 16:11:12.000000 nrel_bird-0.0.7/bird/meshing/block_rect_mesh_templates/sub_blocks/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    26151 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/stir_tank_mesh.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.625473 nrel_bird-0.0.7/bird/meshing/stir_tank_mesh_templates/
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.640218 nrel_bird-0.0.7/bird/meshing/stir_tank_mesh_templates/base_tank/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      824 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4337 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/meshing/stl_mesh_tools.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.640811 nrel_bird-0.0.7/bird/postProcess/
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.641185 nrel_bird-0.0.7/bird/postProcess/computeQoI/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6108 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/postProcess/computeQoI/compute_QOI.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4573 2024-05-03 20:29:34.000000 nrel_bird-0.0.7/bird/postProcess/conditional_mean.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.642112 nrel_bird-0.0.7/bird/postProcess/data_early/
--rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    13092 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/postProcess/data_early/150rpm_1e8.csv
--rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    16781 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/postProcess/data_early/150rpm_5e7.csv
--rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    48787 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/postProcess/data_early/240rpm_1e8.csv
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     9024 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/postProcess/early_pred.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.625962 nrel_bird-0.0.7/bird/preprocess/
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.642761 nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6539 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/main.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6003 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/main_rep.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.643148 nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/util/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1803 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/util/argument_inhomo.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3839 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/util/fromMomtoPdf.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       72 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/requirements.txt
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.644771 nrel_bird-0.0.7/bird/utilities/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     7182 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/utilities/bubble_col_util.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      976 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/utilities/folderManagement.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1894 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/utilities/label_plot.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1194 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/utilities/mathtools.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4751 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/utilities/ofio.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1430 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/bird/utilities/stl_plotting.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       56 2024-05-06 16:15:38.000000 nrel_bird-0.0.7/bird/version.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:17:08.646174 nrel_bird-0.0.7/nrel_bird.egg-info/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12900 2024-05-06 16:17:08.000000 nrel_bird-0.0.7/nrel_bird.egg-info/PKG-INFO
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4887 2024-05-06 16:17:08.000000 nrel_bird-0.0.7/nrel_bird.egg-info/SOURCES.txt
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        1 2024-05-06 16:17:08.000000 nrel_bird-0.0.7/nrel_bird.egg-info/dependency_links.txt
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       72 2024-05-06 16:17:08.000000 nrel_bird-0.0.7/nrel_bird.egg-info/requires.txt
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        5 2024-05-06 16:17:08.000000 nrel_bird-0.0.7/nrel_bird.egg-info/top_level.txt
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       38 2024-05-06 16:17:08.646913 nrel_bird-0.0.7/setup.cfg
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1446 2024-05-03 20:29:35.000000 nrel_bird-0.0.7/setup.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.098424 nrel_bird-0.0.8/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1523 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/LICENSE
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12900 2024-05-13 20:17:43.097985 nrel_bird-0.0.8/PKG-INFO
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12061 2024-05-13 20:17:02.000000 nrel_bird-0.0.8/README.md
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.066652 nrel_bird-0.0.8/bird/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      923 2024-05-13 20:17:02.000000 nrel_bird-0.0.8/bird/__init__.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.068499 nrel_bird-0.0.8/bird/meshing/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12016 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/_mesh_tools.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4295 2024-05-13 20:17:02.000000 nrel_bird-0.0.8/bird/meshing/_stir_tank_reactor.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    17267 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.063771 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.069213 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1308 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      835 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn/input.yaml
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1144 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.069761 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      803 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      550 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.070299 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1164 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      829 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.070882 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1215 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1669 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.073224 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle_projected/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1043 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle_projected/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      834 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle_projected/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.074044 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1216 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.074566 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1044 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      840 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.075050 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1125 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1163 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.075609 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1217 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.076186 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2769 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3943 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.076668 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2815 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3943 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.077412 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2524 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3797 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.077904 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1690 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.078435 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1969 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2572 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.079031 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2247 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3176 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.079545 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2247 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3176 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.080038 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2524 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3797 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.080591 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2273 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1938 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.081211 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1288 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.081771 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1289 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.082598 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1249 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.083043 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1249 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.083742 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1722 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.084285 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1722 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.084826 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1287 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.085288 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1287 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/topology.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     7158 2024-05-13 20:17:02.000000 nrel_bird-0.0.8/bird/meshing/block_rect_mesh.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.064098 nrel_bird-0.0.8/bird/meshing/block_rect_mesh_templates/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.085516 nrel_bird-0.0.8/bird/meshing/block_rect_mesh_templates/loopReactor/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      535 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_rect_mesh_templates/loopReactor/input.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.085770 nrel_bird-0.0.8/bird/meshing/block_rect_mesh_templates/sub_blocks/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      541 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/block_rect_mesh_templates/sub_blocks/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    26151 2024-05-13 20:17:02.000000 nrel_bird-0.0.8/bird/meshing/stir_tank_mesh.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.064298 nrel_bird-0.0.8/bird/meshing/stir_tank_mesh_templates/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.086039 nrel_bird-0.0.8/bird/meshing/stir_tank_mesh_templates/base_tank/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      824 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4337 2024-05-13 20:17:02.000000 nrel_bird-0.0.8/bird/meshing/stl_mesh_tools.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.086467 nrel_bird-0.0.8/bird/postProcess/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.086815 nrel_bird-0.0.8/bird/postProcess/computeQoI/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6108 2024-05-07 21:40:42.000000 nrel_bird-0.0.8/bird/postProcess/computeQoI/compute_QOI.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4573 2024-05-13 20:17:02.000000 nrel_bird-0.0.8/bird/postProcess/conditional_mean.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.088229 nrel_bird-0.0.8/bird/postProcess/data_early/
+-rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    13092 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/postProcess/data_early/150rpm_1e8.csv
+-rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    16781 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/postProcess/data_early/150rpm_5e7.csv
+-rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    48787 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/postProcess/data_early/240rpm_1e8.csv
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     9024 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/postProcess/early_pred.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.064794 nrel_bird-0.0.8/bird/preProcess/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.090850 nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6539 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/main.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6003 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/main_rep.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.091880 nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/util/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1803 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/util/argument_inhomo.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3839 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/util/fromMomtoPdf.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       72 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/requirements.txt
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.093581 nrel_bird-0.0.8/bird/utilities/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     7182 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/utilities/bubble_col_util.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      976 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/utilities/folderManagement.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1894 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/utilities/label_plot.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1194 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/utilities/mathtools.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4751 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/utilities/ofio.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1430 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/bird/utilities/stl_plotting.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       56 2024-05-13 20:17:14.000000 nrel_bird-0.0.8/bird/version.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-13 20:17:43.095528 nrel_bird-0.0.8/nrel_bird.egg-info/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12900 2024-05-13 20:17:43.000000 nrel_bird-0.0.8/nrel_bird.egg-info/PKG-INFO
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     5080 2024-05-13 20:17:43.000000 nrel_bird-0.0.8/nrel_bird.egg-info/SOURCES.txt
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        1 2024-05-13 20:17:43.000000 nrel_bird-0.0.8/nrel_bird.egg-info/dependency_links.txt
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       72 2024-05-13 20:17:43.000000 nrel_bird-0.0.8/nrel_bird.egg-info/requires.txt
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        5 2024-05-13 20:17:43.000000 nrel_bird-0.0.8/nrel_bird.egg-info/top_level.txt
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       38 2024-05-13 20:17:43.098492 nrel_bird-0.0.8/setup.cfg
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1446 2024-05-07 21:40:43.000000 nrel_bird-0.0.8/setup.py
```

### Comparing `nrel_bird-0.0.7/LICENSE` & `nrel_bird-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/PKG-INFO` & `nrel_bird-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrel-bird
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bio Reactor Design (BiRD): a toolbox to simulate and analyze different designs of bioreactors in OpenFOAM
 Home-page: https://github.com/NREL/BioReactorDesign
 Author: Malik Hassanaly
 License: BSD 3-Clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -239,24 +239,24 @@
 blockMesh
 cd $root
 ```
 
 Will generate this
 
 <p float="left">
-  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/assets/loop_react.png" width="250"/>
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/assets/loop_react.png" width="400"/>
 </p>
 
 
 #### How to change the block rectangular geometry
 
 The geometry of the block cylindrical mesh is defined within a 3D domain (X,Y,Z). The blocks that represent the fluid domain are a subset of a block rectangular background domain. The fluid blocks are defined using the geometry corners. For the mesh shown above, the geometry corners are the red blocks shown below 
 
 <p float="left">
-  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/bird/meshing/block_rect_mesh_templates/loopReactor/loop_schematic.png" width="250"/>
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/bird/meshing/block_rect_mesh_templates/loopReactor/loop_schematic.png" width="700"/>
 </p>
  
 The corners are defined in the `input.json`
 ```
 "Geometry": {
         "Fluids": [
                 [ [0,0,0], [9,0,0], [9,0,4], [0,0,4] ],
```

### Comparing `nrel_bird-0.0.7/README.md` & `nrel_bird-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -214,24 +214,24 @@
 blockMesh
 cd $root
 ```
 
 Will generate this
 
 <p float="left">
-  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/assets/loop_react.png" width="250"/>
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/assets/loop_react.png" width="400"/>
 </p>
 
 
 #### How to change the block rectangular geometry
 
 The geometry of the block cylindrical mesh is defined within a 3D domain (X,Y,Z). The blocks that represent the fluid domain are a subset of a block rectangular background domain. The fluid blocks are defined using the geometry corners. For the mesh shown above, the geometry corners are the red blocks shown below 
 
 <p float="left">
-  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/bird/meshing/block_rect_mesh_templates/loopReactor/loop_schematic.png" width="250"/>
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/bird/meshing/block_rect_mesh_templates/loopReactor/loop_schematic.png" width="700"/>
 </p>
  
 The corners are defined in the `input.json`
 ```
 "Geometry": {
         "Fluids": [
                 [ [0,0,0], [9,0,0], [9,0,4], [0,0,4] ],
```

### Comparing `nrel_bird-0.0.7/bird/__init__.py` & `nrel_bird-0.0.8/bird/__init__.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/_mesh_tools.py` & `nrel_bird-0.0.8/bird/meshing/_mesh_tools.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/_stir_tank_reactor.py` & `nrel_bird-0.0.8/bird/meshing/_stir_tank_reactor.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh.py` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn/input.yaml` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn/input.yaml`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle_projected/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle_projected/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/circle_projected/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/circle_projected/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/input.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/topology.json` & `nrel_bird-0.0.8/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/topology.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_rect_mesh.py` & `nrel_bird-0.0.8/bird/meshing/block_rect_mesh.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_rect_mesh_templates/loopReactor/input.json` & `nrel_bird-0.0.8/bird/meshing/block_rect_mesh_templates/loopReactor/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/block_rect_mesh_templates/sub_blocks/input.json` & `nrel_bird-0.0.8/bird/meshing/block_rect_mesh_templates/sub_blocks/input.json`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/stir_tank_mesh.py` & `nrel_bird-0.0.8/bird/meshing/stir_tank_mesh.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml` & `nrel_bird-0.0.8/bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/meshing/stl_mesh_tools.py` & `nrel_bird-0.0.8/bird/meshing/stl_mesh_tools.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/postProcess/computeQoI/compute_QOI.py` & `nrel_bird-0.0.8/bird/postProcess/computeQoI/compute_QOI.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/postProcess/conditional_mean.py` & `nrel_bird-0.0.8/bird/postProcess/conditional_mean.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/postProcess/data_early/150rpm_1e8.csv` & `nrel_bird-0.0.8/bird/postProcess/data_early/150rpm_1e8.csv`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/postProcess/data_early/150rpm_5e7.csv` & `nrel_bird-0.0.8/bird/postProcess/data_early/150rpm_5e7.csv`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/postProcess/data_early/240rpm_1e8.csv` & `nrel_bird-0.0.8/bird/postProcess/data_early/240rpm_1e8.csv`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/postProcess/early_pred.py` & `nrel_bird-0.0.8/bird/postProcess/early_pred.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/main.py` & `nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/main.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/main_rep.py` & `nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/main_rep.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/util/argument_inhomo.py` & `nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/util/argument_inhomo.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/preprocess/inhomogeneousBC/util/fromMomtoPdf.py` & `nrel_bird-0.0.8/bird/preProcess/inhomogeneousBC/util/fromMomtoPdf.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/utilities/bubble_col_util.py` & `nrel_bird-0.0.8/bird/utilities/bubble_col_util.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/utilities/folderManagement.py` & `nrel_bird-0.0.8/bird/utilities/folderManagement.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/utilities/label_plot.py` & `nrel_bird-0.0.8/bird/utilities/label_plot.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/utilities/mathtools.py` & `nrel_bird-0.0.8/bird/utilities/mathtools.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/utilities/ofio.py` & `nrel_bird-0.0.8/bird/utilities/ofio.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/bird/utilities/stl_plotting.py` & `nrel_bird-0.0.8/bird/utilities/stl_plotting.py`

 * *Files identical despite different names*

### Comparing `nrel_bird-0.0.7/nrel_bird.egg-info/PKG-INFO` & `nrel_bird-0.0.8/nrel_bird.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrel-bird
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bio Reactor Design (BiRD): a toolbox to simulate and analyze different designs of bioreactors in OpenFOAM
 Home-page: https://github.com/NREL/BioReactorDesign
 Author: Malik Hassanaly
 License: BSD 3-Clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -239,24 +239,24 @@
 blockMesh
 cd $root
 ```
 
 Will generate this
 
 <p float="left">
-  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/assets/loop_react.png" width="250"/>
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/assets/loop_react.png" width="400"/>
 </p>
 
 
 #### How to change the block rectangular geometry
 
 The geometry of the block cylindrical mesh is defined within a 3D domain (X,Y,Z). The blocks that represent the fluid domain are a subset of a block rectangular background domain. The fluid blocks are defined using the geometry corners. For the mesh shown above, the geometry corners are the red blocks shown below 
 
 <p float="left">
-  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/bird/meshing/block_rect_mesh_templates/loopReactor/loop_schematic.png" width="250"/>
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/bird/meshing/block_rect_mesh_templates/loopReactor/loop_schematic.png" width="700"/>
 </p>
  
 The corners are defined in the `input.json`
 ```
 "Geometry": {
         "Fluids": [
                 [ [0,0,0], [9,0,0], [9,0,4], [0,0,4] ],
```

### Comparing `nrel_bird-0.0.7/nrel_bird.egg-info/SOURCES.txt` & `nrel_bird-0.0.8/nrel_bird.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -68,14 +68,18 @@
 bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml
 bird/postProcess/conditional_mean.py
 bird/postProcess/early_pred.py
 bird/postProcess/computeQoI/compute_QOI.py
 bird/postProcess/data_early/150rpm_1e8.csv
 bird/postProcess/data_early/150rpm_5e7.csv
 bird/postProcess/data_early/240rpm_1e8.csv
+bird/preProcess/inhomogeneousBC/main.py
+bird/preProcess/inhomogeneousBC/main_rep.py
+bird/preProcess/inhomogeneousBC/util/argument_inhomo.py
+bird/preProcess/inhomogeneousBC/util/fromMomtoPdf.py
 bird/preprocess/inhomogeneousBC/main.py
 bird/preprocess/inhomogeneousBC/main_rep.py
 bird/preprocess/inhomogeneousBC/util/argument_inhomo.py
 bird/preprocess/inhomogeneousBC/util/fromMomtoPdf.py
 bird/utilities/bubble_col_util.py
 bird/utilities/folderManagement.py
 bird/utilities/label_plot.py
```

### Comparing `nrel_bird-0.0.7/setup.py` & `nrel_bird-0.0.8/setup.py`

 * *Files identical despite different names*

