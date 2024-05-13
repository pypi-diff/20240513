# Comparing `tmp/epyt_flow-0.1.0.tar.gz` & `tmp/epyt_flow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epyt_flow-0.1.0.tar", last modified: Fri May 10 05:34:19 2024, max compression
+gzip compressed data, was "epyt_flow-0.1.1.tar", last modified: Mon May 13 08:55:45 2024, max compression
```

## Comparing `epyt_flow-0.1.0.tar` & `epyt_flow-0.1.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.508081 epyt_flow-0.1.0/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5202 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1076 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/LICENSE
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      316 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/MANIFEST.in
--rw-r--r--   0 aartelt   (1000) aartelt   (1000)     5093 2024-05-10 05:34:19.508081 epyt_flow-0.1.0/PKG-INFO
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3640 2024-05-09 08:54:53.000000 epyt_flow-0.1.0/README.md
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      174 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/REQUIREMENTS.txt
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.496081 epyt_flow-0.1.0/epyt_flow/
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.496081 epyt_flow-0.1.0/epyt_flow/EPANET/
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.492081 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.504081 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      925 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/AUTHORS
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1070 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/LICENSE
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1005 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/Readme_SRC_Engines.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4351 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/enumstxt.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)   171230 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25173 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7782 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.def
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2786 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/errors.dat
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5991 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/funcs.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    32936 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/genmmd.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4018 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hash.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      838 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hash.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    33821 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hydcoeffs.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    32358 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hydraul.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    23669 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hydsolver.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13947 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hydstatus.c
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.504081 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/include/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13955 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    69518 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_2.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    19874 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_enums.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24745 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/inpfile.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24278 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/input1.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25371 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/input2.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    67160 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/input3.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2563 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/main.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3600 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/mempool.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      654 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/mempool.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    26660 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/output.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    41722 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/project.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    19500 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/quality.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21691 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/qualreact.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21516 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/qualroute.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    43451 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/report.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    36206 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/rules.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25997 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/smatrix.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    17375 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/text.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    30772 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/types.h
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.496081 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1536 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/MSX_Updates.txt
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.500081 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      941 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/dispersion.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2848 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/hash.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      412 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/hash.h
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.500081 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/include/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3429 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1054 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx_export.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    23189 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1342 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4283 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/mempool.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      455 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/mempool.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    35046 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxchem.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10817 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxcompiler.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2147 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxdict.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    14274 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxdispersion.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3055 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxerr.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7068 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfile.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4364 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1337 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    38985 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxinp.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11342 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxout.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21817 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxproj.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    57734 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxqual.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11505 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxrpt.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12126 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtank.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    33854 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtoolkit.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24060 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtypes.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12104 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1811 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4387 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/newton.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1090 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/newton.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9778 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/rk5.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1280 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/rk5.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     8542 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/ros2.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1249 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/ros2.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    28375 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1567 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      911 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/readme.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      453 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/EPANET/compile.sh
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        6 2024-05-09 08:54:41.000000 epyt_flow-0.1.0/epyt_flow/VERSION
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      872 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/__init__.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.504081 epyt_flow-0.1.0/epyt_flow/data/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        0 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/__init__.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.504081 epyt_flow-0.1.0/epyt_flow/data/benchmarks/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      754 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/benchmarks/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11175 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/benchmarks/batadal.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      880 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/benchmarks/batadal_data.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    20167 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/benchmarks/battledim.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3373 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/benchmarks/battledim_data.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10985 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/benchmarks/gecco_water_quality.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25445 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/benchmarks/leakdb.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)   507058 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/benchmarks/leakdb_data.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4778 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/benchmarks/water_usage.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24343 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/data/networks.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.504081 epyt_flow-0.1.0/epyt_flow/gym/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      115 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/gym/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1281 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/gym/control_gyms.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2950 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/gym/scenario_control_env.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12883 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/metrics.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.504081 epyt_flow-0.1.0/epyt_flow/models/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       75 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/models/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      789 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/models/event_detector.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3624 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/models/sensor_interpolation_detector.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.508081 epyt_flow-0.1.0/epyt_flow/rest_api/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      126 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/rest_api/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1886 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/rest_api/base_handler.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2342 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/rest_api/res_manager.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    16115 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/rest_api/scada_data_handler.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11471 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/rest_api/scenario_handler.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4928 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/rest_api/server.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12893 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/serialization.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.508081 epyt_flow-0.1.0/epyt_flow/simulation/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      164 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/__init__.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.508081 epyt_flow-0.1.0/epyt_flow/simulation/events/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      185 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/events/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7903 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/events/actuator_events.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2603 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/events/event.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    14569 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/events/leakages.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     8447 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/events/sensor_faults.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7538 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/events/sensor_reading_attack.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     6785 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/events/sensor_reading_event.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2396 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/events/system_event.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     6508 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/parallel_simulation.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.508081 epyt_flow-0.1.0/epyt_flow/simulation/scada/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       90 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/scada/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4489 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/scada/advanced_control.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    76694 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/scada/scada_data.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9860 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/scada/scada_data_export.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    27168 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/scenario_config.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    80517 2024-05-09 08:54:53.000000 epyt_flow-0.1.0/epyt_flow/simulation/scenario_simulator.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2186 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/scenario_visualizer.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    58161 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/simulation/sensor_config.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9795 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/topology.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.508081 epyt_flow-0.1.0/epyt_flow/uncertainty/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       89 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/uncertainty/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13592 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/uncertainty/model_uncertainty.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2324 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/uncertainty/sensor_noise.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    17669 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/uncertainty/uncertainties.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5315 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/uncertainty/utils.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9817 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/epyt_flow/utils.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-10 05:34:19.508081 epyt_flow-0.1.0/epyt_flow.egg-info/
--rw-r--r--   0 aartelt   (1000) aartelt   (1000)     5093 2024-05-10 05:34:19.000000 epyt_flow-0.1.0/epyt_flow.egg-info/PKG-INFO
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5471 2024-05-10 05:34:19.000000 epyt_flow-0.1.0/epyt_flow.egg-info/SOURCES.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        1 2024-05-10 05:34:19.000000 epyt_flow-0.1.0/epyt_flow.egg-info/dependency_links.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      175 2024-05-10 05:34:19.000000 epyt_flow-0.1.0/epyt_flow.egg-info/requires.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       41 2024-05-10 05:34:19.000000 epyt_flow-0.1.0/epyt_flow.egg-info/top_level.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1445 2024-05-09 08:54:53.000000 epyt_flow-0.1.0/pyproject.toml
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       38 2024-05-10 05:34:19.508081 epyt_flow-0.1.0/setup.cfg
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       38 2024-05-08 14:44:26.000000 epyt_flow-0.1.0/setup.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.824519 epyt_flow-0.1.1/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5202 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1076 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/LICENSE
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      316 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/MANIFEST.in
+-rw-r--r--   0 aartelt   (1000) aartelt   (1000)     5815 2024-05-13 08:55:45.824519 epyt_flow-0.1.1/PKG-INFO
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4361 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/README.md
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      174 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/REQUIREMENTS.txt
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.808516 epyt_flow-0.1.1/epyt_flow/
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.808516 epyt_flow-0.1.1/epyt_flow/EPANET/
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.804516 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      925 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/AUTHORS
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1070 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/LICENSE
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1005 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/Readme_SRC_Engines.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4351 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/enumstxt.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)   171230 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25173 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7782 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.def
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2786 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/errors.dat
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5991 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/funcs.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    32936 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/genmmd.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4018 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hash.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      838 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hash.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    33821 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydcoeffs.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    32358 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydraul.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    23669 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydsolver.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13947 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydstatus.c
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13955 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    69518 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_2.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    19874 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_enums.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24745 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/inpfile.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24278 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input1.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25371 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input2.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    67160 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input3.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2563 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/main.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3600 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/mempool.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      654 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/mempool.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    26660 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/output.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    41722 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/project.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    19500 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/quality.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21691 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/qualreact.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21516 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/qualroute.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    43451 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/report.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    36206 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/rules.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25997 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/smatrix.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    17375 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/text.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    30772 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/types.h
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.808516 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1536 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/MSX_Updates.txt
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.812517 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      941 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/dispersion.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2848 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/hash.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      412 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/hash.h
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.812517 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3429 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1054 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx_export.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    23189 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1342 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4283 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mempool.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      455 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mempool.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    35046 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxchem.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10817 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxcompiler.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2147 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxdict.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    14274 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxdispersion.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3055 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxerr.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7068 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfile.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4364 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1337 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    38985 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxinp.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11342 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxout.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21817 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxproj.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    57734 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxqual.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11505 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxrpt.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12126 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtank.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    33854 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtoolkit.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24060 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtypes.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12104 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1811 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4387 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/newton.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1090 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/newton.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9778 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/rk5.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1280 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/rk5.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     8542 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/ros2.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1249 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/ros2.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    28375 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1567 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      911 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/readme.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      453 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/compile.sh
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        6 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/epyt_flow/VERSION
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1230 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/epyt_flow/__init__.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/data/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        0 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/__init__.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/data/benchmarks/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      754 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11175 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/batadal.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      880 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/batadal_data.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    20167 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/battledim.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3373 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/battledim_data.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10985 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/gecco_water_quality.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25445 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/leakdb.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)   507058 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/leakdb_data.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4778 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/water_usage.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24343 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/networks.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/gym/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      115 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/gym/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1281 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/gym/control_gyms.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2950 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/gym/scenario_control_env.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12883 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/metrics.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/models/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       75 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/models/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      789 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/models/event_detector.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3624 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/models/sensor_interpolation_detector.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/rest_api/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      126 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1886 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/base_handler.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2342 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/res_manager.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    16115 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/scada_data_handler.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11471 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/scenario_handler.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4928 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/server.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12893 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/serialization.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/simulation/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      164 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/__init__.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/simulation/events/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      185 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7903 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/actuator_events.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2603 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/event.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    14569 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/leakages.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     8447 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_faults.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7538 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_reading_attack.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     6785 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_reading_event.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2396 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/system_event.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     6508 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/parallel_simulation.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/simulation/scada/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       90 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scada/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4489 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scada/advanced_control.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    76694 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scada/scada_data.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9860 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scada/scada_data_export.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    27168 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scenario_config.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    81432 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/epyt_flow/simulation/scenario_simulator.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2186 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scenario_visualizer.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    58161 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/epyt_flow/simulation/sensor_config.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9795 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/topology.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/uncertainty/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       89 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13592 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/model_uncertainty.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2324 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/sensor_noise.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    17669 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/uncertainties.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5315 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/utils.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9817 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/utils.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow.egg-info/
+-rw-r--r--   0 aartelt   (1000) aartelt   (1000)     5815 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/PKG-INFO
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5471 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/SOURCES.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        1 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/dependency_links.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      175 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/requires.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       41 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/top_level.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1446 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/pyproject.toml
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       38 2024-05-13 08:55:45.824519 epyt_flow-0.1.1/setup.cfg
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       38 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/setup.py
```

### Comparing `epyt_flow-0.1.0/CODE_OF_CONDUCT.md` & `epyt_flow-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/LICENSE` & `epyt_flow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/PKG-INFO` & `epyt_flow-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: epyt-flow
-Version: 0.1.0
+Version: 0.1.1
 Summary: EPyT-Flow -- EPANET Python Toolkit - Flow
 Author-email: André Artelt <aartelt@techfak.uni-bielefeld.de>, "Marios S. Kyriakou" <kiriakou.marios@ucy.ac.cy>, "Stelios G. Vrachimis" <vrachimis.stelios@ucy.ac.cy>
 License: MIT License
 Project-URL: Homepage, https://github.com/WaterFutures/EPyT-Flow
-Project-URL: Documentation, https://epytflow.readthedocs.io/en/latest/
+Project-URL: Documentation, https://epyt-flow.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/WaterFutures/EPyT-Flow.git
 Project-URL: Issues, https://github.com/WaterFutures/EPyT-Flow/issues
 Keywords: epanet,water,networks,hydraulics,quality,simulations
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: epyt>=1.1.3
+Requires-Dist: epyt>=1.1.6
 Requires-Dist: requests>=2.31.0
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: u-msgpack-python>=2.8.0
 Requires-Dist: networkx>=3.2.1
 Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: tqdm>=4.66.2
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: falcon>=3.1.3
 Requires-Dist: multiprocess>=0.70.16
 Requires-Dist: psutil
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pypi](https://img.shields.io/pypi/v/epyt-flow.svg)](https://pypi.org/project/epyt-flow/)
+[![build](https://github.com/WaterFutures/EPyT-Flow/actions/workflows/build_tests.yml/badge.svg)](https://github.com/WaterFutures/EPyT-Flow/actions/workflows/build_tests.yml)
+[![Documentation Status](https://readthedocs.org/projects/epyt-flow/badge/?version=stable)](https://epyt-flow.readthedocs.io/en/stable/?badge=stable)
+[![Downloads](https://static.pepy.tech/badge/epyt-flow)](https://pepy.tech/project/epyt-flow)
+[![Downloads](https://static.pepy.tech/badge/epyt-flow/month)](https://pepy.tech/project/epyt-flow)
+
 # EPyT-Flow -- EPANET Python Toolkit - Flow
 
 EPyT-Flow is a Python package building on top of [EPyT](https://github.com/OpenWaterAnalytics/EPyT) 
 for providing easy access to water distribution network simulations.
 It aims to provide a high-level interface for the easy generation of hydraulic and water quality scenario data.
 However, it also provides access to low-level functions by [EPANET](https://github.com/USEPA/EPANET2.2) 
 and [EPANET-MSX](https://github.com/USEPA/EPANETMSX/).
@@ -45,15 +52,15 @@
 
 ![](https://github.com/WaterFutures/EPyT-Flow/blob/main/docs/_static/net1_plot.png?raw=true)
 
 ## Installation
 
 EPyT-Flow supports Python 3.9 - 3.12
 
-Note that [EPANET and EPANET-MSX sources](epyt_flow/EPANET/) are compiled and overrite the binaries
+Note that [EPANET and EPANET-MSX sources](epyt_flow/EPANET/) are compiled and overwrite the binaries
 shipped by EPyT IF EPyT-Flow is installed on a Linux system. By this we not only aim to achieve
 a better performance of the simulations but also avoid any compatibility problems of pre-compiled binaries.
 
 ### PyPI
 
 ```
 pip install epyt-flow
@@ -109,15 +116,15 @@
         # Show sensor readings over the entire simulation
         print(f"Pressure readings: {scada_data.get_data_pressures()}")
         print(f"Flow readings: {scada_data.get_data_flows()}")
 ```
 
 ## Documentation
 
-Documentation is available on readthedocs: [https://epytflow.readthedocs.io/en/latest/](https://epytflow.readthedocs.io/en/latest/)
+Documentation is available on readthedocs:[https://epyt-flow.readthedocs.io/en/latest/](https://epyt-flow.readthedocs.io/en/stable)
 
 ## License
 
 MIT license -- see [LICENSE](LICENSE)
 
 ## How to Cite?
```

### Comparing `epyt_flow-0.1.0/README.md` & `epyt_flow-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pypi](https://img.shields.io/pypi/v/epyt-flow.svg)](https://pypi.org/project/epyt-flow/)
+[![build](https://github.com/WaterFutures/EPyT-Flow/actions/workflows/build_tests.yml/badge.svg)](https://github.com/WaterFutures/EPyT-Flow/actions/workflows/build_tests.yml)
+[![Documentation Status](https://readthedocs.org/projects/epyt-flow/badge/?version=stable)](https://epyt-flow.readthedocs.io/en/stable/?badge=stable)
+[![Downloads](https://static.pepy.tech/badge/epyt-flow)](https://pepy.tech/project/epyt-flow)
+[![Downloads](https://static.pepy.tech/badge/epyt-flow/month)](https://pepy.tech/project/epyt-flow)
+
 # EPyT-Flow -- EPANET Python Toolkit - Flow
 
 EPyT-Flow is a Python package building on top of [EPyT](https://github.com/OpenWaterAnalytics/EPyT) 
 for providing easy access to water distribution network simulations.
 It aims to provide a high-level interface for the easy generation of hydraulic and water quality scenario data.
 However, it also provides access to low-level functions by [EPANET](https://github.com/USEPA/EPANET2.2) 
 and [EPANET-MSX](https://github.com/USEPA/EPANETMSX/).
@@ -11,15 +18,15 @@
 
 ![](https://github.com/WaterFutures/EPyT-Flow/blob/main/docs/_static/net1_plot.png?raw=true)
 
 ## Installation
 
 EPyT-Flow supports Python 3.9 - 3.12
 
-Note that [EPANET and EPANET-MSX sources](epyt_flow/EPANET/) are compiled and overrite the binaries
+Note that [EPANET and EPANET-MSX sources](epyt_flow/EPANET/) are compiled and overwrite the binaries
 shipped by EPyT IF EPyT-Flow is installed on a Linux system. By this we not only aim to achieve
 a better performance of the simulations but also avoid any compatibility problems of pre-compiled binaries.
 
 ### PyPI
 
 ```
 pip install epyt-flow
@@ -75,15 +82,15 @@
         # Show sensor readings over the entire simulation
         print(f"Pressure readings: {scada_data.get_data_pressures()}")
         print(f"Flow readings: {scada_data.get_data_flows()}")
 ```
 
 ## Documentation
 
-Documentation is available on readthedocs: [https://epytflow.readthedocs.io/en/latest/](https://epytflow.readthedocs.io/en/latest/)
+Documentation is available on readthedocs:[https://epyt-flow.readthedocs.io/en/latest/](https://epyt-flow.readthedocs.io/en/stable)
 
 ## License
 
 MIT license -- see [LICENSE](LICENSE)
 
 ## How to Cite?
```

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/AUTHORS` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/AUTHORS`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/LICENSE` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/LICENSE`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/Readme_SRC_Engines.txt` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/Readme_SRC_Engines.txt`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/enumstxt.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/enumstxt.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.def` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.def`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/errors.dat` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/errors.dat`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/funcs.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/funcs.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/genmmd.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/genmmd.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hash.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hash.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hash.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hash.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hydcoeffs.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydcoeffs.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hydraul.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydraul.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hydsolver.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydsolver.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/hydstatus.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydstatus.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_2.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_2.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_enums.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_enums.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/inpfile.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/inpfile.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/input1.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input1.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/input2.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input2.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/input3.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input3.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/main.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/main.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/mempool.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/mempool.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/mempool.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/mempool.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/output.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/output.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/project.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/project.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/quality.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/quality.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/qualreact.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/qualreact.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/qualroute.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/qualroute.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/report.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/report.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/rules.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/rules.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/smatrix.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/smatrix.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/text.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/text.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET/SRC_engines/types.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/types.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/MSX_Updates.txt` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/MSX_Updates.txt`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/dispersion.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/dispersion.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/hash.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/hash.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx_export.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx_export.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/mempool.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mempool.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxchem.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxchem.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxcompiler.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxcompiler.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxdict.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxdict.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxdispersion.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxdispersion.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxerr.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxerr.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfile.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfile.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxinp.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxinp.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxout.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxout.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxproj.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxproj.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxqual.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxqual.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxrpt.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxrpt.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtank.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtank.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtoolkit.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtoolkit.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtypes.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtypes.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/newton.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/newton.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/newton.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/newton.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/rk5.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/rk5.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/rk5.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/rk5.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/ros2.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/ros2.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/ros2.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/ros2.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.c` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.h` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/EPANET/EPANET-MSX/readme.txt` & `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/readme.txt`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/__init__.py` & `epyt_flow-0.1.1/epyt_flow/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-import sys
 import subprocess
-import os
+import warnings
 import shutil
-
+import sys
+import os
 
 with open(os.path.join(os.path.dirname(__file__), 'VERSION'), encoding="utf-8") as f:
     VERSION = f.read().strip()
 
-
 if sys.platform.startswith("linux"):
-    path_to_custom_libs = os.path.join(os.path.dirname(__file__), "customlibs")
-    path_to_lib_epanet = os.path.join(path_to_custom_libs, "libepanet2_2.so")
-
-    update = False
-    if os.path.isfile(path_to_lib_epanet):
-        if os.path.getmtime(__file__) > os.path.getmtime(path_to_lib_epanet):
-            update = True
+    def compile_libraries():
+        """Compile EPANET and EPANET-MSX libraries if needed."""
+        path_to_custom_libs = os.path.join(os.path.dirname(__file__), "customlibs")
+        path_to_lib_epanet = os.path.join(path_to_custom_libs, "libepanet2_2.so")
+        path_to_epanet = os.path.join(os.path.dirname(__file__), "EPANET")
+
+        update = False
+        if os.path.isfile(path_to_lib_epanet):
+            if os.path.getmtime(__file__) > os.path.getmtime(path_to_lib_epanet):
+                update = True
+
+        if not os.path.isfile(path_to_lib_epanet) or update:
+            if shutil.which("gcc") is not None:
+                print("Compiling EPANET and EPANET-MSX...")
+                subprocess.check_call(f"cd \"{path_to_epanet}\"; bash compile.sh", shell=True)
+            else:
+                warnings.warn("GCC is not available to compile the required libraries.\n" +
+                              "Falling back to pre-compiled library shipped by EPyT.")
 
-    if not os.path.isfile(path_to_lib_epanet) or update is True:
-        if shutil.which("gcc") is not None:
-            print("Compiling EPANET and EPANET-MSX...")
-            path_to_epanet = os.path.join(os.path.dirname(__file__), "EPANET")
-            subprocess.check_call(f"cd \"{path_to_epanet}\"; bash compile.sh", shell=True)
+    compile_libraries()
```

### Comparing `epyt_flow-0.1.0/epyt_flow/data/benchmarks/__init__.py` & `epyt_flow-0.1.1/epyt_flow/data/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/data/benchmarks/batadal.py` & `epyt_flow-0.1.1/epyt_flow/data/benchmarks/batadal.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/data/benchmarks/batadal_data.py` & `epyt_flow-0.1.1/epyt_flow/data/benchmarks/batadal_data.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/data/benchmarks/battledim.py` & `epyt_flow-0.1.1/epyt_flow/data/benchmarks/battledim.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/data/benchmarks/battledim_data.py` & `epyt_flow-0.1.1/epyt_flow/data/benchmarks/battledim_data.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/data/benchmarks/gecco_water_quality.py` & `epyt_flow-0.1.1/epyt_flow/data/benchmarks/gecco_water_quality.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/data/benchmarks/leakdb.py` & `epyt_flow-0.1.1/epyt_flow/data/benchmarks/leakdb.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/data/benchmarks/leakdb_data.py` & `epyt_flow-0.1.1/epyt_flow/data/benchmarks/leakdb_data.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/data/benchmarks/water_usage.py` & `epyt_flow-0.1.1/epyt_flow/data/benchmarks/water_usage.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/data/networks.py` & `epyt_flow-0.1.1/epyt_flow/data/networks.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/gym/control_gyms.py` & `epyt_flow-0.1.1/epyt_flow/gym/control_gyms.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/gym/scenario_control_env.py` & `epyt_flow-0.1.1/epyt_flow/gym/scenario_control_env.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/metrics.py` & `epyt_flow-0.1.1/epyt_flow/metrics.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/models/event_detector.py` & `epyt_flow-0.1.1/epyt_flow/models/event_detector.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/models/sensor_interpolation_detector.py` & `epyt_flow-0.1.1/epyt_flow/models/sensor_interpolation_detector.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/rest_api/base_handler.py` & `epyt_flow-0.1.1/epyt_flow/rest_api/base_handler.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/rest_api/res_manager.py` & `epyt_flow-0.1.1/epyt_flow/rest_api/res_manager.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/rest_api/scada_data_handler.py` & `epyt_flow-0.1.1/epyt_flow/rest_api/scada_data_handler.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/rest_api/scenario_handler.py` & `epyt_flow-0.1.1/epyt_flow/rest_api/scenario_handler.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/rest_api/server.py` & `epyt_flow-0.1.1/epyt_flow/rest_api/server.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/serialization.py` & `epyt_flow-0.1.1/epyt_flow/serialization.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/events/actuator_events.py` & `epyt_flow-0.1.1/epyt_flow/simulation/events/actuator_events.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/events/event.py` & `epyt_flow-0.1.1/epyt_flow/simulation/events/event.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/events/leakages.py` & `epyt_flow-0.1.1/epyt_flow/simulation/events/leakages.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/events/sensor_faults.py` & `epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_faults.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/events/sensor_reading_attack.py` & `epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_reading_attack.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/events/sensor_reading_event.py` & `epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_reading_event.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/events/system_event.py` & `epyt_flow-0.1.1/epyt_flow/simulation/events/system_event.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/parallel_simulation.py` & `epyt_flow-0.1.1/epyt_flow/simulation/parallel_simulation.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/scada/advanced_control.py` & `epyt_flow-0.1.1/epyt_flow/simulation/scada/advanced_control.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/scada/scada_data.py` & `epyt_flow-0.1.1/epyt_flow/simulation/scada/scada_data.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/scada/scada_data_export.py` & `epyt_flow-0.1.1/epyt_flow/simulation/scada/scada_data_export.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/scenario_config.py` & `epyt_flow-0.1.1/epyt_flow/simulation/scenario_config.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/scenario_simulator.py` & `epyt_flow-0.1.1/epyt_flow/simulation/scenario_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,23 +325,23 @@
                     bulk_species.append(species_id)
                 elif species_type == "WALL":
                     surface_species.append(species_id)
 
         node_id_to_idx = {node_id: self.epanet_api.getNodeIndex(node_id) - 1 for node_id in nodes}
         link_id_to_idx = {link_id: self.epanet_api.getLinkIndex(link_id) - 1 for link_id in links}
         valve_id_to_idx = None  # {valve_id: self.epanet_api.getLinkValveIndex(valve_id) for valve_id in valves}
-        pump_id_to_idx = None # {pump_id: self.epanet_api.getLinkPumpIndex(pump_id) - 1 for pump_id in pumps}
-        tank_id_to_idx = None #{tank_id: self.epanet_api.getNodeTankIndex(tank_id) - 1 for tank_id in tanks}
+        pump_id_to_idx = None  # {pump_id: self.epanet_api.getLinkPumpIndex(pump_id) - 1 for pump_id in pumps}
+        tank_id_to_idx = None  # {tank_id: self.epanet_api.getNodeTankIndex(tank_id) - 1 for tank_id in tanks}
         bulkspecies_id_to_idx = None
         surfacespecies_id_to_idx = None
 
         if nodes != self.__sensor_config.nodes or links != self.__sensor_config.links or \
-            valves != self.__sensor_config.valves or pumps != self.__sensor_config.pumps or \
-            tanks != self.__sensor_config.tanks or \
-            bulk_species != self.__sensor_config.bulk_species or \
+                valves != self.__sensor_config.valves or pumps != self.__sensor_config.pumps or \
+                tanks != self.__sensor_config.tanks or \
+                bulk_species != self.__sensor_config.bulk_species or \
                 surface_species != self.__sensor_config.surface_species:
             # Adapt sensor configuration if anything in the network topology changed
             new_sensor_config = SensorConfig(nodes=nodes, links=links, valves=valves, pumps=pumps,
                                              tanks=tanks, bulk_species=bulk_species,
                                              surface_species=surface_species,
                                              node_id_to_idx=node_id_to_idx,
                                              link_id_to_idx=link_id_to_idx,
@@ -512,16 +512,16 @@
             Estimated memory consumption in MB.
         """
         self.__adapt_to_network_changes()
 
         n_time_steps = int(self.epanet_api.getTimeSimulationDuration() /
                            self.epanet_api.getTimeReportingStep())
         n_quantities = self.epanet_api.getNodeCount() * 3 + self.epanet_api.getNodeTankCount() + \
-            self.epanet_api.getLinkValveCount() + self.epanet_api.getLinkPumpCount() + \
-            self.epanet_api.getLinkCount() * 2
+                       self.epanet_api.getLinkValveCount() + self.epanet_api.getLinkPumpCount() + \
+                       self.epanet_api.getLinkCount() * 2
         n_bytes_per_quantity = 64
 
         return n_time_steps * n_quantities * n_bytes_per_quantity * .000001
 
     def get_topology(self) -> NetworkTopology:
         """
         Gets the topology (incl. information such as elevations, pipe diameters, etc.) of this WDN.
@@ -975,33 +975,48 @@
             Quality simulation results as SCADA data.
         """
         result = None
 
         gen = self.run_advanced_quality_simulation_as_generator
         for scada_data in gen(hyd_file_in=hyd_file_in,
                               verbose=verbose,
+                              return_as_dict=True,
                               frozen_sensor_config=frozen_sensor_config):
             if result is None:
-                result = scada_data
+                result = {}
+                for data_type, data in scada_data.items():
+                    result[data_type] = [data]
             else:
-                result.concatenate(scada_data)
+                for data_type, data in scada_data.items():
+                    result[data_type].append(data)
 
-        return result
+        # Build ScadaData instance
+        for data_type in result:
+            if not any(d is None for d in result[data_type]):
+                result[data_type] = np.concatenate(result[data_type], axis=0)
+            else:
+                result[data_type] = None
+
+        return ScadaData(**result,
+                         sensor_config=self.__sensor_config,
+                         sensor_reading_events=self.__sensor_reading_events,
+                         sensor_noise=self.__sensor_noise,
+                         frozen_sensor_config=frozen_sensor_config)
 
     def run_advanced_quality_simulation_as_generator(self, hyd_file_in: str, verbose: bool = False,
                                                      support_abort: bool = False,
                                                      return_as_dict: bool = False,
                                                      frozen_sensor_config: bool = False
-                                                     ) -> Generator[Union[ScadaData, dict],
-                                                                    bool, None]:
+                                                     ) -> Generator[Union[ScadaData, dict], bool, None]:
         """
         Runs an advanced quality analysis using EPANET-MSX.
 
         Parameters
         ----------
+        support_abort : `bool`, optional
         hyd_file_in : `str`
             Path to an EPANET .hyd file for storing the simulated hydraulics --
             the quality analysis is computed using those hydraulics.
         verbose : `bool`
             If True, method will be verbose (e.g. showing a progress bar).
         return_as_dict : `bool`, optional
             If True, simulation results/states are returned as a dictionary instead of a
@@ -1050,70 +1065,73 @@
                 msx_get_cur_value = self.epanet_api.getMSXSpeciesConcentration
 
             # Bulk species
             bulk_species_node_concentrations = []
             bulk_species_link_concentrations = []
             for species_idx in bulk_species_idx:
                 cur_species_concentrations = []
-                for node_idx in range(1, n_nodes+1):
+                for node_idx in range(1, n_nodes + 1):
                     concen = msx_get_cur_value(0, node_idx, species_idx)
                     cur_species_concentrations.append(concen)
                 bulk_species_node_concentrations.append(cur_species_concentrations)
 
                 cur_species_concentrations = []
-                for link_idx in range(1, n_links+1):
+                for link_idx in range(1, n_links + 1):
                     concen = msx_get_cur_value(1, link_idx, species_idx)
                     cur_species_concentrations.append(concen)
                 bulk_species_link_concentrations.append(cur_species_concentrations)
 
             if len(bulk_species_node_concentrations) == 0:
                 bulk_species_node_concentrations = None
             else:
-                bulk_species_node_concentrations = np.array(bulk_species_node_concentrations).\
+                bulk_species_node_concentrations = np.array(bulk_species_node_concentrations). \
                     reshape((1, len(bulk_species_idx), n_nodes))
 
             if len(bulk_species_link_concentrations) == 0:
                 bulk_species_link_concentrations = None
             else:
-                bulk_species_link_concentrations = np.array(bulk_species_link_concentrations).\
+                bulk_species_link_concentrations = np.array(bulk_species_link_concentrations). \
                     reshape((1, len(bulk_species_idx), n_links))
 
             # Surface species
             surface_species_concentrations = []
             for species_idx in surface_species_idx:
                 cur_species_concentrations = []
 
-                for link_idx in range(1, n_links+1):
+                for link_idx in range(1, n_links + 1):
                     concen = msx_get_cur_value(1, link_idx, species_idx)
                     cur_species_concentrations.append(concen)
 
                 surface_species_concentrations.append(cur_species_concentrations)
 
             if len(surface_species_concentrations) == 0:
                 surface_species_concentrations = None
             else:
-                surface_species_concentrations = np.array(surface_species_concentrations).\
+                surface_species_concentrations = np.array(surface_species_concentrations). \
                     reshape((1, len(surface_species_idx), n_links))
 
             return bulk_species_node_concentrations, bulk_species_link_concentrations, \
                 surface_species_concentrations
 
         # Initial concentrations:
         bulk_species_node_concentrations, bulk_species_link_concentrations, \
             surface_species_concentrations = __get_concentrations(init_qual=True)
 
         if verbose is True:
-            next(progress_bar)
+            try:
+                next(progress_bar)
+            except StopIteration:
+                pass
 
         if reporting_time_start == 0:
             if return_as_dict is True:
                 yield {"bulk_species_node_concentration_raw": bulk_species_node_concentrations,
                        "bulk_species_link_concentration_raw": bulk_species_link_concentrations,
                        "surface_species_concentration_raw": surface_species_concentrations,
-                       "sensor_readings_time": np.array([total_time])}
+                       "sensor_readings_time": np.array([0])}
             else:
                 yield ScadaData(sensor_config=self.__sensor_config,
                                 bulk_species_node_concentration_raw=bulk_species_node_concentrations,
                                 bulk_species_link_concentration_raw=bulk_species_link_concentrations,
                                 surface_species_concentration_raw=surface_species_concentrations,
                                 sensor_readings_time=np.array([0]),
                                 sensor_reading_events=self.__sensor_reading_events,
@@ -1127,29 +1145,32 @@
                 abort = yield
                 if abort is not False:
                     break
 
             # Compute current time step
             total_time, tleft = self.epanet_api.stepMSXQualityAnalysisTimeLeft()
 
+            if verbose is True:
+                try:
+                    next(progress_bar)
+                except StopIteration:
+                    pass
+
             # Fetch data at regular time intervals
             if total_time % hyd_time_step == 0:
                 bulk_species_node_concentrations, bulk_species_link_concentrations, \
                     surface_species_concentrations = __get_concentrations()
 
-                if verbose is True:
-                    next(progress_bar)
-
                 # Report results in a regular time interval only!
                 if total_time % reporting_time_step == 0 and total_time >= reporting_time_start:
                     if return_as_dict is True:
                         yield {"bulk_species_node_concentration_raw":
-                               bulk_species_node_concentrations,
+                                   bulk_species_node_concentrations,
                                "bulk_species_link_concentration_raw":
-                               bulk_species_link_concentrations,
+                                   bulk_species_link_concentrations,
                                "surface_species_concentration_raw": surface_species_concentrations,
                                "sensor_readings_time": np.array([total_time])}
                     else:
                         yield ScadaData(sensor_config=self.__sensor_config,
                                         bulk_species_node_concentration_raw=
                                         bulk_species_node_concentrations,
                                         bulk_species_link_concentration_raw=
@@ -1212,21 +1233,21 @@
                          sensor_noise=self.__sensor_noise,
                          frozen_sensor_config=frozen_sensor_config)
 
     def run_basic_quality_simulation_as_generator(self, hyd_file_in: str, verbose: bool = False,
                                                   support_abort: bool = False,
                                                   return_as_dict: bool = False,
                                                   frozen_sensor_config: bool = False,
-                                                  ) -> Generator[Union[ScadaData, dict],
-                                                                 bool, None]:
+                                                  ) -> Generator[Union[ScadaData, dict], bool, None]:
         """
         Runs a basic quality analysis using EPANET.
 
         Parameters
         ----------
+        support_abort : `bool`, optional
         hyd_file_in : `str`
             Path to an EPANET .hyd file for storing the simulated hydraulics --
             the quality analysis is computed using those hydraulics.
         verbose : `bool`, optional
             If True, method will be verbose (e.g. showing a progress bar).
 
             The default is False.
@@ -1273,24 +1294,24 @@
 
             if first_itr is True:  # Fix current time in the first iteration
                 tstep = 0
                 first_itr = False
 
             if verbose is True:
                 if (total_time + tstep) % requested_time_step == 0:
-                    next(progress_bar)
+                    try:
+                        next(progress_bar)
+                    except StopIteration:
+                        pass
 
             # Compute current time step
             t = self.epanet_api.runQualityAnalysis()
             total_time = t
 
             # Fetch data
-            quality_node_data = None
-            quality_link_data = None
-
             quality_node_data = self.epanet_api.getNodeActualQuality().reshape(1, -1)
             quality_link_data = self.epanet_api.getLinkActualQuality().reshape(1, -1)
 
             # Yield results in a regular time interval only!
             if total_time % reporting_time_step == 0 and total_time >= reporting_time_start:
                 if return_as_dict is True:
                     yield {"node_quality_data_raw": quality_node_data,
@@ -1377,15 +1398,19 @@
                              verbose=verbose,
                              frozen_sensor_config=frozen_sensor_config)
             result.join(result_msx)
 
             if hyd_export_old is not None:
                 shutil.copyfile(hyd_export, hyd_export_old)
 
-            os.remove(hyd_export)
+            try:
+                # temp solution
+                os.remove(hyd_export)
+            except:
+                warnings.warn(f"Failed to remove temporary file '{hyd_export}'")
 
         return result
 
     def run_simulation_as_generator(self, hyd_export: str = None, verbose: bool = False,
                                     support_abort: bool = False,
                                     return_as_dict: bool = False,
                                     frozen_sensor_config: bool = False,
@@ -1460,36 +1485,31 @@
                         break
 
                 if first_itr is True:  # Fix current time in the first iteration
                     tstep = 0
                     first_itr = False
 
                 if verbose is True:
-                    if (total_time + tstep) % requested_time_step == 0:
+                    #if (total_time + tstep) % requested_time_step == 0:
+                    try:
                         next(progress_bar)
+                    except StopIteration:
+                        pass
 
                 # Apply system events in a regular time interval only!
                 if (total_time + tstep) % requested_time_step == 0:
                     for event in self.__system_events:
                         event.step(total_time + tstep)
 
                 # Compute current time step
                 t = self.epanet_api.runHydraulicAnalysis()
                 self.epanet_api.runQualityAnalysis()
                 total_time = t
 
                 # Fetch data
-                pressure_data = None
-                flow_data = None
-                demand_data = None
-                quality_node_data = None
-                quality_link_data = None
-                pumps_state_data = None
-                valves_state_data = None
-
                 pressure_data = self.epanet_api.getNodePressure().reshape(1, -1)
                 flow_data = self.epanet_api.getLinkFlows().reshape(1, -1)
                 demand_data = self.epanet_api.getNodeActualDemand().reshape(1,
                                                                             -1)  # TODO: Does not go back after emitter coefficient is changed back to zero
                 quality_node_data = self.epanet_api.getNodeActualQuality().reshape(1, -1)
                 quality_link_data = self.epanet_api.getLinkActualQuality().reshape(1, -1)
                 pumps_state_data = self.epanet_api.getLinkPumpState().reshape(1, -1)
```

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/scenario_visualizer.py` & `epyt_flow-0.1.1/epyt_flow/simulation/scenario_visualizer.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/simulation/sensor_config.py` & `epyt_flow-0.1.1/epyt_flow/simulation/sensor_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,15 +608,15 @@
         links = epanet_api.getLinkNameID()
         valves = epanet_api.getLinkValveNameID()
         pumps = epanet_api.getLinkPumpNameID()
         tanks = epanet_api.getNodeTankNameID()
 
         bulk_species = []
         surface_species = []
-        if hasattr(epanet_api, "msx"):
+        if epanet_api.msx is not None:
             for species_id, species_type in zip(epanet_api.getMSXSpeciesNameID(),
                                                 epanet_api.getMSXSpeciesType()):
                 if species_type == "BULK":
                     bulk_species.append(species_id)
                 elif species_type == "WALL":
                     surface_species.append(species_id)
```

### Comparing `epyt_flow-0.1.0/epyt_flow/topology.py` & `epyt_flow-0.1.1/epyt_flow/topology.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/uncertainty/model_uncertainty.py` & `epyt_flow-0.1.1/epyt_flow/uncertainty/model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/uncertainty/sensor_noise.py` & `epyt_flow-0.1.1/epyt_flow/uncertainty/sensor_noise.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/uncertainty/uncertainties.py` & `epyt_flow-0.1.1/epyt_flow/uncertainty/uncertainties.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/uncertainty/utils.py` & `epyt_flow-0.1.1/epyt_flow/uncertainty/utils.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow/utils.py` & `epyt_flow-0.1.1/epyt_flow/utils.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/epyt_flow.egg-info/PKG-INFO` & `epyt_flow-0.1.1/epyt_flow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: epyt-flow
-Version: 0.1.0
+Version: 0.1.1
 Summary: EPyT-Flow -- EPANET Python Toolkit - Flow
 Author-email: André Artelt <aartelt@techfak.uni-bielefeld.de>, "Marios S. Kyriakou" <kiriakou.marios@ucy.ac.cy>, "Stelios G. Vrachimis" <vrachimis.stelios@ucy.ac.cy>
 License: MIT License
 Project-URL: Homepage, https://github.com/WaterFutures/EPyT-Flow
-Project-URL: Documentation, https://epytflow.readthedocs.io/en/latest/
+Project-URL: Documentation, https://epyt-flow.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/WaterFutures/EPyT-Flow.git
 Project-URL: Issues, https://github.com/WaterFutures/EPyT-Flow/issues
 Keywords: epanet,water,networks,hydraulics,quality,simulations
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: epyt>=1.1.3
+Requires-Dist: epyt>=1.1.6
 Requires-Dist: requests>=2.31.0
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: u-msgpack-python>=2.8.0
 Requires-Dist: networkx>=3.2.1
 Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: tqdm>=4.66.2
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: falcon>=3.1.3
 Requires-Dist: multiprocess>=0.70.16
 Requires-Dist: psutil
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pypi](https://img.shields.io/pypi/v/epyt-flow.svg)](https://pypi.org/project/epyt-flow/)
+[![build](https://github.com/WaterFutures/EPyT-Flow/actions/workflows/build_tests.yml/badge.svg)](https://github.com/WaterFutures/EPyT-Flow/actions/workflows/build_tests.yml)
+[![Documentation Status](https://readthedocs.org/projects/epyt-flow/badge/?version=stable)](https://epyt-flow.readthedocs.io/en/stable/?badge=stable)
+[![Downloads](https://static.pepy.tech/badge/epyt-flow)](https://pepy.tech/project/epyt-flow)
+[![Downloads](https://static.pepy.tech/badge/epyt-flow/month)](https://pepy.tech/project/epyt-flow)
+
 # EPyT-Flow -- EPANET Python Toolkit - Flow
 
 EPyT-Flow is a Python package building on top of [EPyT](https://github.com/OpenWaterAnalytics/EPyT) 
 for providing easy access to water distribution network simulations.
 It aims to provide a high-level interface for the easy generation of hydraulic and water quality scenario data.
 However, it also provides access to low-level functions by [EPANET](https://github.com/USEPA/EPANET2.2) 
 and [EPANET-MSX](https://github.com/USEPA/EPANETMSX/).
@@ -45,15 +52,15 @@
 
 ![](https://github.com/WaterFutures/EPyT-Flow/blob/main/docs/_static/net1_plot.png?raw=true)
 
 ## Installation
 
 EPyT-Flow supports Python 3.9 - 3.12
 
-Note that [EPANET and EPANET-MSX sources](epyt_flow/EPANET/) are compiled and overrite the binaries
+Note that [EPANET and EPANET-MSX sources](epyt_flow/EPANET/) are compiled and overwrite the binaries
 shipped by EPyT IF EPyT-Flow is installed on a Linux system. By this we not only aim to achieve
 a better performance of the simulations but also avoid any compatibility problems of pre-compiled binaries.
 
 ### PyPI
 
 ```
 pip install epyt-flow
@@ -109,15 +116,15 @@
         # Show sensor readings over the entire simulation
         print(f"Pressure readings: {scada_data.get_data_pressures()}")
         print(f"Flow readings: {scada_data.get_data_flows()}")
 ```
 
 ## Documentation
 
-Documentation is available on readthedocs: [https://epytflow.readthedocs.io/en/latest/](https://epytflow.readthedocs.io/en/latest/)
+Documentation is available on readthedocs:[https://epyt-flow.readthedocs.io/en/latest/](https://epyt-flow.readthedocs.io/en/stable)
 
 ## License
 
 MIT license -- see [LICENSE](LICENSE)
 
 ## How to Cite?
```

### Comparing `epyt_flow-0.1.0/epyt_flow.egg-info/SOURCES.txt` & `epyt_flow-0.1.1/epyt_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.0/pyproject.toml` & `epyt_flow-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.12"
 ]
 keywords=["epanet", "water", "networks", "hydraulics", "quality", "simulations"]
 dynamic = ["version", "readme", "dependencies"]
 
 [project.urls]
 Homepage = "https://github.com/WaterFutures/EPyT-Flow"
-Documentation = "https://epytflow.readthedocs.io/en/latest/"
+Documentation = "https://epyt-flow.readthedocs.io/en/latest/"
 Repository = "https://github.com/WaterFutures/EPyT-Flow.git"
 Issues = "https://github.com/WaterFutures/EPyT-Flow/issues"
 
 [tool.setuptools.packages]
 find = {}
 
 [tool.setuptools.dynamic]
```

