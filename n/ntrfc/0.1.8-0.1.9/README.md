# Comparing `tmp/ntrfc-0.1.8.tar.gz` & `tmp/ntrfc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntrfc-0.1.8.tar", last modified: Tue Oct 31 20:18:57 2023, max compression
+gzip compressed data, was "ntrfc-0.1.9.tar", last modified: Sun Mar 17 10:29:35 2024, max compression
```

## Comparing `ntrfc-0.1.8.tar` & `ntrfc-0.1.9.tar`

### file list

```diff
@@ -1,196 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.840433 ntrfc-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-10-12 23:21:30.000000 ntrfc-0.1.8/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3646 2023-10-12 23:21:30.000000 ntrfc-0.1.8/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-10-31 17:50:11.000000 ntrfc-0.1.8/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-10-12 23:21:30.000000 ntrfc-0.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-10-12 23:21:30.000000 ntrfc-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4602 2023-10-31 20:18:57.840433 ntrfc-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2639 2023-10-12 23:21:30.000000 ntrfc-0.1.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.156425 ntrfc-0.1.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.cascade_case.domain.rst
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.cascade_case.rst
--rw-rw-rw-   0 root         (0) root         (0)     1035 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.cascade_case.solution.case_modules.rst
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.cascade_case.solution.rst
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.dictutils.rst
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.filehandling.rst
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.fluid.rst
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.geometry.rst
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.math.rst
--rw-rw-rw-   0 root         (0) root         (0)     1125 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.meshquality.rst
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.rst
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.timeseries.rst
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.turbo.airfoil_generators.rst
--rw-rw-rw-   0 root         (0) root         (0)     1484 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/ntrfc.turbo.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/readme.rst
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-10-12 23:21:30.000000 ntrfc-0.1.8/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.169425 ntrfc-0.1.8/ntrfc/
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.178425 ntrfc-0.1.8/ntrfc/cascade_case/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/cascade_case/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.179425 ntrfc-0.1.8/ntrfc/cascade_case/casemeta/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/cascade_case/casemeta/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/cascade_case/casemeta/casemeta.py
--rw-rw-rw-   0 root         (0) root         (0)     3991 2023-10-27 18:52:17.000000 ntrfc-0.1.8/ntrfc/cascade_case/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     8566 2023-10-31 20:17:48.000000 ntrfc-0.1.8/ntrfc/cascade_case/solution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.209425 ntrfc-0.1.8/ntrfc/cascade_case/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/cascade_case/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3797 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/cascade_case/utils/domain_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/cascade_case/utils/probecontainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/cascade_case/utils/sliceseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.210425 ntrfc-0.1.8/ntrfc/data/
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.227425 ntrfc-0.1.8/ntrfc/data/compressor_cascade/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/compressor_cascade/README.md
--rw-rw-rw-   0 root         (0) root         (0)    43591 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/compressor_cascade/profilepoints.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.247426 ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.335427 ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/boundary/
--rw-rw-rw-   0 root         (0) root         (0)   271732 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/boundary/blade_wall.vtp
--rw-rw-rw-   0 root         (0) root         (0)     9792 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/boundary/inlet.vtp
--rw-rw-rw-   0 root         (0) root         (0)    13301 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/boundary/outlet.vtp
--rw-rw-rw-   0 root         (0) root         (0)  4359505 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/internal.vtu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.050423 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.050423 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.050423 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.379427 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0/
--rw-rw-rw-   0 root         (0) root         (0)    79550 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0/T
--rw-rw-rw-   0 root         (0) root         (0)   235840 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0/U
--rw-rw-rw-   0 root         (0) root         (0)    79550 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0/p
--rw-rw-rw-   0 root         (0) root         (0)    79550 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0/rho
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.442428 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/
--rw-rw-rw-   0 root         (0) root         (0)    68770 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/T
--rw-rw-rw-   0 root         (0) root         (0)   203912 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/U
--rw-rw-rw-   0 root         (0) root         (0)    68770 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/p
--rw-rw-rw-   0 root         (0) root         (0)    68770 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/rho
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.478428 ntrfc-0.1.8/ntrfc/data/t106_cascadecase_how5/
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/t106_cascadecase_how5/Readme.md
--rw-rw-rw-   0 root         (0) root         (0)    11780 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/t106_cascadecase_how5/profilepoints.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.490429 ntrfc-0.1.8/ntrfc/data/turbine_cascade/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/turbine_cascade/README.md
--rw-rw-rw-   0 root         (0) root         (0)     9945 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/data/turbine_cascade/profilepoints.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.502429 ntrfc-0.1.8/ntrfc/filehandling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/filehandling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/filehandling/datafiles.py
--rw-rw-rw-   0 root         (0) root         (0)     3407 2023-10-27 18:52:17.000000 ntrfc-0.1.8/ntrfc/filehandling/mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.518429 ntrfc-0.1.8/ntrfc/fluid/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/fluid/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1863 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/fluid/fluid.py
--rw-rw-rw-   0 root         (0) root         (0)     5774 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/fluid/isentropic.py
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/fluid/turbulence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.528429 ntrfc-0.1.8/ntrfc/geometry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/geometry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6176 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/geometry/alphashape.py
--rw-rw-rw-   0 root         (0) root         (0)     1387 2023-10-27 18:52:17.000000 ntrfc-0.1.8/ntrfc/geometry/line.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/geometry/plane.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/geometry/surface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.586429 ntrfc-0.1.8/ntrfc/gmsh/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/gmsh/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9567 2023-10-27 18:52:17.000000 ntrfc-0.1.8/ntrfc/gmsh/turbo_cascade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.605430 ntrfc-0.1.8/ntrfc/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8837 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/math/methods.py
--rw-rw-rw-   0 root         (0) root         (0)     8026 2023-10-27 18:52:17.000000 ntrfc-0.1.8/ntrfc/math/vectorcalc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.626430 ntrfc-0.1.8/ntrfc/meshquality/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/meshquality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1021 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/meshquality/aspect_ratio.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/meshquality/grid_convergece_index.py
--rw-rw-rw-   0 root         (0) root         (0)     1149 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/meshquality/meshexpansion.py
--rw-rw-rw-   0 root         (0) root         (0)     8206 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/meshquality/nondimensionals.py
--rw-rw-rw-   0 root         (0) root         (0)     1655 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/meshquality/skewness.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/ntrfc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.630430 ntrfc-0.1.8/ntrfc/timeseries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/timeseries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2292 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/timeseries/integral_scales.py
--rw-rw-rw-   0 root         (0) root         (0)    12693 2023-10-27 18:52:17.000000 ntrfc-0.1.8/ntrfc/timeseries/stationarity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.664430 ntrfc-0.1.8/ntrfc/turbo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.687431 ntrfc-0.1.8/ntrfc/turbo/airfoil_generators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/airfoil_generators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9570 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/airfoil_generators/naca_airfoil_creator.py
--rw-rw-rw-   0 root         (0) root         (0)    24178 2023-10-27 18:52:17.000000 ntrfc-0.1.8/ntrfc/turbo/airfoil_generators/parametric_turbine_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/airfoil_generators/parsec_airfoil_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/bladeloading.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/cascade_geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     5679 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/domaingen_cascade.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/integrals.py
--rw-rw-rw-   0 root         (0) root         (0)     8876 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/pointcloud_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-10-12 23:21:30.000000 ntrfc-0.1.8/ntrfc/turbo/probegeneration.py
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-10-27 18:52:17.000000 ntrfc-0.1.8/ntrfc/turbo/profile_tele_extraction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.173425 ntrfc-0.1.8/ntrfc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4602 2023-10-31 20:18:56.000000 ntrfc-0.1.8/ntrfc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5273 2023-10-31 20:18:57.000000 ntrfc-0.1.8/ntrfc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-31 20:18:56.000000 ntrfc-0.1.8/ntrfc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-10-31 20:18:56.000000 ntrfc-0.1.8/ntrfc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-31 20:18:56.000000 ntrfc-0.1.8/ntrfc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      240 2023-10-31 20:18:56.000000 ntrfc-0.1.8/ntrfc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-10-31 20:18:56.000000 ntrfc-0.1.8/ntrfc.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-10-31 20:18:57.841432 ntrfc-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-10-31 17:50:11.000000 ntrfc-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.705431 ntrfc-0.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.706431 ntrfc-0.1.8/tests/cascadecase/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/cascadecase/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.707431 ntrfc-0.1.8/tests/cascadecase/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/cascadecase/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/cascadecase/domain/test_ntrfc_domaingen_cascade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.712431 ntrfc-0.1.8/tests/cascadecase/solution/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/cascadecase/solution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/cascadecase/solution/test_probecontainer.py
--rw-rw-rw-   0 root         (0) root         (0)     3872 2023-10-31 17:50:11.000000 ntrfc-0.1.8/tests/cascadecase/solution/test_solution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.721431 ntrfc-0.1.8/tests/filehandling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/filehandling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/filehandling/test_ntrfc_datafiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/filehandling/test_ntrfc_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.736431 ntrfc-0.1.8/tests/fluid/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/fluid/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2188 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/fluid/test_ntrfc_fluid.py
--rw-rw-rw-   0 root         (0) root         (0)     2174 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/fluid/test_ntrfc_isentropic.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/fluid/test_ntrfc_turbulence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.740431 ntrfc-0.1.8/tests/geometry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/geometry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-10-27 18:52:17.000000 ntrfc-0.1.8/tests/geometry/test_ntrfc_alphashape.py
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-10-27 18:52:17.000000 ntrfc-0.1.8/tests/geometry/test_ntrfc_geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2023-10-27 18:52:17.000000 ntrfc-0.1.8/tests/geometry/test_ntrfc_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1383 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/geometry/test_ntrfc_plane.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/geometry/test_ntrfc_surface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.741431 ntrfc-0.1.8/tests/gmsh/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/gmsh/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-10-27 18:52:17.000000 ntrfc-0.1.8/tests/gmsh/test_meshing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.763432 ntrfc-0.1.8/tests/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8342 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/math/test_ntrfc_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     3807 2023-10-27 18:52:17.000000 ntrfc-0.1.8/tests/math/test_ntrfc_vectorcalc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.791432 ntrfc-0.1.8/tests/meshquality/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/meshquality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/meshquality/test_ntrfc_aspect_ratio.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/meshquality/test_ntrfc_grid_convergence_index.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/meshquality/test_ntrfc_meshexpansion.py
--rw-rw-rw-   0 root         (0) root         (0)    13631 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/meshquality/test_ntrfc_nondimensionals.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/meshquality/test_ntrfc_skewness.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/test_ntrfc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.803432 ntrfc-0.1.8/tests/timeseries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/timeseries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/timeseries/test_ntrfc_integral_scales.py
--rw-rw-rw-   0 root         (0) root         (0)     9451 2023-10-27 18:52:17.000000 ntrfc-0.1.8/tests/timeseries/test_ntrfc_stationarity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.821432 ntrfc-0.1.8/tests/turbo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-31 20:18:57.838432 ntrfc-0.1.8/tests/turbo/airfoil_generators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/airfoil_generators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/airfoil_generators/test_naca_airfoil_creator.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-10-27 18:52:17.000000 ntrfc-0.1.8/tests/turbo/airfoil_generators/test_parametric_turbine_creator.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/airfoil_generators/test_parsec_airfoil_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/test_ntrfc_bladeloading.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/test_ntrfc_cascade_geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     2161 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/test_ntrfc_domaingen_cascade.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/test_ntrfc_integrals.py
--rw-rw-rw-   0 root         (0) root         (0)     2598 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/test_ntrfc_pointcloud_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2023-10-12 23:21:30.000000 ntrfc-0.1.8/tests/turbo/test_ntrfc_probegeneration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:35.013980 ntrfc-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-03-02 21:25:47.000000 ntrfc-0.1.9/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3646 2024-03-02 21:25:47.000000 ntrfc-0.1.9/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      989 2024-03-17 10:05:57.000000 ntrfc-0.1.9/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-03-02 21:25:47.000000 ntrfc-0.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-03-02 21:25:47.000000 ntrfc-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4807 2024-03-17 10:29:35.013980 ntrfc-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2024-03-02 21:25:47.000000 ntrfc-0.1.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.310971 ntrfc-0.1.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.cascade_case.domain.rst
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.cascade_case.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.cascade_case.solution.case_modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.cascade_case.solution.rst
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.dictutils.rst
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.filehandling.rst
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.fluid.rst
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.geometry.rst
+-rw-rw-rw-   0 root         (0) root         (0)      471 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.math.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1125 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.meshquality.rst
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.timeseries.rst
+-rw-rw-rw-   0 root         (0) root         (0)      740 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.turbo.airfoil_generators.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/ntrfc.turbo.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/readme.rst
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-03-02 21:25:47.000000 ntrfc-0.1.9/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.311971 ntrfc-0.1.9/ntrfc/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.315971 ntrfc-0.1.9/ntrfc/data/
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.316971 ntrfc-0.1.9/ntrfc/data/compressor_cascade/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/compressor_cascade/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    43591 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/compressor_cascade/profilepoints.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.317971 ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.336971 ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/boundary/
+-rw-rw-rw-   0 root         (0) root         (0)   271732 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/boundary/blade_wall.vtp
+-rw-rw-rw-   0 root         (0) root         (0)     9792 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/boundary/inlet.vtp
+-rw-rw-rw-   0 root         (0) root         (0)    13301 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/boundary/outlet.vtp
+-rw-rw-rw-   0 root         (0) root         (0)  4359505 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/internal.vtu
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.224970 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.225970 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.225970 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.339972 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0/
+-rw-rw-rw-   0 root         (0) root         (0)    79550 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0/T
+-rw-rw-rw-   0 root         (0) root         (0)   235840 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0/U
+-rw-rw-rw-   0 root         (0) root         (0)    79550 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0/p
+-rw-rw-rw-   0 root         (0) root         (0)    79550 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0/rho
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.342972 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/
+-rw-rw-rw-   0 root         (0) root         (0)    68770 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/T
+-rw-rw-rw-   0 root         (0) root         (0)   203912 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/U
+-rw-rw-rw-   0 root         (0) root         (0)    68770 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/p
+-rw-rw-rw-   0 root         (0) root         (0)    68770 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/rho
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.343972 ntrfc-0.1.9/ntrfc/data/t106_cascadecase_how5/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/t106_cascadecase_how5/Readme.md
+-rw-rw-rw-   0 root         (0) root         (0)    11780 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/t106_cascadecase_how5/profilepoints.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.344972 ntrfc-0.1.9/ntrfc/data/turbine_cascade/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/turbine_cascade/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9945 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/data/turbine_cascade/profilepoints.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.345972 ntrfc-0.1.9/ntrfc/filehandling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/filehandling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/filehandling/datafiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     3441 2024-03-02 22:47:21.000000 ntrfc-0.1.9/ntrfc/filehandling/mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.347972 ntrfc-0.1.9/ntrfc/fluid/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/fluid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/fluid/fluid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5738 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/fluid/isentropic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/fluid/turbulence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.349972 ntrfc-0.1.9/ntrfc/geometry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/geometry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6176 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/geometry/alphashape.py
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/geometry/line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-03-02 22:13:42.000000 ntrfc-0.1.9/ntrfc/geometry/plane.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/geometry/surface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.351972 ntrfc-0.1.9/ntrfc/math/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/math/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8837 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/math/methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     8164 2024-03-02 22:47:21.000000 ntrfc-0.1.9/ntrfc/math/vectorcalc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.354972 ntrfc-0.1.9/ntrfc/meshquality/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/meshquality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2024-03-02 22:13:42.000000 ntrfc-0.1.9/ntrfc/meshquality/aspect_ratio.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/meshquality/grid_convergece_index.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2024-03-02 22:13:42.000000 ntrfc-0.1.9/ntrfc/meshquality/meshexpansion.py
+-rw-rw-rw-   0 root         (0) root         (0)     8206 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/meshquality/nondimensionals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2024-03-02 22:13:42.000000 ntrfc-0.1.9/ntrfc/meshquality/skewness.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/meshquality/standards.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/ntrfc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.355972 ntrfc-0.1.9/ntrfc/timeseries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/timeseries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2024-03-02 22:13:42.000000 ntrfc-0.1.9/ntrfc/timeseries/integral_scales.py
+-rw-rw-rw-   0 root         (0) root         (0)    12693 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/timeseries/stationarity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.359972 ntrfc-0.1.9/ntrfc/turbo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.361972 ntrfc-0.1.9/ntrfc/turbo/airfoil_generators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/airfoil_generators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9590 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/airfoil_generators/naca_airfoil_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)    24178 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/airfoil_generators/parametric_turbine_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/airfoil_generators/parsec_airfoil_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/bladeloading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.362972 ntrfc-0.1.9/ntrfc/turbo/cascade_case/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.363972 ntrfc-0.1.9/ntrfc/turbo/cascade_case/casemeta/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/casemeta/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/casemeta/casemeta.py
+-rw-rw-rw-   0 root         (0) root         (0)    13310 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     8280 2024-03-15 12:57:05.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/post.py
+-rw-rw-rw-   0 root         (0) root         (0)     3331 2024-03-02 22:13:42.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/solution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.365972 ntrfc-0.1.9/ntrfc/turbo/cascade_case/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6443 2024-03-15 12:57:05.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/utils/domain_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/utils/probecontainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_case/utils/sliceseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/cascade_geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     5275 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/domaingen_cascade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.366972 ntrfc-0.1.9/ntrfc/turbo/gmsh/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/gmsh/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9365 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/gmsh/turbo_cascade.py
+-rw-rw-rw-   0 root         (0) root         (0)    10689 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/gmsh/windtunnel_cascade.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/integrals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/pointcloud_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     4648 2024-03-02 21:25:48.000000 ntrfc-0.1.9/ntrfc/turbo/probegeneration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4448 2024-03-15 12:57:05.000000 ntrfc-0.1.9/ntrfc/turbo/profile_tele_extraction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:35.012981 ntrfc-0.1.9/ntrfc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4807 2024-03-17 10:29:34.000000 ntrfc-0.1.9/ntrfc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5560 2024-03-17 10:29:34.000000 ntrfc-0.1.9/ntrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-17 10:29:34.000000 ntrfc-0.1.9/ntrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2024-03-17 10:29:34.000000 ntrfc-0.1.9/ntrfc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-17 10:29:34.000000 ntrfc-0.1.9/ntrfc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      255 2024-03-17 10:29:34.000000 ntrfc-0.1.9/ntrfc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-03-17 10:29:34.000000 ntrfc-0.1.9/ntrfc.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      422 2024-03-17 10:29:35.015981 ntrfc-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2024-03-17 10:05:57.000000 ntrfc-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.376972 ntrfc-0.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.435973 ntrfc-0.1.9/tests/filehandling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/filehandling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/filehandling/test_ntrfc_datafiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/filehandling/test_ntrfc_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.462973 ntrfc-0.1.9/tests/fluid/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/fluid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2188 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/fluid/test_ntrfc_fluid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2174 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/fluid/test_ntrfc_isentropic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/fluid/test_ntrfc_turbulence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.466973 ntrfc-0.1.9/tests/geometry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/geometry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/geometry/test_ntrfc_alphashape.py
+-rw-rw-rw-   0 root         (0) root         (0)     4160 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/geometry/test_ntrfc_geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/geometry/test_ntrfc_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1383 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/geometry/test_ntrfc_plane.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/geometry/test_ntrfc_surface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.483973 ntrfc-0.1.9/tests/math/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/math/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8342 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/math/test_ntrfc_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     3807 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/math/test_ntrfc_vectorcalc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.791978 ntrfc-0.1.9/tests/meshquality/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/meshquality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/meshquality/test_ntrfc_aspect_ratio.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-03-15 12:57:05.000000 ntrfc-0.1.9/tests/meshquality/test_ntrfc_grid_convergence_index.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/meshquality/test_ntrfc_meshexpansion.py
+-rw-rw-rw-   0 root         (0) root         (0)    13631 2024-03-15 12:57:05.000000 ntrfc-0.1.9/tests/meshquality/test_ntrfc_nondimensionals.py
+-rw-rw-rw-   0 root         (0) root         (0)      659 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/meshquality/test_ntrfc_skewness.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2024-03-15 12:57:05.000000 ntrfc-0.1.9/tests/meshquality/test_ntrfc_standards.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/test_ntrfc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.803978 ntrfc-0.1.9/tests/timeseries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/timeseries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/timeseries/test_ntrfc_integral_scales.py
+-rw-rw-rw-   0 root         (0) root         (0)     9451 2024-03-15 12:57:05.000000 ntrfc-0.1.9/tests/timeseries/test_ntrfc_stationarity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.903979 ntrfc-0.1.9/tests/turbo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.946980 ntrfc-0.1.9/tests/turbo/airfoil_generators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/airfoil_generators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/airfoil_generators/test_naca_airfoil_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/airfoil_generators/test_parametric_turbine_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/airfoil_generators/test_parsec_airfoil_creator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.961980 ntrfc-0.1.9/tests/turbo/cascadecase/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/cascadecase/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.963980 ntrfc-0.1.9/tests/turbo/cascadecase/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/cascadecase/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      754 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/cascadecase/domain/test_ntrfc_domaingen_cascade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:34.985980 ntrfc-0.1.9/tests/turbo/cascadecase/solution/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/cascadecase/solution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/cascadecase/solution/test_probecontainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2024-03-02 22:13:42.000000 ntrfc-0.1.9/tests/turbo/cascadecase/test_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2024-03-02 22:13:42.000000 ntrfc-0.1.9/tests/turbo/cascadecase/test_solution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 10:29:35.006981 ntrfc-0.1.9/tests/turbo/gmsh/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/gmsh/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3609 2024-03-02 22:13:42.000000 ntrfc-0.1.9/tests/turbo/gmsh/test_meshing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/test_ntrfc_bladeloading.py
+-rw-rw-rw-   0 root         (0) root         (0)      809 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/test_ntrfc_cascade_geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2163 2024-03-02 22:13:42.000000 ntrfc-0.1.9/tests/turbo/test_ntrfc_domaingen_cascade.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/test_ntrfc_integrals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1501 2024-03-02 21:25:48.000000 ntrfc-0.1.9/tests/turbo/test_ntrfc_pointcloud_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     2294 2024-03-15 12:57:05.000000 ntrfc-0.1.9/tests/turbo/test_ntrfc_probegeneration.py
```

### Comparing `ntrfc-0.1.8/CONTRIBUTING.rst` & `ntrfc-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/HISTORY.rst` & `ntrfc-0.1.9/HISTORY.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 =======
 History
 =======
+=======
+0.1.9 (2024-03-15)
+------------------
+
+- cascade_case refactoring
+- cleanup
+- le-te-extraction fix
+- cascadebox meshing (gmsh)
 
 0.1.8 (2023-10-31)
 ------------------
 
 - bladeloading fix: reliable variable name usage
```

### Comparing `ntrfc-0.1.8/LICENSE` & `ntrfc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/PKG-INFO` & `ntrfc-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ntrfc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Numerical Test Rig for Cascades. A workflows-library for cfd-analysis of cascade-flows
 Home-page: https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC
 Author: Malte Nyhuis
 Author-email: nyhuis@tfd.uni-hannover.de
 License: MIT license
 Keywords: ntrfc
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: pip>=23
 Requires-Dist: matplotlib==3.7.1
 Requires-Dist: pytest==7.2.2
 Requires-Dist: trame==2.5.2
 Requires-Dist: pyvista[all]==0.42.3
@@ -28,14 +29,15 @@
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: statsmodels>=0.13.5
 Requires-Dist: imageio==2.30.0
 Requires-Dist: scikit-learn
 Requires-Dist: jupyter
 Requires-Dist: sphinx
 Requires-Dist: gmsh==4.11.1
+Requires-Dist: shapely==2.0.1
 
 ============
 NTRfC README
 ============
 
 **Numerical Test Rig for Cascades.**
 
@@ -120,14 +122,22 @@
 - [Cookiecutter](https://github.com/audreyr/cookiecutter)
 - [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
 
 
 =======
 History
 =======
+=======
+0.1.9 (2024-03-15)
+------------------
+
+- cascade_case refactoring
+- cleanup
+- le-te-extraction fix
+- cascadebox meshing (gmsh)
 
 0.1.8 (2023-10-31)
 ------------------
 
 - bladeloading fix: reliable variable name usage
```

### Comparing `ntrfc-0.1.8/README.rst` & `ntrfc-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/Makefile` & `ntrfc-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/conf.py` & `ntrfc-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/installation.rst` & `ntrfc-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/make.bat` & `ntrfc-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.cascade_case.domain.rst` & `ntrfc-0.1.9/docs/ntrfc.cascade_case.domain.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.cascade_case.solution.case_modules.rst` & `ntrfc-0.1.9/docs/ntrfc.cascade_case.solution.case_modules.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.cascade_case.solution.rst` & `ntrfc-0.1.9/docs/ntrfc.cascade_case.solution.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.filehandling.rst` & `ntrfc-0.1.9/docs/ntrfc.filehandling.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.fluid.rst` & `ntrfc-0.1.9/docs/ntrfc.fluid.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.geometry.rst` & `ntrfc-0.1.9/docs/ntrfc.geometry.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.meshquality.rst` & `ntrfc-0.1.9/docs/ntrfc.meshquality.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.timeseries.rst` & `ntrfc-0.1.9/docs/ntrfc.timeseries.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.turbo.airfoil_generators.rst` & `ntrfc-0.1.9/docs/ntrfc.turbo.airfoil_generators.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/docs/ntrfc.turbo.rst` & `ntrfc-0.1.9/docs/ntrfc.turbo.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/cascade_case/utils/probecontainer.py` & `ntrfc-0.1.9/ntrfc/turbo/cascade_case/utils/probecontainer.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/cascade_case/utils/sliceseries.py` & `ntrfc-0.1.9/ntrfc/turbo/cascade_case/utils/sliceseries.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/compressor_cascade/profilepoints.txt` & `ntrfc-0.1.9/ntrfc/data/compressor_cascade/profilepoints.txt`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/boundary/blade_wall.vtp` & `ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/boundary/blade_wall.vtp`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/boundary/inlet.vtp` & `ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/boundary/inlet.vtp`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/boundary/outlet.vtp` & `ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/boundary/outlet.vtp`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_cascade_case/internal.vtu` & `ntrfc-0.1.9/ntrfc/data/openfoam_cascade_case/internal.vtu`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0/T` & `ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0/T`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0/U` & `ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0/U`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0/p` & `ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0/p`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0/rho` & `ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0/rho`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/T` & `ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/T`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/U` & `ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/U`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/p` & `ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/p`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/rho` & `ntrfc-0.1.9/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/rho`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/t106_cascadecase_how5/profilepoints.txt` & `ntrfc-0.1.9/ntrfc/data/t106_cascadecase_how5/profilepoints.txt`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/data/turbine_cascade/profilepoints.txt` & `ntrfc-0.1.9/ntrfc/data/turbine_cascade/profilepoints.txt`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/filehandling/datafiles.py` & `ntrfc-0.1.9/ntrfc/filehandling/datafiles.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/filehandling/mesh.py` & `ntrfc-0.1.9/ntrfc/filehandling/mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,38 +57,41 @@
     mesh = pv.UnstructuredGrid()
     for base in bases:
         ndomains = base.n_blocks
         domainnames = [base.get_block_name(i) for i in range(ndomains)]
         domains = [base[i] for i in domainnames]
         if all(isinstance(grid, pv.UnstructuredGrid) for grid in domains):
             for domain in domains:
-                if type(domain) == pv.UnstructuredGrid:
+                if isinstance(domain, pv.UnstructuredGrid):
                     mesh = mesh.merge(domain)
-                if type(domain) == pv.StructuredGrid:
+                if isinstance(domain, pv.StructuredGrid):
                     mesh = mesh.merge(domain)
         else:
             # not all elements are UnstructuredGrid objects
             for domain in domains:
                 nblocks = domain.n_blocks
                 blocks = [domain[b] for b in range(nblocks)]
                 for block in blocks:
-                    if type(block) == pv.UnstructuredGrid:
+                    if isinstance(block, pv.UnstructuredGrid):
                         mesh = mesh.merge(block)
-                    if type(block) == pv.StructuredGrid:
+                    if isinstance(block, pv.StructuredGrid):
                         mesh = mesh.merge(block)
     return mesh
 
 
 def load_mesh(path_to_mesh):
     """Load a mesh file and return the corresponding mesh object.
 
     Parameters
     ----------
     path_to_mesh : str
-        The file path to the mesh file to be loaded. The file extension should be one of ".vtk", ".vtp", ".vtu", ".vtm", ".cgns", ".msh".
+        The file path to the mesh file to be loaded.
+        The file extension should be one of:
+
+        ".vtk", ".vtp", ".vtu", ".vtm", ".cgns", ".msh".
 
     Returns
     -------
     mesh : pyvista.UnstructuredGrid or pyvista.StructuredGrid
         The mesh object constructed from the input file.
     """
     assert os.path.isfile(path_to_mesh), f"{path_to_mesh} is not a valid file"
```

### Comparing `ntrfc-0.1.8/ntrfc/fluid/fluid.py` & `ntrfc-0.1.9/ntrfc/fluid/fluid.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/fluid/isentropic.py` & `ntrfc-0.1.9/ntrfc/fluid/isentropic.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,20 +27,18 @@
 def temp_is(kappa, ma, Tt):
     # Calculates static temperature in isentropic flow
     # Source: https://www.grc.nasa.gov/www/BGH/isentrop.html
     T = Tt / (1 + ((kappa - 1) / 2.0) * ma ** 2)
     return T
 
 
-def mach_is_x(kappa, p, pt):
+def mach_is_x(kappa, p_blade, p_frestream):
     # Calculates local isentropic Mach number
-    if p > 0 and pt > 0 and pt >= p:
-        y = np.sqrt(2 / (kappa - 1) * ((pt / p) ** ((kappa - 1) / kappa) - 1))
-    else:
-        y = 0.0
+    y = np.sqrt(2 / (kappa - 1) * ((p_frestream / p_blade) ** ((kappa - 1) / kappa) - 1))
+
     return y
 
 
 def isentropic_mach_number(isentropic_pressure, kappa, static_pressure, mach, gas_constant, static_temperature):
     """
     Calculates the isentropic Mach number.
```

### Comparing `ntrfc-0.1.8/ntrfc/fluid/turbulence.py` & `ntrfc-0.1.9/ntrfc/fluid/turbulence.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/geometry/alphashape.py` & `ntrfc-0.1.9/ntrfc/geometry/alphashape.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/geometry/line.py` & `ntrfc-0.1.9/ntrfc/geometry/line.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/geometry/plane.py` & `ntrfc-0.1.9/ntrfc/geometry/plane.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import numpy as np
 from matplotlib import path as mpltPath
 
 from ntrfc.math.vectorcalc import vecAbs, vecProjection
 
 
 def massflow_plane(mesh, rhoname="rho", velocityname="U"):
-    if not "Normals" in mesh.array_names:
-        mesh = mesh.compute_normals()
-    if not "Area" in mesh.array_names:
-        mesh = mesh.compute_cell_sizes()
-    mesh = mesh.point_data_to_cell_data()
-    normals = mesh.cell_normals
+    normals = mesh.compute_normals(point_normals=False, cell_normals=True)["Normals"]
     rhos = mesh[rhoname]
-    areas = mesh["Area"]
+    areas = mesh.compute_cell_sizes()["Area"]
     velocities = mesh[velocityname]
 
     massflow = np.array(
         [vecAbs(vecProjection(velocities[i], normals[i])) for i in range(mesh.number_of_cells)]) ** 2 * rhos * areas
 
     return massflow
 
@@ -27,15 +22,15 @@
     mass_ave = np.sum(mesh[valname] * massflow) / np.sum(massflow)
 
     return mass_ave
 
 
 def areaave_plane(mesh, valname):
     array = mesh[valname]
-    if not "Area" in mesh.array_names:
+    if "Area" not in mesh.array_names:
         mesh = mesh.compute_cell_sizes()
     areas = mesh["Area"]
     area_ave = np.sum((array.T * areas).T) / np.sum(areas)
     return area_ave
 
 
 def inside_poly(polygon, points):
```

### Comparing `ntrfc-0.1.8/ntrfc/geometry/surface.py` & `ntrfc-0.1.9/ntrfc/geometry/surface.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/gmsh/turbo_cascade.py` & `ntrfc-0.1.9/ntrfc/turbo/gmsh/turbo_cascade.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Import modules:
 from dataclasses import dataclass
 
 import gmsh
 import numpy as np
-import pyvista as pv
 
 from ntrfc.geometry.line import lines_from_points
+from ntrfc.turbo.cascade_case.domain import CascadeDomain2D
 
 
 # Initialize gmsh:
 
 
 @dataclass
 class MeshConfig:
@@ -30,49 +30,46 @@
     progression_halfss_te: float = 0.99
     progression_te_halfps: float = 1.1
     progression_halfps_le: float = 0.9
     spansize: float = 0.1
     spanres: int = 5
 
 
-def generate_turbocascade(domain2d,
+def generate_turbocascade(domain2d: CascadeDomain2D,
                           meshconfig: MeshConfig,
-                          filename: str,
-                          verbose=False):
+                          filename: str):
     """
     Generate a mesh for a turbocascade
     :param domain2d: Domain2D object
     :param meshconfig: MeshConfig object
     :param filename: Filename for mesh
     :param verbose: Print gmsh output
     :return:
     """
 
     # Initialize gmsh:
     gmsh.initialize()
     gmsh.model.add("cascade")
     points = {}
     splines = {}
-    lines = {}
     curveloops = {}
-    surfaceloops = {}
     surfaces = {}
 
     # Set meshing options:
-    profilepoints_rolled_le = pv.PolyData(np.roll(domain2d.profilepoints.points, -domain2d.le_index, axis=0))
-    le_index = 0
-    te_index = (domain2d.te_index - domain2d.le_index) % domain2d.profilepoints.number_of_points
+    profilepoints_rolled_le = domain2d.blade.sortedpointsrolled_pv
 
-    domain2d.profilepoints_line = lines_from_points(profilepoints_rolled_le.points).compute_cell_sizes()
+    te_index = domain2d.blade.ite
 
-    lc_blade = np.sum(domain2d.profilepoints_line["Length"]) / meshconfig.bladeres
+    profilepoints_line = lines_from_points(profilepoints_rolled_le.points).compute_cell_sizes()
 
-    sslengths = lines_from_points(domain2d.profilepoints_line.points[:te_index]).compute_cell_sizes()
+    lc_blade = np.sum(profilepoints_line["Length"]) / meshconfig.bladeres
+
+    sslengths = lines_from_points(profilepoints_line.points[:te_index]).compute_cell_sizes()
     sslength = np.sum(sslengths["Length"])
-    pslengths = lines_from_points(domain2d.profilepoints_line.points[te_index:]).compute_cell_sizes()
+    pslengths = lines_from_points(profilepoints_line.points[te_index:]).compute_cell_sizes()
     pslength = np.sum(pslengths["Length"])
 
     ss_half_idx = np.where(np.cumsum(sslengths["Length"]) >= sslength / 2)[0][0]
     ps_half_idx = np.where(np.cumsum(pslengths["Length"]) >= pslength / 2)[0][0] + te_index
 
     # domain2d.profilepoints_spline = lines_from_points(domain2d.profilepoints.points)
     inlet_spline = lines_from_points(domain2d.inlet.points)
@@ -146,61 +143,56 @@
     # Wake Resolution
     w = gmsh.model.mesh.field.add('Cylinder')
     gmsh.model.mesh.field.setNumber(w, "VIn", meshconfig.wake_lc)
     gmsh.model.mesh.field.setNumber(w, "VOut", meshconfig.max_lc)
     gmsh.model.mesh.field.setNumber(w, "Radius", meshconfig.wake_width)
     gmsh.model.mesh.field.setNumber(w, "XAxis", 0.5 * meshconfig.wake_length)
 
-    minx = np.min(domain2d.profilepoints.points[::, 0])
-    maxx = np.max(domain2d.profilepoints.points[::, 0])
-    miny = np.min(domain2d.profilepoints.points[::, 1])
-    maxy = np.max(domain2d.profilepoints.points[::, 1])
+    minx = np.min(profilepoints_rolled_le.points[::, 0])
+    maxx = np.max(profilepoints_rolled_le.points[::, 0])
+    miny = np.min(profilepoints_rolled_le.points[::, 1])
+    # maxy = np.max(profilepoints_rolled_le.points[::, 1])
 
-    wake_angle = np.deg2rad(domain2d.beta_trailing)
+    wake_angle = np.deg2rad(te_index)
     gmsh.model.mesh.field.setNumber(w, "XCenter", minx + (maxx - minx) + 0.5 * meshconfig.wake_length)
     gmsh.model.mesh.field.setNumber(w, "YCenter",
                                     meshconfig.fake_yShiftCylinder + miny - 0.5 * meshconfig.wake_length * np.tan(
                                         wake_angle))
     gmsh.model.mesh.field.setNumber(w, "ZAxis", 0)
     gmsh.model.mesh.field.setNumber(w, "YAxis", -0.5 * meshconfig.wake_length * np.tan(wake_angle))
     gmsh.model.mesh.field.setNumber(w, "XAxis", 0.5 * meshconfig.wake_length)
     gmsh.model.mesh.field.setAsBackgroundMesh(w)
     gmsh.model.occ.synchronize()
     surfaceTags = gmsh.model.getEntities(2)
 
-
     gmsh.option.set_number("Mesh.Algorithm", 6)
     gmsh.option.setNumber("Mesh.ElementOrder", 1)
     # mesh options
     gmsh.option.setNumber("Mesh.RecombineAll", 1)
     gmsh.option.setNumber("Mesh.RecombinationAlgorithm", 1)
     # gmsh.option.setNumber("Mesh.SubdivisionAlgorithm", 2)  # all hexahedra
 
     gmsh.model.mesh.setOrder(1)
     gmsh.model.occ.synchronize()
     gmsh.model.occ.extrude(surfaceTags, dx=0, dy=0, dz=meshconfig.spansize,
-                                     numElements=[meshconfig.spanres],
-                                     recombine=True)
+                           numElements=[meshconfig.spanres],
+                           recombine=True)
     gmsh.model.occ.synchronize()
 
-
-    gmsh.model.addPhysicalGroup(3,[1], name="fluid")
-    gmsh.model.addPhysicalGroup(2,[2], name="inlet")
-    gmsh.model.addPhysicalGroup(2,[4], name="outlet")
-    gmsh.model.addPhysicalGroup(2,[6,7,8,9], name="blade")
-    gmsh.model.addPhysicalGroup(2,[1], name="z_lower")
-    gmsh.model.addPhysicalGroup(2,[10], name="z_upper")
-    gmsh.model.addPhysicalGroup(2,[3], name="y_upper")
-    gmsh.model.addPhysicalGroup(2,[5], name="y_lower")
+    gmsh.model.addPhysicalGroup(3, [1], name="fluid")
+    gmsh.model.addPhysicalGroup(2, [2], name="inlet")
+    gmsh.model.addPhysicalGroup(2, [4], name="outlet")
+    gmsh.model.addPhysicalGroup(2, [6, 7, 8, 9], name="blade")
+    gmsh.model.addPhysicalGroup(2, [1], name="z_lower")
+    gmsh.model.addPhysicalGroup(2, [10], name="z_upper")
+    gmsh.model.addPhysicalGroup(2, [3], name="y_upper")
+    gmsh.model.addPhysicalGroup(2, [5], name="y_lower")
 
     gmsh.model.occ.synchronize()
 
-
     gmsh.model.mesh.generate(3)
     gmsh.model.occ.synchronize()
 
     gmsh.write(filename)
     gmsh.model.removePhysicalGroups(gmsh.model.occ.getEntities(0))
     gmsh.model.removePhysicalGroups(gmsh.model.occ.getEntities(1))
     gmsh.finalize()
-
-
```

### Comparing `ntrfc-0.1.8/ntrfc/math/methods.py` & `ntrfc-0.1.9/ntrfc/math/methods.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/math/vectorcalc.py` & `ntrfc-0.1.9/ntrfc/math/vectorcalc.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,28 @@
 
 
 def distant_node_index(node, nodes):
     closest_index = distance.cdist([node], nodes).argmax()
     return closest_index
 
 
-def calc_largedistant_idx(x_koords, y_koords):
+def calc_largedistant_idx(x_coords, y_coords):
     """
     tested method to find indices of coordinates of a 2d-pointcloud with the biggest distance
-    :param x_koords: array of xcords
-    :param y_koords: array of ycords
-    :return: index_1,index_2 (int)
+    :param x_coords: array of x coordinates
+    :param y_coords: array of y coordinates
+    :return: index_1, index_2 (int)
     """
-    A = np.dstack((x_koords, y_koords))[0]
-    D = squareform(pdist(A))
-    #    N = np.max(D)
-    I = np.argmax(D)
-    I_row, I_col = np.unravel_index(I, D.shape)
+    coordinates = np.dstack((x_coords, y_coords))[0]
+    distances = squareform(pdist(coordinates))
+    max_distance_index = np.argmax(distances)
+    max_distance_index_row, max_distance_index_col = np.unravel_index(max_distance_index, distances.shape)
 
-    index_1 = I_row
-    index_2 = I_col
+    index_1 = max_distance_index_row
+    index_2 = max_distance_index_col
 
     return index_1, index_2
 
 
 def symToMatrix(symTensor):
     """
     tested translates symmetric tensor notation to complete matrix
```

### Comparing `ntrfc-0.1.8/ntrfc/meshquality/aspect_ratio.py` & `ntrfc-0.1.9/ntrfc/meshquality/aspect_ratio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,43 @@
+import warnings
+
 import numpy as np
 import pyvista as pv
 import vtk
 
+from ntrfc.meshquality.standards import classify_mesh_quality
+
 
 def compute_cell_aspect_ratios(grid: pv.UnstructuredGrid) -> np.ndarray:
     """Compute the aspect ratio of each cell in an unstructured grid.
 
     The aspect ratio of a cell is defined as the ratio of the longest edge length
     to the shortest edge length of the cell.
 
     Parameters:
         grid (pv.UnstructuredGrid): The unstructured grid.
 
     Returns:
         np.ndarray: An array of aspect ratios, one for each cell in the grid.
     """
+    qualityname = "AspectRatio"
+
     cellids = range(0, grid.number_of_cells)
     # Compute the edge lengths for each cell
     aspect_ratios = []
     vtk.vtkLogger.SetStderrVerbosity(vtk.vtkLogger.VERBOSITY_OFF)
     for cellid in cellids:
         # Get the indices of the points that make up the cell
         cell = grid.extract_cells(cellid)
 
         edges = cell.extract_all_edges().compute_cell_sizes(length=True, area=False, volume=False)
 
         aspect_ratios.append(max(edges["Length"]) / min(edges["Length"]))
 
-    return np.array(aspect_ratios)
+    aspect_ratios = np.array(aspect_ratios)
+
+    meshok = classify_mesh_quality(qualityname, aspect_ratios)
+
+    if not meshok:
+        warnings.warn(f"Mesh quality ({qualityname}) is bad, consider refining the mesh.")
+
+    return aspect_ratios
```

### Comparing `ntrfc-0.1.8/ntrfc/meshquality/grid_convergece_index.py` & `ntrfc-0.1.9/ntrfc/meshquality/grid_convergece_index.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/meshquality/meshexpansion.py` & `ntrfc-0.1.9/ntrfc/meshquality/meshexpansion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+import warnings
+
 import numpy as np
 import pyvista as pv
 
+from ntrfc.meshquality.standards import classify_mesh_quality
+
 
 def compute_expansion_factors(grid: pv.UnstructuredGrid) -> np.ndarray:
+    qualityname = "MeshExpansion"
+
     # Compute cell volumes
     cell_volumes = grid.compute_cell_sizes()["Volume"]
 
     # Number of cells in the grid
     n_cells = grid.n_cells
 
     # Initialize array to store expansion factors
@@ -19,14 +25,21 @@
 
         # Find the volume of the largest neighboring cell
         max_neighbor_volume = max([cell_volumes[j] for j in neighbor_indices])
 
         # Compute expansion factor for the current cell
         expansion_factors[i] = max_neighbor_volume / cell_volumes[i]
 
+    expansion_factors = np.array(expansion_factors)
+
+    meshok = classify_mesh_quality(qualityname, expansion_factors)
+
+    if not meshok:
+        warnings.warn(f"Mesh quality ({qualityname}) is bad, consider refining the mesh.")
+
     return expansion_factors
 
 
 def get_neighbor_cell_ids(grid, cell_idx):
     """Helper to get neighbor cell IDs."""
     cell = grid.GetCell(cell_idx)
     pids = pv.vtk_id_list_to_array(cell.GetPointIds())
```

### Comparing `ntrfc-0.1.8/ntrfc/meshquality/nondimensionals.py` & `ntrfc-0.1.9/ntrfc/meshquality/nondimensionals.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/meshquality/skewness.py` & `ntrfc-0.1.9/ntrfc/meshquality/skewness.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+import warnings
+
 import numpy as np
 
+from ntrfc.meshquality.standards import classify_mesh_quality
+
 
 def compute_cell_skewness(grid):
     """
     Compute the skewness of each cell in an unstructured grid.
 
     Parameters
     ----------
@@ -11,21 +15,27 @@
         The input unstructured grid.
 
     Returns
     -------
     skewness : list
         A list of the skewness of each cell in the grid.
     """
-    # Get the centroids of each cell
+    qualityname = "Skewness"
 
     # Compute the skewness of each cell
     skewnesses = []
     for i in range(grid.n_cells):
         cell = grid.extract_cells(i)
         skewnesses.append(skewness(cell.points))
+    skewnesses = np.array(skewnesses)
+
+    meshok = classify_mesh_quality(qualityname, skewnesses)
+
+    if not meshok:
+        warnings.warn(f"Mesh quality ({qualityname}) is bad, consider refining the mesh.")
 
     return skewnesses
 
 
 def skewness(points):
     """
     Compute the skewness of a set of points.
```

### Comparing `ntrfc-0.1.8/ntrfc/timeseries/integral_scales.py` & `ntrfc-0.1.9/ntrfc/timeseries/integral_scales.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,26 +30,29 @@
 def get_self_correlating_frequencies(timesteps, signal):
     """
     Calculate the self-correlating frequencies in a signal.
 
     Parameters
     ----------
     timesteps : ndarray
-        An array of uniformly spaced timesteps, corresponding to the time intervals between samples in the signal.
+        An array of uniformly spaced timesteps, corresponding to the time intervals
+        between samples in the signal.
     signal : ndarray
         The input signal to analyze.
 
     Returns
     -------
     frequencies : ndarray
         An array of self-correlating frequencies, in units of inverse timesteps.
 
     Notes
     -----
-    This function calculates the autocorrelation of the input signal, and finds the local maxima in the autocorrelation signal. These local maxima correspond to the self-correlating frequencies in the signal.
+    This function calculates the autocorrelation of the input signal,
+    and finds the local maxima in the autocorrelation signal.
+    These local maxima correspond to the self-correlating frequencies in the signal.
     """
     # Calculate the autocorrelation of the signal
     autocorr_signal = autocorr(signal)
 
     # Find self-correlating frequencies by finding the local maxima in the autocorrelation signal
     self_correlating_frequencies = argrelmax(autocorr_signal)[0]
     ts_shifted = timesteps - timesteps[0]
```

### Comparing `ntrfc-0.1.8/ntrfc/timeseries/stationarity.py` & `ntrfc-0.1.9/ntrfc/timeseries/stationarity.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/turbo/airfoil_generators/naca_airfoil_creator.py` & `ntrfc-0.1.9/ntrfc/turbo/airfoil_generators/naca_airfoil_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,10 +286,11 @@
         # Setting radius
         radius = 5
 
         # Generating x and y data
         x = radius * np.cos(theta)
         y = radius * np.sin(theta)
         """
-    poly = pv.PolyData(np.stack([X, Y, np.zeros(len(X))]).T)
+    points = np.stack([X, Y, np.zeros(len(X))]).T
+    poly = pv.PolyData(points)
     poly = poly.clean(tolerance=1e-6)
     return poly.points[::, 0], poly.points[::, 1]
```

### Comparing `ntrfc-0.1.8/ntrfc/turbo/airfoil_generators/parametric_turbine_generator.py` & `ntrfc-0.1.9/ntrfc/turbo/airfoil_generators/parametric_turbine_generator.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/turbo/airfoil_generators/parsec_airfoil_creator.py` & `ntrfc-0.1.9/ntrfc/turbo/airfoil_generators/parsec_airfoil_creator.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/turbo/bladeloading.py` & `ntrfc-0.1.9/ntrfc/turbo/bladeloading.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 def calc_inflow_cp(px, pt1, p1):
     """
     :param px: pressure at position
     :param pt1: total pressure inlet
     :param p1: pressure inlet
     :return: lift coefficient
     """
-    cp = (px - pt1) / (p1 - pt1)
+    cp = (px - p1) / (pt1 - p1)
     return cp
 
 
 # Totaldruckverlustbeiwert
 def calc_zeta(pt1, pt2x, p2):
     """
     Calculates the Total Pressure Loss Coefficient (Zeta) for a fluid system.
```

### Comparing `ntrfc-0.1.8/ntrfc/turbo/cascade_geometry.py` & `ntrfc-0.1.9/ntrfc/turbo/cascade_geometry.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/ntrfc/turbo/domaingen_cascade.py` & `ntrfc-0.1.9/ntrfc/turbo/domaingen_cascade.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import tempfile
 
 import numpy as np
 import pyvista as pv
 
-from ntrfc.turbo.pointcloud_methods import extract_geo_paras, calcMidPassageStreamLine
+from ntrfc.turbo.cascade_case.utils.domain_utils import Blade2D
+from ntrfc.turbo.pointcloud_methods import calcMidPassageStreamLine
 
 
 def cascade_2d_domain(profilepoints2d, x_inlet, x_outlet, pitch, unit, blade_shift, alpha, path=False):
     """
     profilepoints2d = 2d numpy array
     """
 
@@ -20,33 +21,20 @@
     unitcoeff = 0
     if unit == "m":
         unitcoeff = 1
     elif unit == "mm":
         unitcoeff = 1 / 1000
     profilepoints2d.points *= unitcoeff
 
-    # =============================================================================
-    # Bestimmung Profilparameter
-    # =============================================================================
-    sortedPoly, psPoly, ssPoly, ind_vk, ind_hk, midsPoly, beta_leading, beta_trailing, camber_angle, alpha = extract_geo_paras(
-        profilepoints2d,
-        alpha,
-        path)
-
-    ##############################################################
-    x_mids = midsPoly.points[::, 0]
-    y_mids = midsPoly.points[::, 1]
-    # x_ss = ssPoly.points[::, 0]
-    # y_ss = ssPoly.points[::, 1]
-    # x_ps = psPoly.points[::, 0]
-    # y_ps = psPoly.points[::, 1]
+    blade = Blade2D(profilepoints2d.points)
+    blade.compute_all_frompoints()
 
-    x_mpsl, y_mpsl = calcMidPassageStreamLine(x_mids, y_mids, beta_leading, beta_trailing,
+    x_mpsl, y_mpsl = calcMidPassageStreamLine(blade.skeletonline_pv.points[::, 0], blade.skeletonline_pv.points[::, 1],
+                                              blade.beta_le, blade.beta_te,
                                               x_inlet, x_outlet, pitch)
-
     y_upper = np.array(y_mpsl) + blade_shift
     per_y_upper = pv.lines_from_points(np.stack((np.array(x_mpsl),
                                                  np.array(y_upper),
                                                  np.zeros(len(x_mpsl)))).T)
     y_lower = y_upper - pitch
     per_y_lower = pv.lines_from_points(np.stack((np.array(x_mpsl),
                                                  np.array(y_lower),
@@ -66,15 +54,15 @@
     p.add_mesh(inletPoly, color="r")
     p.add_mesh(per_y_lower, color="r")
     p.add_mesh(per_y_upper, color="r")
     p.add_mesh(profilepoints2d, color="k")
     p.view_xy()
     p.screenshot(path)
 
-    return sortedPoly, psPoly, ssPoly, per_y_upper, per_y_lower, inletPoly, outletPoly
+    return blade.sortedpointsrolled_pv, blade.ps_pv, blade.ss_pv, per_y_upper, per_y_lower, inletPoly, outletPoly
 
 
 def cascade_3d_domain(sortedPoly, psPoly, ssPoly, per_y_upper, per_y_lower, inletPoly, outletPoly, zspan, avdr=1,
                       path=None):
     if path is None:
         tmpdir = tempfile.mkdtemp()
         path = tmpdir + "/plot.png"
```

### Comparing `ntrfc-0.1.8/ntrfc/turbo/probegeneration.py` & `ntrfc-0.1.9/ntrfc/turbo/probegeneration.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     ref_psPoly = pv.PolyData(ref_ps_points)
 
     # Convert the PolyData objects to polylines
     ref_ss_poly = polyline_from_points(ref_ssPoly.points)
     ref_ps_poly = polyline_from_points(ref_psPoly.points)
 
     # Extrude the polylines along the z-axis to create 3D face models
-    ref_ss_face = ref_ss_poly.extrude((0, 0, midspan_z * 2)).compute_normals()
-    ref_ps_face = ref_ps_poly.extrude((0, 0, midspan_z * 2)).compute_normals()
+    ref_ss_face = ref_ss_poly.extrude((0, 0, midspan_z * 2), capping=False).compute_normals()
+    ref_ps_face = ref_ps_poly.extrude((0, 0, midspan_z * 2), capping=False).compute_normals()
 
     # Shift the 3D faces slightly along their normals
     ref_ss_face_shift = ref_ss_face.copy()
     ref_ss_face_shift.points += tolerance * ref_ss_face_shift.point_data["Normals"]
     ref_ps_face_shift = ref_ps_face.copy()
     ref_ps_face_shift.points += tolerance * ref_ps_face_shift.point_data["Normals"]
```

### Comparing `ntrfc-0.1.8/ntrfc/turbo/profile_tele_extraction.py` & `ntrfc-0.1.9/ntrfc/turbo/profile_tele_extraction.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import numpy as np
-import pyvista as pv
 from scipy.interpolate import splprep, splev
 from scipy.spatial import KDTree
 from scipy.spatial import Voronoi
+from shapely.geometry import Polygon, LineString
 
-from ntrfc.geometry.line import lines_from_points, polyline_from_points
+from ntrfc.geometry.line import refine_spline
 from ntrfc.geometry.plane import inside_poly
-from ntrfc.math.vectorcalc import findNearest, vecDir, compute_minmax_distance_in_pointcloud
+from ntrfc.math.vectorcalc import findNearest, vecDir
 
 
-def clean_sites(sites, boundary, tolerance_factor=3e-2):
+def clean_sites(sites, boundary, tolerance_factor=5e-2):
     # Build the KDTree from the "boundary" point cloud.
     tree = KDTree(boundary)
 
     # Query the KDTree to find the nearest neighbors for each point in "point_cloud_a."
 
     distances, _ = tree.query(sites)
-    deg_res = 2
+    deg_res = 4
 
     theta = np.linspace(0, 2 * np.pi, 360 * deg_res)
     cleaned = []
     radii = []
     for xc, yc, r in zip(sites[:, 0], sites[:, 1], distances):
 
         circlepoints = np.stack([np.cos(theta) * r + xc, np.sin(theta) * r + yc]).T
@@ -38,68 +38,67 @@
                 cleaned.append([xc, yc])
                 radii.append(r)
     print(f"ratio of cleaned sites: {len(cleaned) / len(sites)}")
 
     return np.array(cleaned), np.array(radii)
 
 
-def extract_vk_hk(sortedPoly, verbose=False):
+def extract_vk_hk(sortedPoly):
     points = sortedPoly.points
 
+    diag_dist = np.sqrt((sortedPoly.bounds[1] - sortedPoly.bounds[0]) ** 2 + (
+        sortedPoly.bounds[3] - sortedPoly.bounds[2]) ** 2)
     points_2d_closed_refined = pointcloud_to_profile(points)
 
     sites_raw_clean, radii = voronoi_skeleton_sites(points_2d_closed_refined)
 
-    tck, u = splprep(sites_raw_clean.T, u=None, s=0.000005, per=0, k=3)
-    res = 4000
-    u_new = np.linspace(u.min(), u.max(), res)
-    x_center, y_center = splev(u_new, tck, der=0)
-    le_ind, te_ind = skeletonline_completion(x_center, y_center, points)
+    le_ind, te_ind = skeletonline_completion(diag_dist, points, points_2d_closed_refined, sites_raw_clean)
 
     return le_ind, te_ind
 
 
+def skeletonline_completion(diag_dist, points, points_2d_closed_refined, sites_raw_clean):
+    sites_refined_clean_tuple = refine_spline(sites_raw_clean[:, 0], sites_raw_clean[:, 1], 100)
+    sites_refined_clean = np.stack([sites_refined_clean_tuple[0], sites_refined_clean_tuple[1]]).T
+    shapelypoly = Polygon(points_2d_closed_refined)
+    shapelymidline = LineString(sites_refined_clean)
+    # i need to extend thhe shapelymidline to the boundary of the polygon
+    # Get the coordinates of the start and end points
+    start_coords = np.array(shapelymidline.coords[0])
+    end_coords = np.array(shapelymidline.coords[-1])
+    # Compute the direction vector
+    direction_start = diag_dist * vecDir(-(shapelymidline.coords[1] - start_coords))
+    direction_end = diag_dist * vecDir(-(shapelymidline.coords[-2] - end_coords))
+    # Extend the line by 1 unit in both directions
+    extended_start = LineString([start_coords, start_coords + direction_start])
+    extended_end = LineString([end_coords, end_coords + direction_end])
+    # Compute the intersection with the polygon
+    intersection_start = extended_start.intersection(shapelypoly)
+    intersection_end = extended_end.intersection(shapelypoly)
+    intersection_point_start = np.array(intersection_start.coords)[1]
+    intersection_point_end = np.array(intersection_end.coords)[1]
+    # find closest point index of points and intersections
+    le_ind = findNearest(points[:, :2], intersection_point_start)
+    te_ind = findNearest(points[:, :2], intersection_point_end)
+    return le_ind, te_ind
+
+
 def voronoi_skeleton_sites(points_2d_closed_refined):
     vor = Voronoi(points_2d_closed_refined)
     voronoi_sites_inside = vor.vertices[inside_poly(points_2d_closed_refined, vor.vertices)]
 
     sort_indices = np.argsort(voronoi_sites_inside[:, 0])
     sites_inside_sorted = voronoi_sites_inside[sort_indices]
 
     clean_sites_inside, radii = clean_sites(sites_inside_sorted, points_2d_closed_refined)
     return clean_sites_inside, radii
 
 
-def skeletonline_completion(x_center, y_center, points):
-    camberpoints = np.stack([x_center, y_center, np.zeros(len(y_center))]).T
-    camberline = lines_from_points(camberpoints)
-    LE_camber = camberline.extract_cells(0)
-    LE_dir = vecDir(LE_camber.points[-1] - LE_camber.points[0])
-    TE_camber = camberline.extract_cells(camberline.number_of_cells - 1)
-    TE_dir = vecDir(TE_camber.points[0] - TE_camber.points[-1])
-    X = points[::, 0]
-    Y = points[::, 1]
-    Z = X * 0
-    profilepoly = polyline_from_points(np.vstack([np.stack([X, Y, Z]).T, np.stack([X[0], Y[0], Z[0]]).T]))
-    chord = compute_minmax_distance_in_pointcloud(points, minmax="max")
-    camber_le_extension = pv.Line(LE_camber.points[0] - LE_dir * chord / 2, camberpoints[0], resolution=400)
-    camber_te_extension = pv.Line(camberpoints[-1], TE_camber.points[0] - TE_dir * chord / 2, resolution=400)
-    camberline_extended = lines_from_points(np.vstack([camber_le_extension.points,
-                                                       camberpoints[1:-2],
-                                                       camber_te_extension.points]))
-    helpersurface = profilepoly.copy().extrude([0, 0, -1], inplace=True)
-    helpersurface = helpersurface.translate([0, 0, .5], inplace=True)
-    camberline_computed = camberline_extended.clip_surface(helpersurface, invert=False)
-    le_ind = findNearest(np.stack([X, Y, Z]).T, camberline_computed.points[0])
-    te_ind = findNearest(np.stack([X, Y, Z]).T, camberline_computed.points[-1])
-
-    return le_ind, te_ind
-
-
 def pointcloud_to_profile(points):
     points_2d_closed = np.vstack((points[:, :2], points[:, :2][0]))
     tck, u = splprep(points_2d_closed.T, u=None, s=0.0, per=1, k=3)
     res = 10000
     u_new = np.linspace(u.min(), u.max(), res)
     x_new, y_new = splev(u_new, tck, der=0)
     points_2d_closed_refined = np.stack([x_new, y_new]).T
+
     return points_2d_closed_refined
```

### Comparing `ntrfc-0.1.8/ntrfc.egg-info/PKG-INFO` & `ntrfc-0.1.9/ntrfc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ntrfc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Numerical Test Rig for Cascades. A workflows-library for cfd-analysis of cascade-flows
 Home-page: https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC
 Author: Malte Nyhuis
 Author-email: nyhuis@tfd.uni-hannover.de
 License: MIT license
 Keywords: ntrfc
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: pip>=23
 Requires-Dist: matplotlib==3.7.1
 Requires-Dist: pytest==7.2.2
 Requires-Dist: trame==2.5.2
 Requires-Dist: pyvista[all]==0.42.3
@@ -28,14 +29,15 @@
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: statsmodels>=0.13.5
 Requires-Dist: imageio==2.30.0
 Requires-Dist: scikit-learn
 Requires-Dist: jupyter
 Requires-Dist: sphinx
 Requires-Dist: gmsh==4.11.1
+Requires-Dist: shapely==2.0.1
 
 ============
 NTRfC README
 ============
 
 **Numerical Test Rig for Cascades.**
 
@@ -120,14 +122,22 @@
 - [Cookiecutter](https://github.com/audreyr/cookiecutter)
 - [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
 
 
 =======
 History
 =======
+=======
+0.1.9 (2024-03-15)
+------------------
+
+- cascade_case refactoring
+- cleanup
+- le-te-extraction fix
+- cascadebox meshing (gmsh)
 
 0.1.8 (2023-10-31)
 ------------------
 
 - bladeloading fix: reliable variable name usage
```

### Comparing `ntrfc-0.1.8/ntrfc.egg-info/SOURCES.txt` & `ntrfc-0.1.9/ntrfc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -36,23 +36,14 @@
 ntrfc.egg-info/PKG-INFO
 ntrfc.egg-info/SOURCES.txt
 ntrfc.egg-info/dependency_links.txt
 ntrfc.egg-info/entry_points.txt
 ntrfc.egg-info/not-zip-safe
 ntrfc.egg-info/requires.txt
 ntrfc.egg-info/top_level.txt
-ntrfc/cascade_case/__init__.py
-ntrfc/cascade_case/domain.py
-ntrfc/cascade_case/solution.py
-ntrfc/cascade_case/casemeta/__init__.py
-ntrfc/cascade_case/casemeta/casemeta.py
-ntrfc/cascade_case/utils/__init__.py
-ntrfc/cascade_case/utils/domain_utils.py
-ntrfc/cascade_case/utils/probecontainer.py
-ntrfc/cascade_case/utils/sliceseries.py
 ntrfc/data/README.md
 ntrfc/data/compressor_cascade/README.md
 ntrfc/data/compressor_cascade/profilepoints.txt
 ntrfc/data/openfoam_cascade_case/README.md
 ntrfc/data/openfoam_cascade_case/internal.vtu
 ntrfc/data/openfoam_cascade_case/boundary/blade_wall.vtp
 ntrfc/data/openfoam_cascade_case/boundary/inlet.vtp
@@ -77,25 +68,24 @@
 ntrfc/fluid/isentropic.py
 ntrfc/fluid/turbulence.py
 ntrfc/geometry/__init__.py
 ntrfc/geometry/alphashape.py
 ntrfc/geometry/line.py
 ntrfc/geometry/plane.py
 ntrfc/geometry/surface.py
-ntrfc/gmsh/__init__.py
-ntrfc/gmsh/turbo_cascade.py
 ntrfc/math/__init__.py
 ntrfc/math/methods.py
 ntrfc/math/vectorcalc.py
 ntrfc/meshquality/__init__.py
 ntrfc/meshquality/aspect_ratio.py
 ntrfc/meshquality/grid_convergece_index.py
 ntrfc/meshquality/meshexpansion.py
 ntrfc/meshquality/nondimensionals.py
 ntrfc/meshquality/skewness.py
+ntrfc/meshquality/standards.py
 ntrfc/timeseries/__init__.py
 ntrfc/timeseries/integral_scales.py
 ntrfc/timeseries/stationarity.py
 ntrfc/turbo/__init__.py
 ntrfc/turbo/bladeloading.py
 ntrfc/turbo/cascade_geometry.py
 ntrfc/turbo/domaingen_cascade.py
@@ -103,53 +93,68 @@
 ntrfc/turbo/pointcloud_methods.py
 ntrfc/turbo/probegeneration.py
 ntrfc/turbo/profile_tele_extraction.py
 ntrfc/turbo/airfoil_generators/__init__.py
 ntrfc/turbo/airfoil_generators/naca_airfoil_creator.py
 ntrfc/turbo/airfoil_generators/parametric_turbine_generator.py
 ntrfc/turbo/airfoil_generators/parsec_airfoil_creator.py
+ntrfc/turbo/cascade_case/__init__.py
+ntrfc/turbo/cascade_case/domain.py
+ntrfc/turbo/cascade_case/post.py
+ntrfc/turbo/cascade_case/solution.py
+ntrfc/turbo/cascade_case/casemeta/__init__.py
+ntrfc/turbo/cascade_case/casemeta/casemeta.py
+ntrfc/turbo/cascade_case/utils/__init__.py
+ntrfc/turbo/cascade_case/utils/domain_utils.py
+ntrfc/turbo/cascade_case/utils/probecontainer.py
+ntrfc/turbo/cascade_case/utils/sliceseries.py
+ntrfc/turbo/gmsh/__init__.py
+ntrfc/turbo/gmsh/turbo_cascade.py
+ntrfc/turbo/gmsh/windtunnel_cascade.py
 tests/__init__.py
 tests/test_ntrfc.py
-tests/cascadecase/__init__.py
-tests/cascadecase/domain/__init__.py
-tests/cascadecase/domain/test_ntrfc_domaingen_cascade.py
-tests/cascadecase/solution/__init__.py
-tests/cascadecase/solution/test_probecontainer.py
-tests/cascadecase/solution/test_solution.py
 tests/filehandling/__init__.py
 tests/filehandling/test_ntrfc_datafiles.py
 tests/filehandling/test_ntrfc_mesh.py
 tests/fluid/__init__.py
 tests/fluid/test_ntrfc_fluid.py
 tests/fluid/test_ntrfc_isentropic.py
 tests/fluid/test_ntrfc_turbulence.py
 tests/geometry/__init__.py
 tests/geometry/test_ntrfc_alphashape.py
 tests/geometry/test_ntrfc_geometry.py
 tests/geometry/test_ntrfc_line.py
 tests/geometry/test_ntrfc_plane.py
 tests/geometry/test_ntrfc_surface.py
-tests/gmsh/__init__.py
-tests/gmsh/test_meshing.py
 tests/math/__init__.py
 tests/math/test_ntrfc_methods.py
 tests/math/test_ntrfc_vectorcalc.py
 tests/meshquality/__init__.py
 tests/meshquality/test_ntrfc_aspect_ratio.py
 tests/meshquality/test_ntrfc_grid_convergence_index.py
 tests/meshquality/test_ntrfc_meshexpansion.py
 tests/meshquality/test_ntrfc_nondimensionals.py
 tests/meshquality/test_ntrfc_skewness.py
+tests/meshquality/test_ntrfc_standards.py
 tests/timeseries/__init__.py
 tests/timeseries/test_ntrfc_integral_scales.py
 tests/timeseries/test_ntrfc_stationarity.py
 tests/turbo/__init__.py
 tests/turbo/test_ntrfc_bladeloading.py
 tests/turbo/test_ntrfc_cascade_geometry.py
 tests/turbo/test_ntrfc_domaingen_cascade.py
 tests/turbo/test_ntrfc_integrals.py
 tests/turbo/test_ntrfc_pointcloud_methods.py
 tests/turbo/test_ntrfc_probegeneration.py
 tests/turbo/airfoil_generators/__init__.py
 tests/turbo/airfoil_generators/test_naca_airfoil_creator.py
 tests/turbo/airfoil_generators/test_parametric_turbine_creator.py
-tests/turbo/airfoil_generators/test_parsec_airfoil_creator.py
+tests/turbo/airfoil_generators/test_parsec_airfoil_creator.py
+tests/turbo/cascadecase/__init__.py
+tests/turbo/cascadecase/test_post.py
+tests/turbo/cascadecase/test_solution.py
+tests/turbo/cascadecase/domain/__init__.py
+tests/turbo/cascadecase/domain/test_ntrfc_domaingen_cascade.py
+tests/turbo/cascadecase/solution/__init__.py
+tests/turbo/cascadecase/solution/test_probecontainer.py
+tests/turbo/gmsh/__init__.py
+tests/turbo/gmsh/test_meshing.py
```

### Comparing `ntrfc-0.1.8/setup.py` & `ntrfc-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,19 +33,20 @@
         'console_scripts': [
             'ntrfc=ntrfc.cli:main',
         ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
+    long_description_content_type='text/markdown',
     include_package_data=True,
     package_data={
         'ntrfc': ['data/*'],
     },
     keywords='ntrfc',
     packages=find_packages(include=['ntrfc', 'ntrfc.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC',
-    version='0.1.8',
+    version='0.1.9',
     zip_safe=False,
 )
```

### Comparing `ntrfc-0.1.8/tests/cascadecase/solution/test_probecontainer.py` & `ntrfc-0.1.9/tests/turbo/cascadecase/solution/test_probecontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pytest
 
-from ntrfc.cascade_case.utils.probecontainer import ProbeContainer
+from ntrfc.turbo.cascade_case.utils.probecontainer import ProbeContainer
 
 
 @pytest.fixture
 def probe_container():
     container = ProbeContainer()
     container.add_probe(
         position=np.array([0, 0, 0]),
```

### Comparing `ntrfc-0.1.8/tests/filehandling/test_ntrfc_datafiles.py` & `ntrfc-0.1.9/tests/filehandling/test_ntrfc_datafiles.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/filehandling/test_ntrfc_mesh.py` & `ntrfc-0.1.9/tests/filehandling/test_ntrfc_mesh.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/fluid/test_ntrfc_fluid.py` & `ntrfc-0.1.9/tests/fluid/test_ntrfc_fluid.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/fluid/test_ntrfc_isentropic.py` & `ntrfc-0.1.9/tests/fluid/test_ntrfc_isentropic.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/fluid/test_ntrfc_turbulence.py` & `ntrfc-0.1.9/tests/fluid/test_ntrfc_turbulence.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/geometry/test_ntrfc_alphashape.py` & `ntrfc-0.1.9/tests/geometry/test_ntrfc_alphashape.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/geometry/test_ntrfc_line.py` & `ntrfc-0.1.9/tests/geometry/test_ntrfc_line.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/geometry/test_ntrfc_plane.py` & `ntrfc-0.1.9/tests/geometry/test_ntrfc_plane.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/math/test_ntrfc_methods.py` & `ntrfc-0.1.9/tests/math/test_ntrfc_methods.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/math/test_ntrfc_vectorcalc.py` & `ntrfc-0.1.9/tests/math/test_ntrfc_vectorcalc.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/meshquality/test_ntrfc_aspect_ratio.py` & `ntrfc-0.1.9/tests/meshquality/test_ntrfc_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/meshquality/test_ntrfc_grid_convergence_index.py` & `ntrfc-0.1.9/tests/meshquality/test_ntrfc_grid_convergence_index.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/meshquality/test_ntrfc_meshexpansion.py` & `ntrfc-0.1.9/tests/meshquality/test_ntrfc_meshexpansion.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/meshquality/test_ntrfc_nondimensionals.py` & `ntrfc-0.1.9/tests/meshquality/test_ntrfc_nondimensionals.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/meshquality/test_ntrfc_skewness.py` & `ntrfc-0.1.9/tests/meshquality/test_ntrfc_skewness.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/timeseries/test_ntrfc_integral_scales.py` & `ntrfc-0.1.9/tests/timeseries/test_ntrfc_integral_scales.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/timeseries/test_ntrfc_stationarity.py` & `ntrfc-0.1.9/tests/timeseries/test_ntrfc_stationarity.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/turbo/airfoil_generators/test_naca_airfoil_creator.py` & `ntrfc-0.1.9/tests/turbo/airfoil_generators/test_naca_airfoil_creator.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/turbo/airfoil_generators/test_parametric_turbine_creator.py` & `ntrfc-0.1.9/tests/turbo/airfoil_generators/test_parametric_turbine_creator.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/turbo/test_ntrfc_bladeloading.py` & `ntrfc-0.1.9/tests/turbo/test_ntrfc_bladeloading.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 
 def test_calc_inflow_cp():
     from ntrfc.turbo.bladeloading import calc_inflow_cp
     # Test case with positive pressure difference
     px = 101325  # Pa
     pt1 = 110000  # Pa
     p1 = 100000  # Pa
-    expected_cp = 0.8675
+    expected_cp = 0.1325
     assert calc_inflow_cp(px, pt1, p1) == expected_cp
 
     # Test case with negative pressure difference
     px = 90000  # Pa
     pt1 = 110000  # Pa
     p1 = 100000  # Pa
-    expected_cp = 2
+    expected_cp = -1.0
     assert calc_inflow_cp(px, pt1, p1) == expected_cp
 
     # Test case with zero pressure difference
     px = 100000  # Pa
     pt1 = 100000  # Pa
     p1 = 110000  # Pa
-    expected_cp = 0
+    expected_cp = 1.0
     assert calc_inflow_cp(px, pt1, p1) == expected_cp
 
 
 def test_calc_zeta():
     from ntrfc.turbo.bladeloading import calc_zeta
     assert calc_zeta(100, 80, 70) == 0.6666666666666666
     assert calc_zeta(50, 20, 10) == 0.75
```

### Comparing `ntrfc-0.1.8/tests/turbo/test_ntrfc_domaingen_cascade.py` & `ntrfc-0.1.9/tests/turbo/test_ntrfc_domaingen_cascade.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 
 import numpy as np
 import pyvista as pv
 
-from ntrfc.turbo.domaingen_cascade import cascade_2d_domain
-
 ON_CI = 'CI' in os.environ
 
 
 def test_cascade_3d_domain():
     from ntrfc.turbo.airfoil_generators.naca_airfoil_creator import naca
     from ntrfc.turbo.domaingen_cascade import cascade_3d_domain
     from ntrfc.turbo.domaingen_cascade import cascade_2d_domain
@@ -30,15 +28,15 @@
 
     cascade_3d_domain(sortedPoly, psPoly, ssPoly, per_y_upper, per_y_lower, inletPoly, outletPoly, zspan=0.2, avdr=1,
                       path=False)
 
 
 def test_cascade_2d_domain():
     from ntrfc.turbo.airfoil_generators.naca_airfoil_creator import naca
-
+    from ntrfc.turbo.domaingen_cascade import cascade_2d_domain
     if ON_CI:
         pv.start_xvfb()
 
     naca_code = "6509"
     angle = 30  # deg
     res = 420
     xs, ys = naca(naca_code, res, half_cosine_spacing=False)
```

### Comparing `ntrfc-0.1.8/tests/turbo/test_ntrfc_integrals.py` & `ntrfc-0.1.9/tests/turbo/test_ntrfc_integrals.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.8/tests/turbo/test_ntrfc_probegeneration.py` & `ntrfc-0.1.9/tests/turbo/test_ntrfc_probegeneration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import numpy as np
 import pyvista as pv
 
 
 def test_createprofileprobes():
     from ntrfc.turbo.probegeneration import create_profileprobes
     from ntrfc.turbo.airfoil_generators.naca_airfoil_creator import naca
-    from ntrfc.turbo.pointcloud_methods import extract_geo_paras
+    from ntrfc.turbo.cascade_case.utils.domain_utils import Blade2D
     naca_code = "6009"
     angle = 10  # deg
     res = 240
     xs, ys = naca(naca_code, res, half_cosine_spacing=False)
     sorted_poly = pv.PolyData(np.stack([xs, ys, np.zeros(len(xs))]).T)
     sorted_poly.rotate_z(angle, inplace=True)
-    sorted_extracted_poly, psPoly, ssPoly, ind_vk, ind_hk, midsPoly, beta_leading, beta_trailing, camber_angle, alpha = extract_geo_paras(
-        sorted_poly, 1)
+    blade = Blade2D(sorted_poly)
+    blade.compute_all_frompoints()
     n_psprobes = 24
     n_ssprobes = 36
-    probes_ss, probes_ps = create_profileprobes(ssPoly, psPoly, 1, n_ssprobes, n_psprobes, tolerance=1e-6)
+    probes_ss, probes_ps = create_profileprobes(blade.ss_pv, blade.ps_pv, 1, n_ssprobes, n_psprobes, tolerance=1e-6)
     assert probes_ps.number_of_points == n_psprobes, "number of pressure side probes not correct"
     assert probes_ss.number_of_points == n_ssprobes, "number of suction side probes not correct"
 
 
 def test_create_midpassageprobes():
     from ntrfc.turbo.probegeneration import create_midpassageprobes
     from ntrfc.turbo.airfoil_generators.naca_airfoil_creator import naca
-    from ntrfc.turbo.pointcloud_methods import extract_geo_paras
+    from ntrfc.turbo.cascade_case.utils.domain_utils import Blade2D
     naca_code = "6009"
     angle = 10  # deg
     res = 240
     xs, ys = naca(naca_code, res, half_cosine_spacing=False)
     sorted_poly = pv.PolyData(np.stack([xs, ys, np.zeros(len(xs))]).T)
     sorted_poly.rotate_z(angle, inplace=True)
-    sorted_extracted_poly, psPoly, ssPoly, ind_vk, ind_hk, midsPoly, beta_leading, beta_trailing, camber_angle, alpha = extract_geo_paras(
-        sorted_poly, 1)
+    blade = Blade2D(sorted_poly)
+    blade.compute_all_frompoints()
+
     nop = 40
-    midspan_probes = create_midpassageprobes(1, -0.3, 0.3, 0.1, beta_leading, beta_trailing, midsPoly, nop)
+    midspan_probes = create_midpassageprobes(1, -0.3, 0.3, 0.1, blade.beta_le, blade.beta_te, blade.skeletonline_pv,
+                                             nop)
     assert midspan_probes.number_of_points == nop, "number of probes on midpassage line not correct"
 
 
 def test_stagnationpointprobes():
     from ntrfc.turbo.probegeneration import create_stagnationpointprobes
     from ntrfc.turbo.airfoil_generators.naca_airfoil_creator import naca
```

