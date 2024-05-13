# Comparing `tmp/pqanalysis-0.5.2.tar.gz` & `tmp/pqanalysis-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqanalysis-0.5.2.tar", last modified: Mon Apr 22 06:38:42 2024, max compression
+gzip compressed data, was "pqanalysis-1.0.tar", last modified: Mon May 13 05:26:43 2024, max compression
```

## Comparing `pqanalysis-0.5.2.tar` & `pqanalysis-1.0.tar`

### file list

```diff
@@ -1,173 +1,457 @@
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.264764 pqanalysis-0.5.2/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.231430 pqanalysis-0.5.2/.github/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/.github/workflows/
--rw-r--r--   0 jag       (1000) jag       (1000)      743 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/.github/workflows/ci.yml
--rw-r--r--   0 jag       (1000) jag       (1000)     1502 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/.github/workflows/docs.yml
--rw-r--r--   0 jag       (1000) jag       (1000)      116 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/.gitignore
--rw-r--r--   0 jag       (1000) jag       (1000)     1113 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/LICENSE
--rw-r--r--   0 jag       (1000) jag       (1000)     2290 2024-04-22 06:38:42.264764 pqanalysis-0.5.2/PKG-INFO
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/PQAnalysis/
--rw-r--r--   0 jag       (1000) jag       (1000)       73 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)      411 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis/_version.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/PQAnalysis/cli/
--rw-r--r--   0 jag       (1000) jag       (1000)       49 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/cli/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1590 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/cli/rst2xyz.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2578 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/cli/traj2box.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1692 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/cli/traj2qmcfc.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/PQAnalysis/core/
--rw-r--r--   0 jag       (1000) jag       (1000)      333 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)    12233 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atom.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/
--rw-r--r--   0 jag       (1000) jag       (1000)       39 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1411 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_decorators.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4022 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_indexing.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4152 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_positions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2848 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_properties.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2395 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_standardProperties.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6197 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/atomicSystem.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6333 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/cell.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1322 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/exceptions.py
--rw-r--r--   0 jag       (1000) jag       (1000)      364 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/exceptions.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/io/
--rw-r--r--   0 jag       (1000) jag       (1000)      709 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3443 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/base.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6671 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/boxWriter.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4459 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/energyFileReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2145 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/exceptions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     8914 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/frameReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4615 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/infoFileReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3660 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/moldescriptorReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6692 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/restartReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3606 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/restartWriter.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4985 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/trajectoryReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     9028 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/trajectoryWriter.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/physicalData/
--rw-r--r--   0 jag       (1000) jag       (1000)       64 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/physicalData/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     7888 2024-04-22 06:35:44.000000 pqanalysis-0.5.2/PQAnalysis/physicalData/energy.py
--rw-r--r--   0 jag       (1000) jag       (1000)      435 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/physicalData/exceptions.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/tools/
--rw-r--r--   0 jag       (1000) jag       (1000)       47 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/tools/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1360 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/tools/traj_to_com_traj.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/topology/
--rw-r--r--   0 jag       (1000) jag       (1000)       98 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)      435 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/exceptions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6971 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/molType.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6251 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/shakeTopology.py
--rw-r--r--   0 jag       (1000) jag       (1000)      285 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/topology.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/traj/
--rw-r--r--   0 jag       (1000) jag       (1000)      241 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1919 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/exceptions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3025 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/formats.py
--rw-r--r--   0 jag       (1000) jag       (1000)     5860 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/frame.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4114 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/trajectory.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1324 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/types.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/utils/
--rw-r--r--   0 jag       (1000) jag       (1000)      108 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/utils/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1313 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/utils/common.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1358 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/utils/decorators.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/PQAnalysis.egg-info/
--rw-r--r--   0 jag       (1000) jag       (1000)     2290 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 jag       (1000) jag       (1000)     4115 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 jag       (1000) jag       (1000)        1 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 jag       (1000) jag       (1000)      140 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 jag       (1000) jag       (1000)      121 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/requires.txt
--rw-r--r--   0 jag       (1000) jag       (1000)       11 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/top_level.txt
--rw-r--r--   0 jag       (1000) jag       (1000)     1223 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/README.md
--rw-r--r--   0 jag       (1000) jag       (1000)       50 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/codecov.yml
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/docs/
--rw-r--r--   0 jag       (1000) jag       (1000)      638 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/docs/Makefile
--rw-r--r--   0 jag       (1000) jag       (1000)      804 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/docs/make.bat
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/docs/source/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.244764 pqanalysis-0.5.2/docs/source/code/
--rw-r--r--   0 jag       (1000) jag       (1000)      510 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.cli.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      823 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.core.rst
--rw-r--r--   0 jag       (1000) jag       (1000)     1196 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.io.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      394 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.physicalData.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      349 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      388 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.tools.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      510 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.traj.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      853 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.utils.rst
--rw-r--r--   0 jag       (1000) jag       (1000)       67 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/modules.rst
--rw-r--r--   0 jag       (1000) jag       (1000)     2418 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/conf.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.244764 pqanalysis-0.5.2/docs/source/developerGuide/
--rw-r--r--   0 jag       (1000) jag       (1000)     1721 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/docs/source/developerGuide/developerGuide.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      377 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/index.rst
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.244764 pqanalysis-0.5.2/docs/source/logo/
--rw-r--r--   0 jag       (1000) jag       (1000)   204575 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/docs/source/logo/PQAnalysis.png
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.234764 pqanalysis-0.5.2/examples/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.248097 pqanalysis-0.5.2/examples/traj2box/
--rw-r--r--   0 jag       (1000) jag       (1000)       17 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/examples/traj2box/.gitignore
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/examples/traj2box/acof_triclinic.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/examples/traj2box/acof_triclinic_2.xyz
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.248097 pqanalysis-0.5.2/examples/traj2comtraj/
--rw-r--r--   0 jag       (1000) jag       (1000)  2600700 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/examples/traj2comtraj/umcm-9-md-01.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)     1247 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/pyproject.toml
--rw-r--r--   0 jag       (1000) jag       (1000)      131 2024-04-22 06:38:42.264764 pqanalysis-0.5.2/setup.cfg
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.251431 pqanalysis-0.5.2/tests/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/__init__.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.251431 pqanalysis-0.5.2/tests/cli/
--rw-r--r--   0 jag       (1000) jag       (1000)     1136 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/cli/test_rst2xyz.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1458 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/cli/test_traj2box.py
--rw-r--r--   0 jag       (1000) jag       (1000)      951 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/cli/test_traj2qmcfc.py
--rw-r--r--   0 jag       (1000) jag       (1000)      646 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/conftest.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.251431 pqanalysis-0.5.2/tests/core/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/__init__.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/core/atomicSystem/
--rw-r--r--   0 jag       (1000) jag       (1000)     5895 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/atomicSystem/test_atomicSystem.py
--rw-r--r--   0 jag       (1000) jag       (1000)      687 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/atomicSystem/test_indexing.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2486 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/atomicSystem/test_positions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2657 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/test_atom.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2889 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/test_cell.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.234764 pqanalysis-0.5.2/tests/data/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/readEnergyFile/
--rw-r--r--   0 jag       (1000) jag       (1000)      481 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readEnergyFile/md-01.en
--rw-r--r--   0 jag       (1000) jag       (1000)      901 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/readEnergyFile/md-01.info
--rw-r--r--   0 jag       (1000) jag       (1000)      468 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readEnergyFile/md-01_noinfo.en
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/readInfoFile/
--rw-r--r--   0 jag       (1000) jag       (1000)      901 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/readInfoFile/md-01.info
--rw-r--r--   0 jag       (1000) jag       (1000)      982 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readInfoFile/md-01.qmcfc.info
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/readMoldescriptor/
--rw-r--r--   0 jag       (1000) jag       (1000)      424 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readMoldescriptor/moldescriptor.dat
--rw-r--r--   0 jag       (1000) jag       (1000)      418 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readMoldescriptor/moldescriptor_withError.dat
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/readRestartFile/
--rw-r--r--   0 jag       (1000) jag       (1000)      322 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readRestartFile/md-01.rst
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/rst2xyz/
--rw-r--r--   0 jag       (1000) jag       (1000)      322 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/rst2xyz/md-01.rst
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.258098 pqanalysis-0.5.2/tests/data/traj2box/
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2box/acof_triclinic.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2box/acof_triclinic_2.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)     8632 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2box/box.dat
--rw-r--r--   0 jag       (1000) jag       (1000)    88940 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2box/box.vmd.xyz
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.258098 pqanalysis-0.5.2/tests/data/traj2qmcfc/
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/traj2qmcfc/acof_triclinic.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/traj2qmcfc/acof_triclinic_2.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)  1575832 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2qmcfc/traj.qmcfc.xyz
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/io/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2796 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_base.py
--rw-r--r--   0 jag       (1000) jag       (1000)     5394 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_boxWriter.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4943 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_energyFileReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4794 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_frameReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3661 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_infoFileReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3034 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_moldescriptorReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4077 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_restartReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3566 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_restartWriter.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2869 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_trajectoryReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     5870 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_trajectoryWriter.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/physicalData/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/physicalData/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1995 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/physicalData/test_energy.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/tools/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/tools/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2335 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/tools/test_traj_to_com_traj.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/topology/
--rw-r--r--   0 jag       (1000) jag       (1000)     2822 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/topology/test_molType.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3607 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/topology/test_shakeTopology.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/traj/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/traj/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3000 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/traj/test_frame.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3510 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/traj/test_trajectory.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/utils/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/utils/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1221 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/utils/test_common.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1295 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/utils/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.147878 pqanalysis-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-13 05:26:28.000000 pqanalysis-1.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 05:26:28.000000 pqanalysis-1.0/.docstr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.059877 pqanalysis-1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.067878 pqanalysis-1.0/.github/.pylint_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-13 05:26:28.000000 pqanalysis-1.0/.github/.pylint_cache/PQAnalysis_1.stats
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.067878 pqanalysis-1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 05:26:28.000000 pqanalysis-1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-13 05:26:28.000000 pqanalysis-1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.067878 pqanalysis-1.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-13 05:26:28.000000 pqanalysis-1.0/.github/scripts/parse_pylint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.067878 pqanalysis-1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-13 05:26:28.000000 pqanalysis-1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-13 05:26:28.000000 pqanalysis-1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-13 05:26:28.000000 pqanalysis-1.0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-13 05:26:28.000000 pqanalysis-1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 05:26:28.000000 pqanalysis-1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-13 05:26:28.000000 pqanalysis-1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 05:26:28.000000 pqanalysis-1.0/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-13 05:26:28.000000 pqanalysis-1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-13 05:26:28.000000 pqanalysis-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-13 05:26:43.147878 pqanalysis-1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.071878 pqanalysis-1.0/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-13 05:26:42.000000 pqanalysis-1.0/PQAnalysis/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.071878 pqanalysis-1.0/PQAnalysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.071878 pqanalysis-1.0/PQAnalysis/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/analysis/rdf/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/analysis/rdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/analysis/rdf/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.071878 pqanalysis-1.0/PQAnalysis/atomic_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/atomic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/atomic_system/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/atomic_system/_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/atomic_system/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/atomic_system/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/atomic_system/atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/atomic_system/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.075878 pqanalysis-1.0/PQAnalysis/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/build_nep_traj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/gen2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/cli/xyz2gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.075878 pqanalysis-1.0/PQAnalysis/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.075878 pqanalysis-1.0/PQAnalysis/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/atom/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/atom/element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.075878 pqanalysis-1.0/PQAnalysis/core/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/cell/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/cell/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/core/residue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.079878 pqanalysis-1.0/PQAnalysis/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/grammar/PQ_inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/grammar/inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/grammar/rules.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/grammar/selection.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/grammar/terminals.lark
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.079878 pqanalysis-1.0/PQAnalysis/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/box_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/conversion_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/energy_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.079878 pqanalysis-1.0/PQAnalysis/io/gen_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/gen_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/gen_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/gen_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/gen_file/gen_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/gen_file/gen_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/info_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.079878 pqanalysis-1.0/PQAnalysis/io/input_file_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17600 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/input_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.083878 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq/output_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.083878 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/moldescriptor_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.083878 pqanalysis-1.0/PQAnalysis/io/nep/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/nep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/nep/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37420 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/nep/nep_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.083878 pqanalysis-1.0/PQAnalysis/io/restart_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/restart_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/restart_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/restart_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/restart_file/restart_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/restart_file/restart_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.083878 pqanalysis-1.0/PQAnalysis/io/topology_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/topology_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/topology_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/topology_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/topology_file/topology_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/topology_file/topology_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.087878 pqanalysis-1.0/PQAnalysis/io/traj_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/traj_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/traj_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/traj_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12689 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/traj_file/frame_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/traj_file/trajectory_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/traj_file/trajectory_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.087878 pqanalysis-1.0/PQAnalysis/io/virial/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/virial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/virial/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/virial/virial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/io/write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.087878 pqanalysis-1.0/PQAnalysis/physical_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/physical_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/physical_data/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/physical_data/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.087878 pqanalysis-1.0/PQAnalysis/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/tools/add_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/tools/traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.087878 pqanalysis-1.0/PQAnalysis/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.087878 pqanalysis-1.0/PQAnalysis/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/bonded_topology/_topology_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/bonded_topology/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/bonded_topology/bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/bonded_topology/bonded_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/bonded_topology/dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/shake_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18093 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/topology/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.091878 pqanalysis-1.0/PQAnalysis/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/traj/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/traj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/traj/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/traj/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.091878 pqanalysis-1.0/PQAnalysis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/utils/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-13 05:26:28.000000 pqanalysis-1.0/PQAnalysis/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.147878 pqanalysis-1.0/PQAnalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-13 05:26:42.000000 pqanalysis-1.0/PQAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15038 2024-05-13 05:26:43.000000 pqanalysis-1.0/PQAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:42.000000 pqanalysis-1.0/PQAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-13 05:26:42.000000 pqanalysis-1.0/PQAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-13 05:26:42.000000 pqanalysis-1.0/PQAnalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 05:26:42.000000 pqanalysis-1.0/PQAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-13 05:26:28.000000 pqanalysis-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.091878 pqanalysis-1.0/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.091878 pqanalysis-1.0/benchmarks/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-13 05:26:28.000000 pqanalysis-1.0/benchmarks/core/benchmark_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 05:26:28.000000 pqanalysis-1.0/benchmarks/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.091878 pqanalysis-1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/autodoc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.091878 pqanalysis-1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.059877 pqanalysis-1.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.091878 pqanalysis-1.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.091878 pqanalysis-1.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/_templates/package.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.115878 pqanalysis-1.0/docs/source/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.analysis.rdf.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.analysis.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.add_molecules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.continue_input.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.gen2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.rst2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.traj2box.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.cli.xyz2gen.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.core.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.core.atom.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.core.atom.element.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.core.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.core.cell.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.core.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.core.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.core.residue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.box_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.conversion_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.energy_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.gen_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.gen_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.info_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.nep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.restart_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.restart_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.topology_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.topology_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.traj_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.traj_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.virial.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.virial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.io.write_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.physical_data.energy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.physical_data.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.physical_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.tools.add_molecule.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.shake_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.topology.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.traj.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.traj.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.traj.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.traj.trajectory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.type_checking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.utils.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.utils.custom_logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.utils.decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.utils.files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.utils.random.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/PQAnalysis.utils.units.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/code/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.115878 pqanalysis-1.0/docs/source/developerGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/developerGuide/developerGuide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.115878 pqanalysis-1.0/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/logo/PQAnalysis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.115878 pqanalysis-1.0/docs/source/userGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/userGuide/inputFile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-13 05:26:28.000000 pqanalysis-1.0/docs/source/userGuide/userGuide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.063877 pqanalysis-1.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.115878 pqanalysis-1.0/examples/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 05:26:28.000000 pqanalysis-1.0/examples/traj2box/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-13 05:26:28.000000 pqanalysis-1.0/examples/traj2box/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-13 05:26:28.000000 pqanalysis-1.0/examples/traj2box/acof_triclinic_2.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.119878 pqanalysis-1.0/examples/traj2comtraj/
+-rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-13 05:26:28.000000 pqanalysis-1.0/examples/traj2comtraj/umcm-9-md-01.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 05:26:28.000000 pqanalysis-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-13 05:26:28.000000 pqanalysis-1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-13 05:26:28.000000 pqanalysis-1.0/pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-13 05:26:43.147878 pqanalysis-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    29303 2024-05-13 05:26:28.000000 pqanalysis-1.0/test
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.123878 pqanalysis-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.123878 pqanalysis-1.0/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.123878 pqanalysis-1.0/tests/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/analysis/rdf/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/analysis/rdf/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/analysis/rdf/test_rdfInputFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/analysis/rdf/test_rdfOutputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.123878 pqanalysis-1.0/tests/atomicSystem/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/atomicSystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23524 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/atomicSystem/test_atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/atomicSystem/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/atomicSystem/test_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.123878 pqanalysis-1.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/cli/test_continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/cli/test_rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/cli/test_traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/cli/test_traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.127878 pqanalysis-1.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.127878 pqanalysis-1.0/tests/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/core/atom/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/core/atom/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/core/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/core/test_residue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.063877 pqanalysis-1.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.127878 pqanalysis-1.0/tests/data/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.127878 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/n_not_matching.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/no_output_files.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/no_start_file.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/run-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/run-09.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/run-10.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/inputFileReader/input_PQ.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.127878 pqanalysis-1.0/tests/data/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/rdf/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/rdf/required_keys_not_given.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.131878 pqanalysis-1.0/tests/data/readEnergyFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/readEnergyFile/md-01.en
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/readEnergyFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/readEnergyFile/md-01_noinfo.en
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.131878 pqanalysis-1.0/tests/data/readInfoFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/readInfoFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/readInfoFile/md-01.qmcfc.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.131878 pqanalysis-1.0/tests/data/readMoldescriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/readMoldescriptor/moldescriptor.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/readMoldescriptor/moldescriptor_withError.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.131878 pqanalysis-1.0/tests/data/readRestartFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/readRestartFile/md-01.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/readRestartFile/moldescriptor.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.131878 pqanalysis-1.0/tests/data/rst2xyz/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/rst2xyz/md-01.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.131878 pqanalysis-1.0/tests/data/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/traj2box/box.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/traj2box/box.vmd.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/traj2box/test.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.135878 pqanalysis-1.0/tests/data/traj2qmcfc/
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/traj2qmcfc/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/traj2qmcfc/acof_triclinic_2.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/data/traj2qmcfc/traj.qmcfc.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.139878 pqanalysis-1.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.139878 pqanalysis-1.0/tests/io/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.143878 pqanalysis-1.0/tests/io/inputFileReader/PQ/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/inputFileReader/PQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.143878 pqanalysis-1.0/tests/io/inputFileReader/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/inputFileReader/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/inputFileReader/PQAnalysis/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/inputFileReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/inputFileReader/test_inputDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/inputFileReader/test_inputFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/inputFileReader/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/inputFileReader/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_boxWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_energyFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_frameReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_infoFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_moldescriptorReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_restartReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_restartWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_trajectoryReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_trajectoryWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/io/test_write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.143878 pqanalysis-1.0/tests/physicalData/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/physicalData/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/physicalData/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/test_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.143878 pqanalysis-1.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/tools/test_traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.143878 pqanalysis-1.0/tests/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.143878 pqanalysis-1.0/tests/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/bonded_topology/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/bonded_topology/test_bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/bonded_topology/test_bondedTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/bonded_topology/test_dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/test_selectionTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/test_shakeTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/topology/test_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.143878 pqanalysis-1.0/tests/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/traj/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/traj/test_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 05:26:43.147878 pqanalysis-1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/utils/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-13 05:26:28.000000 pqanalysis-1.0/tests/utils/test_decorators.py
```

### Comparing `pqanalysis-0.5.2/.github/workflows/ci.yml` & `pqanalysis-1.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-name: CI
+name: Test Coverage
 
 on:
   push:
-    branches: [main]
+    branches: 
+      - main
+      - dev
+  pull_request:
+    branches:
+      - '*'
   workflow_dispatch:
 
 jobs:
   build:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@master
     - name: Setup Python
-      uses: actions/setup-python@master
+      uses: actions/setup-python@v2
       with:
-        python-version: '3.10'
+        python-version: 3.x
 
     - name: build PQAnalysis
       run: |
         pip install .[test]
 
     - name: Generate coverage report
       run: |
-        pip install pytest
-        pip install pytest-cov
-        python -m pytest --cov=PQAnalysis --cov-report=xml
+        bash pytest.sh
+      shell: bash
 
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         env_vars: OS,PYTHON
         fail_ci_if_error: true
```

### Comparing `pqanalysis-0.5.2/LICENSE` & `pqanalysis-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/PQAnalysis/cli/traj2box.py` & `pqanalysis-1.0/PQAnalysis/cli/traj2box.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,108 @@
 """
+.. _cli.traj2box:
+
+Command Line Tool for Converting Trajectory Files to Box Files
+--------------------------------------------------------------
+
+"""
+
+from PQAnalysis.config import code_base_url
+from PQAnalysis.io import traj2box
+from ._argument_parser import _ArgumentParser
+from ._cli_base import CLIBase
+
+__outputdoc__ = """
+
 Converts multiple trajectory files to a box file.
 
 Without the --vmd option the output is printed in a data file format.
 The first column represents the step starting from 1, the second to fourth column
 represent the box vectors a, b, c, the fifth to seventh column represent the box angles.
 
 With the --vmd option the output is printed in a VMD file format. Meaning the output is
 in xyz format with 8 particle entries representing the vertices of the box. The comment
 line contains the information about the box dimensions a, b and c and the box angles.
 """
 
-import argparse
+__epilog__ = "\n"
+__epilog__ += "For more information on the VMD file format please visit "
+__epilog__ += f"{code_base_url}PQAnalysis.io.formats.html#PQAnalysis.io.formats.VMDFileFormat."
+__epilog__ += "\n"
+__epilog__ += "\n"
 
-from beartype.typing import List
+__doc__ += __outputdoc__
 
-from ..io import BoxWriter, TrajectoryReader
 
 
-def main():
+class Traj2BoxCLI(CLIBase):
+
     """
-    Wrapper for the command line interface of traj2box.
+    Command Line Tool for Converting Trajectory Files to Box Files
     """
-    parser = argparse.ArgumentParser(description=__doc__)
-    parser.add_argument('trajectory_file', type=str, nargs='+',
-                        help='The trajectory file(s) to be converted.')
-    parser.add_argument('-v', '--vmd', action='store_true',
-                        help='Output in VMD format.')
-    parser.add_argument('-o', '--output', type=str, default=None,
-                        help='The output file. If not specified, the output is printed to stdout.')
-    args = parser.parse_args()
 
-    traj2box(args.trajectory_file, args.vmd, args.output)
+    @classmethod
+    def program_name(cls) -> str:
+        """
+        Returns the name of the program.
+
+        Returns
+        -------
+        str
+            The name of the program.
+        """
+        return 'traj2box'
+
+    @classmethod
+    def add_arguments(cls, parser: _ArgumentParser) -> None:
+        """
+        Adds the arguments to the parser.
+
+        Parameters
+        ----------
+        parser : _ArgumentParser
+            The parser to which the arguments should be added.
+        """
+        parser.parse_output_file()
+
+        parser.add_argument(
+            'trajectory_file',
+            type=str,
+            nargs='+',
+            help='The trajectory file(s) to be converted.'
+        )
+
+        parser.add_argument(
+            '--vmd',
+            action='store_true',
+            help='Output in VMD format.'
+        )
+
+        parser.parse_mode()
+
+    @classmethod
+    def run(cls, args):
+        """
+        Runs the command line tool.
+
+        Parameters
+        ----------
+        args : argparse.Namespace
+            The arguments parsed by the parser.
+        """
+        traj2box(args.trajectory_file, args.vmd, args.output, args.mode)
 
 
-def traj2box(trajectory_files: List[str], vmd: bool, output: str | None = None) -> None:
-    """
-    Converts multiple trajectory files to a box file.
 
-    Without the --vmd option the output is printed in a data file format.
-    The first column represents the step starting from 1, the second to fourth column
-    represent the box vectors a, b, c, the fifth to seventh column represent the box angles.
-
-    With the --vmd option the output is printed in a VMD file format. Meaning the output is
-    in xyz format with 8 particle entries representing the vertices of the box. The comment
-    line contains the information about the box dimensions a, b and c and the box angles.
-
-    Parameters
-    ----------
-    trajectory_file : list of str
-        The trajectory file(s) to be converted.
-    vmd : bool
-        Output in VMD format.
-    output : str, optional
-        The output file. If not specified, the output is printed to stdout.
+def main():
     """
+    Main function of the traj2box command line tool, which is basically just a 
+    wrapper for the traj2box function. For more information on the traj2box
+    function please visit :py:func:`PQAnalysis.io.api.traj2box`.
+    """
+    parser = _ArgumentParser(description=__outputdoc__, epilog=__epilog__)
+
+    Traj2BoxCLI.add_arguments(parser)
 
-    if vmd:
-        output_format = "vmd"
-    else:
-        output_format = None
-
-    writer = BoxWriter(filename=output, format=output_format)
-    for filename in trajectory_files:
-        reader = TrajectoryReader(filename)
-        trajectory = reader.read()
+    args = parser.parse_args()
 
-        writer.write(trajectory, reset_counter=False)
+    Traj2BoxCLI.run(args)
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_positions.py` & `pqanalysis-1.0/PQAnalysis/atomic_system/_positions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,163 @@
 """
 A module containing a Mixin class for related information to the positions of an atomic system.
-
-...
-
-Classes
--------
-_PositionsMixin
-    A mixin class containing methods for related information to the positions of an atomic system.
 """
 
 import numpy as np
 
-from multimethod import multimethod
-from beartype.typing import List, Tuple
-from beartype.door import is_bearable
+from beartype.typing import Tuple
+
+from PQAnalysis.core import distance
+from PQAnalysis.topology import SelectionCompatible, Selection
+from PQAnalysis.type_checking import runtime_type_checking
+from PQAnalysis.types import (
+    Np2DIntArray,
+    Np2DNumberArray,
+    Np1DIntArray,
+    PositiveInt,
+    Np1DNumberArray
+)
 
 from ._decorators import check_atoms_pos
 
-from ..atom import Atom
-from ...types import Np2DIntArray, Np2DNumberArray, Np1DIntArray
 
 
 class _PositionsMixin:
+
     """
-    A mixin class containing methods for related information to the positions of an atomic system.
+    A mixin class containing methods for related 
+    information to the positions of an atomic system.
     """
 
     @check_atoms_pos
-    def _nearest_neighbours(self,
-                            n: int = 1,
-                            indices: Np1DIntArray | None = None
-                            ) -> Tuple[Np2DIntArray, Np2DNumberArray]:
+    def _nearest_neighbours(
+        self,
+        n: PositiveInt = 1,
+        indices: Np1DIntArray | None = None
+    ) -> Tuple[Np2DIntArray,
+        Np2DNumberArray]:
         """
-        Returns the n nearest neighbours of each atom in the system.
+        Returns the 'n' nearest neighbours of selected atoms in the system.
+
+        If no indices are given, the 'n' nearest neighbours of all atoms are returned.
+        With the parameter 'n' the number of nearest neighbours can be specified.
 
         Parameters
         ----------
-        n : int, optional
+        n : PositiveInt, optional
             The number of nearest neighbours to return, by default 1
+        indices : Np1DIntArray, optional
+            The indices of the atoms to get the nearest neighbours of,
+            by default None (all atoms)
 
         Returns
         -------
         nearest_neighbours : Np2DIntArray
-            The n nearest neighbours of each atom in the system.
+            The n nearest neighbour indices of each atom in the system.
         nearest_neighbours_distances : Np2DNumberArray
             The distances to the n nearest neighbours of each atom in the system.
-        indices : Np1DIntArray, optional
-            The indices of the atoms to get the nearest neighbours of, by default None (all atoms)
         """
 
-        if indices is None:
-            indices = np.arange(self.n_atoms)
+        indices = np.arange(self.n_atoms) if indices is None else indices
 
         nearest_neighbours = []
         nearest_neighbours_distances = []
 
-        for atom_position in self.pos[indices]:
-            delta_pos = self.pos - atom_position
-
-            delta_pos = self.cell.image(delta_pos)
-
-            distances = np.linalg.norm(delta_pos, axis=1)
-
-            nearest_neighbours_atom = np.argsort(distances)[1:n+1]
-
-            nearest_neighbours.append(nearest_neighbours_atom)
-            nearest_neighbours_distances.append(
-                distances[nearest_neighbours_atom])
-
-        return np.array(nearest_neighbours), np.array(nearest_neighbours_distances)
+        distances = distance(self.pos[indices], self.pos, self.cell)
 
-    def nearest_neighbours(self,
-                           n: int = 1,
-                           atoms: List[Atom] | List[str] | Np1DIntArray | None = None,
-                           use_full_atom_info: bool = False
-                           ) -> Tuple[Np2DIntArray, Np2DNumberArray]:
+        nearest_neighbours = np.argsort(distances, axis=-1)[:, 1:n + 1]
+        nearest_neighbours_distances = np.take_along_axis(
+            distances,
+            nearest_neighbours,
+            axis=-1
+        )
+
+        return nearest_neighbours, nearest_neighbours_distances
+
+    @runtime_type_checking
+    def nearest_neighbours(
+        self,
+        n: PositiveInt = 1,
+        selection: SelectionCompatible = None,
+        use_full_atom_info: bool = False
+    ) -> Tuple[Np2DIntArray,
+        Np2DNumberArray]:
         """
         Returns the n nearest neighbours of the given atoms in the system.
 
-        It is possible to specify the atoms by their element type, by their name or by their index 
-        or by the full Atom object. The parameter n specifies the number of closest nearest neighbours to return.
-        With the parameter use_full_atom_info it is possible to specify if the atoms should be searched for as 
-        only their element types or as their full atom object. (default: element types)
-
-        for example:
-            The object Atom('H1', 1) is equal to atom Atom('H') and Atom(1) if use_full_atom_info is False.
-            The object Atom('H1', 1) is not equal to atom Atom('H') and Atom(1) if use_full_atom_info is True, 
-            because also the atom_type name is compared.
+        If no selection of target atoms is given, the n nearest neighbours 
+        of all atoms are returned. With the parameter 'n' the number of 
+        nearest neighbours can be specified.
+
+        Examples
+        --------
+        >>> import numpy as np
+        >>> from PQAnalysis.atomic_system import AtomicSystem
+        >>> from PQAnalysis.core import Atom
+
+        >>> pos = np.array([[0, 0, 0], [0.5, 0.5, 0.5], [1, 1, 1]])
+        >>> atoms = [Atom('H'), Atom('H'), Atom('H')]
+        >>> system = AtomicSystem(atoms=atoms, pos=pos)
+
+        >>> system.nearest_neighbours()
+        (array([[1], [0], [1]]), array([[0.8660254], [0.8660254], [0.8660254]]))
+
+        >>> system.nearest_neighbours(n=2)
+        (array([[1, 2],
+               [0, 2],
+               [1, 0]]), array([[0.8660254 , 1.73205081],
+               [0.8660254 , 0.8660254 ],
+               [0.8660254 , 1.73205081]]))
+
+        >>> system.nearest_neighbours(selection=np.array([0]))
+        (array([[1]]), array([[0.8660254]]))
 
         Parameters
         ----------
-        n : int, optional
+        n : PositiveInt, optional
             The number of nearest neighbours to return, by default 1
-        atoms : List[Atom] | List[str] | Np1DIntArray | None, optional
-            The atoms to get the nearest neighbours of, by default None (all atoms)
+        selection : SelectionCompatible, optional
+            Selection is either a selection object or any object that can 
+            be initialized via 'Selection(selection)',
+            default None (all atoms)
         use_full_atom_info : bool, optional
-            If the full atom object should be used to match the atoms, by default False
+            If the full atom object should be used to match the 
+            atoms or only the element type, 
+            by default False
 
         Returns
         -------
         Tuple[Np2DIntArray, Np2DNumberArray]
             The n nearest neighbours of the given atoms in the system.
-            The first array contains the indices of the nearest neighbours and the second array contains the distances to the nearest neighbours.
+            The first array contains the indices of the nearest 
+            neighbours and the second array contains the distances 
+            to the nearest neighbours.
         """
 
-        indices = self.indices_from_atoms(atoms, use_full_atom_info)
+        indices = Selection(selection
+                            ).select(self.topology,
+            use_full_atom_info)
 
         return self._nearest_neighbours(n=n, indices=indices)
+
+    def image(self) -> None:
+        """
+        Images the positions of the system back into the cell.
+        """
+        self.pos = self.cell.image(self.pos)
+
+    @runtime_type_checking
+    def center(self, position: Np1DNumberArray, image: bool = True) -> None:
+        """
+        Center the positions of the system to a given position.
+
+        Parameters
+        ----------
+        position : Np1DIntArray
+            The position to recenter the system to.
+        image : bool, optional
+            If the system should be imaged back into the cell, by default True
+        """
+        self.pos -= position
+
+        if image:
+            self.image()
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/atomicSystem.py` & `pqanalysis-1.0/PQAnalysis/core/atom/atom.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,202 +1,229 @@
 """
-A module containing the AtomicSystem class
+A module containing the Atom class and some associated functions.
 
-...
-
-Classes
--------
-AtomicSystem
-    A class for storing atomic systems.
+The Atom class is used to represent an atom in a molecule. It contains the
+following attributes:
+    
+        - name: the name of the atom (e.g. 'C')
+        - element: the element of the atom (e.g. 'C')
+
+The atomic number and mass are automatically determined from the name or symbol
+of the atom. The name and symbol are automatically determined from the atomic
+number. The name is the symbol in lower case.
 """
 
-from __future__ import annotations
+import logging
+
+from numbers import Real
+
+from beartype.typing import Any, List, TypeVar
 
-import numpy as np
+from PQAnalysis import __package_name__
+from PQAnalysis.utils.custom_logging import setup_logger
+from PQAnalysis.type_checking import runtime_type_checking
 
-from beartype.typing import List, Any
-from multimethod import multimethod
+from .element import Element
+from ..exceptions import AtomError
 
-from ._decorators import check_atoms_pos, check_atoms_has_mass
-from ._properties import _PropertiesMixin
-from ._standardProperties import _StandardPropertiesMixin
-from ._indexing import _IndexingMixin
-from ._positions import _PositionsMixin
+#: A type hint for a list of atoms
+Atoms = TypeVar("Atoms", bound=List["PQAnalysis.core.Atom"])
 
-from .. import Atom, Cell
-from ...types import Np2DNumberArray, Np1DNumberArray, Np1DIntArray
 
 
-class AtomicSystem(_PropertiesMixin, _StandardPropertiesMixin, _IndexingMixin, _PositionsMixin):
+class Atom():
+
     """
-    A class for storing atomic systems.
+    A class used to represent an atom in a molecule.
+
+    There are three ways to initialize an Atom object:
 
-    Inherits from the Mixins: _PropertiesMixin, _StandardPropertiesMixin, _IndexingMixin, _PositionsMixin
-        - The _StandardPropertiesMixin contains the standard properties of an atomic system (i.e. standard getter and setter methods).
-        - The _PropertiesMixin contains special properties derived from the standard properties
-        - The _IndexingMixin contains methods for indexing the atomic system
-        - The _PositionsMixin contains methods for computing properties based on the positions of the atoms
+    1) By giving the name of the atom_type (e.g. 'C1')
+       If use_guess_element is True (default), the atom_type name has to be
+       a valid element symbol (e.g. 'C'). If use_guess_element is False, the
+       atom_type name can be anything and an empty element is created.
+
+    2) By giving the name of the atom_type (e.g. 'C1') and the id of the atom_type
+       (e.g. 6). The id can be either an integer (atomic number) or a string (element symbol).
+
+    3) By giving the id of the atom_type (e.g. 6). The id can be either an integer (atomic number) 
+       or a string (element symbol).
+
+    Examples
+    --------
+    >>> atom = Atom('C1') # use_guess_element is True by default
+    Traceback (most recent call last):
+        ...
+    ElementNotFoundError: Id C1 is not a valid element identifier.
+
+    >>> atom = Atom('C1', use_guess_element=False)
+    >>> (atom.name, atom.element)
+    ('C1', Element(None, None, None))
+
+    >>> atom = Atom('C1', 'C')
+    >>> (atom.name, atom.element)
+    ('C1', Element(c, 6, 12.0107))
+
+    >>> atom = Atom('C1', 6)
+    >>> (atom.name, atom.element)
+    ('C1', Element(c, 6, 12.0107))
+
+    >>> atom = Atom(6)
+    >>> (atom.name, atom.element)
+    ('c', Element(c, 6, 12.0107))
+
+    >>> atom = Atom('C')
+    >>> (atom.name, atom.element)
+    ('C', Element(c, 6, 12.0107))
     """
 
-    def __init__(self,
-                 atoms: List[Atom] | None = None,
-                 pos: Np2DNumberArray | None = None,
-                 vel: Np2DNumberArray | None = None,
-                 forces: Np2DNumberArray | None = None,
-                 charges: Np1DNumberArray | None = None,
-                 cell: Cell = Cell()
-                 ) -> None:
-        """
-        Initializes the AtomicSystem with the given parameters.
+    logger = logging.getLogger(__package_name__).getChild(__qualname__)
+    logger = setup_logger(logger)
+
+    @runtime_type_checking
+    def __init__(
+        self,
+        name: str | int,
+        element_id: int | str | None = None,
+        use_guess_element: bool = True,
+        **_kwargs
+    ) -> None:
+        """
+        Constructs all the necessary attributes for the Atom object.
+
+        If use_guess_element is True, the symbol, atomic number and mass are
+        determined from the name of the atom_type. If use_guess_element is
+        False, the symbol, atomic number and mass are set to None, meaning that
+        an empty element is created (Element()).
 
         Parameters
         ----------
-        atoms : List[Atom], optional
-            A list of Atom objects, by default []
-        pos : Np2DNumberArray, optional
-            A 2d numpy.ndarray containing the positions of the atoms, by default np.zeros((0, 3)).
-        vel : Np2DNumberArray, optional
-            A 2d numpy.ndarray containing the velocities of the atoms, by default np.zeros((0, 3)).
-        forces : Np2DNumberArray, optional
-            A 2d numpy.ndarray containing the forces on the atoms, by default np.zeros((0, 3)).
-        charges : Np1DNumberArray, optional
-            A 1d numpy.ndarray containing the charges of the atoms, by default np.zeros(0).
-        cell : Cell, optional
-            The unit cell of the system. Defaults to a Cell with no periodic boundary conditions, by default Cell()
-        """
-        if atoms is None:
-            atoms = []
-
-        if pos is None:
-            pos = np.zeros((0, 3))
-
-        if vel is None:
-            vel = np.zeros((0, 3))
-
-        if forces is None:
-            forces = np.zeros((0, 3))
-
-        if charges is None:
-            charges = np.zeros(0)
-
-        self._atoms = atoms
-        self._pos = pos
-        self._vel = vel
-        self._forces = forces
-        self._charges = charges
-        self._cell = cell
+        name : str | int
+            The name of the atom_type (e.g. 'C1')
+            If this parameter is an integer, it is interpreted as the atomic number of the 
+            element symbol and cannot be used together with the id parameter.
+        element_id : int | str, optional
+            The atomic number or element symbol of the atom_type (e.g. 6 or 'C') 
+            If his parameter is not given, the name parameter is used to determine 
+            the element type of the atom_type.
+        use_guess_element : bool, optional
+            Whether to use the guess_element function to determine
+            the element type of the atom_type by its name,
+            by default True
+        **_kwargs
+            Additional keyword arguments that are not used by the function but 
+            by the runtime type checker.
+
+        Raises
+        ------
+        ValueError
+            If the name of the atom_type is an integer and the id is given.
+        """
+
+        if element_id is not None and isinstance(name, int):
+
+            self.logger.error(
+                "The name of the atom_type cannot be an integer if the id is given.",
+                exception=AtomError
+            )
+
+        if element_id is not None and isinstance(name, str):
+
+            self._name = name
+            self._element = Element(element_id)
+
+        elif isinstance(name, int):
+
+            self._element = Element(name)
+            self._name = self._element.symbol.lower()
+
+        else:
+
+            self._name = name
+            if use_guess_element:
+                self._element = Element(name)
+            else:
+                self._element = Element()
 
     def __eq__(self, other: Any) -> bool:
         """
-        Checks whether the AtomicSystem is equal to another AtomicSystem.
+        Checks whether the Atom is equal to another Atom.
 
         Parameters
         ----------
-        other : AtomicSystem
-            The other AtomicSystem to compare to.
+        other : Any
+            The other Atom to compare to.
 
         Returns
         -------
         bool
-            Whether the AtomicSystem is equal to the other AtomicSystem.
+            True if the Atom is equal to the other Atom, False otherwise.
         """
-        if not isinstance(other, AtomicSystem):
-            return False
-
-        elif self.n_atoms != other.n_atoms:
-            return False
-
-        elif self.cell != other.cell:
-            return False
-
-        elif self.atoms != other.atoms:
-            return False
-
-        elif np.shape(self.pos) != np.shape(other.pos):
-            return False
-
-        elif np.shape(self.vel) != np.shape(other.vel):
-            return False
-
-        elif np.shape(self.forces) != np.shape(other.forces):
-            return False
-
-        elif np.shape(self.charges) != np.shape(other.charges):
+        if not isinstance(other, Atom):
             return False
 
         is_equal = True
-        is_equal &= np.allclose(self.pos, other.pos)
-        is_equal &= np.allclose(self.vel, other.vel)
-        is_equal &= np.allclose(self.forces, other.forces)
-        is_equal &= np.allclose(self.charges, other.charges)
-
+        is_equal &= self.name.lower() == other.name.lower()
+        is_equal &= self._element == other._element
         return is_equal
 
-    # TODO: add possibility to index with atom list etc... similar to nearest neighbours
-    @multimethod
-    def __getitem__(self, key: Atom) -> AtomicSystem:
+    def __str__(self) -> str:
         """
-        Returns a new AtomicSystem with the given key.
-
-        Parameters
-        ----------
-        key : Atom
-            The key as an atom to get the new AtomicSystem with only the matching atoms.
+        Returns a string representation of the Atom.
 
         Returns
         -------
-        AtomicSystem
-            The new AtomicSystem with the given key.
+        str
+            A string representation of the Atom.
         """
-        indices = np.argwhere(np.array(self.atoms) == key).flatten()
+        return f"Atom({self.name}, {self.atomic_number}, {self.symbol}, {self.mass})"
 
-        return self.__getitem__(indices)
-
-    @multimethod
-    def __getitem__(self, key: int | slice | Np1DIntArray) -> AtomicSystem:
+    def __repr__(self) -> str:
         """
-        Returns a new AtomicSystem with the given key.
-
-        Parameters
-        ----------
-        key : int | slice | Np1DIntArray
-            The key to get the new AtomicSystem with.
+        Returns a representation of the Atom.
 
         Returns
         -------
-        AtomicSystem
-            The new AtomicSystem with the given key.
+        str
+            A representation of the Atom.
         """
+        return self.__str__()
 
-        if isinstance(key, int):
-            keys = np.array([key])
-        elif isinstance(key, slice):
-            keys = np.array(range(self.n_atoms)[key])
-        else:
-            keys = np.array(key)
-
-        if self.atoms != []:
-            atoms = [self.atoms[key] for key in keys]
-        else:
-            atoms = None
-
-        if np.shape(self.pos)[0] > 0:
-            pos = self.pos[keys]
-        else:
-            pos = None
-
-        if np.shape(self.vel)[0] > 0:
-            vel = self.vel[keys]
-        else:
-            vel = None
-
-        if np.shape(self.forces)[0] > 0:
-            forces = self.forces[keys]
-        else:
-            forces = None
-
-        if np.shape(self.charges)[0] > 0:
-            charges = self.charges[keys]
-        else:
-            charges = None
-
-        return AtomicSystem(atoms=atoms, pos=pos, vel=vel, forces=forces, charges=charges, cell=self.cell)
+    #######################
+    #                     #
+    # standard properties #
+    #                     #
+    #######################
+
+    @property
+    def name(self) -> str:
+        """str: The name of the atom_type (e.g. 'C1')"""
+        return self._name
+
+    @property
+    def symbol(self) -> str | None:
+        """str: The symbol of the element (e.g. 'c')"""
+        return self._element.symbol
+
+    @property
+    def atomic_number(self) -> int | None:
+        """int | None: The atomic number of the element (e.g. 6)"""
+        return self._element.atomic_number
+
+    @property
+    def mass(self) -> Real | None:
+        """Real | None: The mass of the element (e.g. 12.011)"""
+        return self._element.mass
+
+    @property
+    def element(self) -> Element:
+        """Element: The element type of the atom"""
+        return self._element
+
+    @element.setter
+    def element(self, element: Element) -> None:
+        self._element = element
+
+    @property
+    def element_name(self) -> str:
+        """str: The name of the element (e.g. 'Carbon')"""
+        return self._element.name
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/core/cell.py` & `pqanalysis-1.0/PQAnalysis/core/cell/cell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,46 @@
 """
 A module containing the Cell class.
-
-...
-
-Classes
--------
-Cell
-    A class for storing unit cell parameters.
 """
 
-from __future__ import annotations
-
-import numpy as np
 import sys
+import warnings
 
-from beartype.typing import Any
 from numbers import Real
 
-from ..types import Np3x3NumberArray, Np2DNumberArray, Np1DNumberArray
+import numpy as np
 
+from beartype.typing import Any, NewType, Annotated
+from beartype.vale import Is
 
-class Cell:
-    '''
-    Class for storing unit cell parameters.
+from PQAnalysis.type_checking import runtime_type_checking
+from PQAnalysis.types import Np3x3NumberArray, Np2DNumberArray, NpnDNumberArray
 
-    ...
+from ._standard_properties import _StandardPropertiesMixin
 
-    Attributes
-    ----------
 
-    x : Real, optional
-        The length of the first box vector. Default is sys.float_info.max.
-    y : Real, optional
-        The length of the second box vector. Default is sys.float_info.max.
-    z : Real, optional
-        The length of the third box vector. Default is sys.float_info.max.
-    alpha : Real, optional
-        The angle between the second and third box vector. Default is 90.
-    beta : Real, optional
-        The angle between the first and third box vector. Default is 90.
-    gamma : Real, optional
-        The angle between the first and second box vector. Default is 90.
-    box_matrix : np.array
-        The matrix containing the box vectors as columns.
-    '''
-
-    def __init__(self,
-                 x: Real = sys.float_info.max,
-                 y: Real = sys.float_info.max,
-                 z: Real = sys.float_info.max,
-                 alpha: Real = 90,
-                 beta: Real = 90,
-                 gamma: Real = 90
-                 ) -> None:
-        """
-        Initializes the Cell with the given parameters.
 
-        If no angles are given, the cell is assumed to be orthorhombic.
-        The box matrix is calculated from the given parameters.
+class Cell(_StandardPropertiesMixin):
+
+    """
+    Class for storing unit cell parameters.
+    """
+
+    @runtime_type_checking
+    def __init__(
+        self,
+        x: Real = sys.float_info.max,
+        y: Real = sys.float_info.max,
+        z: Real = sys.float_info.max,
+        alpha: Real = 90,
+        beta: Real = 90,
+        gamma: Real = 90
+    ) -> None:
+        """
+        A cell object can be initialized with the following parameters:
 
         Parameters
         ----------
         x : Real
             The length of the first box vector.
         y : Real
             The length of the second box vector.
@@ -69,130 +48,113 @@
             The length of the third box vector.
         alpha : Real, optional
             The angle between the second and third box vector.
         beta : Real, optional
             The angle between the first and third box vector.
         gamma : Real, optional
             The angle between the first and second box vector.
-        """
-        self.x = x
-        self.y = y
-        self.z = z
-        self.alpha = alpha
-        self.beta = beta
-        self.gamma = gamma
-        self.box_matrix = self.setup_box_matrix()
+
+        Notes
+        -----
+        A vacuum cell can be created by calling Cell(), which is equivalent to 
+        Cell(x=sys.float_info.max, y=sys.float_info.max, z=sys.float_info.max,
+        alpha=90, beta=90, gamma=90).
+        """
+        self._box_lengths = np.array([x, y, z])
+        self._box_angles = np.array([alpha, beta, gamma])
+        self._box_matrix = self.setup_box_matrix()
 
     def setup_box_matrix(self) -> Np3x3NumberArray:
         """
         Calculates the box matrix from the given parameters.
 
         Returns
         -------
         box matrix: Np3x3NumberArray
             The box matrix.
         """
         matrix = np.array([[0.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]])
 
-        alpha = np.deg2rad(self.alpha)
-        beta = np.deg2rad(self.beta)
-        gamma = np.deg2rad(self.gamma)
-
-        matrix[0][0] = self.x
-        matrix[0][1] = self.y * np.cos(gamma)
-        matrix[0][2] = self.z * np.cos(beta)
-        matrix[1][1] = self.y * np.sin(gamma)
-        matrix[1][2] = self.z * \
-            (np.cos(alpha) - np.cos(beta) * np.cos(gamma)) / np.sin(gamma)
-        matrix[2][2] = self.z * np.sqrt(1 - np.cos(beta)**2 - (
-            np.cos(alpha) - np.cos(beta) * np.cos(gamma))**2 / np.sin(gamma)**2)
+        alpha, beta, gamma = np.deg2rad(self.box_angles)
+        cos_alpha, cos_beta, cos_gamma = np.cos([alpha, beta, gamma])
+        sin_gamma = np.sin(gamma)
+        sin_beta = np.sin(beta)
+        x, y, z = self.box_lengths
+
+        matrix[0][0] = x
+        matrix[0][1] = y * cos_gamma
+        matrix[0][2] = z * cos_beta
+        matrix[1][1] = y * sin_gamma
+        matrix[1][2] = z * (cos_alpha - cos_beta * cos_gamma) / sin_gamma
+        matrix[2][2] = z * np.sqrt(
+            sin_beta**2 - (cos_alpha - cos_beta * cos_gamma)**2 / sin_gamma**2
+        )
 
         return matrix
 
     @property
     def bounding_edges(self) -> Np2DNumberArray:
-        """
-        calculates the coordinates of the eight corners of the unit cell.
-
-        Returns
-        -------
-        edges: Np2DNumberArray of shape (8, 3)
-            The coordinates of the eight corners of the unit cell.
-        """
+        """Np2DNumberArray: The 8 corners of the bounding box of the unit cell."""
         edges = np.zeros((8, 3))
         for i, x in enumerate([-0.5, 0.5]):
             for j, y in enumerate([-0.5, 0.5]):
                 for k, z in enumerate([-0.5, 0.5]):
                     edges[i*4+j*2+k, :] = self.box_matrix @ np.array([x, y, z])
 
         return edges
 
     @property
     def volume(self) -> Real:
-        """
-        Returns the volume of the unit cell.
-
-        Returns
-        -------
-        Real
-            The volume of the unit cell.
-        """
-        return np.linalg.det(self.box_matrix)
-
-    @property
-    def box_lengths(self) -> Np1DNumberArray:
-        """
-        Returns the lengths of the box vectors.
+        """volume: The volume of the unit cell."""
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                message="overflow encountered in det"
+            )
+            volume = np.linalg.det(self.box_matrix)
 
-        Returns
-        -------
-        box_lengths: Np1DNumberArray of shape (3,)
-            The lengths of the box vectors.
-        """
-        return np.array([self.x, self.y, self.z])
+        return volume
 
     @property
-    def box_angles(self) -> Np1DNumberArray:
-        """
-        Returns the angles between the box vectors.
-
-        Returns
-        -------
-        box_angles: Np1DNumberArray of shape (3,)
-            The lengths of the box vectors.
-        """
-        return np.array([self.alpha, self.beta, self.gamma])
-
-    def image(self, pos: Np2DNumberArray | Np1DNumberArray) -> Np2DNumberArray | Np1DNumberArray:
-        """
-        Returns the image of the given position in the unit cell.
+    def is_vacuum(self) -> bool:
+        """bool: Returns whether the unit cell is a vacuum."""
+        return bool(self.volume > 1e100)
+
+    @runtime_type_checking
+    def image(self, pos: NpnDNumberArray) -> NpnDNumberArray:
+        """
+        Images the given position(s) into the unit cell.
+
+        This class can be used to image positions of arbitrary shape into the unit cell.
+        The shape of the input is preserved. The only requirement is that the last 
+        dimension of the input is 3, representing the x, y and z coordinates of the position(s).
 
         Parameters
         ----------
-        pos : Np2DNumberArray, Np1DNumberArray
+        pos : NpnDNumberArray
             The position to get the image of.
 
         Returns
         -------
-        imaged_positions: Np2DNumberArray, Np1DNumberArray
+        imaged_positions: NpnDNumberArray
             The image of the position(s) in the unit cell.
         """
 
         original_shape = np.shape(pos)
+        pos = np.reshape(pos, (-1, 3))
 
-        if original_shape == (3,):
-            pos = np.reshape(pos, (1, 3))
+        if self.alpha == 90 and self.beta == 90 and self.gamma == 90:
+            pos = pos - self.box_lengths * np.round(pos / self.box_lengths)
+        else:
 
-        fractional_pos = np.array(
-            [np.linalg.inv(self.box_matrix) @ pos_i for pos_i in pos])
+            fractional_pos = pos @ self.inverse_box_matrix.T
 
-        fractional_pos -= np.round(fractional_pos)
+            fractional_pos -= np.round(fractional_pos)
 
-        pos = np.array(
-            [self.box_matrix @ fractional_pos_i for fractional_pos_i in fractional_pos])
+            pos = fractional_pos @ self.box_matrix.T
 
         return np.reshape(pos, original_shape)
 
     def __eq__(self, other: Any) -> bool:
         """
         Checks if the Cell is equal to another Cell.
 
@@ -207,14 +169,93 @@
             True if the Cells are equal, False otherwise.
         """
 
         if not isinstance(other, Cell):
             return False
 
         is_equal = True
-        is_equal &= np.allclose(self.x, other.x)
-        is_equal &= np.allclose(self.y, other.y)
-        is_equal &= np.allclose(self.z, other.z)
-        is_equal &= np.allclose(self.alpha, other.alpha)
-        is_equal &= np.allclose(self.beta, other.beta)
-        is_equal &= np.allclose(self.gamma, other.gamma)
+        is_equal &= np.allclose(self.box_lengths, other.box_lengths)
+        is_equal &= np.allclose(self.box_angles, other.box_angles)
         return is_equal
+
+    def __str__(self) -> str:
+        """
+        Returns a string representation of the Cell.
+
+        Returns
+        -------
+        str
+            A string representation of the Cell.
+        """
+        x = self.x
+        y = self.y
+        z = self.z
+        alpha = self.alpha
+        beta = self.beta
+        gamma = self.gamma
+
+        if self != Cell():
+            return f"Cell({x=}, {y=}, {z=}, {alpha=}, {beta=}, {gamma=})"
+
+        return "Cell()"
+
+    def __repr__(self) -> str:
+        """
+        Returns a string representation of the Cell.
+
+        Returns
+        -------
+        str
+            A string representation of the Cell.
+        """
+        return self.__str__()
+
+    @classmethod
+    @runtime_type_checking
+    def init_from_box_matrix(cls, box_matrix: Np3x3NumberArray) -> "Cell":
+        """
+        Initializes a Cell object from a box matrix.
+
+        Parameters
+        ----------
+        box_matrix : Np3x3NumberArray
+            The box matrix.
+
+        Returns
+        -------
+        Cell
+            The Cell object.
+        """
+        x = np.linalg.norm(np.transpose(box_matrix)[0])
+        y = np.linalg.norm(np.transpose(box_matrix)[1])
+        z = np.linalg.norm(np.transpose(box_matrix)[2])
+
+        gamma = np.arccos(box_matrix[0][1] / y)
+        beta = np.arccos(box_matrix[0][2] / z)
+        alpha = np.arccos(
+            (
+            box_matrix[0][1] * box_matrix[0][2] +
+            box_matrix[1][1] * box_matrix[1][2]
+            ) / (y * z)
+        )
+
+        print(alpha, beta, gamma)
+        print(np.rad2deg(alpha), np.rad2deg(beta), np.rad2deg(gamma))
+
+        return cls(
+            x,
+            y,
+            z,
+            np.rad2deg(alpha),
+            np.rad2deg(beta),
+            np.rad2deg(gamma)
+        )
+
+
+
+#: A type hint for a list of cells
+Cells = NewType(
+    "Cells",
+    Annotated[list,
+    Is[lambda list: all(isinstance(atom,
+    Cell) for atom in list)]]
+)
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/io/boxWriter.py` & `pqanalysis-1.0/PQAnalysis/io/box_writer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,131 @@
 """
 A module containing the BoxWriter class and its associated methods.
-
-...
-
-Classes
--------
-BoxWriter
-    A class for writing a trajectory to a box file.
 """
 
-from . import BaseWriter, BoxWriterError
-from ..utils import instance_function_count_decorator
-from ..traj import Trajectory
-
-
-def write_box(traj, filename: str | None = None, format: str | None = None) -> None:
-    '''
-    Wrapper for BoxWriter to write a trajectory to a file.
-
-    Parameters
-    ----------
-    traj : Trajectory
-        The trajectory to write.
-    filename : str, optional
-        The name of the file to write to. If None, the output is printed to stdout.
-    format : str, optional
-        The format of the file. If None, the format is inferred as a data file format.
-        (see BoxWriter.formats for available formats)
-    '''
+import logging
+
+from PQAnalysis.traj import Trajectory
+from PQAnalysis.utils import instance_function_count_decorator
+from PQAnalysis.utils.custom_logging import setup_logger
+from PQAnalysis import __package_name__
+from PQAnalysis.type_checking import runtime_type_checking, runtime_type_checking_setter
+
+from .base import BaseWriter
+from .formats import BoxFileFormat, FileWritingMode
+from .exceptions import BoxWriterError
 
-    writer = BoxWriter(filename, format)
-    writer.write(traj)
 
 
 class BoxWriter(BaseWriter):
+
     """
     A class for writing a trajectory to a box file.
-    Inherits from BaseWriter. See BaseWriter for more information.
+    Inherits from BaseWriter
 
-    It can write a trajectory to a box file in either a data file format or a VMD file format.
-
-    ...
-
-    Class Attributes
-    ----------------
-    formats : list of str
-        The available formats for the box file.
-
-    Attributes
-    ----------
-    format : str
-        The format of the file. If None, the format is inferred as a data file format.
-        (see BoxWriter.formats for available formats)
+    It can write a trajectory to a box file in either a data file
+    format or a VMD file format. For more information see
+    :py:class:`~PQAnalysis.io.formats.BoxFileFormat`.
     """
-    formats = [None, 'data', 'vmd']
 
-    def __init__(self, filename: str | None = None, format: str | None = None, mode='w') -> None:
-        """
-        Initializes the BoxWriter with the given filename, format and mode.
+    logger = logging.getLogger(__package_name__).getChild(__qualname__)
+    logger = setup_logger(logger)
 
+    @runtime_type_checking
+    def __init__(
+        self,
+        filename: str | None = None,
+        output_format: str | BoxFileFormat = 'data',
+        mode: str | FileWritingMode = 'w'
+    ) -> None:
+        """
         Parameters
         ----------
         filename : str, optional
-            The name of the file to write to. If None, the output is printed to stdout.
-        format : str, optional
-            The format of the file. If None, the format is inferred as a data file format.
-            (see BoxWriter.formats for available formats)
-        mode : str, optional
-            The mode of the file. Either 'w' for write or 'a' for append.
+            The name of the file to write to.
+            If None, the output is printed to stdout.
+        output_format : str | BoxFileFormat, optional
+            The format of the file.
+            The default is 'data' i.e. BoxFileFormat.DATA.
+        mode : str | FileWritingMode, optional
+            The mode of the file. Either 'w' for write,
+            'a' for append or 'o' for overwrite. The default is 'w'.
 
         Raises
         ------
         ValueError
-            If the given format is not in BoxWriter.formats. TODO: make an enum for these formats!!!
+            If the given format is not in :py:class:`~PQAnalysis.io.formats.BoxFileFormat`.
         """
 
-        super().__init__(filename, mode)
-        if format not in self.formats:
-            raise ValueError(
-                'Invalid format. Has to be either \'vmd\', \'data\' or \'None\'.')
-
-        if format is None:
-            format = 'data'
-
-        self.format = format
+        super().__init__(filename, FileWritingMode(mode))
+        self.output_format = BoxFileFormat(output_format)
 
+    @runtime_type_checking
     def write(self, traj: Trajectory, reset_counter: bool = True) -> None:
         """
         Wrapper to write the given trajectory to the file.
         Depending on the format, either write_vmd or write_box_file is called.
 
         Parameters
         ----------
         traj : Trajectory
             The trajectory to write.
         reset_counter : bool, optional
-            If True, the function execution counter of write_box_file 
+            If True, the function execution counter of write_box_file
             is reset to 0, otherwise it is not reset.
         """
 
         self.open()
-        if self.format == "vmd":
+        if self.output_format == BoxFileFormat.VMD:
             self.write_vmd(traj)
         else:
             self.write_box_file(traj, reset_counter=reset_counter)
 
         self.close()
 
+    @runtime_type_checking
     def write_vmd(self, traj: Trajectory) -> None:
         """
         Writes the given trajectory to the file in VMD format.
 
-        The format looks in general like this:
-
-                8
-                Box  1.0 1.0 1.0    90.0 90.0 90.0
-                X   0.0 0.0 0.0
-                X   1.0 0.0 0.0
-                X   0.0 1.0 0.0
-                X   1.0 1.0 0.0
-                X   0.0 0.0 1.0
-                X   1.0 0.0 1.0
-                X   0.0 1.0 1.0
-                X   1.0 1.0 1.0
-                8
-                Box  1.0 1.0 1.0    90.0 90.0 90.0
-                X   0.0 0.0 0.0
-                ...
-
-        where all X represent the vertices of the box. The first line contains the number of vertices.
-        The second line contains the box dimensions and box angles as the comment line for a xyz file.
-
         Parameters
         ----------
         traj : Trajectory
             The trajectory to write.
         """
-        self.__check_PBC__(traj)
+        self.__check_pbc__(traj)
 
         for frame in traj:
             cell = frame.cell
 
             print("8", file=self.file)
             print(
-                f"Box   {cell.x} {cell.y} {cell.z}    {cell.alpha} {cell.beta} {cell.gamma}", file=self.file)
+                (
+                f"Box   "
+                f"{cell.x} {cell.y} {cell.z}    "
+                f"{cell.alpha} {cell.beta} {cell.gamma}"
+                ),
+                file=self.file
+            )
+
             edges = cell.bounding_edges
+
             for edge in edges:
                 print(f"X   {edge[0]} {edge[1]} {edge[2]}", file=self.file)
 
     @instance_function_count_decorator
-    def write_box_file(self, traj: Trajectory, reset_counter: bool = True) -> None:
+    @runtime_type_checking
+    def write_box_file(
+        self,
+        traj: Trajectory,
+        reset_counter: bool = True  # pylint: disable=unused-argument # is needed for the decorator
+    ) -> None:
         """
         Writes the given trajectory to the file in data file format.
 
-        The format looks in general like this:
-
-                1 1.0 1.0 1.0 90.0 90.0 90.0
-                2 1.0 1.0 1.0 90.0 90.0 90.0
-                ...
-                n 1.1 1.1 1.1 90.0 90.0 90.0
-
-        where the first column represents the step starting from 1, the second to fourth column
-        represent the box vectors a, b, c, the fifth to seventh column represent the box angles.
-
         The @count_decorator is used to count the number of frames written to the file. The default
         way is that the counter is reset to 0 after each call of the function. This can be changed
         by setting the reset_counter parameter to False.
 
 
         Parameters
         ----------
@@ -176,35 +135,53 @@
             If True, the counter is reset to 0, otherwise it is not reset.
 
         Raises
         ------
         BoxWriterError
             If the cell of a frame of the trajectory is None.
         """
-        self.__check_PBC__(traj)
+        self.__check_pbc__(traj)
 
-        counter = self.counter[BoxWriter.write_box_file.__name__]
-        counter = len(traj)*(counter - 1)
+        counter = self.counter[BoxWriter.write_box_file.__name__]  # pylint: disable=no-member # is added via decorator
+        counter = len(traj) * (counter - 1)
 
         for i, frame in enumerate(traj):
             cell = frame.cell
             print(
-                f"{counter + i+1} {cell.x} {cell.y} {cell.z} {cell.alpha} {cell.beta} {cell.gamma}", file=self.file)
+                (
+                f"{counter + i+1} "
+                f"{cell.x} {cell.y} {cell.z} "
+                f"{cell.alpha} {cell.beta} {cell.gamma}"
+                ),
+                file=self.file
+            )
 
-    def __check_PBC__(self, traj: Trajectory) -> None:
+    def __check_pbc__(self, traj: Trajectory) -> None:
         """
         Checks if the cell of the trajectory is not None.
 
         Parameters
         ----------
         traj : Trajectory
             The trajectory to check.
 
         Raises
         ------
         ValueError
             If the cell of a frame of the trajectory is None.
         """
 
-        if not traj.check_PBC():
-            raise BoxWriterError(
-                "At least on cell of the trajectory is None. Cannot write box file.")
+        if not traj.check_pbc():
+            self.logger.error(
+                "At least on cell of the trajectory is None. Cannot write box file.",
+                exception=BoxWriterError
+            )
+
+    @property
+    def output_format(self) -> BoxFileFormat:
+        """BoxFileFormat: The format of the file."""
+        return self._output_format
+
+    @output_format.setter
+    @runtime_type_checking_setter
+    def output_format(self, output_format: str | BoxFileFormat) -> None:
+        self._output_format = BoxFileFormat(output_format)
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/io/energyFileReader.py` & `pqanalysis-1.0/PQAnalysis/io/energy_file_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,85 @@
 """
 A module containing the EnergyFileReader class.
-
-...
-
-Classes
--------
-EnergyFileReader
-    A class to read energy files.
 """
 
 import os
+import logging
 import numpy as np
 
-from . import BaseReader, InfoFileReader
-from ..physicalData import Energy
-from ..traj import MDEngineFormat
+from PQAnalysis.physical_data import Energy
+from PQAnalysis.traj import MDEngineFormat
+from PQAnalysis.utils.custom_logging import setup_logger
+from PQAnalysis import __package_name__
+from PQAnalysis.exceptions import PQFileNotFoundError
+from PQAnalysis.type_checking import runtime_type_checking
+
+from .base import BaseReader
+from .info_file_reader import InfoFileReader
+
 
 
 class EnergyFileReader(BaseReader):
-    """
-    A class to read energy files.
 
-    Parameters
-    ----------
-    BaseReader : BaseReader
-        A base class for all readers.
-
-    Attributes
-    ----------
-    filename : str
-        The name of the file to read from.
-    info_filename : str
-        The name of the info file to read from.
-    withInfoFile : bool
-        If True, the info file was found.
-    format : MDEngineFormat
-        The format of the file. Default is MDEngineFormat.PIMD_QMCF.
+    """
+    A class to read energy files from molecular dynamics simulations.
     """
 
-    def __init__(self,
-                 filename: str,
-                 info_filename: str | None = None,
-                 use_info_file: bool = True,
-                 format: MDEngineFormat | str = MDEngineFormat.PIMD_QMCF
-                 ) -> None:
-        """
-        Initializes the EnergyFileReader with the given filename.
+    logger = logging.getLogger(__package_name__).getChild(__qualname__)
+    logger = setup_logger(logger)
 
-        If no info_filename is given, the energy filename is used to find the
-        info file. If a info_filename is given, this filename is used to find the
-        info file. If the info_filename was explicitly set to a non-existing file,
+    @runtime_type_checking
+    def __init__(
+        self,
+        filename: str,
+        info_filename: str | None = None,
+        use_info_file: bool = True,
+        engine_format: MDEngineFormat | str = MDEngineFormat.PQ
+    ) -> None:
+        """
+        For the initialization of the EnergyFileReader, the filename of the energy
+        file has to be given. The info_filename can be given as well. If no
+        info_filename is given, the energy filename is used to find the info 
+        file with the proper extension and the base name of the energy file. 
+        If a info_filename is given, this filename is used to find the info 
+        file. If the info_filename was explicitly set to a non-existing file,
         a FileNotFoundError is raised. If use_info_file is set to False, no info
         file is searched for.
 
+        Providing info files is optional, but where possible, it is recommended to 
+        provide an info file. The info file contains information about the physical
+        quantities stored in the energy file. If an info file is provided, the 
+        physical quantities are assumed to be in the order of the info file. The 
+        info file can also contain units for the physical quantities. If units are
+        provided, the units are stored in the Energy object, which is returned by 
+        the read method.
+
+        For more information about the energy object, see
+        :py:class:`~PQAnalysis.physicalData.energy.Energy`.
+
         Parameters
         ----------
         filename : str
             The name of the file to read from.
         info_filename : str, optional
             The name of the info file to read from, by default None
         use_info_file : bool, optional
             If True, the info file is searched for, by default True
-        format : MDEngineFormat | str, optional
-            The format of the file, by default MDEngineFormat.PIMD_QMCF
+        engine_format : MDEngineFormat | str, optional
+            The format of the file, by default MDEngineFormat.PQ
         """
         super().__init__(filename)
         self.info_filename = info_filename
 
         if use_info_file:
-            self.withInfoFile = self.__info_file_found__()
+            self.with_info_file = self.__info_file_found__()
         else:
-            self.withInfoFile = False
+            self.with_info_file = False
 
-        self.format = MDEngineFormat(format)
+        self.format = MDEngineFormat(engine_format)
 
     def read(self) -> Energy:
         """
         Reads the energy file.
 
         The data of the energy file is returned as a np.array within a Energy object.
         The data array is stored in a way that each column corresponds to a physical
@@ -87,27 +90,32 @@
         Energy
             The data of the energy file as a np.array within a Energy object.
             In addition, the info and units of the info file are stored in the Energy
             object, if an info file was found.
         """
         info, units = None, None
 
-        if self.withInfoFile:
-            reader = InfoFileReader(self.info_filename, format=self.format)
+        if self.with_info_file:
+
+            reader = InfoFileReader(
+                self.info_filename,
+                engine_format=self.format
+            )
+
             info, units = reader.read()
 
-        with open(self.filename, "r") as file:
+        with open(self.filename, "r", encoding='utf-8') as file:
 
             data = []
 
             for line in file:
                 if line.startswith("#"):
                     continue
 
-                data_line = map(lambda x: float(x), line.split())
+                data_line = [float(x) for x in line.split()]
                 data.append(list(data_line))
 
         return Energy(np.array(data).T, info, units)
 
     def __info_file_found__(self) -> bool:
         """
         Checks if a info file exists for the given file.
@@ -126,19 +134,24 @@
         ------
         FileNotFoundError
             If an explicitly given info file does not exist.
         """
         if self.info_filename is None:
 
             self.info_filename = os.path.splitext(self.filename)[0] + ".info"
+
             try:
                 BaseReader(self.info_filename)
-            except FileNotFoundError:
+            except PQFileNotFoundError:
                 self.info_filename = None
+
         else:
+
             try:
                 BaseReader(self.info_filename)
-            except FileNotFoundError:
-                raise FileNotFoundError(
-                    f"Info File {self.info_filename} not found.")
+            except PQFileNotFoundError:
+                self.logger.error(
+                    f"Info File {self.info_filename} not found.",
+                    exception=PQFileNotFoundError
+                )
 
         return self.info_filename is not None
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/io/trajectoryReader.py` & `pqanalysis-1.0/PQAnalysis/io/traj_file/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,165 @@
 """
-A module containing classes for reading a trajectory from a file.
+A module containing different API functions for reading and writing trajectory files.
+"""
 
-...
+from beartype.typing import Generator
 
-Classes
--------
-TrajectoryReader
-    A class for reading a trajectory from a file.
-"""
+from PQAnalysis.topology import Topology
+from PQAnalysis.atomic_system import AtomicSystem
+from PQAnalysis.io.formats import FileWritingMode
+from PQAnalysis.type_checking import runtime_type_checking
+
+from PQAnalysis.io.traj_file import (
+    TrajectoryWriter,
+    TrajectoryReader,
+)
+
+from PQAnalysis.traj import (
+    Trajectory,
+    MDEngineFormat,
+    TrajectoryFormat,
+)
+
+
+
+@runtime_type_checking
+def write_trajectory(
+    traj: Trajectory | AtomicSystem,
+    filename: str | None = None,
+    engine_format: MDEngineFormat | str = MDEngineFormat.PQ,
+    traj_type: TrajectoryFormat | str = TrajectoryFormat.XYZ,
+    mode: FileWritingMode | str = FileWritingMode.WRITE,
+) -> None:
+    """Wrapper for TrajectoryWriter to write a trajectory to a file.
+
+    if format is None, the default PQ format is used
+    (see TrajectoryWriter.formats for available formats).
+    if format is 'qmcfc', the QMCFC format is used
+    (see TrajectoryWriter.formats for more information).
+
+    Parameters
+    ----------
+    traj : Trajectory
+        The trajectory to write.
+    filename : str, optional
+        The name of the file to write to. If None, the output is printed to stdout.
+    engine_format : MDEngineFormat | str, optionalsssss
+        The format of the md engine for the output file.
+        The default is MDEngineFormat.PQ.
+    traj_type : TrajectoryFormat | str, optional
+        The type of the data to write to the file.
+        Default is TrajectoryFormat.XYZ.
+    mode : FileWritingMode | str, optional
+        The mode of the file. Either 'w' for write, 
+        'a' for append or 'o' for overwrite. The default is 'w'.
+
+    """
+
+    writer = TrajectoryWriter(filename, engine_format=engine_format, mode=mode)
+    writer.write(traj, traj_type=traj_type)
+
+
+
+@runtime_type_checking
+def read_trajectory(
+    filename: str,
+    md_format: MDEngineFormat | str = MDEngineFormat.PQ,
+    traj_format: TrajectoryFormat | str = TrajectoryFormat.AUTO,
+    topology: Topology | None = None,
+    constant_topology: bool = True
+) -> Trajectory:
+    """
+    API function for reading a trajectory from a file.
+
+    Parameters
+    ----------
+    filename : str
+        The name of the file to read from.
+    md_format : MDEngineFormat | str, optional
+        The format of the trajectory, by default MDEngineFormat.PQ
+    traj_format : TrajectoryFormat | str, optional
+        The format of the trajectory, by default TrajectoryFormat.AUTO.
+        The format is inferred from the file extension.
+    topology : Topology | None, optional
+        The topology of the trajectory, by default None
+    constant_topology : bool, optional
+        Whether the topology is constant over the trajectory or does change, by default True
+
+    Returns
+    -------
+    Trajectory
+        The trajectory read from the file.
+    """
+
+    reader = TrajectoryReader(
+        filename,
+        traj_format=traj_format,
+        md_format=md_format,
+        topology=topology,
+        constant_topology=constant_topology
+    )
+
+    return reader.read()
 
-from beartype.typing import List
 
-from . import BaseReader, TrajectoryReaderError, FrameReader
-from ..traj import Trajectory, TrajectoryFormat, MDEngineFormat
-from ..core import Cell
 
+@runtime_type_checking
+def calculate_frames_of_trajectory_file(filename: str):
+    """
+    Calculate the number of frames in a trajectory file.
+
+    Parameters
+    ----------
+    filename : str
+        The name of the file to read.
 
-class TrajectoryReader(BaseReader):
+    Returns
+    -------
+    int
+        The number of frames in the trajectory file.
     """
-    A class for reading a trajectory from a file.
+    reader = TrajectoryReader(filename)
+    return reader.calculate_number_of_frames()
 
-    Inherited from BaseReader.
 
-    ...
 
-    Attributes
+@runtime_type_checking
+def read_trajectory_generator(
+    filename: str,
+    md_format: MDEngineFormat | str = MDEngineFormat.PQ,
+    traj_format: TrajectoryFormat | str = TrajectoryFormat.AUTO,
+    topology: Topology | None = None,
+    constant_topology: bool = True
+) -> Generator[AtomicSystem]:
+    """
+    API function for building a frame generator from a trajectory file.
+
+    Parameters
     ----------
     filename : str
         The name of the file to read from.
-    frames : list of Frame
-        The list of frames read from the file.
+    md_format : MDEngineFormat | str, optional
+        The format of the trajectory, by default MDEngineFormat.PQ
+    traj_format : TrajectoryFormat | str, optional
+        The format of the trajectory, by default TrajectoryFormat.AUTO.
+        The format is inferred from the file extension.
+    topology : Topology | None, optional
+        The topology of the trajectory, by default None
+    constant_topology : bool, optional
+        Whether the topology is constant over the trajectory or does change, by default True
+
+    Returns
+    -------
+    Generator[AtomicSystem]
+        A generator for the frames in the trajectory.
     """
 
-    def __init__(self, filename: str | List[str], format: TrajectoryFormat | str = TrajectoryFormat.XYZ) -> None:
-        """
-        Initializes the TrajectoryReader with the given filename.
-
-        Parameters
-        ----------
-        filename : str or list of str
-            The name of the file to read from or a list of filenames to read from.
-        """
-        super().__init__(filename)
-        self.frames = []
-        self.format = format
-
-    def read(self, md_format: MDEngineFormat | str = MDEngineFormat.PIMD_QMCF) -> Trajectory:
-        """
-        Reads the trajectory from the file.
-
-        It reads the trajectory from the file and concatenates the lines of the same frame.
-        The frame information is then read from the concatenated string with the FrameReader class and
-        a Frame object is created.
-
-        In order to read the cell information given in the file, the cell information of the last frame is used for
-        all following frames that do not have cell information.
-
-        If the trajectory is split into multiple files, the files are read one after another and the frames are
-        concatenated into a single trajectory.
-
-        Returns
-        -------
-        Trajectory
-            The trajectory read from the file.
-        """
-        if not self.multiple_files:
-            return self._read_single_file(md_format)
-
-        else:
-
-            traj = Trajectory()
-            for filename in self.filenames:
-                self.filename = filename
-                traj += self._read_single_file(md_format)
-
-            self.filename = None
-            return traj
-
-    def _read_single_file(self, md_format: MDEngineFormat | str = MDEngineFormat.PIMD_QMCF) -> Trajectory:
-        """
-        Reads the trajectory from the file.
-
-        It reads the trajectory from the file and concatenates the lines of the same frame.
-        The frame information is then read from the concatenated string with the FrameReader class and
-        a Frame object is created.
-
-        In order to read the cell information given in the file, the cell information of the last frame is used for
-        all following frames that do not have cell information.
-
-        Returns
-        -------
-        Trajectory
-            The trajectory read from the file.
-        """
-        frame_reader = FrameReader()
-        with open(self.filename, 'r') as f:
-
-            # Concatenate lines of the same frame
-            frame_string = ''
-            for line in f:
-                if line.strip() == '':
-                    frame_string += line
-                elif line.split()[0].isdigit():
-                    if frame_string != '':
-                        self._read_single_frame(
-                            frame_string, frame_reader, md_format)
-
-                    frame_string = line
-                else:
-                    frame_string += line
-
-            self._read_single_frame(frame_string, frame_reader, md_format)
-
-        traj = Trajectory(self.frames)
-        self.frames = []
-
-        return traj
-
-    def _read_single_frame(self, frame_string: str, frame_reader: FrameReader,  md_format: MDEngineFormat | str) -> None:
-        """
-        Reads a single frame from the given string.
-
-        Parameters
-        ----------
-        frame_string : str
-            The string containing the frame information.
-
-        Raises
-        ------
-        TrajectoryReaderError
-            If the first atom in the frame is not X for QMCFC.
-        """
-        frame = frame_reader.read(frame_string, format=self.format)
-
-        # to make sure X particle is not included in the trajectory for QMCFC
-        if MDEngineFormat(md_format) == MDEngineFormat.PIMD_QMCF:
-            self.frames.append(frame)
-        elif MDEngineFormat(md_format) == MDEngineFormat.QMCFC:
-            if frame.atoms[0].name.upper() != 'X':
-                raise TrajectoryReaderError(
-                    "The first atom in one of the frames is not X. Please use pimd_qmcf (default) md engine instead")
-            else:
-                self.frames.append(frame[1:])
-
-        # If the read frame does not have cell information, use the cell information of the previous frame
-        if len(self.frames) > 1 and self.frames[-1].cell == Cell():
-            self.frames[-1].cell = self.frames[-2].cell
+    reader = TrajectoryReader(
+        filename,
+        traj_format=traj_format,
+        md_format=md_format,
+        topology=topology,
+        constant_topology=constant_topology
+    )
+
+    return reader.frame_generator()
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/io/trajectoryWriter.py` & `pqanalysis-1.0/PQAnalysis/io/traj_file/trajectory_writer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,203 +1,146 @@
 """
 A module containing the TrajectoryWriter class and its associated methods.
-
-...
-
-Classes
--------
-TrajectoryWriter
-    A class for writing a trajectory to a file.
 """
 
 from beartype.typing import List
 
-from . import BaseWriter
-from ..traj import Trajectory, TrajectoryFormat, MDEngineFormat, Frame
-from ..core import Cell, Atom
-from ..types import Np2DNumberArray, Np1DNumberArray
-
-
-def write_trajectory(traj,
-                     filename: str | None = None,
-                     format: MDEngineFormat | str = MDEngineFormat.PIMD_QMCF,
-                     type: TrajectoryFormat | str = TrajectoryFormat.XYZ
-                     ) -> None:
-    """
-    Wrapper for TrajectoryWriter to write a trajectory to a file.
-
-    if format is None, the default PIMD-QMCF format is used. (see TrajectoryWriter.formats for available formats)
-    if format is 'qmcfc', the QMCFC format is used (see TrajectoryWriter.formats for more information).
-
-    Parameters
-    ----------
-    traj : Trajectory
-        The trajectory to write.
-    filename : str, optional
-        The name of the file to write to. If None, the output is printed to stdout.
-    format : MDEngineFormat | str, optional
-        The format of the md engine for the output file. The default is MDEngineFormat.PIMD_QMCF.
-    type : TrajectoryFormat | str, optional
-        The type of the data to write to the file. Default is TrajectoryFormat.XYZ.
-
-    """
+from PQAnalysis.io.base import BaseWriter
+from PQAnalysis.io.formats import FileWritingMode
+from PQAnalysis.traj import Trajectory, TrajectoryFormat, MDEngineFormat
+from PQAnalysis.core import Cell, Atom
+from PQAnalysis.types import Np2DNumberArray, Np1DNumberArray
+from PQAnalysis.atomic_system import AtomicSystem
+from PQAnalysis.type_checking import runtime_type_checking, runtime_type_checking_setter
 
-    writer = TrajectoryWriter(filename, format=format)
-    writer.write(traj, type=type)
 
 
 class TrajectoryWriter(BaseWriter):
+
     """
     A class for writing a trajectory to a file.
     Inherits from BaseWriter. See BaseWriter for more information.
 
-    It can write a trajectory to a file in either a PIMD-QMCF format or a QMCFC format.
-
-    ...
-
-    Class Attributes
-    ----------------
-    formats : list of str
-        The available formats for the trajectory file.
-
-            #TODO: put this description into formats!!!
-            PIMD-QMCF format for one frame:
-                header line containing the number of atoms and the cell information (if available)
-                arbitrary comment line
-                coordinates of the atoms in the format 'element x y z'
-
-            QMCFC format for one frame:
-                header line containing the number of atoms and the cell information (if available)
-                arbitrary comment line
-                X 0.0 0.0 0.0
-                coordinates of the atoms in the format 'element x y z'
-
-    _type : TrajectoryFormat
-        The type of the data to write to the file. Default is TrajectoryFormat.XYZ.
-
-    Attributes
-    ----------
-    format : MDEngineFormat
-        The format of the md engine for the output file. The default is MDEngineFormat.PIMD_QMCF.
+    It can write a trajectory to a file in either a PQ format or a QMCFC format.
     """
 
-    _format: MDEngineFormat
-    _type: TrajectoryFormat = TrajectoryFormat.XYZ
-
-    def __init__(self,
-                 filename: str | None = None,
-                 format: MDEngineFormat | str = MDEngineFormat.PIMD_QMCF,
-                 mode: str = 'w'
-                 ) -> None:
+    @runtime_type_checking
+    def __init__(
+        self,
+        filename: str | None = None,
+        engine_format: MDEngineFormat | str = MDEngineFormat.PQ,
+        mode: str | FileWritingMode = 'w'
+    ) -> None:
         """
-        It sets the file to write to - either a file or stdout (if filename is None) - and the mode of the file.
-
         Parameters
         ----------
         filename : str, optional
             The name of the file to write to. If None, the output is printed to stdout.
-        format : MDEngineFormat | str, optional
-            The format of the md engine for the output file. The default is MDEngineFormat.PIMD_QMCF.
+        engine_format : MDEngineFormat | str, optional
+            The format of the md engine for the output file. The default is MDEngineFormat.PQ.
         mode : str, optional
-            The mode of the file. Either 'w' for write or 'a' for append.
+            The mode of the file. Either 'w' for write, 
+            'a' for append or 'o' for overwrite. The default is 'w'.
         """
 
-        super().__init__(filename, mode)
+        super().__init__(filename, FileWritingMode(mode))
 
-        self.format = MDEngineFormat(format)
+        self.format = MDEngineFormat(engine_format)
 
-    def write(self, trajectory: Trajectory | Frame, type: TrajectoryFormat | str = TrajectoryFormat.XYZ) -> None:
+    @runtime_type_checking
+    def write(
+        self,
+        trajectory: Trajectory | AtomicSystem,
+        traj_type: TrajectoryFormat | str = TrajectoryFormat.XYZ
+    ) -> None:
         """
         Writes the trajectory to the file.
 
         Parameters
         ----------
-        traj : Trajectory
+        trajectory : Trajectory | AtomicSystem
             The trajectory to write.
+        traj_type : TrajectoryFormat | str, optional
+            The type of the data to write to the file. Default is TrajectoryFormat.XYZ.
         """
 
-        if isinstance(trajectory, Frame):
-            trajectory = Trajectory([trajectory])
+        self.type = TrajectoryFormat(traj_type)
 
-        self._type = TrajectoryFormat(type)
-        if self._type == TrajectoryFormat.XYZ:
-            self.write_positions(trajectory)
-        elif self._type == TrajectoryFormat.VEL:
-            self.write_velocities(trajectory)
-        elif self._type == TrajectoryFormat.FORCE:
-            self.write_forces(trajectory)
-        elif self._type == TrajectoryFormat.CHARGE:
-            self.write_charges(trajectory)
+        if isinstance(trajectory, AtomicSystem):
+            trajectory = Trajectory([trajectory])
 
-        self.close()
+        if self.type == TrajectoryFormat.XYZ:
+            self._write_positions(trajectory)
+        elif self.type == TrajectoryFormat.VEL:
+            self._write_velocities(trajectory)
+        elif self.type == TrajectoryFormat.FORCE:
+            self._write_forces(trajectory)
+        elif self.type == TrajectoryFormat.CHARGE:
+            self._write_charges(trajectory)
 
-    def write_positions(self, trajectory: Trajectory) -> None:
+    def _write_positions(self, trajectory: Trajectory) -> None:
         """
         Writes the positions of the trajectory to the file.
 
         Parameters
         ----------
-        traj : Trajectory
+        trajectory : Trajectory
             The trajectory to write.
         """
-        self._type = TrajectoryFormat.XYZ
         self.open()
         for frame in trajectory:
             self._write_header(frame.n_atoms, frame.cell)
             self._write_comment(frame)
             self._write_xyz(frame.pos, frame.atoms)
 
         self.close()
 
-    def write_velocities(self, trajectory: Trajectory) -> None:
+    def _write_velocities(self, trajectory: Trajectory) -> None:
         """
         Writes the velocities of the trajectory to the file.
 
         Parameters
         ----------
-        traj : Trajectory
+        trajectory : Trajectory
             The trajectory to write.
         """
-        self._type = TrajectoryFormat.VEL
         self.open()
         for frame in trajectory:
             self._write_header(frame.n_atoms, frame.cell)
             self._write_comment(frame)
             self._write_xyz(frame.vel, frame.atoms)
 
         self.close()
 
-    def write_forces(self, trajectory: Trajectory) -> None:
+    def _write_forces(self, trajectory: Trajectory) -> None:
         """
         Writes the forces of the trajectory to the file.
 
         Parameters
         ----------
-        traj : Trajectory
+        trajectory : Trajectory
             The trajectory to write.
         """
-        self._type = TrajectoryFormat.FORCE
         self.open()
         for frame in trajectory:
             self._write_header(frame.n_atoms, frame.cell)
             self._write_comment(frame)
             self._write_xyz(frame.forces, frame.atoms)
 
         self.close()
 
-    def write_charges(self, trajectory: Trajectory) -> None:
+    def _write_charges(self, trajectory: Trajectory) -> None:
         """
         Writes the charges of the trajectory to the file.
 
         Parameters
         ----------
-        traj : Trajectory
+        trajectory : Trajectory
             The trajectory to write.
         """
-        self._type = TrajectoryFormat.CHARGE
         self.open()
         for frame in trajectory:
             self._write_header(frame.n_atoms, frame.cell)
             self._write_comment(frame)
             self._write_scalar(frame.charges, frame.atoms)
 
         self.close()
@@ -212,32 +155,43 @@
             The number of atoms in the frame.
         cell : Cell
             The cell of the frame. Default is Cell().
         """
 
         if cell != Cell():
             print(
-                f"{n_atoms} {cell.x} {cell.y} {cell.z} {cell.alpha} {cell.beta} {cell.gamma}", file=self.file)
+                (
+                f"{n_atoms} "
+                f"{cell.x} {cell.y} {cell.z} "
+                f"{cell.alpha} {cell.beta} {cell.gamma}"
+                ),
+                file=self.file
+            )
         else:
             print(f"{n_atoms}", file=self.file)
 
-    def _write_comment(self, frame: Frame) -> None:
+    def _write_comment(self, frame: AtomicSystem) -> None:
         """
         Writes the comment line of the frame to the file.
 
         Parameters
         ----------
-        frame : Frame
+        frame : AtomicSystem
             The frame to write the comment line of.
         """
 
-        if self._type == TrajectoryFormat.FORCE:
+        if self.type == TrajectoryFormat.FORCE:
             sum_forces = sum(frame.forces)
             print(
-                f"sum of forces: {sum_forces[0]} {sum_forces[1]} {sum_forces[2]}", file=self.file)
+                (
+                f"sum of forces: {sum_forces[0]:e} "
+                f"{sum_forces[1]:e} {sum_forces[2]:e}"
+                ),
+                file=self.file
+            )
         else:
             print("", file=self.file)
 
     def _write_xyz(self, xyz: Np2DNumberArray, atoms: List[Atom]) -> None:
         """
         Writes the xyz of the frame to the file.
 
@@ -250,34 +204,63 @@
         atoms : Elements
             The elements of the frame.
         """
 
         if self.format == MDEngineFormat.QMCFC and self._type == TrajectoryFormat.XYZ:
             print("X   0.0 0.0 0.0", file=self.file)
 
-        for i in range(len(atoms)):
-            print(
-                f"{atoms[i].name} {xyz[i][0]} {xyz[i][1]} {xyz[i][2]}", file=self.file)
-
-    def _write_scalar(self, scalar: Np1DNumberArray, atoms: List[Atom]) -> None:
+        for i, atom in enumerate(atoms):
+            if self.type == TrajectoryFormat.VEL:
+                print(
+                    (
+                    f"{atom.name} {xyz[i][0]:16.12e} "
+                    f"{xyz[i][1]:16.12e} {xyz[i][2]:16.12e}"
+                    ),
+                    file=self.file
+                )
+            else:
+                print(
+                    (
+                    f"{atom.name} {xyz[i][0]:16.10f} "
+                    f"{xyz[i][1]:16.10f} {xyz[i][2]:16.10f}"
+                    ),
+                    file=self.file
+                )
+
+    def _write_scalar(
+        self,
+        scalar: Np1DNumberArray,
+        atoms: List[Atom]
+    ) -> None:
         """
         Writes the charges of the frame to the file.
 
         Parameters
         ----------
         scalar : np.array
             scalar data of the atoms (atm only charges).
         atoms : Elements
             The elements of the frame.
         """
 
-        for i in range(len(atoms)):
-            print(
-                f"{atoms[i].name} {scalar[i]}", file=self.file)
+        for i, atom in enumerate(atoms):
+            print(f"{atom.name} {scalar[i]}", file=self.file)
 
     @property
     def format(self) -> MDEngineFormat:
+        """MDEngineFormat: The format of the md engine for the output file."""
         return self._format
 
     @format.setter
-    def format(self, format: MDEngineFormat | str) -> None:
-        self._format = MDEngineFormat(format)
+    @runtime_type_checking_setter
+    def format(self, engine_format: MDEngineFormat | str) -> None:
+        self._format = MDEngineFormat(engine_format)
+
+    @property
+    def type(self) -> TrajectoryFormat:
+        """TrajectoryFormat: The type of the data to write to the file."""
+        return self._type
+
+    @type.setter
+    @runtime_type_checking_setter
+    def type(self, traj_type: TrajectoryFormat | str) -> None:
+        self._type = TrajectoryFormat(traj_type)
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/physicalData/energy.py` & `pqanalysis-1.0/PQAnalysis/physical_data/energy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,103 @@
 """
 A module containing the Energy class.
+"""
 
-...
+import logging
 
-Classes
--------
-Energy
-    A class to store the data of an energy file.
-"""
+from collections import defaultdict
 
 import numpy as np
 
 from beartype.typing import Dict
-from collections import defaultdict
 
-from . import EnergyError
-from ..types import Np2DNumberArray, Np1DNumberArray
+from PQAnalysis.types import Np2DNumberArray, Np1DNumberArray
+from PQAnalysis.utils.custom_logging import setup_logger
+from PQAnalysis import __package_name__
+from PQAnalysis.type_checking import runtime_type_checking
+
+from .exceptions import EnergyError
+
 
 
 class Energy():
+
     """
     A class to store the data of an energy file.
 
     The data array is stored in a way that each column corresponds to a physical
     quantity. The order of the columns is the same as in the info file. The info
     and units of the info file are stored in the Energy object, if an info file
     was found.
-
-    Attributes
-    ----------
-    data : np.array
-        The data of the energy file as a np.array with shape (n, m), where n is the
-        number of data entries and m is the number of physical properties.
-    info : dict
-        The information strings of the info file as a dictionary.
-        The keys are the names of the information strings. The values are the
-        corresponding data entry (columns in energy file).
-    units : dict
-        The units of the info file as a dictionary. The keys are the names of the
-        information strings. The values are the corresponding units.
-    info_given : bool
-        A info dictionary was given.
-    units_given : bool
-        A units dictionary was given.
     """
 
-    def __init__(self,
-                 data: Np1DNumberArray | Np2DNumberArray,
-                 info: Dict | None = None,
-                 units: Dict | None = None
-                 ) -> None:
-        """
-        Creates an Energy object.
+    logger = logging.getLogger(__package_name__).getChild(__qualname__)
+    logger = setup_logger(logger)
 
+    @runtime_type_checking
+    def __init__(
+        self,
+        data: Np1DNumberArray | Np2DNumberArray,
+        info: Dict | None = None,
+        units: Dict | None = None
+    ) -> None:
+        """
         Parameters
         ----------
-        data : np.array
+        data : Np1DNumberArray | Np2DNumberArray
             The data of the energy file as a np.array with shape (n, m), where n is the
             number of data entries and m is the number of physical properties. If the data
             is a 1D array, it is converted to a 2D array with shape (1, n).
         info : dict, optional
             the info dictionary, by default None
         units : dict, optional
             the units dictionary, by default None
+
+        Notes
+        -----
+        If no info dictionary is given, a default dictionary is created,
+        where the keys are the indices of the data array and the values 
+        are the indices of the data array. Furthermore a units dictionary
+        can be given, where the keys have to match the keys of the info
+        dictionary and the values are the units of the physical properties.
+        If no units dictionary is given, the units are set to None.
+
+        The attributes of any Energy object are created for each physical
+        property found in the info file. The attribute names can be found 
+        in the __data_attributes__ dictionary. The attribute names are the
+        keys of the dictionary and the values are the names of the physical 
+        properties found in the info file. The attributes are created
+        as follows:
+
+        - The attribute name is the key of the __data_attributes__ dictionary.
+        - The attribute value is the corresponding data entry (column in energy file).
+        - The attribute name + "_unit" is the corresponding unit.
+        - The attribute name + "_with_unit" is a tuple of the corresponding data entry
+          and the corresponding unit.
+
+        For example, the attribute "simulation_time" is created for the physical property
+        "SIMULATION-TIME" found in the info file. The attribute "simulation_time" is the
+        corresponding data entry (column in energy file). The attribute "simulation_time_unit"
+        is the corresponding unit. The attribute "simulation_time_with_unit" is a tuple of
+        the corresponding data entry and the corresponding unit.
         """
         if len(np.shape(data)) == 1:
             data = np.array([data])
 
         self.data = np.array(data)
 
-        self.__setup_info_dictionary__(info, units)
+        self._setup_info_dictionary(info, units)
 
-        self.__make_attributes__()
+        self._make_attributes()
 
-    def __setup_info_dictionary__(self, info: Dict | None = None, units: Dict | None = None) -> None:
+    def _setup_info_dictionary(
+        self,
+        info: Dict | None = None,
+        units: Dict | None = None
+    ) -> None:
         """
         Sets up the info dictionary.
 
         If no info dictionary is given, a default dictionary is created, where
         the keys are the indices of the data array and the values are the indices
         of the data array. Furthermore a units dictionary can be given, where the
         where the keys have to match the keys of the info dictionary and the values
@@ -107,34 +127,41 @@
 
         if info is None:
             self.info_given = False
             info = defaultdict(lambda: None)
         else:
             self.info_given = True
             if len(info) != len(self.data):
-                raise EnergyError(
-                    "The length of info dictionary has to be equal to the length of data.")
+                self.logger.error(
+                    "The length of info dictionary has to be equal to the length of data.",
+                    exception=EnergyError
+                )
 
         if units is None:
             self.units_given = False
             units = defaultdict(lambda: None)
         else:
             self.units_given = True
             if len(units) != len(self.data):
-                raise EnergyError(
-                    "The length of units dictionary has to be equal to the length of data.")
+                self.logger.error(
+                    "The length of units dictionary has to be equal to the length of data.",
+                    exception=EnergyError
+                )
 
         self.info = info
         self.units = units
 
-        if self.info_given and self.units_given and units.keys() != info.keys():
-            raise EnergyError(
-                "The keys of the info and units dictionary do not match.")
+        if self.info_given and self.units_given and units.keys() != info.keys(
+        ):
+            self.logger.error(
+                "The keys of the info and units dictionary do not match.",
+                exception=EnergyError
+            )
 
-    def __make_attributes__(self) -> None:
+    def _make_attributes(self) -> None:
         """
         Creates attributes for the physical properties of the Energy object.
 
         The attributes are created for each physical property found in the info file.
         The attribute names can be found in the __data_attributes__ dictionary. The
         attribute names are the keys of the dictionary and the values are the names
         of the physical properties found in the info file. The attributes are created
@@ -148,23 +175,26 @@
 
         For example, the attribute "simulation_time" is created for the physical property
         "SIMULATION-TIME" found in the info file. The attribute "simulation_time" is the
         corresponding data entry (column in energy file). The attribute "simulation_time_unit"
         is the corresponding unit. The attribute "simulation_time_with_unit" is a tuple of
         the corresponding data entry and the corresponding unit.
         """
-        for attribute in self.__data_attributes__:
+
+        for attribute, value in self.__data_attributes__.items():
             info_string = attribute
             if info_string in self.info or info_string in self.units:
-                setattr(self, self.__data_attributes__[attribute],
-                        self.data[self.info[attribute]])
-                setattr(self, self.__data_attributes__[attribute] + "_unit",
-                        self.units[attribute])
-                setattr(self, self.__data_attributes__[attribute] + "_with_unit", (self.data[self.info[
-                        attribute]], self.units[attribute]))
+                setattr(self, value, self.data[self.info[attribute]])
+                setattr(self, value + "_unit", self.units[attribute])
+                setattr(
+                    self,
+                    value + "_with_unit",
+                    (self.data[self.info[attribute]],
+                    self.units[attribute])
+                )
 
     ################################################
     #                                              #
     # from here all attributes possible are listed #
     #                                              #
     ################################################
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/tools/traj_to_com_traj.py` & `pqanalysis-1.0/PQAnalysis/tools/traj_to_com_traj.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 """
 A module containing the tool to compute a center of mass trajectory for a given selection.
 """
 
-from ..traj import Trajectory
+from PQAnalysis.traj import Trajectory
+from PQAnalysis.type_checking import runtime_type_checking
 
 
-# TODO: add atom to element mapper if atomname not element names
+
+# TODO: add atom to element mapper if atom name not element names
 # TODO rethink concept of selection/getitem/slices
-def traj_to_com_traj(trajectory: Trajectory, selection=None, group=None) -> Trajectory:
+@runtime_type_checking
+def traj_to_com_traj(
+    trajectory: Trajectory,
+    selection=None,
+    group=None
+) -> Trajectory:
     """
     Function that computes the center of mass trajectory for a given selection.
 
     With the group parameter, the trajectory will be group according to the given group.
     For example if group = 2, the trajectory will be grouped in pairs of 2 and the center 
     of mass of each pair will be computed.
 
     Parameters
     ----------
     trajectory : Trajectory
         The trajectory to compute the center of mass trajectory for.
     selection : Selection, optional
-        The selection to compute the center of mass trajectory for. If None, the selection is all atoms.
+        The selection to compute the center of mass trajectory for. 
+        If None, the selection is all atoms.
     group : int, optional
-        The group to compute the center of mass trajectory for. If None, the group is all atoms.
+        The group to compute the center of mass trajectory for.
+        If None, the group is all atoms.
     """
 
     if len(trajectory) == 0:
         return Trajectory()
 
     com_traj = Trajectory()
     for frame in trajectory:
 
         if selection is None:
             selection = slice(0, frame.n_atoms)
 
         frame = frame[selection]
-        com_traj.append(frame.compute_com_frame(group=group))
+        com_traj.append(frame.compute_com_atomic_system(group=group))
 
     return com_traj
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/topology/shakeTopology.py` & `pqanalysis-1.0/PQAnalysis/io/conversion_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,178 +1,237 @@
 """
-A module containing the ShakeTopologyGenerator class.
-
-...
-
-Classes
--------
-ShakeTopologyGenerator
-    A class for generating the shake topology for a given trajectory.
+A module containing API functions to convert between different file formats.
 """
-import numpy as np
 
 from beartype.typing import List
 
-from ..core import Atom
-from ..traj import Trajectory
-from ..types import Np1DIntArray, Np2DIntArray, Np1DNumberArray
-from ..io import BaseWriter
+from PQAnalysis.core import Cell
+from PQAnalysis.traj import MDEngineFormat
+from PQAnalysis.io.formats import FileWritingMode
+from PQAnalysis.type_checking import runtime_type_checking
+
+from .traj_file import (
+    TrajectoryWriter,
+    TrajectoryReader,
+)
+from .box_writer import BoxWriter
+from .formats import BoxFileFormat
+from .gen_file import (
+    write_gen_file,
+    read_gen_file,
+)
+from .restart_file.api import read_restart_file
+from .traj_file.api import write_trajectory
+
+
+
+@runtime_type_checking
+def gen2xyz(
+    gen_file: str,
+    output: str | None = None,
+    md_format: MDEngineFormat | str = MDEngineFormat.PQ,
+    print_box: bool = True,
+    mode: FileWritingMode | str = "w"
+) -> None:
+    """
+    Converts a gen file to a xyz file and prints it to stdout or writes it to a file.
+
+    Parameters
+    ----------
+    gen_file : str
+        The gen file to be converted.
+    output : str | None
+        The output file. If not specified, the output is printed to stdout.
+    md_format : MDEngineFormat | str, optional
+        The format of the md engine for the output file. The default is MDEngineFormat.PQ.
+    print_box : bool, optional
+        If True, the box is not printed. If False, the box is printed. Default is False.
+    mode : FileWritingMode | str, optional
+        The writing mode, by default "w". The following modes are available:
+        - "w": write
+        - "a": append
+        - "o": overwrite
+    """
+    system = read_gen_file(gen_file)
+
+    if not print_box:
+        system.cell = Cell()
+
+    write_trajectory(
+        system,
+        output,
+        engine_format=md_format,
+        traj_type="xyz",
+        mode=mode
+    )
+
 
 
-class ShakeTopologyGenerator:
+@runtime_type_checking
+def xyz2gen(
+    xyz_file: str,
+    output: str | None = None,
+    periodic: bool | None = None,
+    mode: FileWritingMode | str = "w",
+    md_format: MDEngineFormat | str = MDEngineFormat.PQ,
+) -> None:
     """
-    A class for generating the shake topology for a given trajectory.
+    Converts a xyz file to a gen file and prints it to stdout or writes it to a file.
 
-    Attributes
+    Parameters
     ----------
-    indices : Np1DIntArray
-        The indices of the atoms to use for the topology.
-    target_indices : Np1DIntArray
-        The indices of the target atoms for the shaked atoms.
-    distances : Np1DNumberArray
-        The average distances between the shaked atoms and the target atoms.
-    """
-
-    def __init__(self,
-                 atoms: List[Atom] | List[str] | Np1DIntArray | None = None,
-                 use_full_atom_info: bool = False
-                 ) -> None:
-        """
-        Initializes the ShakeTopologyGenerator with the given parameters.
-
-        It can be initialized with a list of atoms, a list of atom names, or a numpy 1d array of atom indices or None.
-
-            - If atoms is None shake distances for all atoms in the system will be computed.
-
-            - If atoms is a list of atoms, shake distances for the given atoms will be computed.
-              For the list of atoms, and additional parameter use_full_atom_info can be given, which
-              determines if the full atom information (name, index, mass) is used for the selection or 
-              only the element type.
-
-            - If atoms is a list of atom names, shake distances for the given atom type names will be computed.
-
-            - If atoms is a numpy 1d array of atom indices, shake distances for the given atom indices will be computed.
-
-        Parameters
-        ----------
-        atoms : List[Atom] | List[str] | Np1DIntArray | None, optional
-            The atoms to use for the topology, by default None
-        use_full_atom_info : bool, optional
-            If True, the full atom information (name, index, mass) is used for the selection, by default False
-            Is always ignored if atoms is not a list of atom objects.
-        """
-
-        self._use_full_atom_info = False
-
-        if atoms is None:
-            self.atoms = None
-        elif isinstance(atoms[0], Atom):
-            self.atoms = atoms
-            self._use_full_atom_info = use_full_atom_info
-        elif isinstance(atoms[0], str):
-            self.atoms = [Atom(name) for name in atoms]
-        else:
-            self.atoms = atoms
-
-    def generate_topology(self, trajectory: Trajectory) -> None:
-        """
-        Generates a tuple of indices, target_indices, and distances for the given trajectory.
-
-        The generated numpy arrays represent all important information about the shake topology for the given trajectory.
-
-            - indices: The indices of the atoms to use for the topology.
-            - target_indices: The indices of the target atoms for the shaked atoms.
-            - distances: The average distances between the shaked atoms and the target atoms.
-
-        Parameters
-        ----------
-        trajectory : Trajectory
-            The trajectory to generate the shake topology for.
-        """
-
-        start_frame = trajectory[0]
-        target_indices, distances = start_frame.system.nearest_neighbours(
-            n=1, atoms=self.atoms, use_full_atom_info=self._use_full_atom_info)
-
-        target_indices = target_indices.flatten()
-        distances = distances.flatten()
-
-        indices = start_frame.system.indices_from_atoms(
-            self.atoms, use_full_atom_info=self._use_full_atom_info)
-
-        distances = [distances]
-
-        for frame in trajectory[1:]:
-            pos = frame.pos[indices]
-            target_pos = frame.pos[target_indices]
-
-            delta_pos = pos - target_pos
-
-            delta_pos = frame.cell.image(delta_pos)
-
-            distances.append(np.linalg.norm(delta_pos, axis=1))
-
-        self.indices = indices
-        self.target_indices = target_indices
-        self.distances = np.mean(np.array(distances), axis=0)
-
-    def average_equivalents(self, indices: List[Np1DIntArray] | Np2DIntArray) -> None:
-        """
-        Averages the distances for equivalent atoms.
-
-        The parameter indices is a numpy 2d array of equivalent atom indices.
-        Each row of the array contains the indices of equivalent atoms.
-        All of the equivalent atoms will be averaged to a single distance.
-
-        Parameters
-        ----------
-        indices : List[Np1DIntArray] | Np2DIntArray
-            The indices of the equivalent atoms.
-        """
-
-        for equivalent_indices in indices:
-            _indices = np.nonzero(np.in1d(self.indices, equivalent_indices))[0]
-
-            mean_distance = np.mean(self.distances[_indices])
-
-            self.distances[_indices] = mean_distance
-
-    def write_topology(self, filename: str | None = None) -> None:
-        """
-        Writes the topology to a file.
-
-        The topology is written to a file with the given filename.
-        The file will contain the indices, target_indices, and distances of the topology.
-        If no filename is given, the topology will be written to stdout.
-
-        Parameters
-        ----------
-        filename : str
-            The filename to write the topology to.
-        """
-
-        writer = BaseWriter(filename)
-        writer.open()
-
-        print(
-            f"SHAKE {len(self.indices)}  {len(np.unique(self.target_indices))}  0", file=writer.file)
-        for i, index in enumerate(self.indices):
-            target_index = self.target_indices[i]
-            distance = self.distances[i]
-
-            print(f"{index+1} {target_index+1} {distance}", file=writer.file)
-
-        print("END", file=writer.file)
-
-    @property
-    def atoms(self) -> List[Atom] | Np1DIntArray | None:
-        """
-        The atoms to use for the topology.
-        """
-        return self._atoms
-
-    @atoms.setter
-    def atoms(self, atoms: List[Atom] | Np1DIntArray | None) -> None:
-        """
-        Sets the atoms to use for the topology.
-        """
-        self._atoms = atoms
+    xyz_file : str
+        The xyz file to be converted.
+    output : str | None
+        The output file. If not specified, the output is printed to stdout.
+    periodic : bool | None, optional
+        The periodicity of the system. If True, the system is considered periodic.
+        If False, the system is considered non-periodic. If None, the periodicity 
+        is inferred from the system, by default None.
+    mode : FileWritingMode | str, optional
+        The writing mode, by default "w". The following modes are available:
+        - "w": write
+        - "a": append
+        - "o": overwrite
+    md_format : MDEngineFormat | str, optional
+        The format of the md engine for the output file. The default is MDEngineFormat.PQ.
+    """
+
+    system = TrajectoryReader(
+        xyz_file,
+        md_format=md_format,
+        traj_format="xyz"
+    ).read()
+
+    write_gen_file(output, system, periodic, mode)
+
+
+
+@runtime_type_checking
+def rst2xyz(
+    restart_file: str,
+    output: str | None = None,
+    print_box: bool = True,
+    md_format: MDEngineFormat | str = MDEngineFormat.PQ,
+    mode: FileWritingMode | str = "w"
+) -> None:
+    """
+    Converts a restart file to a xyz file and prints it to stdout or writes it to a file.
+
+    When the print_box flag is set to True, the box is printed as well.
+    This means that after the number of atoms the box is printed in the
+    same line in the format a b c alpha beta gamma.
+
+    Parameters
+    ----------
+    restart_file : str
+        The restart file to be converted.
+    output : str | None
+        The output file. If not specified, the output is printed to stdout.
+    print_box : bool
+        If True, the box is printed. If False, the box is not printed. Default is True.
+    md_format : MDEngineFormat | str, optional
+        The format of the md engine for the output file. The default is MDEngineFormat.PQ.
+    mode : FileWritingMode | str, optional
+        The writing mode, by default "w". The following modes are available:
+        - "w": write
+        - "a": append
+        - "o": overwrite
+    """
+    system = read_restart_file(restart_file)
+
+    if not print_box:
+        system.cell = Cell()
+
+    write_trajectory(
+        system,
+        output,
+        engine_format=md_format,
+        traj_type="xyz",
+        mode=mode
+    )
+
+
+
+@runtime_type_checking
+def traj2box(
+    trajectory_files: List[str],
+    vmd: bool,
+    output: str | None = None,
+    mode: FileWritingMode | str = "w"
+) -> None:
+    """
+    Converts multiple trajectory files to a box file and 
+    prints it to stdout or writes it to a file.
+
+    Without the vmd option the output is printed in a data file format.
+    The first column represents the step starting from 1, the second to fourth column
+    represent the box vectors a, b, c, the fifth to seventh column represent the box angles.
+
+    With the vmd option the output is printed in a VMD file format. Meaning the output is
+    in xyz format with 8 particle entries representing the vertices of the box. The comment
+    line contains the information about the box dimensions a, b and c and the box angles.
+
+    Parameters
+    ----------
+    trajectory_files : list of str
+        The trajectory file(s) to be converted.
+    vmd : bool
+        Output in VMD format.
+    output : str | None, optional
+        The output file. If not specified, the output is printed to stdout. Default is None.
+    mode : FileWritingMode | str, optional
+        The writing mode, by default "w". The following modes are available:
+        - "w": write
+        - "a": append
+        - "o": overwrite
+    """
+
+    if vmd:
+        output_format = BoxFileFormat.VMD
+    else:
+        output_format = BoxFileFormat.DATA
+
+    writer = BoxWriter(filename=output, output_format=output_format, mode=mode)
+
+    for filename in trajectory_files:
+        reader = TrajectoryReader(filename)
+        trajectory = reader.read()
+
+        writer.write(trajectory, reset_counter=False)
+
+
+
+@runtime_type_checking
+def traj2qmcfc(
+    trajectory_files: List[str],
+    output: str | None = None,
+    mode: FileWritingMode | str = "w"
+) -> None:
+    """
+    Converts multiple trajectory files from a PQ format to a 
+    QMCFC format and prints it to stdout or writes it to a file.
+
+    Parameters
+    ----------
+    trajectory_files : list of str
+        The trajectory file(s) to be converted.
+    output : str, optional
+        The output file. If not specified, the output is printed to stdout.
+    mode : FileWritingMode | str, optional
+        The writing mode, by default "w". The following modes are available:
+        - "w": write
+        - "a": append
+        - "o": overwrite
+    """
+
+    writer = TrajectoryWriter(
+        filename=output,
+        engine_format="qmcfc",
+        mode=mode
+    )
+
+    for filename in trajectory_files:
+        reader = TrajectoryReader(filename)
+        trajectory = reader.read()
+
+        writer.write(trajectory)
```

### Comparing `pqanalysis-0.5.2/PQAnalysis/traj/formats.py` & `pqanalysis-1.0/PQAnalysis/formats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,18 @@
 """
-A module containing different format types of the trajectory.
-
-...
-
-Classes
--------
-Format
-    An enumeration super class of the various supported trajectory formats.
-TrajectoryFormat
-    An enumeration of the supported trajectory formats.
-MDEngineFormat
-    An enumeration of the supported MD engine formats.
+A module containing the base class for all Format enumerations.
 """
 
 from enum import Enum
-from beartype.typing import Any
+from beartype.typing import Any, List
 
-from . import TrajectoryFormatError, MDEngineFormatError
 
 
-class Format(Enum):
+class BaseEnumFormat(Enum):
+
     """
     An enumeration super class of the various supported trajectory formats.
     """
 
     @classmethod
     def member_repr(cls) -> str:
         """
@@ -36,99 +25,67 @@
         """
 
         return ', '.join([str(member) for member in cls])
 
     @classmethod
     def value_repr(cls) -> str:
         """
-        This method returns a string representation of the values of the members of the enumeration.
+        This method returns a string representation of
+        the values of the members of the enumeration.
 
         Returns
         -------
         str
             A string representation of the values of the members of the enumeration.
         """
 
         return ', '.join([str(member.value) for member in cls])
 
-
-class TrajectoryFormat(Format):
-    """
-    An enumeration of the supported trajectory formats.
-
-    ...
-
-    Attributes
-    ----------
-    XYZ : str
-        The XYZ format.
-    VEL : str
-        The VEL format.
-    FORCE : str
-        The FORCE format.
-    CHARGE : str
-        The CHARGE format.
-    """
-
-    XYZ = "XYZ"
-    VEL = "VEL"
-    FORCE = "FORCE"
-    CHARGE = "CHARGE"
-
     @classmethod
-    def _missing_(cls, value: object) -> Any:
+    def _missing_(cls, value: object, exception: type(Exception)) -> Any:  # pylint: disable=arguments-differ
         """
-        This method allows a TrajectoryFormat to be retrieved from a string.
+        This method allows a FileWriteMode to be retrieved from a string.
+
+        Parameters
+        ----------
+        value : object
+            The value to return.
+        exception : Exception
+            The exception to raise if the value is not found.
+
+        Raises
+        ------
+        exception
+            If the value is not found.
         """
         value = value.lower()
+
         for member in cls:
             if member.value.lower() == value:
                 return member
 
-        raise TrajectoryFormatError(value, cls)
-
-
-class MDEngineFormat(Format):
-    """
-    An enumeration of the supported MD engine formats.
-
-    ...
-
-    Attributes
-    ----------
-    PIMD-QMCF: str
-        The PIMD-QMCF format.
-    QMCFC: str
-        The QMCFC format.
-    """
-
-    PIMD_QMCF = "PIMD-QMCF"
-    QMCFC = "QMCFC"
+        raise exception(value, cls)
 
     @classmethod
-    def _missing_(cls, value: object) -> Any:
+    def values(cls) -> List[str]:
         """
-        This method allows an MDEngineFormat format to be retrieved from a string.
+        This method returns a list of all values of the enumeration.
+
+        Returns
+        -------
+        List[str]
+            A list of all values of the enumeration.
         """
-        value = value.lower()
-        for member in cls:
-            if member.value.lower() == value:
-                return member
 
-        raise MDEngineFormatError(value, cls)
+        return [member.value for member in cls]
 
-    @classmethod
-    def isQMCFType(cls, format: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
+        """
+        Checks if the given EnumFormat is equal to this Format or not.
         """
-        This method checks if the given format is a QMCF format.
 
-        Parameters
-        ----------
-        format : Any
-            The format to check.
+        if not isinstance(other, type(self)) and not isinstance(other, str):
+            return False
 
-        Returns
-        -------
-        bool
-            True if the format is a QMCF format, False otherwise.
-        """
-        return format in [cls.PIMD_QMCF, cls.QMCFC]
+        other = type(self)(other)
+
+        return self.value == other.value
```

### Comparing `pqanalysis-0.5.2/README.md` & `pqanalysis-1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PQAnalysis
 
 [![CI](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml/badge.svg)](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml)
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-The main purpose of this package is to provide useful tools for the analysis of the Molecular Dynamics software package [PIMD-QMCF](https://github.com/MolarVerse/pimd_qmcf). Furthermore, the intent of this package is to enable straightforward implementations of newly developed analysis tools on top of the provided API.
+The main purpose of this package is to provide useful tools for the analysis of the Molecular Dynamics software package [PQ](https://github.com/MolarVerse/PQ). Furthermore, the intent of this package is to enable straightforward implementations of newly developed analysis tools on top of the provided API.
 
 The future development of this package focuses on two main goals. On the one hand the enhancement of the provided analysis tools and extending its API to be compatible with many other different Molecular Dynamics engines. As this project is only a *hobby* project of the maintainers, any contributions considering enhancement or bug fixes are highly welcomed.
```

### Comparing `pqanalysis-0.5.2/docs/Makefile` & `pqanalysis-1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/docs/make.bat` & `pqanalysis-1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/docs/source/logo/PQAnalysis.png` & `pqanalysis-1.0/docs/source/logo/PQAnalysis.png`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/examples/traj2box/acof_triclinic.xyz` & `pqanalysis-1.0/examples/traj2box/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/examples/traj2box/acof_triclinic_2.xyz` & `pqanalysis-1.0/examples/traj2box/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/examples/traj2comtraj/umcm-9-md-01.xyz` & `pqanalysis-1.0/examples/traj2comtraj/umcm-9-md-01.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/pyproject.toml` & `pqanalysis-1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -8,46 +8,65 @@
     "version"
 ]
 authors = [
   { name="Jakob Gamper", email="97gamjak@gmail.com" },
   { name="Josef M. Gallmetzer", email="gallmetzer.josef@gmail.com" },
   { name="Clarissa A. Seidler", email="clarissa.seidler@gmail.com" },
 ]
-description = "PQAnalysis is a python package for the analysis of PIMD-QMCF simulations."
-requires-python = ">=3.10"
+description = "PQAnalysis is a python package for the analysis of PQ simulations."
+requires-python = ">=3.12"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "numpy",
+    "scipy",
     "beartype",
     "multimethod",
+    "lark",
+    "tqdm",
+    "decorator",
+    "argcomplete",
+    "yapf",
+    "rich-argparse",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "coverage",
-    "pytest-cov"
+    "pytest-cov",
+    "pylint",
+    "pylint-django",
+    "docstr-coverage",
 ]
 docs = [
     "sphinx",
     "sphinx-sitemap",
     "myst-parser",
-    "sphinx-rtd-theme"
+    "sphinx-rtd-theme",
+    "better-apidoc",
+    "six",
+    "docstr-coverage",
 ]
 
 [tool.setuptools_scm]
 version_file = "PQAnalysis/_version.py"
 
 [project.scripts]
+pqanalysis = "PQAnalysis.cli.main:main"
 traj2box = "PQAnalysis.cli.traj2box:main"
 traj2qmcfc = "PQAnalysis.cli.traj2qmcfc:main"
 rst2xyz = "PQAnalysis.cli.rst2xyz:main"
+continue_input = "PQAnalysis.cli.continue_input:main"
+rdf = "PQAnalysis.cli.rdf:main"
+add_molecules = "PQAnalysis.cli.add_molecules:main"
+activate_argcomplete = "PQAnalysis.cli.activate_argcomplete:main"
+build_nep_traj = "PQAnalysis.cli.build_nep_traj:main"
 
 [project.urls]
 "Homepage" = "https://github.com/MolarVerse/PQAnalysis"
-"PIMD-QMCF" = "https://github.com/MolarVerse/pimd_qmcf"
+"PQ" = "https://github.com/MolarVerse/PQ"
```

### Comparing `pqanalysis-0.5.2/tests/cli/test_traj2qmcfc.py` & `pqanalysis-1.0/tests/cli/test_traj2qmcfc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 import pytest
-import sys
-import argparse
 
 from filecmp import cmp as filecmp
 from unittest import mock
 
 from PQAnalysis.cli.traj2qmcfc import traj2qmcfc, main
 
+from . import ArgparseNamespace
+
+
 
 @pytest.mark.parametrize("example_dir", ["traj2qmcfc"], indirect=False)
 def test_traj2qmcfc(test_with_data_dir):
-    traj2qmcfc(trajectory_files=[
-        "acof_triclinic.xyz", "acof_triclinic_2.xyz"], output="test_traj.qmcfc.xyz")
+    traj2qmcfc(
+        trajectory_files=["acof_triclinic.xyz",
+        "acof_triclinic_2.xyz"],
+        output="test_traj.qmcfc.xyz"
+    )
 
     assert filecmp("traj.qmcfc.xyz", "test_traj.qmcfc.xyz")
 
 
+
 @pytest.mark.parametrize("example_dir", ["traj2qmcfc"], indirect=False)
 def test_main(test_with_data_dir):
     main_traj2qmcfc()
 
 
-@mock.patch('argparse.ArgumentParser.parse_args',
-            return_value=argparse.Namespace(trajectory_file=["acof_triclinic.xyz",
-                                                             "acof_triclinic_2.xyz"], vmd=False, output="test_traj.qmcfc.xyz"))
+
+@mock.patch(
+    'argparse.ArgumentParser.parse_args',
+    return_value=ArgparseNamespace(
+    trajectory_file=["acof_triclinic.xyz",
+    "acof_triclinic_2.xyz"],
+    vmd=False,
+    output="test_traj.qmcfc.xyz",
+    log_file=None,
+    logging_level="INFO",
+    )
+)
 def main_traj2qmcfc(mock_args):
     main()
     assert filecmp("traj.qmcfc.xyz", "test_traj.qmcfc.xyz")
```

### Comparing `pqanalysis-0.5.2/tests/core/test_atom.py` & `pqanalysis-1.0/tests/core/atom/test_atom.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,25 @@
 import pytest
 import numpy as np
 
 from multimethod import DispatchError
 
-from PQAnalysis.core.atom import Atom, guess_element
-from PQAnalysis.core.exceptions import ElementNotFoundError
+from PQAnalysis.core.atom import Atom, Element
+from PQAnalysis.core.exceptions import ElementNotFoundError, AtomError
+from PQAnalysis.type_checking import get_type_error_message
+from PQAnalysis.exceptions import PQTypeError
 
+from .. import pytestmark
+from ...conftest import assert_logging_with_exception
 
-def test_guess_element():
-    with pytest.raises(ElementNotFoundError) as exception:
-        guess_element("CH")
-    assert str(exception.value) == "Id CH is not a valid element identifier."
-
-    with pytest.raises(ElementNotFoundError) as exception:
-        guess_element(-1)
-    assert str(exception.value) == "Id -1 is not a valid element identifier."
-
-    symbol, atomic_number, mass = guess_element('C')
-    assert symbol == 'c'
-    assert atomic_number == 6
-    assert np.isclose(mass, 12.0107)
-
-    symbol, atomic_number, mass = guess_element(6)
-    assert symbol == 'c'
-    assert atomic_number == 6
-    assert np.isclose(mass, 12.0107)
 
 
 class TestAtom:
-    def test__init__(self):
+
+    def test__init__(self, caplog):
         element = Atom('C')
         assert element.symbol == 'c'
         assert element.atomic_number == 6
         assert np.isclose(element.mass, 12.0107)
 
         element = Atom(2)
         assert element.symbol == 'he'
@@ -53,25 +40,56 @@
 
         element = Atom('C1', use_guess_element=False)
         assert element.name == 'C1'
         assert element.symbol is None
         assert element.atomic_number is None
         assert element.mass is None
 
-        with pytest.raises(ElementNotFoundError) as exception:
-            Atom('C1')
-        assert str(exception.value) == "Id C1 is not a valid element identifier."
-
-        with pytest.raises(DispatchError) as exception:
-            Atom(1.2)
-
-        with pytest.raises(ElementNotFoundError) as exception:
-            Atom(-1)
-        assert str(
-            exception.value) == "Id -1 is not a valid element identifier."
+        assert_logging_with_exception(
+            caplog,
+            Element.__qualname__,
+            "ERROR",
+            "Id C1 is not a valid element identifier.",
+            ElementNotFoundError,
+            Atom,
+            'C1'
+        )
+
+        assert_logging_with_exception(
+            caplog,
+            "TypeChecking",
+            "ERROR",
+            get_type_error_message("name",
+            1.2,
+            str | int),
+            PQTypeError,
+            Atom,
+            1.2
+        )
+
+        assert_logging_with_exception(
+            caplog,
+            Element.__qualname__,
+            "ERROR",
+            "Id -1 is not a valid element identifier.",
+            ElementNotFoundError,
+            Atom,
+            -1
+        )
+
+        assert_logging_with_exception(
+            caplog,
+            Atom.__qualname__,
+            "ERROR",
+            "The name of the atom_type cannot be an integer if the id is given.",
+            AtomError,
+            Atom,
+            1,
+            2
+        )
 
     def test__eq__(self):
         element1 = Atom('C')
         element2 = Atom('C', 6)
         element3 = Atom('H')
         assert element1 == element2
         assert element1 != element3
@@ -81,7 +99,11 @@
     def test__str__(self):
         element = Atom('C')
         assert str(element) == 'Atom(C, 6, c, 12.0107)'
 
     def test__repr__(self):
         element = Atom('C')
         assert repr(element) == str(element)
+
+    def test_property_element(self):
+        element = Atom('C')
+        assert element.element == Element('C')
```

### Comparing `pqanalysis-0.5.2/tests/data/readEnergyFile/md-01.info` & `pqanalysis-1.0/tests/data/readEnergyFile/md-01.info`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 -----------------------------------------------------------------------------------------
-|                                  PIMD-QMCF info file                                  |
+|                                  PQ info file                                  |
 -----------------------------------------------------------------------------------------
 |   SIMULATION-TIME         5.00000 ps       TEMPERATURE           294.45308 K          |
 |   PRESSURE             2875.71714 bar      E(TOT)            -186008.40141 kcal/mol   |
 |   E(QM)             -186197.10854 kcal/mol N(QM-ATOMS)             0.00000 -          |
 |   E(KIN)                188.70714 kcal/mol E(INTRA)                0.00000 kcal/mol   |
 |   VOLUME               4310.41014 A^3      DENSITY                 0.83455 g/cm^3     |
 |   MOMENTUM                2.5e-10 amuA/fs  LOOPTIME                0.90443 s          |
```

### Comparing `pqanalysis-0.5.2/tests/data/readInfoFile/md-01.info` & `pqanalysis-1.0/tests/data/readInfoFile/md-01.info`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 -----------------------------------------------------------------------------------------
-|                                  PIMD-QMCF info file                                  |
+|                                  PQ info file                                  |
 -----------------------------------------------------------------------------------------
 |   SIMULATION-TIME         5.00000 ps       TEMPERATURE           294.45308 K          |
 |   PRESSURE             2875.71714 bar      E(TOT)            -186008.40141 kcal/mol   |
 |   E(QM)             -186197.10854 kcal/mol N(QM-ATOMS)             0.00000 -          |
 |   E(KIN)                188.70714 kcal/mol E(INTRA)                0.00000 kcal/mol   |
 |   VOLUME               4310.41014 A^3      DENSITY                 0.83455 g/cm^3     |
 |   MOMENTUM                2.5e-10 amuA/fs  LOOPTIME                0.90443 s          |
```

### Comparing `pqanalysis-0.5.2/tests/data/readInfoFile/md-01.qmcfc.info` & `pqanalysis-1.0/tests/data/readInfoFile/md-01.qmcfc.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/tests/data/traj2box/acof_triclinic.xyz` & `pqanalysis-1.0/tests/data/traj2qmcfc/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/tests/data/traj2box/acof_triclinic_2.xyz` & `pqanalysis-1.0/tests/data/traj2qmcfc/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-0.5.2/tests/io/test_base.py` & `pqanalysis-1.0/tests/io/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,68 @@
 import pytest
 import os
 import sys
 
-from PQAnalysis.io import BaseWriter, BaseReader
+from . import pytestmark
+
+from PQAnalysis.io import BaseWriter, BaseReader, FileWritingMode
+from PQAnalysis.io.exceptions import FileWritingModeError
+from PQAnalysis.exceptions import PQFileNotFoundError
+
 
 
 class TestBaseWriter:
 
     @pytest.mark.usefixtures("tmpdir")
     def test__init__(self):
 
         filename = "tmp"
 
-        with pytest.raises(ValueError) as exception:
+        with pytest.raises(FileWritingModeError) as exception:
             BaseWriter(filename, "r")
-        assert str(
-            exception.value) == "Invalid mode - has to be either \'w\' or \'a\'."
+            assert str(
+                exception.value
+            ) == """"
+'r' is not a valid FileWritingMode.
+Possible values are: FileWritingMode.OVERWRITE, FileWritingMode.APPEND, FileWritingMode.WRITE
+or their case insensitive string representation: o, a, w"""
 
         open(filename, "w")
 
-        with pytest.raises(ValueError) as exception:
+        with pytest.raises(FileWritingModeError) as exception:
             BaseWriter(filename, "w")
         assert str(
-            exception.value) == "File tmp already exists. Use mode \'a\' to append to file."
+            exception.value
+        ) == "File tmp already exists. Use mode \'a\' to append to the file or mode 'o' to overwrite the file."
+
+        writer = BaseWriter(filename, "o")
+        assert writer.file is None
+        assert writer.mode == FileWritingMode.WRITE
+        assert writer.filename == filename
 
         writer = BaseWriter(filename, "a")
         assert writer.file is None
-        assert writer.mode == "a"
+        assert writer.mode == FileWritingMode.APPEND
         assert writer.filename == filename
 
         os.remove(filename)
 
         writer = BaseWriter(filename, "w")
         assert writer.file is None
-        assert writer.mode == "a"
+        assert writer.mode == FileWritingMode.WRITE
+        assert writer.filename == filename
+
+        writer = BaseWriter(filename, "o")
+        assert writer.file is None
+        assert writer.mode == FileWritingMode.WRITE
         assert writer.filename == filename
 
         writer = BaseWriter()
         assert writer.file == sys.stdout
-        assert writer.mode == "a"
+        assert writer.mode == FileWritingMode.WRITE
         assert writer.filename is None
 
     @pytest.mark.usefixtures("tmpdir")
     def test_open(self):
 
         filename = "tmp"
 
@@ -71,34 +91,37 @@
         writer.open()
         assert writer.file is not None
 
         writer.close()
         assert writer.file is None
 
 
+
 class TestBaseReader:
+
     @pytest.mark.usefixtures("tmpdir")
     def test__init__(self):
-        with pytest.raises(FileNotFoundError) as exception:
+        with pytest.raises(PQFileNotFoundError) as exception:
             BaseReader("tmp")
         assert str(exception.value) == "File tmp not found."
 
         filename = "tmp"
         file = open(filename, "w")
         print("test", file=file)
         file.close()
 
         reader = BaseReader(filename)
         assert reader.filename == filename
         assert reader.multiple_files is False
 
-        with pytest.raises(FileNotFoundError) as exception:
+        with pytest.raises(PQFileNotFoundError) as exception:
             BaseReader([filename, "tmp2"])
         assert str(
-            exception.value) == "At least one of the given files does not exist. File tmp2 not found."
+            exception.value
+        ) == "At least one of the given files does not exist. File tmp2 not found."
 
         filename2 = "tmp2"
         file = open(filename2, "w")
         print("test2", file=file)
         file.close()
 
         reader = BaseReader([filename, filename2])
```

### Comparing `pqanalysis-0.5.2/tests/io/test_boxWriter.py` & `pqanalysis-1.0/tests/io/test_boxWriter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,99 +1,108 @@
 import pytest
 import numpy as np
 
+from . import pytestmark
+
 from _pytest.capture import CaptureFixture
 
-from PQAnalysis.io.boxWriter import BoxWriter, write_box
-from PQAnalysis.io.exceptions import BoxWriterError
-from PQAnalysis.traj import Trajectory, Frame
-from PQAnalysis.core import Cell, Atom, AtomicSystem
+from PQAnalysis.io import BoxWriter, write_box, BoxFileFormat, FileWritingMode
+from PQAnalysis.io.exceptions import BoxWriterError, BoxFileFormatError
+from PQAnalysis.traj import Trajectory
+from PQAnalysis.core import Cell, Atom
+from PQAnalysis.atomic_system import AtomicSystem
+
 
 
 class TestBoxWriter:
 
     def test__init__(self):
-        with pytest.raises(ValueError) as exception:
-            BoxWriter(filename="tmp", format="r")
-        assert str(
-            exception.value) == "Invalid format. Has to be either \'vmd\', \'data\' or \'None\'."
+        with pytest.raises(BoxFileFormatError) as exception:
+            BoxWriter(filename="tmp", output_format="r")
+        assert str(exception.value) == (
+            "\n"
+            "'r' is not a valid BoxFileFormat.\n"
+            "Possible values are: BoxFileFormat.VMD, BoxFileFormat.DATA "
+            "or their case insensitive string representation: "
+            "vmd, data"
+        )
 
-        writer = BoxWriter(filename="tmp", format="vmd")
+        writer = BoxWriter(filename="tmp", output_format="vmd")
         assert writer.file is None
-        assert writer.mode == "a"
+        assert writer.mode == FileWritingMode.WRITE
         assert writer.filename == "tmp"
-        assert writer.format == "vmd"
+        assert writer.output_format == BoxFileFormat.VMD
 
-        writer = BoxWriter(filename="tmp", format="data")
+        writer = BoxWriter(filename="tmp", output_format="data")
         assert writer.file is None
-        assert writer.mode == "a"
+        assert writer.mode == FileWritingMode.WRITE
         assert writer.filename == "tmp"
-        assert writer.format == "data"
+        assert writer.output_format == BoxFileFormat.DATA
 
         writer = BoxWriter(filename="tmp")
         assert writer.file is None
-        assert writer.mode == "a"
+        assert writer.mode == FileWritingMode.WRITE
         assert writer.filename == "tmp"
-        assert writer.format == "data"
+        assert writer.output_format == BoxFileFormat.DATA
 
     atoms1 = [Atom("H")]
     pos1 = np.array([[0, 1, 2]])
     cell1 = Cell(10, 10, 10)
 
     def test__check_PBC__(self):
         system1 = AtomicSystem(
-            atoms=self.atoms1, pos=self.pos1, cell=self.cell1)
+            atoms=self.atoms1,
+            pos=self.pos1,
+            cell=self.cell1
+        )
         system2 = AtomicSystem(atoms=self.atoms1, pos=self.pos1)
 
-        frame1 = Frame(system1)
-        frame2 = Frame(system2)
+        frame1 = system1
+        frame2 = system2
 
         traj1 = Trajectory([frame1, frame1])
         traj2 = Trajectory([frame1, frame2])
 
         writer = BoxWriter()
 
         try:
-            writer.__check_PBC__(traj1)
+            writer.__check_pbc__(traj1)
         except:
             assert False
 
         with pytest.raises(BoxWriterError) as exception:
-            writer.__check_PBC__(traj2)
+            writer.__check_pbc__(traj2)
         assert str(
-            exception.value) == "At least on cell of the trajectory is None. Cannot write box file."
+            exception.value
+        ) == "At least on cell of the trajectory is None. Cannot write box file."
 
     def test_write_box_file(self, capsys: CaptureFixture):
         writer = BoxWriter()
 
         cell1 = Cell(10, 10, 10, 90, 90, 90)
         cell2 = Cell(10, 10, 11, 90, 90, 120)
 
-        frame1 = Frame(AtomicSystem(
-            atoms=self.atoms1, pos=self.pos1, cell=cell1))
-        frame2 = Frame(AtomicSystem(
-            atoms=self.atoms1, pos=self.pos1, cell=cell2))
+        frame1 = AtomicSystem(atoms=self.atoms1, pos=self.pos1, cell=cell1)
+        frame2 = AtomicSystem(atoms=self.atoms1, pos=self.pos1, cell=cell2)
 
         traj = Trajectory([frame1, frame2])
 
         writer.write_box_file(traj, reset_counter=True)
 
         captured = capsys.readouterr()
 
         assert captured.out == "1 10 10 10 90 90 90\n2 10 10 11 90 90 120\n"
 
     def test_write_vmd(self, capsys: CaptureFixture):
         writer = BoxWriter()
 
         cell1 = Cell(10, 10, 10, 90, 90, 90)
         cell2 = Cell(10, 10, 11, 90, 90, 90)
-        frame1 = Frame(AtomicSystem(
-            atoms=self.atoms1, pos=self.pos1, cell=cell1))
-        frame2 = Frame(AtomicSystem(
-            atoms=self.atoms1, pos=self.pos1, cell=cell2))
+        frame1 = AtomicSystem(atoms=self.atoms1, pos=self.pos1, cell=cell1)
+        frame2 = AtomicSystem(atoms=self.atoms1, pos=self.pos1, cell=cell2)
 
         traj = Trajectory([frame1, frame2])
 
         print("")
         writer.write_vmd(traj)
 
         captured = capsys.readouterr()
@@ -122,26 +131,24 @@
 """
 
     def test_write(self, capsys: CaptureFixture):
         writer = BoxWriter()
 
         cell1 = Cell(10, 10, 10, 90, 90, 90)
         cell2 = Cell(10, 10, 11, 90, 90, 90)
-        frame1 = Frame(AtomicSystem(
-            atoms=self.atoms1, pos=self.pos1, cell=cell1))
-        frame2 = Frame(AtomicSystem(
-            atoms=self.atoms1, pos=self.pos1, cell=cell2))
+        frame1 = AtomicSystem(atoms=self.atoms1, pos=self.pos1, cell=cell1)
+        frame2 = AtomicSystem(atoms=self.atoms1, pos=self.pos1, cell=cell2)
 
         traj = Trajectory([frame1, frame2])
 
         print("")
-        writer.format = "data"
+        writer.output_format = "data"
         writer.write(traj)
         print("")
-        writer.format = "vmd"
+        writer.output_format = "vmd"
         writer.write(traj)
 
         captured = capsys.readouterr()
 
         assert captured.out == """
 1 10 10 10 90 90 90
 2 10 10 11 90 90 90
@@ -168,25 +175,23 @@
 X   5.0 5.0 5.5
 """
 
     def test_write_box(self, capsys: CaptureFixture):
 
         cell1 = Cell(10, 10, 10, 90, 90, 90)
         cell2 = Cell(10, 10, 11, 90, 90, 90)
-        frame1 = Frame(AtomicSystem(
-            atoms=self.atoms1, pos=self.pos1, cell=cell1))
-        frame2 = Frame(AtomicSystem(
-            atoms=self.atoms1, pos=self.pos1, cell=cell2))
+        frame1 = AtomicSystem(atoms=self.atoms1, pos=self.pos1, cell=cell1)
+        frame2 = AtomicSystem(atoms=self.atoms1, pos=self.pos1, cell=cell2)
 
         traj = Trajectory([frame1, frame2])
 
         print("")
-        write_box(traj, format="data")
+        write_box(traj, output_format="data")
         print("")
-        write_box(traj, format="vmd")
+        write_box(traj, output_format="vmd")
 
         captured = capsys.readouterr()
 
         assert captured.out == """
 1 10 10 10 90 90 90
 2 10 10 11 90 90 90
```

### Comparing `pqanalysis-0.5.2/tests/io/test_energyFileReader.py` & `pqanalysis-1.0/tests/io/test_energyFileReader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,132 @@
 import pytest
 import numpy as np
 
+from . import pytestmark
+
 from collections import defaultdict
 
 from PQAnalysis.io import EnergyFileReader, InfoFileReader
 from PQAnalysis.traj import MDEngineFormat
 from PQAnalysis.traj.exceptions import MDEngineFormatError
+from PQAnalysis.exceptions import PQFileNotFoundError
+
 
 
 class TestEnergyReader:
+
     @pytest.mark.parametrize("example_dir", ["readEnergyFile"], indirect=False)
     def test__init__(self, test_with_data_dir):
-        with pytest.raises(FileNotFoundError) as exception:
+        with pytest.raises(PQFileNotFoundError) as exception:
             EnergyFileReader("tmp")
         assert str(exception.value) == "File tmp not found."
 
         reader = EnergyFileReader("md-01.en")
         assert reader.filename == "md-01.en"
         assert reader.info_filename == "md-01.info"
-        assert reader.withInfoFile == True
-        assert reader.format == MDEngineFormat.PIMD_QMCF
+        assert reader.with_info_file == True
+        assert reader.format == MDEngineFormat.PQ
 
         reader = EnergyFileReader("md-01.en", use_info_file=False)
         assert reader.filename == "md-01.en"
         assert reader.info_filename == None
-        assert reader.withInfoFile == False
-        assert reader.format == MDEngineFormat.PIMD_QMCF
+        assert reader.with_info_file == False
+        assert reader.format == MDEngineFormat.PQ
 
         reader = EnergyFileReader("md-01_noinfo.en")
         assert reader.filename == "md-01_noinfo.en"
         assert reader.info_filename == None
-        assert reader.withInfoFile == False
-        assert reader.format == MDEngineFormat.PIMD_QMCF
+        assert reader.with_info_file == False
+        assert reader.format == MDEngineFormat.PQ
 
-        with pytest.raises(FileNotFoundError) as exception:
+        with pytest.raises(PQFileNotFoundError) as exception:
             EnergyFileReader(
-                "md-01_noinfo.en", info_filename="md-01_noinfo.info", use_info_file=True)
-        assert str(
-            exception.value) == "Info File md-01_noinfo.info not found."
+                "md-01_noinfo.en",
+                info_filename="md-01_noinfo.info",
+                use_info_file=True
+            )
+        assert str(exception.value) == "Info File md-01_noinfo.info not found."
 
         reader = EnergyFileReader(
-            "md-01_noinfo.en", info_filename="md-01.info")
+            "md-01_noinfo.en",
+            info_filename="md-01.info"
+        )
         assert reader.filename == "md-01_noinfo.en"
         assert reader.info_filename == "md-01.info"
-        assert reader.withInfoFile == True
-        assert reader.format == MDEngineFormat.PIMD_QMCF
+        assert reader.with_info_file == True
+        assert reader.format == MDEngineFormat.PQ
 
-        reader = EnergyFileReader("md-01.en", format="qmcfc")
+        reader = EnergyFileReader("md-01.en", engine_format="qmcfc")
         assert reader.filename == "md-01.en"
         assert reader.info_filename == "md-01.info"
-        assert reader.withInfoFile == True
+        assert reader.with_info_file == True
         assert reader.format == MDEngineFormat.QMCFC
 
         with pytest.raises(MDEngineFormatError) as exception:
-            EnergyFileReader("md-01.en", format="tmp")
-        assert str(
-            exception.value) == f"""
-'tmp' is not a valid MDEngineFormat.
-Possible values are: {MDEngineFormat.member_repr()}
-or their case insensitive string representation: {MDEngineFormat.value_repr()}"""
+            EnergyFileReader("md-01.en", engine_format="tmp")
+        assert str(exception.value) == (
+            "\n"
+            "'tmp' is not a valid MDEngineFormat.\n"
+            f"Possible values are: {MDEngineFormat.member_repr()} "
+            "or their case insensitive string representation: "
+            f"{MDEngineFormat.value_repr()}"
+        )
 
     @pytest.mark.parametrize("example_dir", ["readEnergyFile"], indirect=False)
     def test__info_file_found__(self, test_with_data_dir):
         reader = EnergyFileReader("md-01.en")
         assert reader.__info_file_found__() == True
 
         reader = EnergyFileReader("md-01_noinfo.en")
         assert reader.__info_file_found__() == False
 
         reader = EnergyFileReader(
-            "md-01_noinfo.en", info_filename="md-01.info")
+            "md-01_noinfo.en",
+            info_filename="md-01.info"
+        )
         assert reader.__info_file_found__() == True
 
-        with pytest.raises(FileNotFoundError) as exception:
+        with pytest.raises(PQFileNotFoundError) as exception:
             EnergyFileReader(
-                "md-01_noinfo.en", info_filename="md-01_noinfo.info", use_info_file=True)
+                "md-01_noinfo.en",
+                info_filename="md-01_noinfo.info",
+                use_info_file=True
+            )
         assert str(exception.value) == "Info File md-01_noinfo.info not found."
 
     @pytest.mark.parametrize("example_dir", ["readEnergyFile"], indirect=False)
     def test_read(self, test_with_data_dir):
-        data_ref = np.array([[1.00000000e+00,  2.00000000e+00],
-                             [2.98066020e+02,  2.98442926e+02],
-                             [2.32566666e+04,  2.39839997e+04],
-                             [-1.85898221e+05, -
-                              1.85719252e+05],
-                             [-1.85903822e+05, -
-                              1.86024132e+05],
-                             [0.00000000e+00,  0.00000000e+00],
-                             [5.60049937e+00,  3.04879280e+02],
-                             [0.00000000e+00,  0.00000000e+00],
-                             [3.72913867e+03,  3.72146189e+03],
-                             [8.34545285e-01,  8.34545285e-01],
-                             [1.12687000e-16,  5.63381000e-17],
-                             [1.07571000e+00,  9.97330000e-01]])
+        data_ref = np.array(
+            [
+            [1.00000000e+00,
+            2.00000000e+00],
+            [2.98066020e+02,
+            2.98442926e+02],
+            [2.32566666e+04,
+            2.39839997e+04],
+            [-1.85898221e+05,
+            -1.85719252e+05],
+            [-1.85903822e+05,
+            -1.86024132e+05],
+            [0.00000000e+00,
+            0.00000000e+00],
+            [5.60049937e+00,
+            3.04879280e+02],
+            [0.00000000e+00,
+            0.00000000e+00],
+            [3.72913867e+03,
+            3.72146189e+03],
+            [8.34545285e-01,
+            8.34545285e-01],
+            [1.12687000e-16,
+            5.63381000e-17],
+            [1.07571000e+00,
+            9.97330000e-01]
+            ]
+        )
 
         infoFileReader = InfoFileReader("md-01.info")
         info, units = infoFileReader.read()
 
         reader = EnergyFileReader("md-01.en")
         energy = reader.read()
```

### Comparing `pqanalysis-0.5.2/tests/io/test_frameReader.py` & `pqanalysis-1.0/tests/io/test_frameReader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,122 +1,150 @@
 import pytest
 import numpy as np
 
-from beartype.roar import BeartypeException
-
-from PQAnalysis.io import FrameReader
-from PQAnalysis.io.exceptions import FrameReaderError
+from PQAnalysis.io import _FrameReader
+from PQAnalysis.io.traj_file.exceptions import FrameReaderError
 from PQAnalysis.core import Cell, Atom
 from PQAnalysis.traj.exceptions import TrajectoryFormatError
 from PQAnalysis.traj import TrajectoryFormat
+from PQAnalysis.topology import Topology
+
+from . import pytestmark
+
 
 
 class TestFrameReader:
 
     def test__read_header_line(self):
-        reader = FrameReader()
+        reader = _FrameReader()
 
         with pytest.raises(FrameReaderError) as exception:
             reader._read_header_line("1 2.0 3.0")
         assert str(
-            exception.value) == "Invalid file format in header line of Frame."
+            exception.value
+        ) == "Invalid file format in header line of Frame."
 
-        n_atoms, cell = reader._read_header_line(
-            "1 2.0 3.0 4.0 5.0 6.0 7.0")
+        n_atoms, cell = reader._read_header_line("1 2.0 3.0 4.0 5.0 6.0 7.0")
         assert n_atoms == 1
         assert np.allclose(cell.box_lengths, [2.0, 3.0, 4.0])
         assert np.allclose(cell.box_angles, [5.0, 6.0, 7.0])
 
         n_atoms, cell = reader._read_header_line("2 2.0 3.0 4.0")
         assert n_atoms == 2
         assert np.allclose(cell.box_lengths, [2.0, 3.0, 4.0])
         assert np.allclose(cell.box_angles, [90.0, 90.0, 90.0])
 
         n_atoms, cell = reader._read_header_line("3")
         assert n_atoms == 3
         assert cell == Cell()
 
     def test__read_xyz(self):
-        reader = FrameReader()
+        reader = _FrameReader()
 
         with pytest.raises(FrameReaderError) as exception:
-            reader._read_xyz(
-                ["", "", "h 1.0 2.0 3.0", "o 2.0 2.0"], n_atoms=2)
+            reader._read_xyz(["", "", "h 1.0 2.0 3.0", "o 2.0 2.0"], n_atoms=2)
         assert str(
-            exception.value) == "Invalid file format in xyz coordinates of Frame."
+            exception.value
+        ) == "Invalid file format in xyz coordinates of Frame."
 
         xyz, atoms = reader._read_xyz(
             ["", "", "h 1.0 2.0 3.0", "o 2.0 2.0 2.0"], n_atoms=2)
         assert np.allclose(xyz, [[1.0, 2.0, 3.0], [2.0, 2.0, 2.0]])
         assert atoms == ["h", "o"]
 
     def test__read_scalar(self):
-        reader = FrameReader()
+        reader = _FrameReader()
 
         with pytest.raises(FrameReaderError) as exception:
             reader._read_scalar(["", "", "h 1.0 2.0 3.0"], n_atoms=1)
         assert str(
-            exception.value) == "Invalid file format in scalar values of Frame."
+            exception.value
+        ) == "Invalid file format in scalar values of Frame."
 
         scalar, atoms = reader._read_scalar(["", "", "h 1.0"], n_atoms=1)
         assert np.allclose(scalar, [1.0])
         assert atoms == ["h"]
 
     def test_read(self):
-        reader = FrameReader()
-
-        with pytest.raises(BeartypeException):
-            reader.read(["tmp"])
+        reader = _FrameReader()
 
         frame = reader.read(
-            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0 2.0 3.0\no 2.0 2.0 2.0")
+            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0 2.0 3.0\no 2.0 2.0 2.0"
+        )
         assert frame.n_atoms == 2
         assert frame.atoms == [Atom(atom) for atom in ["h", "o"]]
-        assert np.allclose(frame.pos, [
-                           [1.0, 2.0, 3.0], [2.0, 2.0, 2.0]])
+        assert np.allclose(frame.pos, [[1.0, 2.0, 3.0], [2.0, 2.0, 2.0]])
         assert frame.cell == Cell(2.0, 3.0, 4.0, 5.0, 6.0, 7.0)
 
         frame = reader.read(
-            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0 2.0 3.0\no1 2.0 2.0 2.0")
+            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0 2.0 3.0\no1 2.0 2.0 2.0"
+        )
         assert frame.n_atoms == 2
-        assert frame.atoms == [Atom(atom, use_guess_element=False)
-                               for atom in ["h", "o1"]]
-        assert np.allclose(frame.pos, [
-                           [1.0, 2.0, 3.0], [2.0, 2.0, 2.0]])
+        assert frame.atoms == [
+            Atom(atom,
+            use_guess_element=False) for atom in ["h",
+            "o1"]
+        ]
+        assert np.allclose(frame.pos, [[1.0, 2.0, 3.0], [2.0, 2.0, 2.0]])
         assert frame.cell == Cell(2.0, 3.0, 4.0, 5.0, 6.0, 7.0)
 
         frame = reader.read(
-            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0 2.0 3.0\no1 2.0 2.0 2.0", format="vel")
+            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0 2.0 3.0\no1 2.0 2.0 2.0",
+            traj_format="vel"
+        )
         assert frame.n_atoms == 2
-        assert frame.atoms == [Atom(atom, use_guess_element=False)
-                               for atom in ["h", "o1"]]
-        assert np.allclose(frame.vel, [
-                           [1.0, 2.0, 3.0], [2.0, 2.0, 2.0]])
+        assert frame.atoms == [
+            Atom(atom,
+            use_guess_element=False) for atom in ["h",
+            "o1"]
+        ]
+        assert np.allclose(frame.vel, [[1.0, 2.0, 3.0], [2.0, 2.0, 2.0]])
         assert frame.cell == Cell(2.0, 3.0, 4.0, 5.0, 6.0, 7.0)
 
         frame = reader.read(
-            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0 2.0 3.0\no1 2.0 2.0 2.0", format="force")
+            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0 2.0 3.0\no1 2.0 2.0 2.0",
+            traj_format="force"
+        )
         assert frame.n_atoms == 2
-        assert frame.atoms == [Atom(atom, use_guess_element=False)
-                               for atom in ["h", "o1"]]
-        assert np.allclose(frame.forces, [
-                           [1.0, 2.0, 3.0], [2.0, 2.0, 2.0]])
+        assert frame.atoms == [
+            Atom(atom,
+            use_guess_element=False) for atom in ["h",
+            "o1"]
+        ]
+        assert np.allclose(frame.forces, [[1.0, 2.0, 3.0], [2.0, 2.0, 2.0]])
         assert frame.cell == Cell(2.0, 3.0, 4.0, 5.0, 6.0, 7.0)
 
         frame = reader.read(
-            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0\no1 2.0", format="charge")
+            "2 2.0 3.0 4.0 5.0 6.0 7.0\n\nh 1.0\no1 2.0",
+            traj_format="charge"
+        )
         assert frame.n_atoms == 2
-        assert frame.atoms == [Atom(atom, use_guess_element=False)
-                               for atom in ["h", "o1"]]
+        assert frame.atoms == [
+            Atom(atom,
+            use_guess_element=False) for atom in ["h",
+            "o1"]
+        ]
         assert np.allclose(frame.charges, [1.0, 2.0])
         assert frame.cell == Cell(2.0, 3.0, 4.0, 5.0, 6.0, 7.0)
 
     def test_read_invalid_format(self):
-        reader = FrameReader()
+        reader = _FrameReader()
 
         with pytest.raises(TrajectoryFormatError) as exception:
-            reader.read("", format="invalid")
-        assert str(
-            exception.value) == f"""
-'invalid' is not a valid TrajectoryFormat.
-Possible values are: {TrajectoryFormat.member_repr()}
-or their case insensitive string representation: {TrajectoryFormat.value_repr()}"""
+            reader.read("", traj_format="invalid")
+        assert str(exception.value) == (
+            "\n"
+            "'invalid' is not a valid TrajectoryFormat.\n"
+            f"Possible values are: {TrajectoryFormat.member_repr()} "
+            "or their case insensitive string representation: "
+            f"{TrajectoryFormat.value_repr()}"
+        )
+
+    def test__get_topology(self):
+        reader = _FrameReader()
+
+        topology = reader._get_topology(["h", "o"], None)
+        assert topology.atoms == [Atom(atom) for atom in ["h", "o"]]
+
+        topology = Topology()
+        topology = reader._get_topology(["h", "o"], topology)
+        assert topology == Topology()
```

### Comparing `pqanalysis-0.5.2/tests/io/test_infoFileReader.py` & `pqanalysis-1.0/tests/io/test_infoFileReader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import pytest
 
-from beartype.roar import BeartypeException
-
 from PQAnalysis.io import InfoFileReader
 from PQAnalysis.traj import MDEngineFormat
 from PQAnalysis.traj.exceptions import MDEngineFormatError
+from PQAnalysis.exceptions import PQFileNotFoundError
+
+from . import pytestmark
+
 
 
 @pytest.mark.parametrize("example_dir", ["readInfoFile"], indirect=False)
 def test__init__(test_with_data_dir):
-    with pytest.raises(FileNotFoundError) as exception:
+    with pytest.raises(PQFileNotFoundError) as exception:
         InfoFileReader("tmp")
     assert str(exception.value) == "File tmp not found."
 
-    with pytest.raises(BeartypeException) as exception:
-        InfoFileReader(
-            "md-01.info", format=None)
-
     with pytest.raises(MDEngineFormatError) as exception:
-        InfoFileReader(
-            "md-01.info", format="tmp")
-    assert str(
-        exception.value) == f"""
-'tmp' is not a valid MDEngineFormat.
-Possible values are: {MDEngineFormat.member_repr()}
-or their case insensitive string representation: {MDEngineFormat.value_repr()}"""
+        InfoFileReader("md-01.info", engine_format="tmp")
+    assert str(exception.value) == (
+        "\n"
+        "'tmp' is not a valid MDEngineFormat.\n"
+        f"Possible values are: {MDEngineFormat.member_repr()} "
+        "or their case insensitive string representation: "
+        f"{MDEngineFormat.value_repr()}"
+    )
 
     reader = InfoFileReader("md-01.info")
     assert reader.filename == "md-01.info"
-    assert reader.format == MDEngineFormat.PIMD_QMCF
+    assert reader.format == MDEngineFormat.PQ
 
-    reader = InfoFileReader("md-01.info", format="qmcfc")
+    reader = InfoFileReader("md-01.info", engine_format="qmcfc")
     assert reader.filename == "md-01.info"
     assert reader.format == MDEngineFormat.QMCFC
 
 
+
 @pytest.mark.parametrize("example_dir", ["readInfoFile"], indirect=False)
 def test_read(test_with_data_dir):
     reader = InfoFileReader("md-01.info")
     info, units = reader.read()
 
     assert info["SIMULATION-TIME"] == 0
     assert units["SIMULATION-TIME"] == "ps"
@@ -72,15 +72,15 @@
 
     assert info["MOMENTUM"] == 10
     assert units["MOMENTUM"] == "amuA/fs"
 
     assert info["LOOPTIME"] == 11
     assert units["LOOPTIME"] == "s"
 
-    reader = InfoFileReader("md-01.qmcfc.info", format="qmcfc")
+    reader = InfoFileReader("md-01.qmcfc.info", engine_format="qmcfc")
     info, units = reader.read()
 
     assert info["SIMULATION TIME"] == 0
     assert info["QM_MOLECULES"] == 1
     assert info["TEMPERATURE"] == 2
     assert info["PRESSURE"] == 3
     assert info["E(QM)"] == 4
@@ -104,13 +104,16 @@
     assert info["MOMENTUM"] == 22
     assert info["LOOPTIME"] == 23
 
     reader = InfoFileReader("md-01.qmcfc.info")
     with pytest.raises(MDEngineFormatError) as exception:
         reader.read()
     assert str(
-        exception.value) == "Info file md-01.qmcfc.info is not in pimd-qmcf format."
+        exception.value
+    ) == "Info file md-01.qmcfc.info is not in PQ format."
 
-    reader = InfoFileReader("md-01.info", format="qmcfc")
+    reader = InfoFileReader("md-01.info", engine_format="qmcfc")
     with pytest.raises(MDEngineFormatError) as exception:
         reader.read()
-    assert str(exception.value) == "Info file md-01.info is not in qmcfc format."
+    assert str(
+        exception.value
+    ) == "Info file md-01.info is not in qmcfc format."
```

### Comparing `pqanalysis-0.5.2/tests/io/test_moldescriptorReader.py` & `pqanalysis-1.0/tests/io/test_moldescriptorReader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import pytest
 import numpy as np
 
+from . import pytestmark
+
 from PQAnalysis.io import MoldescriptorReader
 from PQAnalysis.io.exceptions import MoldescriptorReaderError
-from PQAnalysis.core import Atom
+from PQAnalysis.core import Element
+from PQAnalysis.exceptions import PQFileNotFoundError
+
 
 
 class TestMoldescriptorReader:
-    @pytest.mark.parametrize("example_dir", ["readMoldescriptor"], indirect=False)
+
+    @pytest.mark.parametrize(
+        "example_dir",
+        ["readMoldescriptor"],
+        indirect=False
+    )
     def test__init__(self, test_with_data_dir):
         reader = MoldescriptorReader("moldescriptor.dat")
         assert reader.filename == "moldescriptor.dat"
 
-        with pytest.raises(FileNotFoundError) as exception:
+        with pytest.raises(PQFileNotFoundError) as exception:
             MoldescriptorReader("tmp")
         assert str(exception.value) == "File tmp not found."
 
     def test_read_mol_type(self):
         mol_type = f"""H2o 3 1.0
 H 1 2.3
 H 1 2.3
@@ -24,58 +33,85 @@
 """
 
         mol_type = MoldescriptorReader._read_mol_type(mol_type.splitlines(), 1)
 
         assert mol_type.name == "H2o"
         assert mol_type.n_atoms == 3
         assert mol_type.total_charge == 1.0
-        assert mol_type.elements == [Atom("H"), Atom("H"), Atom("O")]
+        assert mol_type.elements == [Element("H"), Element("H"), Element("O")]
         assert np.allclose(mol_type.atom_types, np.array([1, 1, 2]))
-        assert np.allclose(mol_type.partial_charges,
-                           np.array([2.3, 2.3, -4.6]))
+        assert np.allclose(
+            mol_type.partial_charges,
+            np.array([2.3,
+            2.3,
+            -4.6])
+        )
         assert mol_type.id == 1
 
         mol_type = f"""H2o 3 1.0
 H 1 2.3
 H 1
 O 2 -4.6
 """
 
         with pytest.raises(MoldescriptorReaderError) as exception:
             MoldescriptorReader._read_mol_type(mol_type.splitlines(), 1)
         assert str(
-            exception.value) == "The number of columns in the body of a mol type must be 3 or 4."
+            exception.value
+        ) == "The number of columns in the body of a mol type must be 3 or 4.\nGot 2 columns instead in text: 'H 1'\n"
 
-    @pytest.mark.parametrize("example_dir", ["readMoldescriptor"], indirect=False)
+    @pytest.mark.parametrize(
+        "example_dir",
+        ["readMoldescriptor"],
+        indirect=False
+    )
     def test_read(self, test_with_data_dir):
         reader = MoldescriptorReader("moldescriptor.dat")
         mol_types = reader.read()
 
         assert len(mol_types) == 2
         water_type = mol_types[0]
 
         assert water_type.name == "H2O"
         assert water_type.n_atoms == 3
         assert np.allclose(water_type.total_charge, 0.0)
-        assert water_type.elements == [Atom("O"), Atom("H"), Atom("H")]
+        assert water_type.elements == [
+            Element("O"),
+            Element("H"),
+            Element("H")
+        ]
         assert np.allclose(water_type.atom_types, np.array([0, 1, 1]))
-        assert np.allclose(water_type.partial_charges,
-                           np.array([-0.65966, 0.32983, 0.32983]))
+        assert np.allclose(
+            water_type.partial_charges,
+            np.array([-0.65966,
+            0.32983,
+            0.32983])
+        )
         assert water_type.id == 1
 
         ammonia_type = mol_types[1]
 
         assert ammonia_type.name == "Ammonia"
         assert ammonia_type.n_atoms == 4
         assert np.allclose(ammonia_type.total_charge, 0.0)
         assert ammonia_type.elements == [
-            Atom("N"), Atom("H"), Atom("H"), Atom("H")]
+            Element("N"),
+            Element("H"),
+            Element("H"),
+            Element("H")
+        ]
         assert np.allclose(ammonia_type.atom_types, np.array([0, 1, 1, 1]))
-        assert np.allclose(ammonia_type.partial_charges,
-                           np.array([-0.8022, 0.2674, 0.2674, 0.2674]))
+        assert np.allclose(
+            ammonia_type.partial_charges,
+            np.array([-0.8022,
+            0.2674,
+            0.2674,
+            0.2674])
+        )
         assert ammonia_type.id == 2
 
         reader = MoldescriptorReader("moldescriptor_withError.dat")
         with pytest.raises(MoldescriptorReaderError) as exception:
             reader.read()
         assert str(
-            exception.value) == "The number of columns in the header of a mol type must be 3."
+            exception.value
+        ) == "The number of columns in the header of a mol type must be 3.\nGot 2 columns instead in text: '  H2O            3'\n"
```

### Comparing `pqanalysis-0.5.2/tests/physicalData/test_energy.py` & `pqanalysis-1.0/tests/physicalData/test_energy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,25 @@
+from collections import defaultdict
+
 import pytest
 import numpy as np
 
-from collections import defaultdict
-from beartype.roar import BeartypeException
+from PQAnalysis.physical_data import Energy, EnergyError
 
-from PQAnalysis.physicalData import Energy, EnergyError
 
 
 class TestEnergy:
-    def test__init__(self):
-        with pytest.raises(BeartypeException):
-            Energy(1)
-
-        with pytest.raises(BeartypeException):
-            Energy([[[1]]])
 
+    def test__init__(self):
         data = np.array([1, 2, 3])
         energy = Energy(data)
 
         assert np.allclose(energy.data, [data])
 
     def test__setup_info_dictionary(self):
-        with pytest.raises(BeartypeException):
-            Energy(np.array([1]), info=1)
-
-        with pytest.raises(BeartypeException):
-            Energy(np.array([1]), units=1)
-
         data = np.array([[1], [2]])
         info = {1: 0, 2: 1}
         units = {1: "a", 2: "b"}
 
         energy = Energy(data, info=info, units=units)
         assert energy.info == info
         assert energy.units == units
@@ -44,18 +33,21 @@
         assert np.allclose(energy.data, data)
         assert energy.info_given == False
         assert energy.units_given == False
 
         with pytest.raises(EnergyError) as exception:
             Energy(data, info={1: 0})
         assert str(
-            exception.value) == "The length of info dictionary has to be equal to the length of data."
+            exception.value
+        ) == "The length of info dictionary has to be equal to the length of data."
 
         with pytest.raises(EnergyError) as exception:
             Energy(data, units={1: 0})
         assert str(
-            exception.value) == "The length of units dictionary has to be equal to the length of data."
+            exception.value
+        ) == "The length of units dictionary has to be equal to the length of data."
 
         with pytest.raises(EnergyError) as exception:
             Energy(data, info={1: 0, 2: 0}, units={1: 0, 3: 0})
         assert str(
-            exception.value) == "The keys of the info and units dictionary do not match."
+            exception.value
+        ) == "The keys of the info and units dictionary do not match."
```

### Comparing `pqanalysis-0.5.2/tests/tools/test_traj_to_com_traj.py` & `pqanalysis-1.0/tests/tools/test_traj_to_com_traj.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 import numpy as np
 
 from PQAnalysis.tools import traj_to_com_traj
 
-from PQAnalysis.traj import Trajectory, Frame
-from PQAnalysis.core import Atom, AtomicSystem
+from PQAnalysis.traj import Trajectory
+from PQAnalysis.core import Atom
+from PQAnalysis.atomic_system import AtomicSystem
+
 
 
 def test_traj_to_com_traj():
     traj = Trajectory()
 
     assert traj_to_com_traj(traj) == Trajectory()
 
     atoms = [Atom(atom) for atom in ['C', 'C', 'C']]
     coordinates = [[0, 0, 0], [1, 1, 1], [2, 2, 2]]
 
-    frame = Frame(AtomicSystem(atoms=atoms, pos=np.array(coordinates)))
+    frame = AtomicSystem(atoms=atoms, pos=np.array(coordinates))
     traj.append(frame)
 
     print(traj[0].n_atoms)
 
     traj_output = traj_to_com_traj(traj)
 
     assert np.allclose(traj_output[0].pos, [[1, 1, 1]])
-    assert traj_output[0].system.combined_name == 'CCC'
+    assert traj_output[0].combined_name == 'CCC'
 
     coordinates = [[0, 0, 1], [1, 1, 2], [2, 2, 3]]
-    frame = Frame(AtomicSystem(atoms=atoms, pos=np.array(coordinates)))
+    frame = AtomicSystem(atoms=atoms, pos=np.array(coordinates))
 
     traj.append(frame)
 
     traj_output = traj_to_com_traj(traj)
 
     assert np.allclose(traj_output[0].pos, [[1, 1, 1]])
-    assert traj_output[0].system.combined_name == 'CCC'
+    assert traj_output[0].combined_name == 'CCC'
     assert np.allclose(traj_output[1].pos, [[1, 1, 2]])
-    assert traj_output[1].system.combined_name == 'CCC'
+    assert traj_output[1].combined_name == 'CCC'
 
     traj_output = traj_to_com_traj(traj, selection=slice(0, 2))
     assert np.allclose(traj_output[0].pos, [[0.5, 0.5, 0.5]])
-    assert traj_output[0].system.combined_name == 'CC'
+    assert traj_output[0].combined_name == 'CC'
     assert np.allclose(traj_output[1].pos, [[0.5, 0.5, 1.5]])
-    assert traj_output[1].system.combined_name == 'CC'
+    assert traj_output[1].combined_name == 'CC'
 
     traj = Trajectory()
     atoms = [Atom(atom) for atom in ['C', 'C', 'H', 'H']]
     coordinates1 = [[0, 0, 1], [1, 1, 2], [2, 2, 3], [3, 3, 4]]
     coordinates2 = [[0, 1, 1], [1, 2, 2], [2, 3, 3], [3, 4, 4]]
-    frame1 = Frame(AtomicSystem(atoms=atoms, pos=np.array(coordinates1)))
-    frame2 = Frame(AtomicSystem(atoms=atoms, pos=np.array(coordinates2)))
+    frame1 = AtomicSystem(atoms=atoms, pos=np.array(coordinates1))
+    frame2 = AtomicSystem(atoms=atoms, pos=np.array(coordinates2))
     traj.append(frame1)
     traj.append(frame2)
 
     traj_output = traj_to_com_traj(traj, group=2)
 
     assert np.allclose(traj_output[0].pos, [[0.5, 0.5, 1.5], [2.5, 2.5, 3.5]])
     assert traj_output[0].atoms == [
-        Atom('CC', use_guess_element=False), Atom('HH', use_guess_element=False)]
-    assert traj_output[0].system.combined_name == 'CCHH'
+        Atom('CC',
+        use_guess_element=False),
+        Atom('HH',
+        use_guess_element=False)
+    ]
+    assert traj_output[0].combined_name == 'CCHH'
     assert np.allclose(traj_output[1].pos, [[0.5, 1.5, 1.5], [2.5, 3.5, 3.5]])
     assert traj_output[1].atoms == [
-        Atom('CC', use_guess_element=False), Atom('HH', use_guess_element=False)]
-    assert traj_output[1].system.combined_name == 'CCHH'
+        Atom('CC',
+        use_guess_element=False),
+        Atom('HH',
+        use_guess_element=False)
+    ]
+    assert traj_output[1].combined_name == 'CCHH'
```

### Comparing `pqanalysis-0.5.2/tests/utils/test_common.py` & `pqanalysis-1.0/tests/utils/test_common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import pytest
+
 from _pytest.capture import CaptureFixture
 
 from PQAnalysis.utils import print_header
 from PQAnalysis._version import __version__
 
 
+
 def test_print_header(capsys: CaptureFixture):
     print_header()
 
     captured = capsys.readouterr()
 
+    print(captured.err)
+
     line = "                                              *"
 
     assert captured.err == f"""
 **************************************************************
 *                                                            *
 *      ____  ____    ___                __           _       *
 *     / __ \/ __ \  /   |  ____  ____ _/ /_  _______(_)____  *
```

### Comparing `pqanalysis-0.5.2/tests/utils/test_decorators.py` & `pqanalysis-1.0/tests/utils/test_decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from PQAnalysis.utils import count_decorator, instance_function_count_decorator
 
 
+
 def test_count_decorator():
+
     @count_decorator
     def test_func(reset_counter=False):
         pass
 
-    assert test_func.counter == 0
     test_func()
     assert test_func.counter == 1
     test_func()
     assert test_func.counter == 2
     test_func(reset_counter=True)
     assert test_func.counter == 1
     test_func()
     assert test_func.counter == 2
 
 
+
 def test_instance_function_count_decorator():
+
     class Class:
+
         def __init__(self):
             self.instance_counter = 0
 
         @instance_function_count_decorator
         def test_func(self, reset_counter=False):
             self.instance_counter = self.counter[Class.test_func.__name__]
```

