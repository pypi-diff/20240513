# Comparing `tmp/ngstrefftz-0.3.2402.dev34.tar.gz` & `tmp/ngstrefftz-0.3.2402.dev35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngstrefftz-0.3.2402.dev34.tar", last modified: Thu May  9 00:42:34 2024, max compression
+gzip compressed data, was "ngstrefftz-0.3.2402.dev35.tar", last modified: Thu May  9 09:31:59 2024, max compression
```

## Comparing `ngstrefftz-0.3.2402.dev34.tar` & `ngstrefftz-0.3.2402.dev35.tar`

### file list

```diff
@@ -1,180 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.330652 ngstrefftz-0.3.2402.dev34/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.334652 ngstrefftz-0.3.2402.dev34/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build_linux_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/ngsolve_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.334652 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/build_in_docker.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/_static/breadcrumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/_static/css/mytheme.css
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/contrib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/docu.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-adv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-helm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-poi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-stokes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-wave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/helmholtz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/laplace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/qtwave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/tunfitted.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/twave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/twavetents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/paper/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/paper/codemeta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.330652 ngstrefftz-0.3.2402.dev34/external_dependencies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.330652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.330652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/
--rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/burgers1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/burgers2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/euler2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/maxwell/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/draw3dtent.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/draw3dvertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/horn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/BurgersMTP.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/INDEX.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/StartPitching.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/
--rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/CausalityCond.png
--rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/dag.png
--rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/map.png
--rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/subtents.png
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/conslaw/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/conslaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/_drawtents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/_drawtents2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.350652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/advection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/burgers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/concurrentqueue.h
--rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/conservationlaw.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/euler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/maxwell.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/paralleldepend.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/python_conslaw.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/python_tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/symbolic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tentsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tentsolver_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/vis3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/vis3d.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/wave.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.354652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_burgers_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_causal_tents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_conslaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_tent_height_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_tentlayers.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/src/
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/airy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/condensedg.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/condensedg.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/diffopmapped.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/embtrefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/embtrefftz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/mesh1dtents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/mesh1dtents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/monomialfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/monomialfespace.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/ngsttd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/planewavefe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/planewavefe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/python_trefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/scalarmappedfe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/scalarmappedfe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/specialcoefficientfunction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/specialcoefficientfunction.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/specialintegrator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/specialintegrator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    56525 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/trefftzfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/trefftzfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    45126 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/twavetents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/twavetents.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/test/
--rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/test/dg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/test/embt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/test/tents.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/test/trefftz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.526741 ngstrefftz-0.3.2402.dev35/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build_linux_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/ngsolve_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/build_in_docker.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/_static/breadcrumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/_static/css/mytheme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/docu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-adv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-helm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-poi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-stokes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-wave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/helmholtz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/laplace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/qtwave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/tunfitted.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/twave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/twavetents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/docs/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/paper/codemeta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.526741 ngstrefftz-0.3.2402.dev35/external_dependencies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.526741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/ngsolve_version.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.526741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/burgers1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/burgers2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/euler2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/maxwell/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/draw3dtent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/draw3dvertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/horn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/BurgersMTP.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/INDEX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/StartPitching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/
+-rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/CausalityCond.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/dag.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/subtents.png
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.542741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/conslaw/
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/conslaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.542741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/_drawtents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/_drawtents2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.542741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/advection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/burgers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/concurrentqueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/conservationlaw.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/maxwell.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/paralleldepend.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/python_conslaw.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/python_tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/symbolic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47173 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tentsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tentsolver_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/vis3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/vis3d.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/wave.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.546742 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_burgers_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_causal_tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_conslaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_tent_height_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_tentlayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/airy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/condensedg.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/condensedg.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/diffopmapped.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/embtrefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/embtrefftz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/mesh1dtents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/mesh1dtents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/monomialfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/monomialfespace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/ngsttd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/planewavefe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/planewavefe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/python_trefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/scalarmappedfe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/scalarmappedfe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/specialcoefficientfunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/specialcoefficientfunction.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/specialintegrator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/specialintegrator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    56525 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/trefftzfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/trefftzfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45126 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/twavetents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/twavetents.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/test/dg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/test/embt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/test/tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/test/trefftz.py
```

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/build.yml` & `ngstrefftz-0.3.2402.dev35/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/build_linux_test.sh` & `ngstrefftz-0.3.2402.dev35/.github/workflows/build_linux_test.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip.ps1`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip.sh`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     #echo $PYDIR
     #$PYDIR/pip install -U pytest-check numpy wheel scikit-build mkl==2021.* mkl-devel==2021.*
     #$PYDIR/pip install netgen-mesher
     #NETGENDIR=/opt/_internal/cpython-3.9.13/bin
 
     #rm -rf /home/app/ngstrefftz/make
     rm -rf _skbuild
-    $PYDIR/pip install pytest-check numpy wheel scikit-build mkl==2023.* mkl-devel==2023.* setuptools setuptools_scm
+    $PYDIR/pip install pytest-check numpy wheel scikit-build mkl==2023.* mkl-devel==2023.* setuptools==69.5.1 setuptools_scm==8.1.0
     $PYDIR/pip install -r ./.github/workflows/ngsolve_version.txt
 
     $PYDIR/pip wheel -vvv .
     #cat src/ngstrefftz.egg-info/SOURCES.txt
     #auditwheel repair ngstrefftz*.whl
     rename linux_ manylinux_2_17_x86_64.manylinux2014_ ngstrefftz*.whl
     mv ngstrefftz*.whl wheelhouse/
```

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip_mac.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2402.dev35/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/Dockerfile` & `ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/build_in_docker.sh` & `ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/build_in_docker.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/merge.py` & `ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/merge.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/requirements.txt` & `ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/CONTRIBUTING.md` & `ngstrefftz-0.3.2402.dev35/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/Dockerfile` & `ngstrefftz-0.3.2402.dev35/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/LICENSE` & `ngstrefftz-0.3.2402.dev35/LICENSE`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/PKG-INFO` & `ngstrefftz-0.3.2402.dev35/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2402.dev34
+Version: 0.3.2402.dev35
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
-Requires-Dist: ngsolve>=6.2.2401.post24.dev0
+Requires-Dist: ngsolve>=6.2.2402
 Requires-Dist: ngstents>=0.0.2.dev39
 Requires-Dist: mkl
 
 NGSTrefftz provides a framework to implement Trefftz finite element spaces for NGSolve, with several Trefftz spaces already implemented. Additionally, Trefftz-DG on tent-pitched meshes for the acoustic wave equation is implemented using meshes provided by ngstents. Furthermore, the package includes an implementation of the embedded Trefftz method.
```

### Comparing `ngstrefftz-0.3.2402.dev34/README.md` & `ngstrefftz-0.3.2402.dev35/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/conf.py` & `ngstrefftz-0.3.2402.dev35/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/docu.rst` & `ngstrefftz-0.3.2402.dev35/docs/docu.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/index.rst` & `ngstrefftz-0.3.2402.dev35/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/intro.rst` & `ngstrefftz-0.3.2402.dev35/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-adv.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-adv.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-helm.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-helm.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-poi.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-poi.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-stokes.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-stokes.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-wave.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-wave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/helmholtz.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/helmholtz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/index.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/laplace.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/laplace.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/qtwave.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/qtwave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/tunfitted.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/tunfitted.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/twave.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/twave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/notebooks/twavetents.ipynb` & `ngstrefftz-0.3.2402.dev35/docs/notebooks/twavetents.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/paper/codemeta.json` & `ngstrefftz-0.3.2402.dev35/docs/paper/codemeta.json`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/paper/paper.bib` & `ngstrefftz-0.3.2402.dev35/docs/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/docs/paper/paper.md` & `ngstrefftz-0.3.2402.dev35/docs/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build.yml` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -20,152 +20,158 @@
              sudo apt-get install -y software-properties-common
              sudo add-apt-repository universe
              sudo add-apt-repository ppa:ngsolve/nightly -y
              sudo apt-get install ngsolve -y
              pip3 install pytest matplotlib numpy
       - name: set path
         run: |
-             echo "PYTHONPATH=/usr/lib/python3/dist-packages/:$GITHUB_WORKSPACE/install" >> $GITHUB_ENV
+             echo "PYTHONPATH=/usr/lib/python3/dist-packages/:$GITHUB_WORKSPACE/install/lib/python3.10/dist-packages" >> $GITHUB_ENV
              echo "NETGENDIR=/usr/bin/" >> $GITHUB_ENV
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: cmake ngstents
-        run: cmake -DCMAKE_INSTALL_PREFIX=$GITHUB_WORKSPACE/install -B$GITHUB_WORKSPACE/make -S$GITHUB_WORKSPACE/src
+        run: cmake -DCMAKE_INSTALL_PREFIX=$GITHUB_WORKSPACE/install -DPY_INSTALL_DIR="" -B$GITHUB_WORKSPACE/make -S$GITHUB_WORKSPACE/src
       - name: compile ngstents
         run: |
              make -C$GITHUB_WORKSPACE/make
              sudo make -C$GITHUB_WORKSPACE/make install  
       - name: test ngstents
         run: |
              cd $GITHUB_WORKSPACE/tests
              pytest .
 
   macos-nightly:
-    runs-on: macos-latest
+    runs-on: macos-13
     steps:     
-      - name: install ngsolve
-        run: |
-             wget https://www.asc.tuwien.ac.at/~mhochsteger/ngsolve/macos/NGSolve_nightly.dmg
-             hdiutil attach NGSolve_nightly.dmg
-             cp -R /Volumes/NGSolve/* /Applications
+      - name: Get Python 
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.12'
       - name: set path
         run: |
-             echo "PYTHONPATH=$PYTHONPATH:/Applications/Netgen.app/Contents/Resources/lib/python3.8/site-packages:." >> $GITHUB_ENV
-             echo "NETGENDIR=/Applications/Netgen.app/Contents/MacOS" >> $GITHUB_ENV
-             echo "DYLD_LIBRARY_PATH=$DYLD_LIBRARY_PATH:$NETGENDIR" >> $GITHUB_ENV
-             echo "DYLD_FRAMEWORK_PATH=$DYLD_FRAMEWORK_PATH:$NETGENDIR/../Frameworks" >> $GITHUB_ENV
-             echo "$NETGENDIR" >> $GITHUB_PATH
-      - uses: actions/checkout@v3
+             echo "PYDIR=${{ env.Python3_ROOT_DIR }}/bin" >> $GITHUB_ENV
+             echo "NETGEN_Dir=${{ env.Python3_ROOT_DIR }}/bin/../lib/python3.12/site-packages/netgen/cmake" >> $GITHUB_ENV
+             echo "NGSolve_Dir=${{ env.Python3_ROOT_DIR }}/bin/../lib/python3.12/site-packages/ngsolve/cmake" >> $GITHUB_ENV
+             echo "/Applications/CMake.app/Contents/bin" >> $GITHUB_PATH
+      - run: echo "CMAKE_PREFIX_PATH=${{ env.CMAKE_PREFIX_PATH }}:${{ env.NGSolve_Dir }}:${{ env.NETGEN_Dir }}" >> $GITHUB_ENV
+      - name: install ngsolve
+        run: pip3 install ngsolve pytest matplotlib
+      - uses: actions/checkout@v4
       - name: cmake ngstents
         run: cmake -B$GITHUB_WORKSPACE/make -S$GITHUB_WORKSPACE/src
       - name: compile ngstents
         run: |
              make -C$GITHUB_WORKSPACE/make
              sudo make -C$GITHUB_WORKSPACE/make install  
+      - name: test ngstents
+        run: |
+             cd $GITHUB_WORKSPACE/tests
+             pytest .
 
   pypi-linux:
     name: Build wheels for linux
     needs: [ubuntu-nightly, macos-nightly]
     runs-on: ubuntu-latest
     steps:
       - name: clear cache
         run: rm -rf /opt/hostedtoolcache
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: 'True'
           path: 'ngstents'
           fetch-depth: 0 # otherwise, you will fail to push refs to dest repo
       - name: pull manylinux
         run: docker pull sameli/manylinux2014_x86_64_cuda_11.7
       - name: build pip
         run: docker run -v $GITHUB_WORKSPACE:/workspace sameli/manylinux2014_x86_64_cuda_11.7 /bin/sh /workspace/ngstents/.github/workflows/build_pip.sh 
       - name: Store the binary wheel
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: python-package-distributions
+          name: python-package-distributions-linux
           path: ngstents/wheelhouse
 
   pypi-mac:
     name: Build wheels for macOS
     needs: [ubuntu-nightly, macos-nightly]
     strategy:
       matrix:
-        py: ['3.8', '3.9', '3.10', '3.11']
+        py: ['3.8', '3.9', '3.10', '3.11', '3.12']
     runs-on: macos-11
     env:
       MACOSX_DEPLOYMENT_TARGET: '10.15'
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
           submodules: recursive
           path: 'ngstents'
       - name: Get Python ${{ matrix.py }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.py }}
       - name: Run build script
         run: cd ngstents/.github/workflows && bash build_pip_mac.sh ${{ matrix.py }}
       - name: Store the binary wheel
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: python-package-distributions
+          name: python-package-distributions-mac-${{ matrix.py }}
           path: ngstents/wheelhouse
 
   pypi-win:
     name: Build wheels for Windows
     needs: [ubuntu-nightly, macos-nightly]
     strategy:
       matrix:
-        py: ['3.8', '3.9', '3.10', '3.11']
+        py: ['3.8', '3.9', '3.10', '3.11', '3.12']
     runs-on: windows-2019
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
           submodules: recursive
           path: 'ngstents'
       - name: Get Python ${{ matrix.py }}
         id: python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.py }}
       - name: Run build script
         run: Set-Location ngstents/.github/workflows; ./build_pip.ps1 ${{ env.pythonLocation }}
       - name: Store the binary wheel
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: python-package-distributions
+          name: python-package-distributions-win-${{ matrix.py }}
           path: ngstents/wheelhouse
 
   publish-pypi:
     name: Publish to PyPI
     needs: [pypi-mac, pypi-linux, pypi-win]
     runs-on: ubuntu-latest
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v4
       with:
-        name: python-package-distributions
+        pattern: python-package-distributions-*
+        merge-multiple: true
         path: ngstents/wheelhouse/
     - name: Publish binary distributions to PyPI
       if: github.ref == 'refs/heads/master'
       #if: github.event_name == 'release' && github.event.action == 'created' 
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         skip-existing: true
         password: ${{ secrets.PYPI_API_TOKEN }}
         packages-dir: ngstents/wheelhouse/
 
   docs:
     needs: [publish-pypi]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # otherwise, you will failed to push refs to dest repo
           submodules: 'True'
           path: 'ngstents'
       - name: apt-get
         run: sudo apt-get update && DEBIAN_FRONTEND="noninteractive" sudo apt-get -y install libxmu-dev tk-dev tcl-dev git libglu1-mesa-dev libblas-dev liblapack-dev python3 python3-pip python3-distutils python3-tk libpython3-dev python3-testresources npm nodejs pandoc -y
       - name: pip install requirements
```

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip.ps1`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 if (test-path dist) {
     cmd.exe /c rd /s /q dist
 }
 if (test-path venv_ngs) {
     cmd.exe /c rd /s /q venv_ngs
 }
 
-pip3 install scikit-build wheel numpy twine mkl-devel==2022.* mkl==2022.*
-pip3 install ngsolve
+Set-Location ../..
+python.exe -m venv .\venv_ngs
+.\venv_ngs\scripts\Activate.ps1
+$env:PATH += Join-Path ";" (Get-Item .).FullName "venv_ngs\bin"
 
-$env:NGSolve_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\ngsolve\cmake"
-$env:Netgen_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\netgen\cmake"
+pip3 install scikit-build wheel numpy twine mkl-devel==2022.* mkl==2022.* setuptools==69.5.1 setuptools_scm==8.1.0
+pip3 install -r .github/workflows/ngsolve_version.txt
+
+#$env:NGSolve_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\ngsolve\cmake"
+#$env:Netgen_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\netgen\cmake"
 
-Set-Location ../..
 python setup.py bdist_wheel -G"Visual Studio 16 2019" -d wheelhouse
```

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip.sh`

 * *Files 23% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 rm -rf wheelhouse
 mkdir wheelhouse
 
 git config --global --add safe.directory '*'
 
 export ORIGINAL_PATH="$PATH"
 
-for pyversion in 38 39 310 311
+for pyversion in 38 39 310 311 312
 do
     export PYDIR="/opt/python/cp${pyversion}-cp${pyversion}/bin"
     export PATH="$ORIGINAL_PATH:$PYDIR"
 
     rm -rf _skbuild
-    $PYDIR/pip install pytest-check numpy wheel scikit-build mkl==2023.* mkl-devel==2023.* setuptools
-    $PYDIR/pip install ngsolve 
+    $PYDIR/pip install pytest-check numpy wheel scikit-build mkl==2023.* mkl-devel==2023.* setuptools==69.5.1 setuptools_scm==8.1.0
+    $PYDIR/pip install -r ./.github/workflows/ngsolve_version.txt
 
     $PYDIR/pip wheel -vvv .
     rename linux_ manylinux_2_17_x86_64.manylinux2014_ ngstents*.whl
     mv ngstents*.whl wheelhouse/
     rm -rf *.whl
-    $PYDIR/pip uninstall -y ngsolve netgen-mesher setuptools pytest-check numpy wheel scikit-build mkl mkl-devel 
+    $PYDIR/pip uninstall -y ngsolve netgen-mesher setuptools setuptools_scm pytest-check numpy wheel scikit-build mkl mkl-devel 
 done
```

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh`

 * *Files 12% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 
 $PYDIR/python3 --version
 
 export PATH=/Applications/CMake.app/Contents/bin:$PATH
 export NETGEN_Dir=$PYDIR/../lib/python$1/site-packages/netgen/cmake
 export NGSolve_Dir=$PYDIR/../lib/python$1/site-packages/ngsolve/cmake
 export CMAKE_PREFIX_PATH=$CMAKE_PREFIX_PATH:$NGSolve_Dir:$NETGEN_Dir
-$PYDIR/pip3 install scikit-build wheel
+$PYDIR/pip3 install scikit-build wheel setuptools==69.5.1 setuptools_scm==8.1.0
 
 export CMAKE_OSX_ARCHITECTURES='arm64;x86_64'
-$PYDIR/pip3 install ngsolve
+$PYDIR/pip3 install -r ./.github/workflows/ngsolve_version.txt
 
 $PYDIR/python3 setup.py bdist_wheel --plat-name macosx-10.15-universal2 -d wheelhouse
```

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/README.md` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 ## Install
 
 Binary installers are available for linux, mac, and windows (with
 python >= 3.9).
 
 * `pip install ngstents`
 
+But note that the binaries are not generally kept up to date. The
+recommended option is to build from source (see below).
 
 ## Build
 
 If you built NGSolve from source, you can build and install `ngstents`.
 After cloning this repository, compile  the c++ code here and install:
 
 * `cd src`
```

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/advection2d.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/advection2d_periodic.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/advection2d_periodic.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/burgers1d.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/burgers1d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/burgers2d.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/burgers2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/euler2d.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/euler2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/maxwell/maxwell3d.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/maxwell/maxwell3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/draw3dtent.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/draw3dtent.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/draw3dvertex.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/draw3dvertex.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/horn.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/horn.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave2d.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave3d.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/BurgersMTP.ipynb` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/BurgersMTP.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/INDEX.ipynb` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/INDEX.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/StartPitching.ipynb` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/StartPitching.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/conf.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/CausalityCond.png` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/CausalityCond.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/dag.png` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/dag.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/map.png` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/map.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/subtents.png` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/subtents.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/index.rst` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/requirements.txt` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/conslaw/__init__.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/conslaw/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/_drawtents.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/_drawtents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/_drawtents2d.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/_drawtents2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/advection.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/advection.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/burgers.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/burgers.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/concurrentqueue.h` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/concurrentqueue.h`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/conservationlaw.hpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/conservationlaw.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/euler.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/euler.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/maxwell.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/maxwell.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/paralleldepend.hpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/paralleldepend.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/python_conslaw.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/python_conslaw.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/python_tents.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/python_tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/symbolic.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/symbolic.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tents.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tents.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -561,15 +561,15 @@
     }
   return std::make_tuple(v2v, v2e);
 }
 
 // Get the periodic vertex associated with a primary vertex in periodic case
 void TentSlabPitcher::GetVertexElements(int vnr_main, Array<int> & elems) const
 {
-  ma->GetVertexElements (vnr_main, elems);
+  elems = ma->GetVertexElements(vnr_main); 
   if(per_verts[vnr_main].Size()==0)
     return;
   else
     {
       for(auto per_v : per_verts[vnr_main])
         for(auto elnr : ma->GetVertexElements(per_v))
           elems.Append(elnr);
```

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tents.hpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tents.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 /// the tentpole as an edge.
 ///
 /// We represent the tent by its projection on space (a vertex patch),
 /// the central vertex, and the heights (times) of its neighboring
 /// vertices.
 ///
 
+
 class NGSTENT_API Tent {
 
 public:
   Tent(const Array<int> &avmap) : vmap(avmap){}
   Tent() = delete;
   int vertex;                 ///< central vertex
   double tbot, ttop;          ///< bottom and top times of central vertex
```

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tentsolver.hpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tentsolver.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tentsolver_impl.hpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tentsolver_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/vis3d.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/vis3d.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/vis3d.hpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/vis3d.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/wave.cpp` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/wave.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_burgers_2D.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_burgers_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_causal_tents.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_causal_tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_conslaw.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_conslaw.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_tent_height_2D.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_tent_height_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_tentlayers.py` & `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_tentlayers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/setup.py` & `ngstrefftz-0.3.2402.dev35/setup.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/CMakeLists.txt` & `ngstrefftz-0.3.2402.dev35/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/__init__.py` & `ngstrefftz-0.3.2402.dev35/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/airy.cpp` & `ngstrefftz-0.3.2402.dev35/src/airy.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/condensedg.cpp` & `ngstrefftz-0.3.2402.dev35/src/condensedg.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/condensedg.hpp` & `ngstrefftz-0.3.2402.dev35/src/condensedg.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/diffopmapped.hpp` & `ngstrefftz-0.3.2402.dev35/src/diffopmapped.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/embtrefftz.cpp` & `ngstrefftz-0.3.2402.dev35/src/embtrefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/embtrefftz.hpp` & `ngstrefftz-0.3.2402.dev35/src/embtrefftz.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/mesh1dtents.cpp` & `ngstrefftz-0.3.2402.dev35/src/mesh1dtents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/monomialfespace.cpp` & `ngstrefftz-0.3.2402.dev35/src/monomialfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/monomialfespace.hpp` & `ngstrefftz-0.3.2402.dev35/src/monomialfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/PKG-INFO` & `ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2402.dev34
+Version: 0.3.2402.dev35
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
-Requires-Dist: ngsolve>=6.2.2401.post24.dev0
+Requires-Dist: ngsolve>=6.2.2402
 Requires-Dist: ngstents>=0.0.2.dev39
 Requires-Dist: mkl
 
 NGSTrefftz provides a framework to implement Trefftz finite element spaces for NGSolve, with several Trefftz spaces already implemented. Additionally, Trefftz-DG on tent-pitched meshes for the acoustic wave equation is implemented using meshes provided by ngstents. Furthermore, the package includes an implementation of the embedded Trefftz method.
```

### Comparing `ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/SOURCES.txt` & `ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 external_dependencies/ngstents/README.md
 external_dependencies/ngstents/setup.py
 external_dependencies/ngstents/.github/workflows/build.yml
 external_dependencies/ngstents/.github/workflows/build_pip.ps1
 external_dependencies/ngstents/.github/workflows/build_pip.sh
 external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
 external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
+external_dependencies/ngstents/.github/workflows/ngsolve_version.txt
 external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
 external_dependencies/ngstents/demo/advection/advection2d.py
 external_dependencies/ngstents/demo/advection/advection2d_periodic.py
 external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
 external_dependencies/ngstents/demo/burgers/burgers1d.py
 external_dependencies/ngstents/demo/burgers/burgers2d.py
 external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
```

### Comparing `ngstrefftz-0.3.2402.dev34/src/planewavefe.cpp` & `ngstrefftz-0.3.2402.dev35/src/planewavefe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/planewavefe.hpp` & `ngstrefftz-0.3.2402.dev35/src/planewavefe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/python_trefftz.cpp` & `ngstrefftz-0.3.2402.dev35/src/python_trefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/scalarmappedfe.cpp` & `ngstrefftz-0.3.2402.dev35/src/scalarmappedfe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/scalarmappedfe.hpp` & `ngstrefftz-0.3.2402.dev35/src/scalarmappedfe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/specialcoefficientfunction.cpp` & `ngstrefftz-0.3.2402.dev35/src/specialcoefficientfunction.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/specialcoefficientfunction.hpp` & `ngstrefftz-0.3.2402.dev35/src/specialcoefficientfunction.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/specialintegrator.cpp` & `ngstrefftz-0.3.2402.dev35/src/specialintegrator.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/specialintegrator.hpp` & `ngstrefftz-0.3.2402.dev35/src/specialintegrator.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/trefftzfespace.cpp` & `ngstrefftz-0.3.2402.dev35/src/trefftzfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/trefftzfespace.hpp` & `ngstrefftz-0.3.2402.dev35/src/trefftzfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/twavetents.cpp` & `ngstrefftz-0.3.2402.dev35/src/twavetents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/src/twavetents.hpp` & `ngstrefftz-0.3.2402.dev35/src/twavetents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/test/dg.py` & `ngstrefftz-0.3.2402.dev35/test/dg.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/test/embt.py` & `ngstrefftz-0.3.2402.dev35/test/embt.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/test/tents.py` & `ngstrefftz-0.3.2402.dev35/test/tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev34/test/trefftz.py` & `ngstrefftz-0.3.2402.dev35/test/trefftz.py`

 * *Files identical despite different names*

