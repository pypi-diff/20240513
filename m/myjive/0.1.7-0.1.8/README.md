# Comparing `tmp/myjive-0.1.7.tar.gz` & `tmp/myjive-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myjive-0.1.7.tar", last modified: Wed Mar 20 15:58:14 2024, max compression
+gzip compressed data, was "myjive-0.1.8.tar", last modified: Mon May 13 11:19:01 2024, max compression
```

## Comparing `myjive-0.1.7.tar` & `myjive-0.1.8.tar`

### file list

```diff
@@ -1,108 +1,112 @@
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.057721 myjive-0.1.7/
--rw-rw-r--   0 anne      (1000) anne      (1000)     1053 2024-03-18 08:57:12.000000 myjive-0.1.7/LICENSE.txt
--rw-r--r--   0 anne      (1000) anne      (1000)     2714 2024-03-20 15:58:14.057721 myjive-0.1.7/PKG-INFO
--rw-rw-r--   0 anne      (1000) anne      (1000)     1921 2024-03-18 10:36:48.000000 myjive-0.1.7/README.md
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.049721 myjive-0.1.7/myjive/
--rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/__init__.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.049721 myjive-0.1.7/myjive/app/
--rw-rw-r--   0 anne      (1000) anne      (1000)       76 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/app/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)    14124 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/app/initmodule.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1310 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/app/main.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1154 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/app/module.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      512 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/app/outputmodule.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     2158 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/declare.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/fem/
--rw-rw-r--   0 anne      (1000) anne      (1000)      265 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1188 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/dofspace.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      565 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/element.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      423 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/elementgroup.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     2340 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/elementset.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1717 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/itemgroup.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1974 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/itemset.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/fem/jit/
--rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/jit/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      464 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/jit/shape.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      445 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/node.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      389 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/nodegroup.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     2228 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/nodeset.py
--rw-rw-r--   0 anne      (1000) anne      (1000)    14454 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/paramshapes.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     8082 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/fem/shape.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/implicit/
--rw-rw-r--   0 anne      (1000) anne      (1000)       58 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/implicit/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     6966 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/implicit/linsolvemodule.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      603 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/implicit/solvermodule.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/model/
--rw-rw-r--   0 anne      (1000) anne      (1000)       21 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/model/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1175 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/model/model.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/names/
--rw-rw-r--   0 anne      (1000) anne      (1000)       25 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/names/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      828 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/names/globnames.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/solver/
--rw-rw-r--   0 anne      (1000) anne      (1000)      333 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      838 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/cgsolver.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      891 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/cholmodsolver.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1921 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/constrainer.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      788 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/constraints.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      722 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/diagprecon.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      821 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/solver/directsolver.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      776 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/icholprecon.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      587 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/idprecon.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     2767 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/solver/iterativesolver.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/solver/jit/
--rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/jit/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     7186 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/jit/cholesky.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1466 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/jit/spsolve.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      864 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/jit/sputil.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1234 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/solver/preconditioner.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1703 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/solver/solver.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1308 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/sparsecholeskysolver.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/solver/util/
--rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/util/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      644 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/solver/util/reorder.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/util/
--rw-rw-r--   0 anne      (1000) anne      (1000)       43 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/util/__init__.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjive/util/jit/
--rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/util/jit/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      456 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/util/jit/xtable.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     5896 2024-03-20 15:54:41.000000 myjive-0.1.7/myjive/util/proputils.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     2615 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/util/table.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     2604 2024-03-18 08:57:12.000000 myjive-0.1.7/myjive/util/xtable.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.057721 myjive-0.1.7/myjive.egg-info/
--rw-r--r--   0 anne      (1000) anne      (1000)     2714 2024-03-20 15:58:13.000000 myjive-0.1.7/myjive.egg-info/PKG-INFO
--rw-rw-r--   0 anne      (1000) anne      (1000)     2317 2024-03-20 15:58:14.000000 myjive-0.1.7/myjive.egg-info/SOURCES.txt
--rw-rw-r--   0 anne      (1000) anne      (1000)        1 2024-03-20 15:58:14.000000 myjive-0.1.7/myjive.egg-info/dependency_links.txt
--rw-rw-r--   0 anne      (1000) anne      (1000)       81 2024-03-20 15:58:14.000000 myjive-0.1.7/myjive.egg-info/requires.txt
--rw-rw-r--   0 anne      (1000) anne      (1000)       15 2024-03-20 15:58:14.000000 myjive-0.1.7/myjive.egg-info/top_level.txt
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.053721 myjive-0.1.7/myjivex/
--rw-rw-r--   0 anne      (1000) anne      (1000)       23 2024-03-18 10:36:48.000000 myjive-0.1.7/myjivex/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1085 2024-03-18 10:36:48.000000 myjive-0.1.7/myjivex/declare.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.057721 myjive-0.1.7/myjivex/materials/
--rw-rw-r--   0 anne      (1000) anne      (1000)      157 2024-03-18 08:57:12.000000 myjive-0.1.7/myjivex/materials/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     2990 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/materials/deterioratedmaterial.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1517 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/materials/heterogeneousmaterial.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     3834 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/materials/isotropicmaterial.py
--rw-rw-r--   0 anne      (1000) anne      (1000)       97 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/materials/material.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      501 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/materials/newmaterial.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.057721 myjive-0.1.7/myjivex/models/
--rw-rw-r--   0 anne      (1000) anne      (1000)      215 2024-03-18 08:57:12.000000 myjive-0.1.7/myjivex/models/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     5971 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/models/barmodel.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1390 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/models/dirimodel.py
--rw-rw-r--   0 anne      (1000) anne      (1000)    15694 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/models/elasticmodel.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.057721 myjive-0.1.7/myjivex/models/jit/
--rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.7/myjivex/models/jit/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1138 2024-03-18 08:57:12.000000 myjive-0.1.7/myjivex/models/jit/solidmodel.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     3686 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/models/loadmodel.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     3006 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/models/neumannmodel.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     5593 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/models/poissonmodel.py
--rw-rw-r--   0 anne      (1000) anne      (1000)    17103 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/models/solidmodel.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     2926 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/models/timoshenkomodel.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.057721 myjive-0.1.7/myjivex/modules/
--rw-rw-r--   0 anne      (1000) anne      (1000)       28 2024-03-18 08:57:12.000000 myjive-0.1.7/myjivex/modules/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     5131 2024-03-20 15:54:41.000000 myjive-0.1.7/myjivex/modules/vtkoutmodule.py
-drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-03-20 15:58:14.057721 myjive-0.1.7/myjivex/util/
--rw-rw-r--   0 anne      (1000) anne      (1000)       27 2024-03-18 08:57:12.000000 myjive-0.1.7/myjivex/util/__init__.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     1816 2024-03-18 13:00:10.000000 myjive-0.1.7/myjivex/util/plotutils.py
--rw-rw-r--   0 anne      (1000) anne      (1000)     6730 2024-03-18 08:57:12.000000 myjive-0.1.7/myjivex/util/quickviewer.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      348 2024-03-18 08:57:12.000000 myjive-0.1.7/myjivex/util/testutils.py
--rw-rw-r--   0 anne      (1000) anne      (1000)      130 2024-03-20 15:58:14.057721 myjive-0.1.7/setup.cfg
--rw-rw-r--   0 anne      (1000) anne      (1000)      912 2024-03-20 15:57:52.000000 myjive-0.1.7/setup.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.593813 myjive-0.1.8/
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1053 2024-03-18 08:57:12.000000 myjive-0.1.8/LICENSE.txt
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2614 2024-05-13 11:19:01.593813 myjive-0.1.8/PKG-INFO
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1951 2024-05-13 11:08:34.000000 myjive-0.1.8/README.md
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.585813 myjive-0.1.8/myjive/
+-rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/__init__.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.585813 myjive-0.1.8/myjive/app/
+-rw-rw-r--   0 anne      (1000) anne      (1000)       76 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/app/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)    14546 2024-04-30 13:23:01.000000 myjive-0.1.8/myjive/app/initmodule.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1542 2024-04-30 13:23:01.000000 myjive-0.1.8/myjive/app/main.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2691 2024-05-07 10:11:38.000000 myjive-0.1.8/myjive/app/module.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     4230 2024-05-08 15:33:19.000000 myjive-0.1.8/myjive/app/outputmodule.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2158 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/declare.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/fem/
+-rw-rw-r--   0 anne      (1000) anne      (1000)      289 2024-04-04 14:33:22.000000 myjive-0.1.8/myjive/fem/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1188 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/dofspace.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      565 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/element.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      423 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/elementgroup.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2340 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/elementset.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1717 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/itemgroup.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1974 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/itemset.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/fem/jit/
+-rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/jit/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      464 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/jit/shape.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      445 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/node.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      389 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/nodegroup.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2228 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/fem/nodeset.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)    14210 2024-04-15 14:53:16.000000 myjive-0.1.8/myjive/fem/paramshapes.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1873 2024-04-04 14:33:22.000000 myjive-0.1.8/myjive/fem/pointset.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     8517 2024-04-12 07:53:16.000000 myjive-0.1.8/myjive/fem/shape.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/implicit/
+-rw-rw-r--   0 anne      (1000) anne      (1000)       58 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/implicit/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     7547 2024-05-08 15:33:53.000000 myjive-0.1.8/myjive/implicit/linsolvemodule.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      689 2024-04-30 13:23:01.000000 myjive-0.1.8/myjive/implicit/solvermodule.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/model/
+-rw-rw-r--   0 anne      (1000) anne      (1000)       21 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/model/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1630 2024-04-30 14:35:53.000000 myjive-0.1.8/myjive/model/model.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/names/
+-rw-rw-r--   0 anne      (1000) anne      (1000)       25 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/names/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      858 2024-04-12 08:48:30.000000 myjive-0.1.8/myjive/names/globnames.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/solver/
+-rw-rw-r--   0 anne      (1000) anne      (1000)      333 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/solver/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      848 2024-04-29 14:56:17.000000 myjive-0.1.8/myjive/solver/cgsolver.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      891 2024-04-04 07:52:21.000000 myjive-0.1.8/myjive/solver/cholmodsolver.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1921 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/solver/constrainer.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      788 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/solver/constraints.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      732 2024-04-29 14:56:17.000000 myjive-0.1.8/myjive/solver/diagprecon.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      831 2024-04-29 14:56:17.000000 myjive-0.1.8/myjive/solver/directsolver.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      786 2024-04-29 14:56:17.000000 myjive-0.1.8/myjive/solver/icholprecon.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      597 2024-04-29 14:56:17.000000 myjive-0.1.8/myjive/solver/idprecon.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2622 2024-04-30 13:23:01.000000 myjive-0.1.8/myjive/solver/iterativesolver.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/solver/jit/
+-rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/solver/jit/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     7186 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/solver/jit/cholesky.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1466 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/solver/jit/spsolve.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      864 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/solver/jit/sputil.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1682 2024-04-30 14:35:53.000000 myjive-0.1.8/myjive/solver/preconditioner.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2119 2024-04-30 14:35:53.000000 myjive-0.1.8/myjive/solver/solver.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1318 2024-04-29 14:56:17.000000 myjive-0.1.8/myjive/solver/sparsecholeskysolver.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/solver/util/
+-rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/solver/util/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      644 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/solver/util/reorder.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/util/
+-rw-rw-r--   0 anne      (1000) anne      (1000)       43 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/util/__init__.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjive/util/jit/
+-rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/util/jit/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      456 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/util/jit/xtable.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     6615 2024-05-08 15:33:19.000000 myjive-0.1.8/myjive/util/proputils.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      916 2024-04-30 14:35:53.000000 myjive-0.1.8/myjive/util/saveconfig.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2615 2024-03-18 08:57:12.000000 myjive-0.1.8/myjive/util/table.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2711 2024-04-05 14:50:58.000000 myjive-0.1.8/myjive/util/xtable.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.585813 myjive-0.1.8/myjive.egg-info/
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2614 2024-05-13 11:19:01.000000 myjive-0.1.8/myjive.egg-info/PKG-INFO
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2423 2024-05-13 11:19:01.000000 myjive-0.1.8/myjive.egg-info/SOURCES.txt
+-rw-rw-r--   0 anne      (1000) anne      (1000)        1 2024-05-13 11:19:01.000000 myjive-0.1.8/myjive.egg-info/dependency_links.txt
+-rw-rw-r--   0 anne      (1000) anne      (1000)       81 2024-05-13 11:19:01.000000 myjive-0.1.8/myjive.egg-info/requires.txt
+-rw-rw-r--   0 anne      (1000) anne      (1000)       15 2024-05-13 11:19:01.000000 myjive-0.1.8/myjive.egg-info/top_level.txt
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjivex/
+-rw-rw-r--   0 anne      (1000) anne      (1000)       23 2024-03-18 10:36:48.000000 myjive-0.1.8/myjivex/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1129 2024-03-27 11:03:54.000000 myjive-0.1.8/myjivex/declare.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.589813 myjive-0.1.8/myjivex/materials/
+-rw-rw-r--   0 anne      (1000) anne      (1000)      157 2024-03-18 08:57:12.000000 myjive-0.1.8/myjivex/materials/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2808 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/materials/deterioratedmaterial.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1486 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/materials/heterogeneousmaterial.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     3587 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/materials/isotropicmaterial.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      729 2024-04-30 14:35:53.000000 myjive-0.1.8/myjivex/materials/material.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      518 2024-04-29 14:56:17.000000 myjive-0.1.8/myjivex/materials/newmaterial.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.593813 myjive-0.1.8/myjivex/models/
+-rw-rw-r--   0 anne      (1000) anne      (1000)      215 2024-03-18 08:57:12.000000 myjive-0.1.8/myjivex/models/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     5710 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/models/barmodel.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1376 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/models/dirimodel.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)    15386 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/models/elasticmodel.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.593813 myjive-0.1.8/myjivex/models/jit/
+-rw-rw-r--   0 anne      (1000) anne      (1000)        0 2024-03-18 08:57:12.000000 myjive-0.1.8/myjivex/models/jit/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1138 2024-03-18 08:57:12.000000 myjive-0.1.8/myjivex/models/jit/solidmodel.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     3805 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/models/loadmodel.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2993 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/models/neumannmodel.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     5374 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/models/poissonmodel.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)    18327 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/models/solidmodel.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     2730 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/models/timoshenkomodel.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.593813 myjive-0.1.8/myjivex/modules/
+-rw-rw-r--   0 anne      (1000) anne      (1000)       54 2024-03-27 11:03:54.000000 myjive-0.1.8/myjivex/modules/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     6753 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/modules/viewmodule.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     5165 2024-04-30 13:23:01.000000 myjive-0.1.8/myjivex/modules/vtkoutmodule.py
+drwxrwxr-x   0 anne      (1000) anne      (1000)        0 2024-05-13 11:19:01.593813 myjive-0.1.8/myjivex/util/
+-rw-rw-r--   0 anne      (1000) anne      (1000)       53 2024-03-27 11:03:54.000000 myjive-0.1.8/myjivex/util/__init__.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     6458 2024-03-27 11:03:54.000000 myjive-0.1.8/myjivex/util/elemviewer.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     1816 2024-03-18 13:00:10.000000 myjive-0.1.8/myjivex/util/plotutils.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)     6730 2024-03-26 10:14:41.000000 myjive-0.1.8/myjivex/util/quickviewer.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      348 2024-03-18 08:57:12.000000 myjive-0.1.8/myjivex/util/testutils.py
+-rw-rw-r--   0 anne      (1000) anne      (1000)      130 2024-05-13 11:19:01.593813 myjive-0.1.8/setup.cfg
+-rw-rw-r--   0 anne      (1000) anne      (1000)      944 2024-05-13 11:08:34.000000 myjive-0.1.8/setup.py
```

### Comparing `myjive-0.1.7/LICENSE.txt` & `myjive-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/PKG-INFO` & `myjive-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: myjive
-Version: 0.1.7
+Version: 0.1.8
 Summary: Personal implementation of jive C++ library in Python
 Home-page: https://gitlab.tudelft.nl/apoot1/myjive
-Download-URL: https://gitlab.tudelft.nl/apoot1/myjive/-/archive/v0.1.7/myjive-v0.1.7.tar.gz
+Download-URL: https://gitlab.tudelft.nl/apoot1/myjive/-/archive/v0.1.8/myjive-v0.1.8.tar.gz
 Author: Anne Poot
 Author-email: a.poot-1@tudelft.nl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: ==3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: matplotlib==3.5.2
-Requires-Dist: numba==0.56.4
-Requires-Dist: numpy==1.23.5
-Requires-Dist: scikit-sparse==0.4.12
-Requires-Dist: scipy==1.8.1
 
 # MyJive
 A personal adaptation of [PyJive](https://gitlab.tudelft.nl/fmeer/pyjive) that is set up in a more "Pythonic" way.
 
 ## Getting started
 Run the following anaconda commands to take care of all dependencies:
 
 ```
 conda env create -f ENVIRONMENT.yml
 conda activate myjive
+conda develop /path/to/myjive
 ```
 
 ## Differences with PyJive
 PyJive is a Python adaptation of the C++ Jive library that stays very close to C++ setup.
 In MyJive, more liberty is taken, since Python offers a lot more flexibility that C++ does not have.
 
 Key differences are:
```

### Comparing `myjive-0.1.7/README.md` & `myjive-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 ## Getting started
 Run the following anaconda commands to take care of all dependencies:
 
 ```
 conda env create -f ENVIRONMENT.yml
 conda activate myjive
+conda develop /path/to/myjive
 ```
 
 ## Differences with PyJive
 PyJive is a Python adaptation of the C++ Jive library that stays very close to C++ setup.
 In MyJive, more liberty is taken, since Python offers a lot more flexibility that C++ does not have.
 
 Key differences are:
```

### Comparing `myjive-0.1.7/myjive/app/initmodule.py` & `myjive-0.1.8/myjive/app/initmodule.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,76 +2,84 @@
 
 from .module import Module
 from ..fem import XNodeSet
 from ..fem import NodeGroup
 from ..fem import XElementSet
 from ..fem import ElementGroup
 from ..fem import DofSpace
-
 from ..names import GlobNames as gn
-
-from ..util.proputils import optional_argument, mandatory_dict
+from ..util.proputils import check_dict, split_off_type
 
 TYPE = "type"
 FILE = "file"
 MODELS = "models"
 
 __all__ = ["InitModule"]
 
 
 class InitModule(Module):
     # Predefine some parameters
     _ctol = 1.0e-5
 
-    def init(self, globdat, **props):
-
-        # Get props
-        modelprops = mandatory_dict(self, props, "modelprops", mandatory_keys=[MODELS])
-        meshprops = mandatory_dict(self, props, "mesh", mandatory_keys=[TYPE, FILE])
-        nodeGroups = optional_argument(self, props, "nodeGroups", default=[])
-        elemGroups = optional_argument(self, props, "elemGroups", default=[])
+    def __init__(self, name):
+        super().__init__(name)
+        self._needs_modelprops = True
+
+    @Module.save_config
+    def configure(self, globdat, *, mesh, nodeGroups=[], elemGroups=[], **groupprops):
+        # Validate input arguments
+        check_dict(self, mesh, [TYPE, FILE])
+        self._meshprops = mesh
+        self._node_groups = nodeGroups
+        self._elem_groups = elemGroups
+        self._groupprops = groupprops
+
+    def init(self, globdat, *, modelprops):
+        # Validate input arguments
+        check_dict(self, modelprops, ["models"])
 
         # Initialize the node/elemenet group dictionaries
         globdat[gn.NGROUPS] = {}
         globdat[gn.EGROUPS] = {}
 
         modelfac = globdat[gn.MODELFACTORY]
 
         # Initialize DofSpace
         print("InitModule: Creating DofSpace...")
         globdat[gn.DOFSPACE] = DofSpace()
 
-        if "gmsh" in meshprops[TYPE]:
-            self._read_gmsh(meshprops[FILE], globdat)
-        elif "manual" in meshprops[TYPE]:
-            self._read_mesh(meshprops[FILE], globdat)
-        elif "meshio" in meshprops[TYPE]:
-            self._read_meshio(meshprops[FILE], globdat)
-        elif "geo" in meshprops[TYPE]:
-            self._read_geo(meshprops[FILE], globdat)
+        if "gmsh" in self._meshprops[TYPE]:
+            self._read_gmsh(self._meshprops[FILE], globdat)
+        elif "manual" in self._meshprops[TYPE]:
+            self._read_mesh(self._meshprops[FILE], globdat)
+        elif "meshio" in self._meshprops[TYPE]:
+            self._read_meshio(self._meshprops[FILE], globdat)
+        elif "geo" in self._meshprops[TYPE]:
+            self._read_geo(self._meshprops[FILE], globdat)
         else:
             raise KeyError("InitModule: Mesh input type unknown")
 
         # Create node groups
-        if nodeGroups is not None:
+        if self._node_groups is not None:
             print("InitModule: Creating node groups...")
-            self._create_ngroups(nodeGroups, globdat, **props)
+            self._create_ngroups(self._node_groups, globdat, **self._groupprops)
 
         # Create element groups
-        if elemGroups is not None:
+        if self._elem_groups is not None:
             print("InitModule: Creating element groups...")
-            self._create_egroups(elemGroups, globdat)
+            self._create_egroups(self._elem_groups, globdat)
 
         # Initialize model
         print("InitModule: Creating models...")
         name_list = modelprops[MODELS]
         model_list = []
         for name in name_list:
-            m = modelfac.get_model(modelprops[name][TYPE], name)
-            m.configure(globdat, **(modelprops[name]))
+            typ, mprops = split_off_type(modelprops[name])
+            m = modelfac.get_model(typ, name)
+            m.configure(globdat, **mprops)
             model_list.append(m)
         globdat[gn.MODELS] = model_list
 
     def run(self, globdat):
         return "ok"
 
     def shutdown(self, globdat):
@@ -219,15 +227,17 @@
                     parse_elems = True
 
                 elif parse_nodes and len(sp) > 1:
                     nodes.add_node(sp[1:], sp[0])
                     globdat[gn.MESHRANK] = len(sp) - 1
 
                 elif parse_elems and len(sp) > 0:
-                    elems.add_element(sp)
+                    inodes = nodes.find_nodes(sp)
+                    elems.add_element(inodes)
+                    globdat[gn.MESHSHAPE] = "Line{}".format(len(inodes))
 
         # Convert the XNodeSet and XElementSet to a normal NodeSet and ElementSet
         globdat[gn.NSET] = nodes.to_nodeset()
         globdat[gn.ESET] = elems.to_elementset()
 
         # Create node and element groups containing all items
         globdat[gn.NGROUPS]["all"] = NodeGroup(nodes, [*range(nodes.size())])
@@ -337,22 +347,22 @@
         globdat[gn.NSET] = nodes.to_nodeset()
         globdat[gn.ESET] = elems.to_elementset()
 
         # Create node and element groups containing all items
         globdat[gn.NGROUPS]["all"] = NodeGroup(nodes, [*range(nodes.size())])
         globdat[gn.EGROUPS]["all"] = ElementGroup(elems, [*range(elems.size())])
 
-    def _create_ngroups(self, groups, globdat, **props):
+    def _create_ngroups(self, groups, globdat, **groupprops):
         coords = globdat[gn.NSET].get_coords()
         cmax = np.max(coords, axis=1)
         cmin = np.min(coords, axis=1)
         cmid = 0.5 * (cmax + cmin)
         for g in groups:
             group = globdat[gn.NGROUPS]["all"].get_indices()
-            gprops = props[g]
+            gprops = groupprops[g]
             if isinstance(gprops, dict):
                 for i, axis in enumerate(["xtype", "ytype", "ztype"]):
                     if axis in gprops:
                         loc = str(gprops[axis])
                         if loc.replace(".", "").isnumeric():
                             lbnd = float(loc) - self._ctol
                             ubnd = float(loc) + self._ctol
```

### Comparing `myjive-0.1.7/myjive/app/main.py` & `myjive-0.1.8/myjive/app/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ..declare import declare_all
 from ..names import GlobNames as gn
+from ..util.proputils import split_off_type
 
 __all__ = ["jive"]
 
 
 def jive(props, extra_declares=[]):
     # Initialize global database, declare models and modules
     globdat = {}
@@ -19,24 +20,29 @@
 
     for name in props:
         # Get the name of each item in the property file
         if "type" in props[name]:
             typ = props[name]["type"]
         else:
             typ = name.title()
+            props[name]["type"] = typ
 
         # If it refers to a module (and not to a model), add it to the chain
         if modulefac.is_module(typ):
             chain.append(modulefac.get_module(typ, name))
 
     # Initialize chain
     for module in chain:
-        modelprops = props[gn.MODELS]
-        moduleprops = props[module._name]
-        module.init(globdat, modelprops=modelprops, **moduleprops)
+        moduleprops = props[module.get_name()]
+        typ, moduleprops = split_off_type(moduleprops)
+        module.configure(globdat, **moduleprops)
+        if module._needs_modelprops:
+            module.init(globdat, modelprops=props[gn.MODELS])
+        else:
+            module.init(globdat)
 
     # Run chain until one of the modules ends the computation
     print("Running chain...")
 
     for module in chain:
         if "exit" in module.run(globdat):
             break
```

### Comparing `myjive-0.1.7/myjive/app/module.py` & `myjive-0.1.8/myjive/solver/preconditioner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,69 @@
-__all__ = ["Module", "ModuleFactory"]
+from ..util import saveconfig as sg
 
+NOTIMPLEMENTEDMSG = "this function needs to be implemented in an derived class"
 
-class ModuleFactory:
+__all__ = ["Preconditioner", "PreconFactory"]
+
+
+class PreconFactory:
     def __init__(self):
-        self._creators = {}
+        self._precons = {}
 
-    def declare_module(self, typ, creator):
-        self._creators[typ] = creator
+    def declare_precon(self, typ, precon):
+        self._precons[typ] = precon
 
-    def get_module(self, typ, name):
-        creator = self._creators.get(typ)
-        if not creator:
+    def get_precon(self, typ, name):
+        precon = self._precons.get(typ)
+        if not precon:
             raise ValueError(typ)
-        return creator(name)
+        return precon(name)
 
-    def is_module(self, typ):
-        return typ in self._creators
+    def is_precon(self, typ):
+        return typ in self._precons
 
 
-class Module:
+class Preconditioner:
     def __init__(self, name):
         self._name = name
+        self._config = {}
+
+    @classmethod
+    def get_type(cls):
+        typ = cls.__name__
+        if typ[-6:] == "Precon":
+            typ = typ[:-6]
+        return typ
 
     @classmethod
     def declare(cls, factory):
-        name = cls.__name__
-        if len(name) > 6 and name[-6:] == "Module":
-            name = name[:-6]
-        factory.declare_module(name, cls)
-
-    def get_relevant_models(self, action, models):
-        model_list = []
-        for model in models:
-            if action in model.list_actions():
-                model_list.append(model)
-        return model_list
-
-    def init(self, globdat, **props):
-        print("Empty module init")
-
-    def run(self, globdat):
-        print("Empty module run")
-        return "exit"
+        typ = cls.get_type()
+        factory.declare_precon(typ, cls)
+
+    @sg.save_config
+    def configure(self, globdat, *, precision=1e-8):
+        self._precision = precision
+
+    def update(self, sourcematrix):
+        raise NotImplementedError(NOTIMPLEMENTEDMSG)
+
+    def dot(self, lhs):
+        raise NotImplementedError(NOTIMPLEMENTEDMSG)
+
+    def solve(self, rhs):
+        raise NotImplementedError(NOTIMPLEMENTEDMSG)
+
+    def get_matrix(self):
+        raise NotImplementedError(NOTIMPLEMENTEDMSG)
+
+    def get_config(self):
+        if len(self._config) == 0:
+            raise NotImplementedError("Empty preconditioner get_config")
+        else:
+            return self._config
+
+    def get_name(self):
+        return self._name
 
-    def shutdown(self, globdat):
-        print("Empty module shutdown")
+    @staticmethod
+    def save_config(configure):
+        return sg.save_config(configure)
```

### Comparing `myjive-0.1.7/myjive/app/outputmodule.py` & `myjive-0.1.8/myjive/implicit/solvermodule.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,41 @@
-from .module import Module
-from ..names import GlobNames as gn
+from ..app import Module
 
-__all__ = ["OutputModule"]
+__all__ = ["SolverModule"]
 
 
-class OutputModule(Module):
-    def init(self, globdat, **props):
+class SolverModule(Module):
+    def configure(self, globdat):
+        pass
+
+    def init(self, globdat):
         pass
 
     def run(self, globdat):
-        # Temporary strat
-        fname = "step" + str(globdat[gn.TIMESTEP]) + ".disp"
-        u = globdat[gn.STATE0]
-        print(u)
-
-        with open(fname, "w") as out:
-            for val in u:
-                out.write(str(val) + "\n")
+        while True:
+            self.advance(globdat)
+
+            self.solve(globdat)
+
+            if self.commit(globdat):
+                break
+
+            print("Solution rejected; retrying\n")
+
+            self.cancel(globdat)
 
         return "ok"
 
+    def advance(self, globat):
+        pass
+
+    def solve(self, globdat):
+        pass
+
+    def cancel(self, globdat):
+        pass
+
     def shutdown(self, globdat):
         pass
+
+    def commit(self, globdat):
+        return True
```

### Comparing `myjive-0.1.7/myjive/declare.py` & `myjive-0.1.8/myjive/declare.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/fem/dofspace.py` & `myjive-0.1.8/myjive/fem/dofspace.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/fem/element.py` & `myjive-0.1.8/myjive/fem/element.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/fem/elementset.py` & `myjive-0.1.8/myjive/fem/elementset.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/fem/itemgroup.py` & `myjive-0.1.8/myjive/fem/itemgroup.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/fem/itemset.py` & `myjive-0.1.8/myjive/fem/itemset.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/fem/nodeset.py` & `myjive-0.1.8/myjive/fem/nodeset.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/fem/paramshapes.py` & `myjive-0.1.8/myjive/fem/paramshapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     "Line2Shape",
     "Line3Shape",
 ]
 
 
 class Tri3Shape(Shape):
     def __init__(self, intscheme):
-        print("Creating Tri3Shape...")
-
         # Set the nodecount and rank of the elements
         self._ncount = 3
         self._rank = 2
 
         # Refer to the Shape class to handle the rest of the initialization
         super().__init__(intscheme)
 
@@ -96,16 +94,14 @@
             return False
         else:
             return True
 
 
 class Tri6Shape(Shape):
     def __init__(self, intscheme):
-        print("Creating Tri6Shape...")
-
         # Set the nodecount and rank of the elements
         self._ncount = 6
         self._rank = 2
 
         # Refer to the Shape class to handle the rest of the initialization
         super().__init__(intscheme)
 
@@ -177,16 +173,14 @@
             return False
         else:
             return True
 
 
 class Quad4Shape(Shape):
     def __init__(self, intscheme):
-        print("Creating Quad4Shape...")
-
         # Set the nodecount and rank of the elements
         self._ncount = 4
         self._rank = 2
 
         # Refer to the Shape class to handle the rest of the initialization
         super().__init__(intscheme)
 
@@ -250,16 +244,14 @@
             return False
         else:
             return True
 
 
 class Quad9Shape(Shape):
     def __init__(self, intscheme):
-        print("Creating Quad9Shape...")
-
         # Set the nodecount and rank of the elements
         self._ncount = 9
         self._rank = 2
 
         # Refer to the Shape class to handle the rest of the initialization
         super().__init__(intscheme)
 
@@ -352,16 +344,14 @@
             return False
         else:
             return True
 
 
 class Line2Shape(Shape):
     def __init__(self, intscheme):
-        print("Creating Line2Shape...")
-
         # Set the nodecount and rank of the elements
         self._ncount = 2
         self._rank = 1
 
         # Refer to the Shape class to handle the rest of the initialization
         super().__init__(intscheme)
 
@@ -413,16 +403,14 @@
             return False
         else:
             return True
 
 
 class Line3Shape(Shape):
     def __init__(self, intscheme):
-        print("Creating Line2Shape...")
-
         # Set the nodecount and rank of the elements
         self._ncount = 3
         self._rank = 1
 
         # Refer to the Shape class to handle the rest of the initialization
         super().__init__(intscheme)
```

### Comparing `myjive-0.1.7/myjive/fem/shape.py` & `myjive-0.1.8/myjive/fem/shape.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from numpy.polynomial.legendre import leggauss
 from scipy.optimize import fsolve
 from warnings import warn
 from .jit.shape import get_shape_gradients_jit
 
 NOTIMPLEMENTEDMSG = "this function needs to be implemented in an derived class"
 
 __all__ = ["Shape", "ShapeFactory"]
@@ -26,24 +27,16 @@
     def __init__(self, intscheme):
         # Note: these two parameters need to be implemented in the derived class
         # self._ncount = None
         # self._rank = None
 
         self._int = intscheme
 
-        if self._int == "Gauss1":
-            self._ipcount = 1
-        elif self._int == "Gauss2":
-            self._ipcount = 2
-        elif self._int == "Gauss3":
-            self._ipcount = 3
-        elif self._int == "Gauss4":
-            self._ipcount = 4
-        elif self._int == "Gauss9":
-            self._ipcount = 9
+        if self._int.lstrip("Gauss").isnumeric():
+            self._ipcount = int(self._int.lstrip("Gauss"))
         else:
             raise ValueError(self._int)
 
         self._ips = np.zeros((self._rank, self._ipcount))
         self._wts = np.zeros(self._ipcount)
 
         if self._rank == 1:
@@ -61,14 +54,17 @@
                 self._ips[0, 0] = -np.sqrt(3.0 / 5.0)
                 self._ips[0, 1] = 0
                 self._ips[0, 2] = np.sqrt(3.0 / 5.0)
                 self._wts[0] = 5.0 / 9.0
                 self._wts[1] = 8.0 / 9.0
                 self._wts[2] = 5.0 / 9.0
 
+            elif self._int.lstrip("Gauss").isnumeric():
+                self._ips[0, :], self._wts[:] = leggauss(self._ipcount)
+
             else:
                 raise ValueError(self._int)
 
         elif self._rank == 2:
             if self._ncount == 3 or self._ncount == 6:
                 if self._int == "Gauss1":
                     self._ips[0, 0] = 1.0 / 3.0
@@ -193,14 +189,18 @@
 
     def get_shape_functions(self):
         return self._N
 
     def eval_shape_functions(self, loc_point):
         raise NotImplementedError(NOTIMPLEMENTEDMSG)
 
+    def eval_global_shape_functions(self, glob_point, glob_coords):
+        loc_point = self.get_local_point(glob_point, glob_coords)
+        return self.eval_shape_functions(loc_point)
+
     def get_global_point(self, loc_point, glob_coords):
         sfuncs = self.eval_shape_functions(loc_point)
         return np.matmul(glob_coords, sfuncs)
 
     def get_local_point(self, glob_point, glob_coords):
         # Note: since this is (in general) a non-linear problem, a non-linear solver must be called.
         # Inherited classes are encouraged to get more efficient implementations
@@ -228,7 +228,13 @@
         raise NotImplementedError(NOTIMPLEMENTEDMSG)
 
     def get_shape_gradients(self, glob_coords):
         return get_shape_gradients_jit(glob_coords, self._dN, self._wts, self._ipcount)
 
     def eval_shape_gradients(self, loc_point):
         raise NotImplementedError(NOTIMPLEMENTEDMSG)
+
+    def eval_global_shape_gradients(self, glob_point, glob_coords):
+        loc_point = self.get_local_point(glob_point, glob_coords)
+        J = glob_coords @ self.eval_shape_gradients(loc_point)
+        J_inv = np.linalg.inv(J)
+        return self.eval_shape_gradients(loc_point) @ J_inv
```

### Comparing `myjive-0.1.7/myjive/implicit/linsolvemodule.py` & `myjive-0.1.8/myjive/implicit/linsolvemodule.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,55 +2,61 @@
 import scipy.sparse as spsp
 
 from ..names import GlobNames as gn
 
 from .solvermodule import SolverModule
 from ..solver import Constraints
 from ..util import Table, to_xtable
-from ..util.proputils import optional_argument
+from ..util.proputils import check_dict, split_off_type
 
 TYPE = "type"
 
 __all__ = ["LinsolveModule"]
 
 
 class LinsolveModule(SolverModule):
-    def init(self, globdat, **props):
+    @SolverModule.save_config
+    def configure(
+        self,
+        globdat,
+        *,
+        solver={TYPE: "Cholmod"},
+        preconditioner={},
+        getMassMatrix=False,
+        getStrainMatrix=False,
+        tables=[],
+        elemTables=[]
+    ):
+        # Validate input arguments
+        check_dict(self, solver, [TYPE])
+        self._get_mass_matrix = getMassMatrix
+        self._get_strain_matrix = getStrainMatrix
+        self._tnames = tables
+        self._etnames = elemTables
 
-        super().init(globdat, **props)
-
-        # Get props
-        solverprops = optional_argument(
-            self, props, "solver", default={TYPE: "Cholmod"}
-        )
-        preconprops = optional_argument(self, props, "preconditioner", default={})
-        self._get_mass_matrix = optional_argument(
-            self, props, "getMassMatrix", default=False
-        )
-        self._get_strain_matrix = optional_argument(
-            self, props, "getStrainMatrix", default=False
-        )
-        self._tnames = optional_argument(self, props, "tables", default=[])
-
-        self._models = globdat[gn.MODELS]
-        self._dc = globdat[gn.DOFSPACE].dof_count()
-
-        solvertype = solverprops[TYPE]
-        self._solver = globdat[gn.SOLVERFACTORY].get_solver(solvertype)
+        solvertype, solverprops = split_off_type(solver)
+        self._solver = globdat[gn.SOLVERFACTORY].get_solver(solvertype, "solver")
         self._solver.configure(globdat, **solverprops)
+        self._config["solver"] = self._solver.get_config()
 
         self._precon = None
 
-        if len(preconprops) > 0:
-            precontype = preconprops[TYPE]
-            self._precon = globdat[gn.PRECONFACTORY].get_precon(precontype)
+        if len(preconditioner) > 0:
+            precontype, preconprops = split_off_type(preconditioner)
+            self._precon = globdat[gn.PRECONFACTORY].get_precon(
+                precontype, "preconditioner"
+            )
             self._precon.configure(globdat, **preconprops)
+            self._config["preconditioner"] = self._precon.get_config()
+
+    def init(self, globdat):
+        pass
 
     def solve(self, globdat):
-        print("Running LinsolverModule")
+        # print("Running LinsolverModule")
         globdat[gn.TIMESTEP] = 1
 
         K = self.update_matrix(globdat)
         f = self.get_ext_vector(globdat)
         c = self.update_constraints(globdat)
 
         # Optionally get the mass matrix
@@ -88,79 +94,94 @@
             globdat[gn.TABLES] = {}
 
         for name in self._tnames:
             nodecount = len(globdat[gn.NSET])
             table = Table(size=nodecount)
             tbwts = np.zeros(nodecount)
 
-            for model in self.get_relevant_models("GETTABLE", self._models):
+            for model in self.get_relevant_models("GETTABLE", globdat[gn.MODELS]):
                 table, tbwts = model.GETTABLE(name, table, tbwts, globdat)
 
             to_xtable(table)
 
             for jcol in range(table.column_count()):
                 values = table.get_col_values(None, jcol)
                 table.set_col_values(None, jcol, values / tbwts)
 
             table.to_table()
             globdat[gn.TABLES][name] = table
 
+        if gn.ELEMTABLES not in globdat:
+            globdat[gn.ELEMTABLES] = {}
+
+        for name in self._etnames:
+            elemcount = len(globdat[gn.ESET])
+            table = Table(size=elemcount)
+
+            for model in self.get_relevant_models("GETELEMTABLE", globdat[gn.MODELS]):
+                table = model.GETELEMTABLE(name, table, globdat)
+
+            globdat[gn.ELEMTABLES][name] = table
+
         return "ok"
 
+    def shutdown(self, globdat):
+        pass
+
     def get_ext_vector(self, globdat):
         f_ext = np.zeros(globdat[gn.DOFSPACE].dof_count())
 
-        for model in self.get_relevant_models("GETEXTFORCE", self._models):
+        for model in self.get_relevant_models("GETEXTFORCE", globdat[gn.MODELS]):
             f_ext = model.GETEXTFORCE(f_ext, globdat)
 
         return f_ext
 
     def get_neumann_vector(self, globdat):
         f_neum = np.zeros(globdat[gn.DOFSPACE].dof_count())
 
-        for model in self.get_relevant_models("GETNEUMANNFORCE", self._models):
+        for model in self.get_relevant_models("GETNEUMANNFORCE", globdat[gn.MODELS]):
             f_neum = model.GETNEUMANNFORCE(f_neum, globdat)
 
         return f_neum
 
     def update_matrix(self, globdat):
         K = self._get_empty_matrix(globdat)
 
-        for model in self.get_relevant_models("GETMATRIX0", self._models):
+        for model in self.get_relevant_models("GETMATRIX0", globdat[gn.MODELS]):
             K = model.GETMATRIX0(K, globdat)
 
         return K
 
     def update_mass_matrix(self, globdat):
         M = self._get_empty_matrix(globdat)
 
-        for model in self.get_relevant_models("GETMATRIX2", self._models):
+        for model in self.get_relevant_models("GETMATRIX2", globdat[gn.MODELS]):
             M = model.GETMATRIX2(M, globdat)
 
         return M
 
     def update_strain_matrix(self, globdat):
         B = self._get_empty_bmatrix(globdat)
         wts = np.zeros(B.shape[0])
 
-        for model in self.get_relevant_models("GETMATRIXB", self._models):
+        for model in self.get_relevant_models("GETMATRIXB", globdat[gn.MODELS]):
             B, wts = model.GETMATRIXB(B, wts, globdat)
 
         # Divide non-zero entries by weights
         str_indices, dof_indices = B.nonzero()
         for i, str_idx in enumerate(str_indices):
             dof_idx = dof_indices[i]
             B[str_idx, dof_idx] /= wts[str_idx]
 
         return B
 
     def update_constraints(self, globdat):
         c = Constraints()
 
-        for model in self.get_relevant_models("GETCONSTRAINTS", self._models):
+        for model in self.get_relevant_models("GETCONSTRAINTS", globdat[gn.MODELS]):
             c = model.GETCONSTRAINTS(c, globdat)
 
         return c
 
     def advance(self, globat):
         pass
```

### Comparing `myjive-0.1.7/myjive/names/globnames.py` & `myjive-0.1.8/myjive/names/globnames.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,12 +22,13 @@
     OLDSTATE0 = "oldstate0"
     BACKUPSTATE0 = "backupstate0"
     HISTORY = "history"
     MATRIX0 = "matrix0"
     MATRIX2 = "matrix2"
     MATRIXB = "matrixB"
     TABLES = "tables"
+    ELEMTABLES = "elemTables"
     LAMBDA = "lambda"
     MODULEDATA = "module"
     SLIDERS = "sliders"
     ACCEPTED = "accepted"
     LBFACTORS = "lbFactors"
```

### Comparing `myjive-0.1.7/myjive/solver/cgsolver.py` & `myjive-0.1.8/myjive/solver/cgsolver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .iterativesolver import IterativeSolver
 
 __all__ = ["CGSolver"]
 
 
 class CGSolver(IterativeSolver):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, name):
+        super().__init__(name)
 
         self._p = None
 
     def start(self):
         self._p = None
 
     def finish(self):
```

### Comparing `myjive-0.1.7/myjive/solver/cholmodsolver.py` & `myjive-0.1.8/myjive/solver/cholmodsolver.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/solver/constrainer.py` & `myjive-0.1.8/myjive/solver/constrainer.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/solver/constraints.py` & `myjive-0.1.8/myjive/solver/constraints.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/solver/diagprecon.py` & `myjive-0.1.8/myjive/solver/diagprecon.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from .preconditioner import Preconditioner
 
 __all__ = ["DiagPrecon"]
 
 
 class DiagPrecon(Preconditioner):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, name):
+        super().__init__(name)
 
         self._sourcematrix = None
         self._M = None
         self._M_inv = None
 
     def update(self, sourcematrix):
         self._sourcematrix = sourcematrix
```

### Comparing `myjive-0.1.7/myjive/solver/directsolver.py` & `myjive-0.1.8/myjive/solver/directsolver.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from .solver import Solver
 from .constrainer import Constrainer
 
 __all__ = ["DirectSolver"]
 
 
 class DirectSolver(Solver):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, name):
+        super().__init__(name)
 
         self._matrix = None
         self._cons = None
         self._conman = None
 
     def update(self, matrix, constraints, preconditioner=None):
         self._cons = constraints
```

### Comparing `myjive-0.1.7/myjive/solver/icholprecon.py` & `myjive-0.1.8/myjive/solver/icholprecon.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from .jit.cholesky import incomplete_cholesky
 from .jit.spsolve import solve_triangular
 
 __all__ = ["ICholPrecon"]
 
 
 class ICholPrecon(Preconditioner):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, name):
+        super().__init__(name)
 
         self._sourcematrix = None
         self._L = None
         self._LT = None
 
     def update(self, sourcematrix):
         self._sourcematrix = sourcematrix
```

### Comparing `myjive-0.1.7/myjive/solver/idprecon.py` & `myjive-0.1.8/myjive/solver/idprecon.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from .preconditioner import Preconditioner
 
 __all__ = ["IdPrecon"]
 
 
 class IdPrecon(Preconditioner):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, name):
+        super().__init__(name)
 
         self._sourcematrix = None
         self._M = None
 
     def update(self, sourcematrix):
         self._sourcematrix = sourcematrix
         self._M = spsp.identity(self._sourcematrix.shape[0], format="csr")
```

### Comparing `myjive-0.1.7/myjive/solver/iterativesolver.py` & `myjive-0.1.8/myjive/solver/iterativesolver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 import numpy as np
 import warnings
 
-from myjive.util.proputils import optional_argument
 from .solver import Solver
 from .constrainer import Constrainer
 
 NOTIMPLEMENTEDMSG = "this function needs to be implemented in an derived class"
 
 __all__ = ["IterativeSolver"]
 
 
 class IterativeSolver(Solver):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, name):
+        super().__init__(name)
 
         self._matrix = None
         self._cons = None
         self._conman = None
         self._precon = None
 
         self._init_guess = None
 
-    def configure(self, globdat, **props):
-        super().configure(globdat, **props)
+    def configure(self, globdat, maxIter=2000, allowMaxIter=False):
+        super().configure(globdat)
 
-        self._maxiter = optional_argument(self, props, "maxIter", default=2000)
-        self._allow_max_iter = optional_argument(
-            self, props, "allowMaxIter", default=False
-        )
+        self._maxiter = maxIter
+        self._allow_max_iter = allowMaxIter
 
     def update(self, matrix, constraints, preconditioner=None):
         self._cons = constraints
         self._conman = Constrainer(self._cons, matrix)
         self._matrix = self._conman.get_output_matrix()
         self._precon = preconditioner
         if self._precon is not None:
```

### Comparing `myjive-0.1.7/myjive/solver/jit/cholesky.py` & `myjive-0.1.8/myjive/solver/jit/cholesky.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/solver/jit/spsolve.py` & `myjive-0.1.8/myjive/solver/jit/spsolve.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/solver/jit/sputil.py` & `myjive-0.1.8/myjive/solver/jit/sputil.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/solver/sparsecholeskysolver.py` & `myjive-0.1.8/myjive/solver/sparsecholeskysolver.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from .jit.cholesky import sparse_cholesky
 from .jit.spsolve import solve_triangular
 
 __all__ = ["SparseCholeskySolver"]
 
 
 class SparseCholeskySolver(DirectSolver):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, name):
+        super().__init__(name)
 
         self._P = None
         self._L = None
         self._LT = None
 
     def update(self, matrix, constraints, preconditioner=None):
         self._cons = constraints
```

### Comparing `myjive-0.1.7/myjive/solver/util/reorder.py` & `myjive-0.1.8/myjive/solver/util/reorder.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/util/proputils.py` & `myjive-0.1.8/myjive/util/proputils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,73 @@
+import numpy as np
+import re
 from ast import literal_eval
+from copy import deepcopy
 
 
 def parse_file(fname):
     fileraw = open(fname, "r").read()
 
     filestr = uncomment_file(fileraw)
 
     data = {}
 
     i = 0
     sp = filestr.split(";")
 
     while i < len(sp):
-        line = sp[i].replace(" ", "")
-        if "{" in line:
+        line = re.sub(r"=\s*{", "={", sp[i])
+
+        if "={" in line:
             key = line.split("={")[0]
+            key = key.strip()
+
             newline = "={".join(line.split("={")[1:])
             data[key], i, sp = read_level(newline, i, sp)
         elif line != "":
             raise RuntimeError("Unable to parse: %s" % line)
 
         i = i + 1
 
     return data
 
 
 def read_level(line, i, sp):
     subdata = {}
 
     while True:
-        if "{" in line:
+        if "={" in line:
             key = line.split("={")[0]
+            key = key.strip()
+
             newline = "={".join(line.split("={")[1:])
             subdata[key], i, sp = read_level(newline, i, sp)
-        elif "}" in line:
-            return subdata, i, sp
         elif "=" in line:
             [key, value] = line.split("=")
+            key = key.strip()
+            value = value.strip()
 
             if value.startswith("[") and value.endswith("]"):
-                valuelist = value.strip("[").strip("]").split(",")
-                parsedlist = []
-                for val in valuelist:
-                    parsedlist.append(try_literal_eval(val))
-                subdata[key] = parsedlist
+                subdata[key] = parse_list(value)
             else:
                 subdata[key] = try_literal_eval(value)
+        elif "}" in line:
+            return subdata, i, sp
 
         elif line != "":
             raise RuntimeError("Unable to parse: %s" % line)
 
         i = i + 1
 
         if i == len(sp):
             raise RuntimeError(
                 "EOF reached while parsing an input block. Did you forget to close a bracket?"
             )
 
-        line = sp[i].replace(" ", "")
+        line = re.sub(r"=\s*{", "={", sp[i])
 
 
 def uncomment_file(fileraw):
     filestr = ""
     comment_mode = False
 
     # Go through all lines in the raw file
@@ -85,15 +91,15 @@
             # If there is a '/*' in the line, enable comment mode, and remove the part after '/*' from the line
             start = line.find("/*")
             if start >= 0:
                 comment_mode = True
                 line = line[:start]
 
         # Add the line to the file string
-        filestr += line.replace("\t", "")
+        filestr += line
 
     return filestr
 
 
 def uncomment_line(line):
     clean_line = line
 
@@ -114,14 +120,42 @@
         else:
             # Exit if no comments are left
             break
 
     return clean_line
 
 
+def parse_list(value):
+    if not value.startswith("[") or not value.endswith("]"):
+        raise ValueError("Not a valid list")
+
+    lst = []
+    val = ""
+    depth = 0
+    for s in value:
+        if s == "[":
+            depth += 1
+
+        if s not in [",", "[", "]"] or depth > 1:
+            val += s
+        elif depth == 1 and s in [",", "]"]:
+            val = val.strip()
+            if val.startswith("[") and val.endswith("]"):
+                val = parse_list(val)
+            else:
+                val = try_literal_eval(val)
+            lst.append(val)
+            val = ""
+
+        if s == "]":
+            depth -= 1
+
+    return lst
+
+
 def try_literal_eval(val):
     try:
         return literal_eval(val)
     except:
         return val
 
 
@@ -155,52 +189,65 @@
     # Add the extra dictionary if applicable
     if extra_dict is not None:
         eval_dict.update(extra_dict)
 
     return eval_dict
 
 
-def optional_argument(obj, props, arg, default=None):
-    val = props.get(arg, default)
-    return val
+def get_core_eval_dict():
+    core_eval_dict = {
+        "exp": np.exp,
+        "sin": np.sin,
+        "cos": np.cos,
+        "tan": np.tan,
+        "pi": np.pi,
+        "sqrt": np.sqrt,
+    }
 
+    return core_eval_dict
 
-def mandatory_argument(obj, props, arg):
+
+def check_dict(obj, dic, keys=[]):
     name = obj.__class__.__name__
-    val = props.get(arg)
-    if val is None:
-        raise ValueError("Unspecified argument in {}".format(name))
-    else:
-        return val
+    if not isinstance(dic, dict):
+        raise ValueError("Argument in {} must be a dict".format(name))
+    for key in keys:
+        if key not in dic.keys():
+            raise ValueError("Argument in {} must contain '{}' key".format(name, key))
 
 
-def mandatory_list(obj, props, arg, min_length=0):
+def check_list(obj, lst):
     name = obj.__class__.__name__
-    val = props.get(arg)
-    if val is None:
-        raise ValueError("Unspecified argument in {}".format(name))
-    elif type(val) is not list:
+    if not isinstance(lst, list):
         raise ValueError("Argument in {} must be a list".format(name))
-    elif len(val) < min_length:
-        raise ValueError(
-            "Argument in {} must be a list containing at least {} values".format(
-                name, min_length
-            )
-        )
-    else:
-        return val
 
 
-def mandatory_dict(obj, props, arg, mandatory_keys=[]):
+def check_value(obj, val, options=[]):
     name = obj.__class__.__name__
-    val = props.get(arg)
     if val is None:
-        raise ValueError("Unspecified argument in {}".format(name))
-    elif type(val) is not dict:
-        raise ValueError("Argument in {} must be a dict".format(name))
-    else:
-        for key in mandatory_keys:
-            if key not in val.keys():
-                raise ValueError(
-                    "Argument in {} must contain '{}' key".format(name, key)
-                )
-        return val
+        raise ValueError("Argument in {} cannot be 'None'".format(name))
+    if len(options) > 0 and val not in options:
+        raise ValueError("Argument in {} must be one of {}".format(name, options))
+
+
+def split_off_type(props):
+    cprops = deepcopy(props)
+    typ = cprops.pop("type")
+    return typ, cprops
+
+
+def get_recursive(dic, keys):
+    sub = dic
+    for key in keys:
+        sub = sub[key]
+    return sub
+
+
+def set_recursive(dic, keys, value):
+    sub = dic
+    for i, key in enumerate(keys):
+        if i == len(keys) - 1:
+            sub[key] = value
+        else:
+            if key not in sub:
+                sub[key] = {}
+            sub = sub[key]
```

### Comparing `myjive-0.1.7/myjive/util/table.py` & `myjive-0.1.8/myjive/util/table.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjive/util/xtable.py` & `myjive-0.1.8/myjive/util/xtable.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 
     def clear_all(self):
         self._header = np.zeros(0)
         self.clear_data()
 
     def reserve(self, rowcount):
         if self.row_count() < rowcount:
-            self._data.resize((rowcount, self.column_count()), refcheck=False)
+            new_data = np.zeros(rowcount, self.column_count())
+            new_data[: self.row_count(), :] = self._data
+            self._data = new_data
 
     def add_column(self, name):
         if self.find_column(name) < 0:
             self._header = np.append(self._header, name)
-            self._data.resize(
-                (self.row_count(), self.column_count() + 1), refcheck=False
-            )
+            new_data = np.zeros((self.row_count(), self.column_count() + 1))
+            new_data[:, :-1] = self._data
+            self._data = new_data
         return self.find_column(name)
 
     def add_columns(self, names):
         for name in names:
             self.add_column(name)
         return self.find_columns(names)
```

### Comparing `myjive-0.1.7/myjive.egg-info/PKG-INFO` & `myjive-0.1.8/myjive.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: myjive
-Version: 0.1.7
+Version: 0.1.8
 Summary: Personal implementation of jive C++ library in Python
 Home-page: https://gitlab.tudelft.nl/apoot1/myjive
-Download-URL: https://gitlab.tudelft.nl/apoot1/myjive/-/archive/v0.1.7/myjive-v0.1.7.tar.gz
+Download-URL: https://gitlab.tudelft.nl/apoot1/myjive/-/archive/v0.1.8/myjive-v0.1.8.tar.gz
 Author: Anne Poot
 Author-email: a.poot-1@tudelft.nl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: ==3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: matplotlib==3.5.2
-Requires-Dist: numba==0.56.4
-Requires-Dist: numpy==1.23.5
-Requires-Dist: scikit-sparse==0.4.12
-Requires-Dist: scipy==1.8.1
 
 # MyJive
 A personal adaptation of [PyJive](https://gitlab.tudelft.nl/fmeer/pyjive) that is set up in a more "Pythonic" way.
 
 ## Getting started
 Run the following anaconda commands to take care of all dependencies:
 
 ```
 conda env create -f ENVIRONMENT.yml
 conda activate myjive
+conda develop /path/to/myjive
 ```
 
 ## Differences with PyJive
 PyJive is a Python adaptation of the C++ Jive library that stays very close to C++ setup.
 In MyJive, more liberty is taken, since Python offers a lot more flexibility that C++ does not have.
 
 Key differences are:
```

### Comparing `myjive-0.1.7/myjive.egg-info/SOURCES.txt` & `myjive-0.1.8/myjive.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 myjive/fem/elementset.py
 myjive/fem/itemgroup.py
 myjive/fem/itemset.py
 myjive/fem/node.py
 myjive/fem/nodegroup.py
 myjive/fem/nodeset.py
 myjive/fem/paramshapes.py
+myjive/fem/pointset.py
 myjive/fem/shape.py
 myjive/fem/jit/__init__.py
 myjive/fem/jit/shape.py
 myjive/implicit/__init__.py
 myjive/implicit/linsolvemodule.py
 myjive/implicit/solvermodule.py
 myjive/model/__init__.py
@@ -52,14 +53,15 @@
 myjive/solver/jit/cholesky.py
 myjive/solver/jit/spsolve.py
 myjive/solver/jit/sputil.py
 myjive/solver/util/__init__.py
 myjive/solver/util/reorder.py
 myjive/util/__init__.py
 myjive/util/proputils.py
+myjive/util/saveconfig.py
 myjive/util/table.py
 myjive/util/xtable.py
 myjive/util/jit/__init__.py
 myjive/util/jit/xtable.py
 myjivex/__init__.py
 myjivex/declare.py
 myjivex/materials/__init__.py
@@ -76,12 +78,14 @@
 myjivex/models/neumannmodel.py
 myjivex/models/poissonmodel.py
 myjivex/models/solidmodel.py
 myjivex/models/timoshenkomodel.py
 myjivex/models/jit/__init__.py
 myjivex/models/jit/solidmodel.py
 myjivex/modules/__init__.py
+myjivex/modules/viewmodule.py
 myjivex/modules/vtkoutmodule.py
 myjivex/util/__init__.py
+myjivex/util/elemviewer.py
 myjivex/util/plotutils.py
 myjivex/util/quickviewer.py
 myjivex/util/testutils.py
```

### Comparing `myjive-0.1.7/myjivex/declare.py` & `myjive-0.1.8/myjivex/declare.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     LoadModel,
     NeumannModel,
     PoissonModel,
     SolidModel,
     TimoshenkoModel,
 )
 
-from .modules import VTKOutModule
+from .modules import VTKOutModule, ViewModule
 
 __all__ = ["declare_all", "declare_models", "declare_modules"]
 
 
 def declare_all(globdat):
     # Declare all core models and modules in one go
     declare_models(globdat)
@@ -39,9 +39,10 @@
     globdat[gn.MODELFACTORY] = factory
 
 
 def declare_modules(globdat):
     factory = globdat.get(gn.MODULEFACTORY, ModuleFactory())
 
     VTKOutModule.declare(factory)
+    ViewModule.declare(factory)
 
     globdat[gn.MODULEFACTORY] = factory
```

### Comparing `myjive-0.1.7/myjivex/materials/deterioratedmaterial.py` & `myjive-0.1.8/myjivex/materials/deterioratedmaterial.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 from .heterogeneousmaterial import HeterogeneousMaterial
 from myjive.names import GlobNames as gn
 from scipy.stats import norm
 import numpy as np
-from myjive.util.proputils import mandatory_argument, optional_argument
 import myjive.util.proputils as pu
 
 
 __all__ = ["DeterioratedMaterial"]
 
 
 class DeterioratedMaterial(HeterogeneousMaterial):
-    def configure(self, globdat, **props):
-        super().configure(globdat, **props)
+    @HeterogeneousMaterial.save_config
+    def configure(
+        self,
+        globdat,
+        *,
+        deteriorations,
+        scale=1.0,
+        locX="x",
+        locY="y",
+        stdX=1.0,
+        stdY=1.0,
+        seed=None,
+        **otherprops
+    ):
+        super().configure(globdat, **otherprops)
 
         # Get props
-        self._ndet = mandatory_argument(self, props, "deteriorations")
-        self._detscale = optional_argument(self, props, "scale", default=1.0)
-        self._locx = optional_argument(self, props, "locX", default="x")
-        self._locy = optional_argument(self, props, "locY", default="y")
-        self._stdx = optional_argument(self, props, "stdX", default=1.0)
-        self._stdy = optional_argument(self, props, "stdY", default=1.0)
-        self._seed = optional_argument(self, props, "seed", default=None)
+        self._ndet = deteriorations
+        self._detscale = scale
+        self._locx, self._locy = locX, locY
+        self._stdx, self._stdy = stdX, stdY
+        self._seed = seed
 
         self._detlocs = np.zeros((self._rank, self._ndet))
         self._detrads = np.zeros((self._rank, self._ndet))
 
         self._generate_deteriorations(globdat)
 
         globdat["detlocs"] = self._detlocs
```

### Comparing `myjive-0.1.7/myjivex/materials/heterogeneousmaterial.py` & `myjive-0.1.8/myjivex/materials/heterogeneousmaterial.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from .isotropicmaterial import IsotropicMaterial
-from myjive.util.proputils import mandatory_argument, optional_argument
 import myjive.util.proputils as pu
-import numpy as np
 
 __all__ = ["HeterogeneousMaterial"]
 
 
 class HeterogeneousMaterial(IsotropicMaterial):
+    @IsotropicMaterial.save_config
+    def configure(
+        self, globdat, *, rank, anmodel, E=1.0, nu=1.0, rho=0.0, area=1.0, params={}
+    ):
+        # Validate input arguments
+        self._rank = rank
+        self._anmodel = anmodel
+        self._E = E
+        self._nu = nu
+        self._rho = rho
+        self._area = area
 
-    def configure(self, globdat, **props):
-
-        # Get props
-        self._rank = mandatory_argument(self, props, "rank")
-        self._anmodel = mandatory_argument(self, props, "anmodel")
-        self._E = optional_argument(self, props, "E", default=1.0)
-        self._nu = optional_argument(self, props, "nu", default=0.0)
-        self._rho = optional_argument(self, props, "rho", default=0.0)
-        self._area = optional_argument(self, props, "area", default=1.0)
+        self._eval_dict = pu.get_core_eval_dict()
+        self._eval_dict.update(params)
 
         self._strcount = self._rank * (self._rank + 1) // 2
         assert self._is_valid_anmodel(self._anmodel), (
             "Analysis model " + self._anmodel + " not valid for rank " + str(self._rank)
         )
 
     def stiff_at_point(self, ipoint=None):
         return self._compute_stiff_matrix(ipoint)
 
     def mass_at_point(self, ipoint=None):
         return self._compute_mass_matrix(ipoint)
 
     def _get_E(self, ipoint=None):
-        return pu.evaluate(self._E, ipoint, self._rank)
+        return pu.evaluate(self._E, ipoint, self._rank, extra_dict=self._eval_dict)
 
     def _get_nu(self, ipoint=None):
-        return pu.evaluate(self._nu, ipoint, self._rank)
+        return pu.evaluate(self._nu, ipoint, self._rank, extra_dict=self._eval_dict)
 
     def _get_rho(self, ipoint=None):
-        return pu.evaluate(self._rho, ipoint, self._rank)
+        return pu.evaluate(self._rho, ipoint, self._rank, extra_dict=self._eval_dict)
 
     def _get_area(self, ipoint=None):
-        return pu.evaluate(self._area, ipoint, self._rank)
+        return pu.evaluate(self._area, ipoint, self._rank, extra_dict=self._eval_dict)
```

### Comparing `myjive-0.1.7/myjivex/materials/isotropicmaterial.py` & `myjive-0.1.8/myjivex/materials/isotropicmaterial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from .material import Material
-from myjive.util.proputils import mandatory_argument, optional_argument
 import numpy as np
 
 BAR = "bar"
 PLANE_STRESS = "plane_stress"
 PLANE_STRAIN = "plane_strain"
 SOLID = "solid"
 
 __all__ = ["IsotropicMaterial"]
 
 
 class IsotropicMaterial(Material):
-    def configure(self, globdat, **props):
-
-        # Get props
-        self._rank = mandatory_argument(self, props, "rank")
-        self._anmodel = mandatory_argument(self, props, "anmodel")
-        self._E = optional_argument(self, props, "E", default=1.0)
-        self._nu = optional_argument(self, props, "nu", default=0.0)
-        self._rho = optional_argument(self, props, "rho", default=0.0)
-        self._area = optional_argument(self, props, "area", default=1.0)
+    @Material.save_config
+    def configure(self, globdat, *, rank, anmodel, E=1.0, nu=1.0, rho=0.0, area=1.0):
+        # Validate input arguments
+        self._rank = rank
+        self._anmodel = anmodel
+        self._E = E
+        self._nu = nu
+        self._rho = rho
+        self._area = area
 
         self._strcount = self._rank * (self._rank + 1) // 2
         assert self._is_valid_anmodel(self._anmodel), (
             "Analysis model " + self._anmodel + " not valid for rank " + str(self._rank)
         )
 
         self._stiff_matrix = np.zeros((self._strcount, self._strcount))
```

### Comparing `myjive-0.1.7/myjivex/models/barmodel.py` & `myjive-0.1.8/myjivex/models/poissonmodel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,91 @@
 import numpy as np
 
 from myjive.names import GlobNames as gn
 from myjive.model.model import Model
-from myjive.util.proputils import mandatory_argument, mandatory_dict, optional_argument
+from myjive.util.proputils import check_dict
 
 TYPE = "type"
 INTSCHEME = "intScheme"
-DOFTYPES = ["dx"]
+DOFTYPES = ["u"]
 
-__all__ = ["BarModel"]
+__all__ = ["PoissonModel"]
 
 
-class BarModel(Model):
+class PoissonModel(Model):
     def GETMATRIX0(self, K, globdat, **kwargs):
         K = self._get_matrix(K, globdat, **kwargs)
         return K
 
     def GETMATRIX2(self, M, globdat, **kwargs):
         M = self._get_mass_matrix(M, globdat, **kwargs)
         return M
 
-    def configure(self, globdat, **props):
-
-        # Get props
-        shapeprops = mandatory_dict(
-            self, props, "shape", mandatory_keys=[TYPE, INTSCHEME]
-        )
-        elements = mandatory_argument(self, props, "elements")
-        self._EA = mandatory_argument(self, props, "EA")
-        self._k = optional_argument(self, props, "k", default=0.0)
-        self._rhoA = optional_argument(self, props, "rhoA", default=0.0)
+    @Model.save_config
+    def configure(self, globdat, *, shape, elements, kappa, rho=0.0):
+        # Validate input arguments
+        check_dict(self, shape, [TYPE, INTSCHEME])
+        self._kappa = kappa
+        self._rho = rho
 
         # Get shape and element info
-        self._shape = globdat[gn.SHAPEFACTORY].get_shape(
-            shapeprops[TYPE], shapeprops[INTSCHEME]
-        )
+        self._shape = globdat[gn.SHAPEFACTORY].get_shape(shape[TYPE], shape[INTSCHEME])
         egroup = globdat[gn.EGROUPS][elements]
         self._elems = egroup.get_elements()
         self._ielems = egroup.get_indices()
         self._nodes = self._elems.get_nodes()
 
+        # Make sure the shape rank and mesh rank are identitcal
+        if self._shape.global_rank() != globdat[gn.MESHRANK]:
+            raise RuntimeError("PoissonModel: Shape rank must agree with mesh rank")
+
         # The rest of the configuration happens in configure_noprops
         self._configure_noprops(globdat)
 
     def _configure_noprops(self, globdat):
         # This function gets additional info from self and globdat
         # It has been split off from configure() to allow it to be used in inherited classes as well.
 
         # Get basic dimensionality info
         self._rank = self._shape.global_rank()
         self._ipcount = self._shape.ipoint_count()
-        self._nodecount = self._shape.node_count()
-        self._dofcount = self._rank * self._nodecount
-        self._strcount = self._rank * (self._rank + 1) // 2  # 1-->1, 2-->3, 3-->6
+        self._dofcount = len(DOFTYPES) * self._shape.node_count()
 
         # Create a new dof for every node and dof type
-        nodes = np.unique([node for elem in self._elems for node in elem.get_nodes()])
         for doftype in DOFTYPES[0 : self._rank]:
             globdat[gn.DOFSPACE].add_type(doftype)
-            for node in nodes:
-                globdat[gn.DOFSPACE].add_dof(node, doftype)
+            for inode in self._elems.get_unique_nodes_of(self._ielems):
+                globdat[gn.DOFSPACE].add_dof(inode, doftype)
 
     def _get_matrix(self, K, globdat):
         if K is None:
             dc = globdat[gn.DOFSPACE].dof_count()
             K = np.zeros((dc, dc))
 
         for ielem in self._ielems:
             # Get the nodal coordinates of each element
             inodes = self._elems.get_elem_nodes(ielem)
-            idofs = globdat[gn.DOFSPACE].get_dofs(inodes, DOFTYPES[0 : self._rank])
+            idofs = globdat[gn.DOFSPACE].get_dofs(inodes, DOFTYPES)
             coords = self._nodes.get_some_coords(inodes)
 
-            # Get the shape functions, gradients, weights and coordinates of each integration point
-            sfuncs = self._shape.get_shape_functions()
+            # Get the gradients, weights and coordinates of each integration point
             grads, weights = self._shape.get_shape_gradients(coords)
             ipcoords = self._shape.get_global_integration_points(coords)
 
             # Reset the element stiffness matrix
             elmat = np.zeros((self._dofcount, self._dofcount))
 
             for ip in range(self._ipcount):
-                # Get the B, N, D and K matrices for each integration point
+                # Get the B and D matrices for each integration point
                 B_elem = self._get_B_matrix(grads[:, :, ip])
-                N_elem = self._get_N_matrix(sfuncs[:, ip])
                 D_elem = self._get_D_matrix(ipcoords[:, ip])
-                K_elem = self._get_K_matrix(ipcoords[:, ip])
 
                 # Compute the element stiffness matrix
-                elmat += weights[ip] * (
-                    np.matmul(np.transpose(B_elem), np.matmul(D_elem, B_elem))
-                    + np.matmul(np.transpose(N_elem), np.matmul(K_elem, N_elem))
+                elmat += weights[ip] * np.matmul(
+                    np.transpose(B_elem), np.matmul(D_elem, B_elem)
                 )
 
             # Add the element stiffness matrix to the global stiffness matrix
             K[np.ix_(idofs, idofs)] += elmat
 
         return K
 
@@ -134,27 +125,23 @@
 
             # Add the element mass matrix to the global mass matrix
             M[np.ix_(idofs, idofs)] += elmat
 
         return M
 
     def _get_N_matrix(self, sfuncs):
-        N = np.zeros((1, self._nodecount))
+        N = np.zeros((1, self._dofcount))
         N[0, :] = sfuncs.transpose()
         return N
 
     def _get_B_matrix(self, grads):
-        B = np.zeros((1, self._nodecount))
-        B[0, :] = grads.transpose()
+        B = np.zeros((self._rank, self._dofcount))
+        B[:, :] = grads.transpose()
         return B
 
     def _get_D_matrix(self, ipcoords):
-        D = np.array([[self._EA]])
+        D = self._kappa * np.identity(self._rank)
         return D
 
-    def _get_K_matrix(self, ipcoords):
-        K = np.array([[self._k]])
-        return K
-
     def _get_M_matrix(self, ipcoords):
-        M = np.array([[self._rhoA]])
+        M = np.array([[self._rho]])
         return M
```

### Comparing `myjive-0.1.7/myjivex/models/dirimodel.py` & `myjive-0.1.8/myjivex/models/dirimodel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import numpy as np
 
 from myjive.names import GlobNames as gn
 from myjive.model.model import Model
-
-from myjive.util.proputils import mandatory_list, optional_argument
+from myjive.util.proputils import check_list
 
 __all__ = ["DirichletModel"]
 
 
 class DirichletModel(Model):
     def GETCONSTRAINTS(self, c, globdat, **kwargs):
         c = self._get_constraints(c, globdat, **kwargs)
         return c
 
     def ADVANCE(self, globdat):
         self._advance_step_constraints(globdat)
 
-    def configure(self, globdat, **props):
-
-        # Get props
-        self._groups = mandatory_list(self, props, "groups")
-        self._dofs = mandatory_list(self, props, "dofs")
-        self._vals = mandatory_list(self, props, "values")
-        dispIncr = optional_argument(self, props, "dispIncr")
+    @Model.save_config
+    def configure(self, globdat, *, groups, dofs, values, dispIncr=None):
+        # Validate input arguments
+        check_list(self, groups)
+        check_list(self, dofs)
+        check_list(self, values)
+        self._groups = groups
+        self._dofs = dofs
+        self._vals = values
 
         self._initDisp = self._vals
         if dispIncr is None:
             self._dispIncr = np.zeros(len(self._vals))
         else:
             self._dispIncr = dispIncr
```

### Comparing `myjive-0.1.7/myjivex/models/elasticmodel.py` & `myjive-0.1.8/myjivex/models/elasticmodel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from myjive.names import GlobNames as gn
 from myjive.model.model import Model
 from myjive.util import Table, to_xtable
-from myjive.util.proputils import mandatory_argument, mandatory_dict, optional_argument
+from myjive.util.proputils import check_dict, check_value
 
 TYPE = "type"
 INTSCHEME = "intScheme"
 DOFTYPES = ["dx", "dy", "dz"]
 PE_STATE = "plane_strain"
 PS_STATE = "plane_stress"
 
@@ -30,38 +30,41 @@
     def GETTABLE(self, name, table, tbwts, globdat, **kwargs):
         if "stress" in name:
             table, tbwts = self._get_stresses(table, tbwts, globdat, **kwargs)
         elif "strain" in name:
             table, tbwts = self._get_strains(table, tbwts, globdat, **kwargs)
         return table, tbwts
 
-    def configure(self, globdat, **props):
-
-        # Get props
-        shapeprops = mandatory_dict(
-            self, props, "shape", mandatory_keys=[TYPE, INTSCHEME]
-        )
-        elements = mandatory_argument(self, props, "elements")
-        self._young = mandatory_argument(self, props, "young")
-        self._rho = optional_argument(self, props, "rho", default=0.0)
-
+    @Model.save_config
+    def configure(
+        self,
+        globdat,
+        *,
+        shape,
+        elements,
+        young,
+        rho=0.0,
+        poisson=None,
+        thickness=1.0,
+        state=None
+    ):
+        # Validate input arguments
+        check_dict(self, shape, [TYPE, INTSCHEME])
         if globdat[gn.MESHRANK] > 1:
-            self._poisson = mandatory_argument(self, props, "poisson")
+            check_value(self, poisson)
         if globdat[gn.MESHRANK] == 2:
-            self._thickness = optional_argument(self, props, "thickness", default=1.0)
-            self._state = mandatory_argument(self, props, "state")
-            if not self._state in (PE_STATE, PS_STATE):
-                raise RuntimeError(
-                    "ElasticModel: state in 2d should be plane_strain or plane_stress"
-                )
+            check_value(self, state, [PE_STATE, PS_STATE])
+        self._young = young
+        self._rho = rho
+        self._poisson = poisson
+        self._thickness = thickness
+        self._state = state
 
         # Get shape and element info
-        self._shape = globdat[gn.SHAPEFACTORY].get_shape(
-            shapeprops[TYPE], shapeprops[INTSCHEME]
-        )
+        self._shape = globdat[gn.SHAPEFACTORY].get_shape(shape[TYPE], shape[INTSCHEME])
         egroup = globdat[gn.EGROUPS][elements]
         self._elems = egroup.get_elements()
         self._ielems = egroup.get_indices()
         self._nodes = self._elems.get_nodes()
 
         # Make sure the shape rank and mesh rank are identitcal
         if self._shape.global_rank() != globdat[gn.MESHRANK]:
```

### Comparing `myjive-0.1.7/myjivex/models/jit/solidmodel.py` & `myjive-0.1.8/myjivex/models/jit/solidmodel.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjivex/models/loadmodel.py` & `myjive-0.1.8/myjivex/models/loadmodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import numpy as np
 
 from myjive.names import GlobNames as gn
 from myjive.model.model import Model
 import myjive.util.proputils as pu
-from myjive.util.proputils import mandatory_argument, mandatory_dict, mandatory_list
+from myjive.util.proputils import check_dict, check_list
 
 TYPE = "type"
 INTSCHEME = "intScheme"
 
 __all__ = ["LoadModel"]
 
 
 class LoadModel(Model):
     def GETEXTFORCE(self, f_ext, globdat, **kwargs):
         f_ext = self._get_body_force(f_ext, globdat, **kwargs)
         return f_ext
 
-    def configure(self, globdat, **props):
-
-        # Get props
-        shapeprops = mandatory_dict(
-            self, props, "shape", mandatory_keys=[TYPE, INTSCHEME]
-        )
-        elements = mandatory_argument(self, props, "elements")
-        self._doftypes = mandatory_list(self, props, "dofs")
-        self._loads = mandatory_list(self, props, "values")
+    @Model.save_config
+    def configure(self, globdat, *, shape, elements, dofs, values, params={}):
+        # Validate input arguments
+        check_dict(self, shape, [TYPE, INTSCHEME])
+        check_list(self, dofs)
+        check_list(self, values)
+        check_dict(self, params)
+        self._doftypes = dofs
+        self._loads = values
 
         # Get shape and element info
-        self._shape = globdat[gn.SHAPEFACTORY].get_shape(
-            shapeprops[TYPE], shapeprops[INTSCHEME]
-        )
+        self._shape = globdat[gn.SHAPEFACTORY].get_shape(shape[TYPE], shape[INTSCHEME])
         egroup = globdat[gn.EGROUPS][elements]
         self._elems = egroup.get_elements()
         self._ielems = egroup.get_indices()
         self._nodes = self._elems.get_nodes()
 
         # Make sure the shape rank and mesh rank are identitcal
         if self._shape.global_rank() != globdat[gn.MESHRANK]:
@@ -51,14 +49,18 @@
         if len(self._doftypes) != len(self._loads):
             raise ValueError("LoadModel: dofs and values must have the same size")
 
         # Get the dofcount (of only the relevant dofs!)
         self._loadcount = len(self._doftypes)
         self._dofcount = self._loadcount * self._shape.node_count()
 
+        # Get the dictionary for load evaluation
+        self._eval_dict = pu.get_core_eval_dict()
+        self._eval_dict.update(params)
+
     def _get_body_force(self, f_ext, globdat):
         if f_ext is None:
             f_ext = np.zeros(globdat[gn.DOFSPACE].dof_count())
 
         for ielem in self._ielems:
             # Get the nodal coordinates of each element
             inodes = self._elems.get_elem_nodes(ielem)
@@ -91,9 +93,11 @@
         for i in range(self._loadcount):
             N[i, i :: self._loadcount] = sfuncs.transpose()
         return N
 
     def _get_b_vector(self, ipcoords):
         b = np.zeros((self._loadcount))
         for i in range(self._loadcount):
-            b[i] = pu.evaluate(self._loads[i], ipcoords, self._rank)
+            b[i] = pu.evaluate(
+                self._loads[i], ipcoords, self._rank, extra_dict=self._eval_dict
+            )
         return b
```

### Comparing `myjive-0.1.7/myjivex/models/neumannmodel.py` & `myjive-0.1.8/myjivex/models/neumannmodel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from myjive.names import GlobNames as gn
 from myjive.model.model import Model
-from myjive.util.proputils import mandatory_list, optional_argument
+from myjive.util.proputils import check_list
 
 __all__ = ["NeumannModel"]
 
 
 class NeumannModel(Model):
     def GETCONSTRAINTS(self, c, globdat, **kwargs):
         c = self._get_constraints(c, globdat, **kwargs)
@@ -23,21 +23,23 @@
     def GETUNITFORCE(self, f_unit, globdat, **kwargs):
         f_unit = self._get_unit_force(f_unit, globdat, **kwargs)
         return f_unit
 
     def ADVANCE(self, globdat):
         self._advance_step(globdat)
 
-    def configure(self, globdat, **props):
-
-        # Get props
-        self._groups = mandatory_list(self, props, "groups")
-        self._dofs = mandatory_list(self, props, "dofs")
-        self._vals = mandatory_list(self, props, "values")
-        loadIncr = optional_argument(self, props, "loadIncr")
+    @Model.save_config
+    def configure(self, globdat, *, groups, dofs, values, loadIncr=None):
+        # Validate input arguments
+        check_list(self, groups)
+        check_list(self, dofs)
+        check_list(self, values)
+        self._groups = groups
+        self._dofs = dofs
+        self._vals = values
 
         self._initLoad = self._vals
         if loadIncr is None:
             self._loadIncr = np.zeros(len(self._vals))
         else:
             self._loadIncr = loadIncr
```

### Comparing `myjive-0.1.7/myjivex/modules/vtkoutmodule.py` & `myjive-0.1.8/myjivex/modules/vtkoutmodule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import numpy as np
 
 from myjive.app import Module
 from myjive.names import GlobNames as gn
 from myjive.util import Table, to_xtable
-from myjive.util.proputils import optional_argument
+from myjive.util.proputils import check_list
 
 
 __all__ = ["VTKOutModule"]
 
 
 class VTKOutModule(Module):
-    def init(self, globdat, **props):
+    @Module.save_config
+    def configure(self, globdat, *, file="", tables=[]):
+        # Validate input arguments
+        check_list(self, tables)
+        self._fname = file
+        self._tnames = tables
 
-        # Get props
-        self._fname = optional_argument(self, props, "file", default="")
-        self._tnames = optional_argument(self, props, "tables", default=[])
+    def init(self, globdat):
+        pass
 
     def run(self, globdat):
         nodes = globdat[gn.NSET]
         elems = globdat[gn.ESET]
         disp = globdat[gn.STATE0]
         dofs = globdat[gn.DOFSPACE]
         types = dofs.get_types()
```

### Comparing `myjive-0.1.7/myjivex/util/plotutils.py` & `myjive-0.1.8/myjivex/util/plotutils.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/myjivex/util/quickviewer.py` & `myjive-0.1.8/myjivex/util/quickviewer.py`

 * *Files identical despite different names*

### Comparing `myjive-0.1.7/setup.py` & `myjive-0.1.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="myjive",
     packages=find_packages(include=["myjive*", "myjivex*"]),
-    version="0.1.7",
+    version="0.1.8",
     license="MIT",
     description="Personal implementation of jive C++ library in Python",
     author="Anne Poot",
     author_email="a.poot-1@tudelft.nl",
     url="https://gitlab.tudelft.nl/apoot1/myjive",
-    download_url="https://gitlab.tudelft.nl/apoot1/myjive/-/archive/v0.1.7/myjive-v0.1.7.tar.gz",
+    download_url="https://gitlab.tudelft.nl/apoot1/myjive/-/archive/v0.1.8/myjive-v0.1.8.tar.gz",
     keywords=[],
+    python_requires="==3.10.*",
     install_requires=[
         "matplotlib==3.5.2",
         "numba==0.56.4",
         "numpy==1.23.5",
         "scikit-sparse==0.4.12",
         "scipy==1.8.1",
     ],
```

