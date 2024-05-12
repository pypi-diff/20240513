# Comparing `tmp/mstool-0.2.0.tar.gz` & `tmp/mstool-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mstool-0.2.0.tar", last modified: Fri Mar 22 18:13:52 2024, max compression
+gzip compressed data, was "mstool-0.3.0.tar", last modified: Sun May 12 22:40:43 2024, max compression
```

## Comparing `mstool-0.2.0.tar` & `mstool-0.3.0.tar`

### file list

```diff
@@ -1,176 +1,194 @@
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.895998 mstool-0.2.0/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    35146 2024-01-11 02:42:52.000000 mstool-0.2.0/LICENSE
--rw-r--r--   0 siyoungkim   (501) staff       (20)    41419 2024-03-22 18:13:52.895691 mstool-0.2.0/PKG-INFO
--rw-r--r--   0 siyoungkim   (501) staff       (20)      462 2024-01-12 23:16:00.000000 mstool-0.2.0/README.md
--rw-r--r--   0 siyoungkim   (501) staff       (20)      567 2024-01-13 19:02:26.000000 mstool-0.2.0/pyproject.toml
--rw-r--r--   0 siyoungkim   (501) staff       (20)       38 2024-03-22 18:13:52.896049 mstool-0.2.0/setup.cfg
--rw-r--r--   0 siyoungkim   (501) staff       (20)     4060 2024-01-31 01:28:37.000000 mstool-0.2.0/setup.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.810979 mstool-0.2.0/src/
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.814672 mstool-0.2.0/src/mstool/
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.811326 mstool-0.2.0/src/mstool/FF/
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.824070 mstool-0.2.0/src/mstool/FF/amber14/
--rw-rw-r--   0 siyoungkim   (501) staff       (20)   105594 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/DNA.OL15.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)   102752 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/DNA.bsc1.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)    97695 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/RNA.OL3.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)      158 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/amber14-all.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)   534086 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/lipid17.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)   224056 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/protein.ff14SB.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)   298257 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/protein.ff15ipq.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)    18755 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/spce.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)    19070 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/tip3p.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)    19596 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/tip3pfb.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)    20076 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/tip4pew.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)    19897 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber14/tip4pfb.xml
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.826361 mstool-0.2.0/src/mstool/FF/amber99/
--rw-rw-r--   0 siyoungkim   (501) staff       (20)   473784 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber99/amber99sbildn.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)      891 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/amber99/tip3p.xml
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.839447 mstool-0.2.0/src/mstool/FF/charmm36/
--rw-r--r--   0 siyoungkim   (501) staff       (20)  5891645 2024-02-01 00:15:52.000000 mstool-0.2.0/src/mstool/FF/charmm36/charmm36.xml
--rw-r--r--   0 siyoungkim   (501) staff       (20)     7480 2023-05-09 01:58:47.000000 mstool-0.2.0/src/mstool/FF/charmm36/clol.xml
--rw-r--r--   0 siyoungkim   (501) staff       (20)    75582 2023-08-12 01:45:57.000000 mstool-0.2.0/src/mstool/FF/charmm36/pip.xml
--rw-rw-r--   0 siyoungkim   (501) staff       (20)     7889 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/charmm36/water.xml
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.846470 mstool-0.2.0/src/mstool/FF/martini2.2/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    22529 2024-03-16 05:09:18.000000 mstool-0.2.0/src/mstool/FF/martini2.2/martini_lipids_add.itp
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1456 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.0_ions.itp
--rw-r--r--   0 siyoungkim   (501) staff       (20)  1185038 2023-07-18 01:29:33.000000 mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.0_lipids_all_201506.itp
--rw-rw-r--   0 siyoungkim   (501) staff       (20)    50916 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.2.itp
--rw-r--r--   0 siyoungkim   (501) staff       (20)    45907 2023-07-18 01:29:33.000000 mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.2.modified.LJ.itp
--rw-r--r--   0 siyoungkim   (501) staff       (20)    52595 2023-07-18 01:29:33.000000 mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.2.modified.itp
--rw-r--r--   0 siyoungkim   (501) staff       (20)      583 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/martini2.2/ti.itp
--rw-r--r--   0 siyoungkim   (501) staff       (20)      424 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/martini2.2/toy.itp
--rw-r--r--   0 siyoungkim   (501) staff       (20)      612 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/FF/martini2.2/tp.itp
--rw-r--r--   0 siyoungkim   (501) staff       (20)     2599 2024-03-16 00:58:04.000000 mstool-0.2.0/src/mstool/__init__.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)       31 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/authors.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.851908 mstool-0.2.0/src/mstool/backup/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    12487 2023-08-18 18:26:49.000000 mstool-0.2.0/src/mstool/backup/backmap.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.852413 mstool-0.2.0/src/mstool/backup/cg2aa/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    35682 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/backup/cg2aa/cg2aa.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     5989 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/backup/fill.bck.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     2548 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/backup/fill_loops.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1942 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/backup/fill_side.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    12782 2023-07-14 14:04:07.000000 mstool-0.2.0/src/mstool/backup/gmx2dms2.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    11808 2023-07-23 21:29:31.000000 mstool-0.2.0/src/mstool/backup/loopmodeler_230719.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    18757 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/backup/martinizedms.231213.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    20475 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/backup/martinizedms.240309.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    18834 2023-07-23 21:29:31.000000 mstool-0.2.0/src/mstool/backup/openmmutils_230719.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)      195 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/backup/pandas2dict.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    29602 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/backup/rem.bck.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    24079 2023-07-23 21:29:31.000000 mstool-0.2.0/src/mstool/backup/rem_230719.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    12975 2023-08-01 11:40:37.000000 mstool-0.2.0/src/mstool/backup/rem_230801.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     2096 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/backup/rock_240306.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     7657 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/backup/sphere_240304.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    12487 2023-08-18 19:00:21.000000 mstool-0.2.0/src/mstool/backup/ungroup.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.860347 mstool-0.2.0/src/mstool/core/
--rw-r--r--   0 siyoungkim   (501) staff       (20)        2 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/core/__init__.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     7393 2024-03-16 03:29:15.000000 mstool-0.2.0/src/mstool/core/backmap.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    14165 2024-03-14 03:34:43.000000 mstool-0.2.0/src/mstool/core/checkstructure.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1600 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/core/checktetrahedron.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     8249 2023-07-14 15:13:37.000000 mstool-0.2.0/src/mstool/core/dms2openmm.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    76494 2024-03-17 03:17:56.000000 mstool-0.2.0/src/mstool/core/dmsfile.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     6632 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/core/fill.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    18510 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/core/gmx2dms.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    13134 2024-02-26 22:29:26.000000 mstool-0.2.0/src/mstool/core/loopmodeler.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     4874 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/core/map.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    20734 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/core/martinizedms.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     2294 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/core/mutate.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     4112 2024-01-13 17:50:18.000000 mstool-0.2.0/src/mstool/core/readmappings.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    18511 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/core/readmartini.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1683 2024-01-13 17:50:56.000000 mstool-0.2.0/src/mstool/core/readxml.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    19937 2024-03-16 00:47:19.000000 mstool-0.2.0/src/mstool/core/rem.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     3605 2023-07-23 21:29:31.000000 mstool-0.2.0/src/mstool/core/seq.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     7034 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/core/solvate_martini.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    14006 2024-01-21 01:05:31.000000 mstool-0.2.0/src/mstool/core/truncateprotein.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    18452 2024-03-16 04:26:12.000000 mstool-0.2.0/src/mstool/core/ungroup.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    30154 2024-03-15 01:05:41.000000 mstool-0.2.0/src/mstool/core/universe.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.812244 mstool-0.2.0/src/mstool/examples/
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.860955 mstool-0.2.0/src/mstool/examples/Backmapping/
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.861994 mstool-0.2.0/src/mstool/examples/Backmapping/Example1_methane/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    10012 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example1_methane/cg.pdb
--rw-r--r--   0 siyoungkim   (501) staff       (20)      520 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example1_methane/ff.xml
--rw-r--r--   0 siyoungkim   (501) staff       (20)       32 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example1_methane/mapping.dat
--rw-r--r--   0 siyoungkim   (501) staff       (20)       79 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example1_methane/run.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.862770 mstool-0.2.0/src/mstool/examples/Backmapping/Example2_ethane/
--rw-r--r--   0 siyoungkim   (501) staff       (20)     9946 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example2_ethane/cg.pdb
--rw-r--r--   0 siyoungkim   (501) staff       (20)       48 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example2_ethane/mapping.dat
--rw-r--r--   0 siyoungkim   (501) staff       (20)       62 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example2_ethane/run.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.863506 mstool-0.2.0/src/mstool/examples/Backmapping/Example3_butene/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    10012 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example3_butene/cg.pdb
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1200 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example3_butene/ff.xml
--rw-r--r--   0 siyoungkim   (501) staff       (20)       84 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example3_butene/mapping.dat
--rw-r--r--   0 siyoungkim   (501) staff       (20)       79 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example3_butene/run.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.864280 mstool-0.2.0/src/mstool/examples/Backmapping/Example4_POPC/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    93449 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example4_POPC/cg.pdb
--rw-r--r--   0 siyoungkim   (501) staff       (20)       39 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example4_POPC/run.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.864470 mstool-0.2.0/src/mstool/examples/Backmapping/Example5_Sphere/
--rw-r--r--   0 siyoungkim   (501) staff       (20)  1339911 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example5_Sphere/cg.pdb
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.869093 mstool-0.2.0/src/mstool/examples/Backmapping/Example6_TRIO/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    91474 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example6_TRIO/cg.pdb
--rw-r--r--   0 siyoungkim   (501) staff       (20)    16798 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example6_TRIO/ff.xml
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1087 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example6_TRIO/mapping.dat
--rw-r--r--   0 siyoungkim   (501) staff       (20)       83 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example6_TRIO/run.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)      217 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example6_TRIO/setup.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.875679 mstool-0.2.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/
--rw-r--r--   0 siyoungkim   (501) staff       (20)   735166 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/cg.pdb
--rw-r--r--   0 siyoungkim   (501) staff       (20)   677022 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/cg_nonprotein.pdb
--rw-r--r--   0 siyoungkim   (501) staff       (20)   400680 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/protein_AA.pdb
--rw-r--r--   0 siyoungkim   (501) staff       (20)       81 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/run.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     3005 2024-01-13 19:01:35.000000 mstool-0.2.0/src/mstool/examples/Backmapping/run_all.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.876304 mstool-0.2.0/src/mstool/examples/BilayerBuilder/
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.876633 mstool-0.2.0/src/mstool/examples/BilayerBuilder/Example5_GPCR/
--rw-r--r--   0 siyoungkim   (501) staff       (20)       96 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/examples/BilayerBuilder/Example5_GPCR/run.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.877262 mstool-0.2.0/src/mstool/examples/BilayerBuilder/Example6_Seipin/
--rw-r--r--   0 siyoungkim   (501) staff       (20)      403 2024-03-16 13:16:30.000000 mstool-0.2.0/src/mstool/examples/BilayerBuilder/Example6_Seipin/run.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)      140 2024-03-16 23:20:01.000000 mstool-0.2.0/src/mstool/examples/BilayerBuilder/Example6_Seipin/showhalf.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.877768 mstool-0.2.0/src/mstool/examples/BilayerBuilder/Example8_SARS/
--rw-r--r--   0 siyoungkim   (501) staff       (20)      486 2024-03-15 17:56:12.000000 mstool-0.2.0/src/mstool/examples/BilayerBuilder/Example8_SARS/run.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.878257 mstool-0.2.0/src/mstool/examples/BilayerBuilder/Example8_SARS_small/
--rw-r--r--   0 siyoungkim   (501) staff       (20)      387 2024-03-14 13:35:14.000000 mstool-0.2.0/src/mstool/examples/BilayerBuilder/Example8_SARS_small/run.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     2180 2024-03-17 03:13:03.000000 mstool-0.2.0/src/mstool/examples/BilayerBuilder/run_all.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)      183 2024-03-22 16:37:46.000000 mstool-0.2.0/src/mstool/examples/BilayerBuilder/showhalf.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.886471 mstool-0.2.0/src/mstool/lib/
--rw-r--r--   0 siyoungkim   (501) staff       (20)     7004 2024-01-31 01:22:15.000000 mstool-0.2.0/src/mstool/lib/align.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1898 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/lib/distance.memory.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     3590 2023-07-15 15:57:39.000000 mstool-0.2.0/src/mstool/lib/distance.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)   460001 2024-02-26 22:28:36.000000 mstool-0.2.0/src/mstool/lib/distancelib.c
--rw-r--r--   0 siyoungkim   (501) staff       (20)     6430 2024-01-31 01:22:15.000000 mstool-0.2.0/src/mstool/lib/distancelib.pyx
--rw-r--r--   0 siyoungkim   (501) staff       (20)  1517897 2024-02-26 22:28:40.000000 mstool-0.2.0/src/mstool/lib/qcprot.c
--rw-r--r--   0 siyoungkim   (501) staff       (20)    16595 2024-01-31 01:22:15.000000 mstool-0.2.0/src/mstool/lib/qcprot.pyx
--rw-r--r--   0 siyoungkim   (501) staff       (20)      205 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/lib/setup.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.887345 mstool-0.2.0/src/mstool/mapping/
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1740 2023-04-04 16:09:42.000000 mstool-0.2.0/src/mstool/mapping/martini.amber14.dat
--rw-r--r--   0 siyoungkim   (501) staff       (20)    18418 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/mapping/martini.lipid.c36.dat
--rw-r--r--   0 siyoungkim   (501) staff       (20)     3451 2023-08-18 18:31:58.000000 mstool-0.2.0/src/mstool/mapping/martini.protein.c36m.dat
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.887736 mstool-0.2.0/src/mstool/mapping/structures/
--rw-r--r--   0 siyoungkim   (501) staff       (20)      615 2024-01-31 01:24:25.000000 mstool-0.2.0/src/mstool/mapping/structures/CHL1.pdb
--rw-r--r--   0 siyoungkim   (501) staff       (20)     5917 2024-01-31 01:26:02.000000 mstool-0.2.0/src/mstool/mapping/structures/CHL1_AA.pdb
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.889609 mstool-0.2.0/src/mstool/membrane/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    12539 2024-03-15 18:27:44.000000 mstool-0.2.0/src/mstool/membrane/bilayer.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    15739 2024-03-21 21:57:11.000000 mstool-0.2.0/src/mstool/membrane/bilayerbuilder.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     4687 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/membrane/lipid.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     8393 2024-03-14 07:00:28.000000 mstool-0.2.0/src/mstool/membrane/sphere.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    14794 2024-03-21 21:57:11.000000 mstool-0.2.0/src/mstool/membrane/spherebuilder.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     4606 2024-03-14 00:59:01.000000 mstool-0.2.0/src/mstool/membrane/sphereprotein.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.894827 mstool-0.2.0/src/mstool/utils/
--rw-r--r--   0 siyoungkim   (501) staff       (20)        2 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/utils/__init__.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     3613 2024-01-10 03:40:42.000000 mstool-0.2.0/src/mstool/utils/add_termini_atoms.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)      966 2023-08-05 14:23:21.000000 mstool-0.2.0/src/mstool/utils/amberselection.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     9657 2024-01-31 01:22:15.000000 mstool-0.2.0/src/mstool/utils/cap_termini_residues.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     3709 2023-08-05 14:23:21.000000 mstool-0.2.0/src/mstool/utils/change_his.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)      619 2023-07-13 02:25:11.000000 mstool-0.2.0/src/mstool/utils/dump.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     5873 2024-03-01 22:50:31.000000 mstool-0.2.0/src/mstool/utils/gmx_energy.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)    40816 2024-03-16 13:48:36.000000 mstool-0.2.0/src/mstool/utils/openmmutils.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1345 2023-11-29 02:21:05.000000 mstool-0.2.0/src/mstool/utils/performance.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)      476 2023-07-23 21:29:31.000000 mstool-0.2.0/src/mstool/utils/protein_sel.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     2275 2024-03-14 00:59:01.000000 mstool-0.2.0/src/mstool/utils/rock.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     1609 2024-03-14 00:59:01.000000 mstool-0.2.0/src/mstool/utils/rockchain.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     2166 2024-03-14 06:53:26.000000 mstool-0.2.0/src/mstool/utils/rockresidue.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)      268 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/utils/saveargs.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     9158 2023-07-16 03:21:25.000000 mstool-0.2.0/src/mstool/utils/sqlcmd.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)     4241 2023-08-18 19:15:41.000000 mstool-0.2.0/src/mstool/utils/util.py
--rw-r--r--   0 siyoungkim   (501) staff       (20)       23 2024-03-11 01:25:34.000000 mstool-0.2.0/src/mstool/version.py
-drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-03-22 18:13:52.895279 mstool-0.2.0/src/mstool.egg-info/
--rw-r--r--   0 siyoungkim   (501) staff       (20)    41419 2024-03-22 18:13:52.000000 mstool-0.2.0/src/mstool.egg-info/PKG-INFO
--rw-r--r--   0 siyoungkim   (501) staff       (20)     5363 2024-03-22 18:13:52.000000 mstool-0.2.0/src/mstool.egg-info/SOURCES.txt
--rw-r--r--   0 siyoungkim   (501) staff       (20)        1 2024-03-22 18:13:52.000000 mstool-0.2.0/src/mstool.egg-info/dependency_links.txt
--rw-r--r--   0 siyoungkim   (501) staff       (20)       18 2024-03-22 18:13:52.000000 mstool-0.2.0/src/mstool.egg-info/requires.txt
--rw-r--r--   0 siyoungkim   (501) staff       (20)        7 2024-03-22 18:13:52.000000 mstool-0.2.0/src/mstool.egg-info/top_level.txt
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.072369 mstool-0.3.0/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    35146 2024-01-11 02:42:52.000000 mstool-0.3.0/LICENSE
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    41440 2024-05-12 22:40:43.072115 mstool-0.3.0/PKG-INFO
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      462 2024-01-12 23:16:00.000000 mstool-0.3.0/README.md
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      580 2024-05-07 02:42:09.000000 mstool-0.3.0/pyproject.toml
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       38 2024-05-12 22:40:43.072409 mstool-0.3.0/setup.cfg
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     4060 2024-01-31 01:28:37.000000 mstool-0.3.0/setup.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:42.901275 mstool-0.3.0/src/
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:42.907847 mstool-0.3.0/src/mstool/
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:42.901961 mstool-0.3.0/src/mstool/FF/
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:42.925253 mstool-0.3.0/src/mstool/FF/amber14/
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)   105594 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/DNA.OL15.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)   102752 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/DNA.bsc1.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)    97695 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/RNA.OL3.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)      158 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/amber14-all.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)   534086 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/lipid17.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)   224056 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/protein.ff14SB.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)   298257 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/protein.ff15ipq.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)    18755 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/spce.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)    19070 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/tip3p.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)    19596 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/tip3pfb.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)    20076 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/tip4pew.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)    19897 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber14/tip4pfb.xml
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:42.927496 mstool-0.3.0/src/mstool/FF/amber99/
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)   473784 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber99/amber99sbildn.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)      891 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/amber99/tip3p.xml
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:42.950764 mstool-0.3.0/src/mstool/FF/charmm36/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)  5891720 2024-05-01 02:39:53.000000 mstool-0.3.0/src/mstool/FF/charmm36/charmm36.xml
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    12485 2024-04-30 13:16:52.000000 mstool-0.3.0/src/mstool/FF/charmm36/chyo.xml
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     7480 2023-05-09 01:58:47.000000 mstool-0.3.0/src/mstool/FF/charmm36/clol.xml
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    75582 2023-08-12 01:45:57.000000 mstool-0.3.0/src/mstool/FF/charmm36/pip.xml
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)     7889 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/charmm36/water.xml
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:42.960374 mstool-0.3.0/src/mstool/FF/martini2.2/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    24164 2024-05-01 10:01:47.000000 mstool-0.3.0/src/mstool/FF/martini2.2/martini_lipids_add.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1456 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.0_ions.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)  1185038 2023-07-18 01:29:33.000000 mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.0_lipids_all_201506.itp
+-rw-rw-r--   0 siyoungkim   (501) staff       (20)    50916 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.2.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    45907 2023-07-18 01:29:33.000000 mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.2.modified.LJ.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    52595 2023-07-18 01:29:33.000000 mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.2.modified.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      583 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/martini2.2/ti.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      424 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/martini2.2/toy.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      612 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/FF/martini2.2/tp.itp
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:42.993385 mstool-0.3.0/src/mstool/FF/martini3.0.0/
+-rw-r--r--   0 siyoungkim   (501) staff       (20) 16031459 2024-05-03 21:23:37.000000 mstool-0.3.0/src/mstool/FF/martini3.0.0/martini.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)   207793 2024-05-03 21:29:55.000000 mstool-0.3.0/src/mstool/FF/martini3.0.0/phospholipids.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     9372 2024-05-03 21:11:45.000000 mstool-0.3.0/src/mstool/FF/martini3.0.0/protein.itp
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     2685 2024-05-11 04:19:53.000000 mstool-0.3.0/src/mstool/__init__.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       31 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/authors.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.006350 mstool-0.3.0/src/mstool/backup/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      966 2023-08-05 14:23:21.000000 mstool-0.3.0/src/mstool/backup/amberselection_20240510.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    12487 2023-08-18 18:26:49.000000 mstool-0.3.0/src/mstool/backup/backmap.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    12539 2024-04-30 01:03:23.000000 mstool-0.3.0/src/mstool/backup/bilayer_240429.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    15739 2024-04-30 01:02:31.000000 mstool-0.3.0/src/mstool/backup/bilayerbuilder_240429.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.007002 mstool-0.3.0/src/mstool/backup/cg2aa/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    35682 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/backup/cg2aa/cg2aa.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     5989 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/backup/fill.bck.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     2548 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/backup/fill_loops.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1942 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/backup/fill_side.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    12782 2023-07-14 14:04:07.000000 mstool-0.3.0/src/mstool/backup/gmx2dms2.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    11808 2023-07-23 21:29:31.000000 mstool-0.3.0/src/mstool/backup/loopmodeler_230719.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    18757 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/backup/martinizedms.231213.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    20475 2024-03-11 01:25:34.000000 mstool-0.3.0/src/mstool/backup/martinizedms.240309.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    18834 2023-07-23 21:29:31.000000 mstool-0.3.0/src/mstool/backup/openmmutils_230719.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      195 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/backup/pandas2dict.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    29602 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/backup/rem.bck.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    24079 2023-07-23 21:29:31.000000 mstool-0.3.0/src/mstool/backup/rem_230719.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    12975 2023-08-01 11:40:37.000000 mstool-0.3.0/src/mstool/backup/rem_230801.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     2096 2024-03-11 01:25:34.000000 mstool-0.3.0/src/mstool/backup/rock_240306.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     7657 2024-03-11 01:25:34.000000 mstool-0.3.0/src/mstool/backup/sphere_240304.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    12487 2023-08-18 19:00:21.000000 mstool-0.3.0/src/mstool/backup/ungroup.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    18457 2024-05-01 02:18:53.000000 mstool-0.3.0/src/mstool/backup/ungroup_240430.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    30438 2024-05-10 20:24:34.000000 mstool-0.3.0/src/mstool/backup/universe_20240510.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    33104 2024-05-11 02:26:00.000000 mstool-0.3.0/src/mstool/backup/universe_20240511.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.018220 mstool-0.3.0/src/mstool/core/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)        2 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/core/__init__.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     7667 2024-05-11 19:03:22.000000 mstool-0.3.0/src/mstool/core/backmap.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    14165 2024-03-14 03:34:43.000000 mstool-0.3.0/src/mstool/core/checkstructure.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1600 2024-03-11 01:25:34.000000 mstool-0.3.0/src/mstool/core/checktetrahedron.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     8249 2023-07-14 15:13:37.000000 mstool-0.3.0/src/mstool/core/dms2openmm.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    76494 2024-03-17 03:17:56.000000 mstool-0.3.0/src/mstool/core/dmsfile.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     6605 2024-05-11 03:47:37.000000 mstool-0.3.0/src/mstool/core/fill.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    18510 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/core/gmx2dms.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    13572 2024-04-13 21:26:08.000000 mstool-0.3.0/src/mstool/core/loopmodeler.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     4847 2024-05-11 03:47:50.000000 mstool-0.3.0/src/mstool/core/map.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    21048 2024-05-11 03:50:10.000000 mstool-0.3.0/src/mstool/core/martinizedms.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     2267 2024-05-11 03:47:58.000000 mstool-0.3.0/src/mstool/core/mutate.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     3853 2024-05-11 15:31:50.000000 mstool-0.3.0/src/mstool/core/orient.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     4112 2024-01-13 17:50:18.000000 mstool-0.3.0/src/mstool/core/readmappings.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    18511 2024-03-11 01:25:34.000000 mstool-0.3.0/src/mstool/core/readmartini.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1725 2024-04-30 13:05:41.000000 mstool-0.3.0/src/mstool/core/readxml.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    20061 2024-05-11 04:43:27.000000 mstool-0.3.0/src/mstool/core/rem.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     3605 2023-07-23 21:29:31.000000 mstool-0.3.0/src/mstool/core/seq.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     7395 2024-05-11 03:48:28.000000 mstool-0.3.0/src/mstool/core/solvate_martini.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    14006 2024-01-21 01:05:31.000000 mstool-0.3.0/src/mstool/core/truncateprotein.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    18711 2024-05-11 19:04:25.000000 mstool-0.3.0/src/mstool/core/ungroup.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    29643 2024-05-12 22:18:29.000000 mstool-0.3.0/src/mstool/core/universe.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:42.903645 mstool-0.3.0/src/mstool/examples/
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.019729 mstool-0.3.0/src/mstool/examples/Backmapping/
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.021402 mstool-0.3.0/src/mstool/examples/Backmapping/Example1_methane/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    10012 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example1_methane/cg.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      520 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example1_methane/ff.xml
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       32 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example1_methane/mapping.dat
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       79 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example1_methane/run.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.023560 mstool-0.3.0/src/mstool/examples/Backmapping/Example2_ethane/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     9946 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example2_ethane/cg.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       48 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example2_ethane/mapping.dat
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       62 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example2_ethane/run.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.025482 mstool-0.3.0/src/mstool/examples/Backmapping/Example3_butene/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    10012 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example3_butene/cg.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1200 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example3_butene/ff.xml
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       84 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example3_butene/mapping.dat
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       79 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example3_butene/run.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.026240 mstool-0.3.0/src/mstool/examples/Backmapping/Example4_POPC/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    93449 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example4_POPC/cg.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       39 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example4_POPC/run.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.026464 mstool-0.3.0/src/mstool/examples/Backmapping/Example5_Sphere/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)  1339911 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example5_Sphere/cg.pdb
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.031623 mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)   136583 2024-05-12 22:36:07.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/cg.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    16798 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/ff.xml
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1087 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/mapping.5.dat
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1033 2024-05-01 01:11:31.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/mapping.dat
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       83 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/run.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      217 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/setup.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.042562 mstool-0.3.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)   735166 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/cg.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)   677022 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/cg_nonprotein.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)   400680 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/protein_AA.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       81 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/run.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     3005 2024-01-13 19:01:35.000000 mstool-0.3.0/src/mstool/examples/Backmapping/run_all.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.043464 mstool-0.3.0/src/mstool/examples/BilayerBuilder/
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.045267 mstool-0.3.0/src/mstool/examples/BilayerBuilder/gpcr/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       96 2024-03-11 01:25:34.000000 mstool-0.3.0/src/mstool/examples/BilayerBuilder/gpcr/run.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     4023 2024-05-11 04:04:01.000000 mstool-0.3.0/src/mstool/examples/BilayerBuilder/run_all.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1884 2024-05-03 22:24:54.000000 mstool-0.3.0/src/mstool/examples/BilayerBuilder/run_martini3.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.045688 mstool-0.3.0/src/mstool/examples/BilayerBuilder/sars/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      486 2024-03-15 17:56:12.000000 mstool-0.3.0/src/mstool/examples/BilayerBuilder/sars/run.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.046092 mstool-0.3.0/src/mstool/examples/BilayerBuilder/sars_small/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      387 2024-03-14 13:35:14.000000 mstool-0.3.0/src/mstool/examples/BilayerBuilder/sars_small/run.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      183 2024-03-22 16:37:46.000000 mstool-0.3.0/src/mstool/examples/BilayerBuilder/showhalf.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.060043 mstool-0.3.0/src/mstool/lib/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     7004 2024-01-31 01:22:15.000000 mstool-0.3.0/src/mstool/lib/align.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1898 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/lib/distance.memory.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     3590 2023-07-15 15:57:39.000000 mstool-0.3.0/src/mstool/lib/distance.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)   460537 2024-04-30 01:41:27.000000 mstool-0.3.0/src/mstool/lib/distancelib.c
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     6430 2024-01-31 01:22:15.000000 mstool-0.3.0/src/mstool/lib/distancelib.pyx
+-rw-r--r--   0 siyoungkim   (501) staff       (20)  1518407 2024-04-30 01:41:33.000000 mstool-0.3.0/src/mstool/lib/qcprot.c
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    16595 2024-01-31 01:22:15.000000 mstool-0.3.0/src/mstool/lib/qcprot.pyx
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      205 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/lib/setup.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.062164 mstool-0.3.0/src/mstool/mapping/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1740 2023-04-04 16:09:42.000000 mstool-0.3.0/src/mstool/mapping/martini.amber14.dat
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    19336 2024-05-01 02:31:18.000000 mstool-0.3.0/src/mstool/mapping/martini.lipid.c36.dat
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     3451 2023-08-18 18:31:58.000000 mstool-0.3.0/src/mstool/mapping/martini.protein.c36m.dat
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     3335 2024-05-03 21:13:57.000000 mstool-0.3.0/src/mstool/mapping/martini3.protein.c36m.dat
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.063815 mstool-0.3.0/src/mstool/mapping/structures/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      615 2024-01-31 01:24:25.000000 mstool-0.3.0/src/mstool/mapping/structures/CHL1.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     5917 2024-01-31 01:26:02.000000 mstool-0.3.0/src/mstool/mapping/structures/CHL1_AA.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      648 2024-05-01 02:36:02.000000 mstool-0.3.0/src/mstool/mapping/structures/CHYO.bck.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      640 2024-05-03 13:03:00.000000 mstool-0.3.0/src/mstool/mapping/structures/CHYO.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     5832 2024-05-01 02:36:28.000000 mstool-0.3.0/src/mstool/mapping/structures/CHYO_AA.bck.pdb
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     5200 2024-05-03 13:05:38.000000 mstool-0.3.0/src/mstool/mapping/structures/CHYO_AA.pdb
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.065779 mstool-0.3.0/src/mstool/membrane/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    14086 2024-05-07 02:32:17.000000 mstool-0.3.0/src/mstool/membrane/bilayer.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    19955 2024-05-12 22:31:07.000000 mstool-0.3.0/src/mstool/membrane/bilayerbuilder.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     4687 2024-03-11 01:25:34.000000 mstool-0.3.0/src/mstool/membrane/lipid.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     8381 2024-05-03 01:35:35.000000 mstool-0.3.0/src/mstool/membrane/sphere.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    15345 2024-05-12 22:32:22.000000 mstool-0.3.0/src/mstool/membrane/spherebuilder.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     4580 2024-05-03 14:02:20.000000 mstool-0.3.0/src/mstool/membrane/sphereprotein.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.071313 mstool-0.3.0/src/mstool/utils/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)        2 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/utils/__init__.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     3613 2024-01-10 03:40:42.000000 mstool-0.3.0/src/mstool/utils/add_termini_atoms.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     3169 2024-05-11 18:41:02.000000 mstool-0.3.0/src/mstool/utils/amberselection.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      615 2024-05-11 16:36:42.000000 mstool-0.3.0/src/mstool/utils/atomic_data.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     9657 2024-01-31 01:22:15.000000 mstool-0.3.0/src/mstool/utils/cap_termini_residues.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     3709 2023-08-05 14:23:21.000000 mstool-0.3.0/src/mstool/utils/change_his.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      619 2023-07-13 02:25:11.000000 mstool-0.3.0/src/mstool/utils/dump.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     5873 2024-03-01 22:50:31.000000 mstool-0.3.0/src/mstool/utils/gmx_energy.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     6855 2024-05-11 16:39:08.000000 mstool-0.3.0/src/mstool/utils/mdautils.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    40816 2024-03-16 13:48:36.000000 mstool-0.3.0/src/mstool/utils/openmmutils.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1345 2023-11-29 02:21:05.000000 mstool-0.3.0/src/mstool/utils/performance.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      476 2023-07-23 21:29:31.000000 mstool-0.3.0/src/mstool/utils/protein_sel.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     2249 2024-05-11 03:52:22.000000 mstool-0.3.0/src/mstool/utils/rock.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     1583 2024-05-11 03:52:35.000000 mstool-0.3.0/src/mstool/utils/rockchain.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     2190 2024-05-11 04:19:33.000000 mstool-0.3.0/src/mstool/utils/rockresidue.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)      268 2024-03-11 01:25:34.000000 mstool-0.3.0/src/mstool/utils/saveargs.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     9158 2023-07-16 03:21:25.000000 mstool-0.3.0/src/mstool/utils/sqlcmd.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     4241 2023-08-18 19:15:41.000000 mstool-0.3.0/src/mstool/utils/util.py
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       23 2024-05-12 22:38:31.000000 mstool-0.3.0/src/mstool/version.py
+drwxr-xr-x   0 siyoungkim   (501) staff       (20)        0 2024-05-12 22:40:43.071739 mstool-0.3.0/src/mstool.egg-info/
+-rw-r--r--   0 siyoungkim   (501) staff       (20)    41440 2024-05-12 22:40:42.000000 mstool-0.3.0/src/mstool.egg-info/PKG-INFO
+-rw-r--r--   0 siyoungkim   (501) staff       (20)     6021 2024-05-12 22:40:42.000000 mstool-0.3.0/src/mstool.egg-info/SOURCES.txt
+-rw-r--r--   0 siyoungkim   (501) staff       (20)        1 2024-05-12 22:40:42.000000 mstool-0.3.0/src/mstool.egg-info/dependency_links.txt
+-rw-r--r--   0 siyoungkim   (501) staff       (20)       24 2024-05-12 22:40:42.000000 mstool-0.3.0/src/mstool.egg-info/requires.txt
+-rw-r--r--   0 siyoungkim   (501) staff       (20)        7 2024-05-12 22:40:42.000000 mstool-0.3.0/src/mstool.egg-info/top_level.txt
```

### Comparing `mstool-0.2.0/LICENSE` & `mstool-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/PKG-INFO` & `mstool-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mstool
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multiscale Simulation Tool for Backmapping
 Author-email: Siyoung Kim <siyoung.k@icloud.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,11 +680,12 @@
 Project-URL: Repository, https://github.com/ksy141/mstool.git
 Project-URL: documentation, https://mstool.readthedocs.io/en/latest/#
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: matplotlib
+Requires-Dist: scipy
 
 # mstool
 
 [mstool](https://mstool.readthedocs.io/en/latest/#) is a multiscale simulation tool that converts a coarse-grained structure into an all-atom structure. It requires minimal user input (mapping and isomeric information of molecules) and is more powerful than the previous backmapping tools. For more details, please check out the [paper](https://pubs.acs.org/doi/10.1021/acs.jpcb.3c05593) and [documentation](https://mstool.readthedocs.io/en/latest/#).
```

### Comparing `mstool-0.2.0/pyproject.toml` & `mstool-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 description = "Multiscale Simulation Tool for Backmapping"
 readme      = "README.md"
 license     = { file = "LICENSE" }
 requires-python = ">= 3.7"
 dynamic     = ['version']
 dependencies = [
     "pandas",
-    "matplotlib"
+    "matplotlib",
+    "scipy"
 ]
 
 [project.urls]
 Repository    = "https://github.com/ksy141/mstool.git"
 documentation = "https://mstool.readthedocs.io/en/latest/#"
```

### Comparing `mstool-0.2.0/setup.py` & `mstool-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/DNA.OL15.xml` & `mstool-0.3.0/src/mstool/FF/amber14/DNA.OL15.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/DNA.bsc1.xml` & `mstool-0.3.0/src/mstool/FF/amber14/DNA.bsc1.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/RNA.OL3.xml` & `mstool-0.3.0/src/mstool/FF/amber14/RNA.OL3.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/lipid17.xml` & `mstool-0.3.0/src/mstool/FF/amber14/lipid17.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/protein.ff14SB.xml` & `mstool-0.3.0/src/mstool/FF/amber14/protein.ff14SB.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/protein.ff15ipq.xml` & `mstool-0.3.0/src/mstool/FF/amber14/protein.ff15ipq.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/spce.xml` & `mstool-0.3.0/src/mstool/FF/amber14/spce.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/tip3p.xml` & `mstool-0.3.0/src/mstool/FF/amber14/tip3p.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/tip3pfb.xml` & `mstool-0.3.0/src/mstool/FF/amber14/tip3pfb.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/tip4pew.xml` & `mstool-0.3.0/src/mstool/FF/amber14/tip4pew.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber14/tip4pfb.xml` & `mstool-0.3.0/src/mstool/FF/amber14/tip4pfb.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber99/amber99sbildn.xml` & `mstool-0.3.0/src/mstool/FF/amber99/amber99sbildn.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/amber99/tip3p.xml` & `mstool-0.3.0/src/mstool/FF/amber99/tip3p.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/charmm36/charmm36.xml` & `mstool-0.3.0/src/mstool/FF/charmm36/charmm36.xml`

 * *Files 0% similar despite different names*

#### Comparing `mstool-0.2.0/src/mstool/FF/charmm36/charmm36.xml` & `mstool-0.3.0/src/mstool/FF/charmm36/charmm36.xml`

```diff
@@ -91217,14 +91217,15 @@
     <Bond k="258571.19999999995" length="0.1111" type1="CTL1" type2="HAL1"/>
     <Bond k="276143.99999999994" length="0.10800000000000001" type1="CTL1" type2="HBL"/>
     <Bond k="258571.19999999995" length="0.1111" type1="CTL2" type2="HAL2"/>
     <Bond k="269449.6" length="0.1111" type1="CTL3" type2="HAL3"/>
     <Bond k="284511.99999999994" length="0.143" type1="CTL3" type2="OSL"/>
     <Bond k="284511.99999999994" length="0.143" type1="CTL2" type2="OSL"/>
     <Bond k="284511.99999999994" length="0.143" type1="CTL1" type2="OSL"/>
+    <Bond k="284511.99999999994" length="0.143" type1="CRL1" type2="OSL"/>
     <Bond k="284511.99999999994" length="0.143" type1="CTL3" type2="OSLP"/>
     <Bond k="284511.99999999994" length="0.143" type1="CTL2" type2="OSLP"/>
     <Bond k="284511.99999999994" length="0.143" type1="CTL1" type2="OSLP"/>
     <Bond k="225935.99999999997" length="0.16000000000000003" type1="OSL" type2="PL"/>
     <Bond k="225935.99999999997" length="0.16000000000000003" type1="OSLP" type2="PL"/>
     <Bond k="485343.9999999999" length="0.148" type1="O2L" type2="PL"/>
     <Bond k="198321.59999999998" length="0.15900000000000003" type1="OHL" type2="PL"/>
```

### Comparing `mstool-0.2.0/src/mstool/FF/charmm36/clol.xml` & `mstool-0.3.0/src/mstool/FF/charmm36/clol.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/charmm36/pip.xml` & `mstool-0.3.0/src/mstool/FF/charmm36/pip.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/charmm36/water.xml` & `mstool-0.3.0/src/mstool/FF/charmm36/water.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/martini2.2/martini_lipids_add.itp` & `mstool-0.3.0/src/mstool/FF/martini2.2/martini_lipids_add.itp`

 * *Files 2% similar despite different names*

```diff
@@ -265,18 +265,74 @@
   5 7 	1 	0.406   5000
   6 7 	1 	0.368 	5000
   7 8 	1 	0.425 	1250
                                                                                 
 [angles]
 ; i j k 	funct 	angle 	force.c.
   4 7 8 	2 	180.0   25.0
+ 
+
+
+; This is a fake CHYO model
+[moleculetype] 
+; molname 	nrexcl
+  CHYO 		1
+                                                                                
+[atoms]
+; id 	type 	resnr 	residu 	atom 	cgnr 	charge
+  1 	SC1 	1 	CHYO 	R0   	1 	0
+  2 	SC1 	1 	CHYO 	R1 	    2 	0
+  3 	SC3 	1 	CHYO 	R2 	    3 	0
+  4 	SC1 	1 	CHYO 	R3 	    4 	0
+  5 	SC1 	1 	CHYO 	R4 	    5 	0
+  6 	SC1 	1 	CHYO 	R5 	    6 	0
+  7 	SC1 	1 	CHYO 	C1 	    7 	0
+  8 	C1 	    1 	CHYO 	C2 	    8 	0
+  9     Na      1   CHYO    ES      9   0
+ 10     C1      1   CHYO    C3     10   0
+ 11     C3      1   CHYO    C4     11   0
+ 12     C1      1   CHYO    C5     12   0
+ 13     C1      1   CHYO    C6     13   0
+
+[bonds]
+; i j 	funct 	length 	force.c.
+  1 2 	1 	0.242 	5000
+  1 3 	1 	0.493   5000
+  1 4 	1 	0.604   5000
+  1 5   1   0.815   5000 ; new
+  1 6   1   0.790   5000 ; new
+  2 3 	1 	0.260 	5000
+  2 4 	1 	0.341 	5000
+  2 5   1   0.570   5000 ; new
+  2 6   1   0.540   5000 ; new
+  3 4 	1 	0.272   5000
+  3 5 	1 	0.346   5000
+  3 6   1   0.380   5000 ; new
+  4 5 	1 	0.294   5000
+  4 6 	1 	0.213 	5000
+  4 7 	1 	0.544 	5000 
+  5 6 	1 	0.203 	5000
+  5 7 	1 	0.406   5000
+  6 7 	1 	0.368 	5000
+  7 8 	1 	0.425 	1250
+   1     9    1       0.470    1250
+   9    10    1       0.470    1250
+  10    11    1       0.470    1250
+  11    12    1       0.470    1250
+  12    13    1       0.470    1250
                                                                                 
-;[exclusions]
-;   2 5 6
-;
+[angles]
+; i j k 	funct 	angle 	force.c.
+   4     7    8 	  2  180.000     25.0
+   1     9   10       2  180.000     25.0
+   9    10   11       2  180.000     25.0
+  10    11   12       2  120.000     45.0
+  11    12   13       2  180.000     25.0 
+   2     1    9       2  180.000     60.0
+
 [moleculetype]
 ; molname      nrexcl
   DMPC          1
 
 [atoms]
 ; id 	type 	resnr 	residu 	atom 	cgnr 	charge
    1 	Q0 	 1 	DMPC 	NC3 	 1 	1.0
```

### Comparing `mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.0_ions.itp` & `mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.0_ions.itp`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.0_lipids_all_201506.itp` & `mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.0_lipids_all_201506.itp`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.2.itp` & `mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.2.itp`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.2.modified.LJ.itp` & `mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.2.modified.LJ.itp`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/martini2.2/martini_v2.2.modified.itp` & `mstool-0.3.0/src/mstool/FF/martini2.2/martini_v2.2.modified.itp`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/martini2.2/ti.itp` & `mstool-0.3.0/src/mstool/FF/martini2.2/ti.itp`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/FF/martini2.2/tp.itp` & `mstool-0.3.0/src/mstool/FF/martini2.2/tp.itp`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/__init__.py` & `mstool-0.3.0/src/mstool/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,20 +19,22 @@
 from .core.seq              import Seq
 from .core.dmsfile          import DMSFile
 from .core.backmap          import Backmap
 from .utils.protein_sel     import three2one, one2three
 from .utils.dump            import dumpsql, dumpdf
 from .utils.gmx_energy      import getGMXEnergy
 from .utils.openmmutils     import *
-from .utils.amberselection  import amberSelection
+from .utils.amberselection  import *
 from .utils.add_termini_atoms import addTerminiAtoms
 from .utils.cap_termini_residues import capTerminiResidues
 from .utils.change_his import changeHIS
 from .utils.performance import Performance
 from .utils.saveargs import saveargs
+from .utils.rockresidue import RockResidue
+from .core.orient import *
 
 from .lib.align import rotation_matrix, _fit_to
 from .membrane.bilayerbuilder import BilayerBuilder
 from .membrane.spherebuilder  import SphereBuilder
 from .membrane.sphereprotein  import SphereProtein
 
 
@@ -45,11 +47,12 @@
 TRIOSTRUCTURE      = pwd + '/examples/Backmapping/Example6_TRIO/cg.pdb'
 TRIOMAPPING        = pwd + '/examples/Backmapping/Example6_TRIO/mapping.dat'
 TRIOFF             = pwd + '/examples/Backmapping/Example6_TRIO/ff.xml'
 TRIOMARTINI        = pwd + '/examples/Backmapping/Example6_TRIO/martini.itp'
 MPCG               = pwd + '/examples/Backmapping/Example7_MembraneProtein/cg.pdb'
 MPAA               = pwd + '/examples/Backmapping/Example7_MembraneProtein/protein_AA.pdb'
 MPAA2              = pwd + '/examples/Backmapping/Example7_MembraneProtein/protein_AA2.pdb'
-GPCR               = pwd + '/examples/BilayerBuilder/Example5_GPCR/gpcr.pdb'
-SEIPIN             = pwd + '/examples/BilayerBuilder/Example6_Seipin/oligomer.pdb'
+GPCR               = pwd + '/examples/BilayerBuilder/3sn6.pdb'
+GPCR2              = pwd + '/examples/BilayerBuilder/4xnv.pdb'
+SEIPIN             = pwd + '/examples/BilayerBuilder/6ds5.pdb'
```

### Comparing `mstool-0.2.0/src/mstool/backup/backmap.py` & `mstool-0.3.0/src/mstool/backup/backmap.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/cg2aa/cg2aa.py` & `mstool-0.3.0/src/mstool/backup/cg2aa/cg2aa.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/fill.bck.py` & `mstool-0.3.0/src/mstool/backup/fill.bck.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/fill_loops.py` & `mstool-0.3.0/src/mstool/backup/fill_loops.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/fill_side.py` & `mstool-0.3.0/src/mstool/backup/fill_side.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/gmx2dms2.py` & `mstool-0.3.0/src/mstool/backup/gmx2dms2.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/loopmodeler_230719.py` & `mstool-0.3.0/src/mstool/backup/loopmodeler_230719.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/martinizedms.231213.py` & `mstool-0.3.0/src/mstool/backup/martinizedms.231213.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/martinizedms.240309.py` & `mstool-0.3.0/src/mstool/backup/martinizedms.240309.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/openmmutils_230719.py` & `mstool-0.3.0/src/mstool/backup/openmmutils_230719.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/rem.bck.py` & `mstool-0.3.0/src/mstool/backup/rem.bck.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/rem_230719.py` & `mstool-0.3.0/src/mstool/backup/rem_230719.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/rem_230801.py` & `mstool-0.3.0/src/mstool/backup/rem_230801.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/rock_240306.py` & `mstool-0.3.0/src/mstool/backup/rock_240306.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/sphere_240304.py` & `mstool-0.3.0/src/mstool/backup/sphere_240304.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/backup/ungroup.py` & `mstool-0.3.0/src/mstool/backup/ungroup.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/backmap.py` & `mstool-0.3.0/src/mstool/core/backmap.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,22 +17,31 @@
                  ff      = [], ff_add = [],
                  Kchiral=300, Kpeptide=300, Kcistrans=300, Kdihedral=300,
                  fcx=1000.0, fcy=1000.0, fcz=1000.0,
                  rock=None, rockCtype='CTL3', rockHtype='HAL3',
                  rcut=1.2, pbc=True, A=100, C=50,
                  add_bonds = True, remversion='v4',
                  water_resname='W', water_chain=None, water_number=4, water_fibor=2.0, water_chain_dms=True, 
-                 use_AA_structure=False, AA_structure=[], AA_structure_add=[], AA_shrink_factor=1.0,
+                 use_AA_structure=False, AA_structure=[], AA_structure_add=[], AA_shrink_factor=0.8,
                  use_existing_workdir=False, fileindex=1, pdbsave=True, cospower=2,
-                 nsteps=10000, T=310):
+                 nsteps=10000, T=310, sanitizeMartini=True,
+                 changename={':CHOL':':CHL1',':ION@NA':':SOD@SOD',':NA@NA':':SOD@SOD',
+                             ':ION@CL':':CLA@CLA',':CL@CL':':CLA@CLA',':ION@CA':':CAL@CAL'}):
 
         ### workdir
         if not use_existing_workdir: os.mkdir(workdir)
         if use_existing_workdir and not os.path.exists(workdir): os.mkdir(workdir)
 
+        ### save args
+        args = locals()
+        with open(workdir + '/args.txt', 'w') as W:
+            for key, value in args.items():
+                if key == 'self': continue
+                W.write(f'{key:30} = {value}\n')
+
         ### Read Mapping and XML and compare these two
         if not isinstance(ff_add, list): ff_add = [ff_add]
         if not isinstance(mapping_add, list): mapping_add = [mapping_add]
         map = ReadMappings(mapping=mapping, mapping_add=mapping_add)
         xml = ReadXML(ff=ff, ff_add=ff_add)
         self.checkMappingXML(map, xml)
 
@@ -50,27 +59,32 @@
             except:
                 rock = AA
                 protein = None
                 print('Some of the residues in the AA argument is not recognizable in openMM')
                 print(f'Using rock="{AA}"')
 
         ### Ungroup
+        if sanitizeMartini:
+            structure = Universe(structure)
+            structure.changeName(changename)
+
         Ungroup(structure, out=workdir + f'/step{fileindex}_ungroup.dms', 
                 mapping=mapping, mapping_add=mapping_add, backbone=backbone,
                 water_resname=water_resname,
                 water_chain=water_chain, water_number=water_number,
                 water_fibor=water_fibor, water_chain_dms=water_chain_dms,
                 sort=True, use_AA_structure=use_AA_structure,
-                AA_structure=AA_structure, AA_structure_add=AA_structure_add)
+                AA_structure=AA_structure, AA_structure_add=AA_structure_add, AA_shrink_factor=0.8)
         
         REM(structure   = workdir + f'/step{fileindex}_ungroup.dms', 
             outrem      = workdir + f'/step{fileindex+1}_rem.dms',
             out         = workdir + f'/step{fileindex+2}_em.dms',
             rockout     = workdir + f'/step{fileindex+2}_rock.dms',
             nonrockout  = workdir + f'/step{fileindex+2}_nonrock.dms',
+            rockprefix  = workdir + '/ROCK',
             protein     = protein,
             rock        = rock,
             rockCtype   = rockCtype,
             rockHtype   = rockHtype,
             mapping     = mapping, 
             mapping_add = mapping_add,
             ff          = ff, 
@@ -93,37 +107,32 @@
 
         ### Combine
         if rock:
             if os.path.exists('ROCK.dms'): os.rename('ROCK.dms', workdir + '/ROCK.dms')
             if os.path.exists('ROCK.xml'): os.rename('ROCK.xml', workdir + '/ROCK.xml')
 
             u1 = Universe(AA)
+            if len(u1.bonds) == 0: u1.addBondFromDistance()
+
             shutil.copyfile(workdir + f'/step{fileindex+2}_nonrock.dms', 
                             workdir + f'/step{fileindex+3}_nonprotein.dms')
 
-            #u2 = Universe(workdir + f'/step{fileindex+2}_nonrock.dms',
-            #              ff=ff, ff_add=ff_add, create_bonds=True)
             u2 = Universe(workdir + f'/step{fileindex+2}_nonrock.dms')
             u = Merge(u1.atoms, u2.atoms)
-            u.bonds = len(u1.atoms) + np.array(u2.bonds)
+            u.bonds = list(u1.bonds) + list(len(u1.atoms) + np.array(u2.bonds))
             u.dimensions = u2.dimensions
             u.cell       = u2.cell
             u.write(workdir + f'/step{fileindex+3}_final.dms')
             u.write(workdir + f'/step{fileindex+3}_final.pdb')
             
             u1.dimensions = u2.dimensions
             u1.cell       = u2.cell
             u1.write(workdir + f'/step{fileindex+3}_protein.pdb')
 
         else:
-            #u = Universe(workdir + f'/step{fileindex+2}_em.dms', 
-            #              ff=ff, ff_add=ff_add,
-            #              create_bonds=True)
-            #u = Universe(workdir + f'/step{fileindex+2}_em.dms')
-            #u.write(workdir + f'/step{fileindex+3}_final.dms')
             shutil.copyfile(workdir + f'/step{fileindex+2}_em.dms',
                             workdir + f'/step{fileindex+3}_final.dms')
             Universe(workdir + f'/step{fileindex+3}_final.dms').write(
                      workdir + f'/step{fileindex+3}_final.pdb')
         
         ### PDB
         if pdbsave:
```

### Comparing `mstool-0.2.0/src/mstool/core/checkstructure.py` & `mstool-0.3.0/src/mstool/core/checkstructure.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/checktetrahedron.py` & `mstool-0.3.0/src/mstool/core/checktetrahedron.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/dms2openmm.py` & `mstool-0.3.0/src/mstool/core/dms2openmm.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/dmsfile.py` & `mstool-0.3.0/src/mstool/core/dmsfile.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/fill.py` & `mstool-0.3.0/src/mstool/core/fill.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         super().__init__(data=self.u.atoms)
         self.sort()
         self.cell       = self.u.cell
         self.dimensions = self.u.dimensions
 
         ### save
-        if out: self.write(out, guess_atomic_number=False)
+        if out: self.write(out)
 
 
     def ExtendTermini(self):
         for chainnum in range(self.nchains):
             if chainnum not in self.extend_termini.keys(): continue
             sU = self.seqfromU.seq[chainnum]['one']
             sF = self.seqfromF.seq[chainnum]['one']
```

### Comparing `mstool-0.2.0/src/mstool/core/gmx2dms.py` & `mstool-0.3.0/src/mstool/core/gmx2dms.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/loopmodeler.py` & `mstool-0.3.0/src/mstool/core/loopmodeler.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from   .fill                  import Fill
 from   .readmappings          import ReadMappings
 from   .universe              import Universe
 from   .map                   import Map
 from   .readmartini           import ReadMartini
 from   .martinizedms          import MartinizeDMS
 from   .dms2openmm            import DMS2openmm
+from   .dmsfile               import DMSFile
 from   .rem                   import REM
 from   .checkstructure        import CheckStructure
 from   .ungroup               import Ungroup
 from   .solvate_martini       import SolvateMartini
 
 from   ..utils.protein_sel    import three2one
 from   ..utils.dump           import dumpsql
@@ -102,34 +103,39 @@
 
         ### step5: create a martini FF dms
         self.makemartini(workdir + '/step4_solvated.pdb',
                          workdir + '/step5_ff.dms')
 
 
         ### step6: run Martini simulation
-        runMartiniEM(dms_in = workdir + '/step5_ff.dms',
-                     out    = workdir + '/step6_minimized.pdb',
-                     soft   = soft,
-                     nonbondedMethod = nonbondedMethod,
-                     nonbondedCutoff = 1.1)
+        dms = DMSFile(workdir + '/step5_ff.dms')
+        dms.createSystem(REM=True, tapering='shift', martini=True, nonbondedMethod=nonbondedMethod)
+        dms.runEMNPT(dt=dt, nsteps=nsteps, dcdfreq=dcdfreq, csvfreq=csvfreq, semiisotropic=False, out=workdir + '/step6_minimized.dms')
+        Universe(workdir + '/step6_minimized.dms').write(workdir + '/step6_minimized.pdb')
+
+        #runMartiniEM(dms_in = workdir + '/step5_ff.dms',
+        #             out    = workdir + '/step6_minimized.pdb',
+        #             soft   = soft,
+        #             nonbondedMethod = nonbondedMethod,
+        #             nonbondedCutoff = 1.1)
 
         if t == 0 or t is None or nsteps == 0:
             shutil.copy(workdir + '/step6_minimized.pdb',
                         workdir + '/step6_NPT.pdb')
-        else:
-            runMartiniEMNPT(dms_in = workdir + '/step5_ff.dms',
-                            pos_in = workdir + '/step6_minimized.pdb',
-                            out    = workdir + '/step6_NPT.pdb',
-                            soft   = False,
-                            nonbondedMethod = nonbondedMethod,
-                            nonbondedCutoff = 1.1,
-                            dt      = dt,
-                            nsteps  = nsteps,
-                            dcdfreq = dcdfreq,
-                            csvfreq = csvfreq)
+        #else:
+        #    runMartiniEMNPT(dms_in = workdir + '/step5_ff.dms',
+        #                    pos_in = workdir + '/step6_minimized.pdb',
+        #                    out    = workdir + '/step6_NPT.pdb',
+        #                    soft   = False,
+        #                    nonbondedMethod = nonbondedMethod,
+        #                    nonbondedCutoff = 1.1,
+        #                    dt      = dt,
+        #                    nsteps  = nsteps,
+        #                    dcdfreq = dcdfreq,
+        #                    csvfreq = csvfreq)
 
 
         ### step7: ungroup (output must be a pdb so that openMM recognizes protein residues)
         Ungroup(structure   = workdir + '/step6_NPT.pdb',
                 out         = workdir + '/step7_backmapped.pdb',
                 mapping     = mapping,
                 mapping_add = mapping_add,
```

### Comparing `mstool-0.2.0/src/mstool/core/map.py` & `mstool-0.3.0/src/mstool/core/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.sort()
 
         # translate
         self.atoms[['x','y','z']] += translate
 
         # save
         if out is not None:
-            self.write(out, guess_atomic_number=False)
+            self.write(out)
 
 
     def add_availableCGAtoms(self, add_notavailableAAAtoms):
         dfresids   = []; dfresnames = [];
         dfchains   = []; dfnames    = [];
         dfx = []; dfy = []; dfz = [];
```

### Comparing `mstool-0.2.0/src/mstool/core/martinizedms.py` & `mstool-0.3.0/src/mstool/core/martinizedms.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             universe.n2t[i]      = nbtype
 
         for index, atom in universe.atoms.iterrows():
             t = atom['type']
             universe.atoms.loc[index, 'nbtype'] = universe.t2n[t]
             universe.atoms.loc[index, 'type']   = t
 
-        universe.write(out, guess_atomic_number=False)
+        universe.write(out)
 
 
     def updateBonds(self):
         for resname in self.resnames:
             bonds = self.martini.martini['molecules'][resname]['bonds']
             for bond in bonds:
                 atom1 = bond[0]
@@ -384,20 +384,28 @@
                     raise AssertionError('{:s} {:s} not exists'.format(ttype1, ttype2))
                 
                 if C6 == 0.0 and C12 == 0.0:
                     sigma   = 0.0
                     epsilon = 0.0
 
                 else:
-                    sigma6  = C12 / C6
-                    sigma   = sigma6 ** (1/6)
-                    epsilon = C6 / 4 / sigma6
+                    if self.martini.martini['energy'].startswith('C12'):
+                        sigma6  = C12 / C6
+                        sigma   = sigma6 ** (1/6)
+                        epsilon = C6 / 4 / sigma6
+
+                    elif self.martini.martini['energy'].startswith('4*eps'):
+                        sigma   = C6
+                        epsilon = C12
+
+                    else:
+                        raise AssertionError('LJ function is not defined')
 
                     sigma   = sigma   * 10      # nm to A
-                    epsilon = epsilon * 0.239  # kJ/mol to kcal/mol
+                    epsilon = epsilon * 0.239   # kJ/mol to kcal/mol
 
                 self.cursor.execute(sql_insert_nonbonded_combined.format(
                     ntype1, ntype2, epsilon, sigma, ttype1 + ' ' + ttype2))
 
 
     def updatePosre(self):
         ### Find the preexisting posre_index
```

### Comparing `mstool-0.2.0/src/mstool/core/mutate.py` & `mstool-0.3.0/src/mstool/core/mutate.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         super().__init__(data = df)
         self.sort()
         self.cell       = self.universe.cell
         self.dimensions = self.universe.dimensions
 
         ### save
         if out is not None:
-            self.write(out, guess_atomic_number=False)
+            self.write(out)
 
     def fixmutation(self):
         '''
         fix mutation (at atomistic level)
         more like save backbone + CB atoms
         '''
```

### Comparing `mstool-0.2.0/src/mstool/core/readmappings.py` & `mstool-0.3.0/src/mstool/core/readmappings.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/readmartini.py` & `mstool-0.3.0/src/mstool/core/readmartini.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/readxml.py` & `mstool-0.3.0/src/mstool/core/readxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import numpy as np
 import xml.etree.ElementTree as ET
 
 pwd  = os.path.dirname(os.path.realpath(__file__))
 aaff = [pwd + '/../FF/charmm36/charmm36.xml',
         pwd + '/../FF/charmm36/pip.xml',
-        pwd + '/../FF/charmm36/water.xml']
+        pwd + '/../FF/charmm36/water.xml',
+        pwd + '/../FF/charmm36/chyo.xml']
 
 class ReadXML:
     def __init__(self, ff=[], ff_add=[]):
 
         if not isinstance(ff, list):
             ff = [ ff ]
```

### Comparing `mstool-0.2.0/src/mstool/core/rem.py` & `mstool-0.3.0/src/mstool/core/rem.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # modeller = Modeller(pdb1.topology, pdb1.positions)
     # modeller.add(pdb2.topology, pdb2.positions)
     # mergedTopology = modeller.topology
     # mergedPositions = modeller.positions
 
     def __init__(self, structure=None, out=None, protein=None, refposre=None, outrem=None,
         rock=None, rockout='ROCK_rem.pdb', nonrockout='NONROCK.dms',
-        rockCtype='CTL3', rockHtype='HAL3',
+        rockCtype='CTL3', rockHtype='HAL3', rockprefix='ROCK',
         rcut=1.2, pbc=True, 
         A=100, C=50,
         mapping = [], mapping_add = [], 
         ff      = [], ff_add = [],
         Kchiral=300, Kpeptide=300, Kcistrans=300, Kdihedral=300,
         fcx = 1000.0, fcy = 1000.0, fcz = 1000.0,
         bfactor_posre = 0.5, add_bonds=True, sort=False, version='v4',
@@ -87,20 +87,20 @@
             #rr         = RockChain(structure=rock, 
             #                       out='ROCK', 
             #                       resname=rockresname,
             #                       rockCtype=rockCtype,
             #                       rockHtype=rockHtype)
 
             rr         = RockResidue(structure=rock, 
-                                     out='ROCK', 
+                                     out=rockprefix, 
                                      rockCtype=rockCtype,
                                      rockHtype=rockHtype)
 
             rrdms      = DesmondDMSFile(rr.dms)
-            ff_add    += ['ROCK.xml']
+            ff_add    += [rockprefix + '.xml']
 
 
         ### Read XML
         mapping    = ReadMappings(mapping=mapping, mapping_add=mapping_add)
         xml        = ReadXML(ff=ff, ff_add=ff_add)
         forcefield = ForceField(*xml.ff)
         self.forcefield = forcefield
@@ -286,25 +286,28 @@
             #nonrockstruct.bonds      = getBonds(nonrockstruct, xml)
             nonrockstruct.write(nonrockout)
 
             new = Universe(data = pd.concat([Universe(rock).atoms, nonrockstruct.atoms], ignore_index=True))
             new.dimensions = u.dimensions
             new.cell       = u.cell
             if out: new.write(out)
-            ff_add.remove('ROCK.xml')
+            ff_add.remove(rockprefix + '.xml')
 
         else:
             #if sort: u.sort()
             #if out.split('.')[-1] == 'dms':
                 #u.update_anum_mass()
                 #u.bonds = addBonds(u, xml)
                 #u.bonds = self.bonds
 
             if out:
-                u.write(out, wrap=True)
+                if pbc:
+                    u.write(out, wrap=True)
+                else:
+                    u.write(out)
         
         #CheckTetrahedron(out, ff=ff, ff_add=ff_add)
         self.universe = u
         self.u        = u
         self.forces   = { force.__class__.__name__ : force for force in self.system.getForces() }
         #print(self.forces.keys())
```

### Comparing `mstool-0.2.0/src/mstool/core/seq.py` & `mstool-0.3.0/src/mstool/core/seq.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/solvate_martini.py` & `mstool-0.3.0/src/mstool/core/solvate_martini.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,49 +47,52 @@
 
     wateru = Universe(data=data)
     wateru.dimensions = u.dimensions
     wateru.cell = u.cell
         
     # waterbox
     if len(u.atoms) == 0:
-        if out: wateru.write(out, guess_atomic_number=False)
+        if out: wateru.write(out)
         return wateru
     
     pos1 = wateru.atoms[['x','y', 'z']].to_numpy(dtype=np.float64)
     pos2 = u.atoms[['x','y', 'z']].to_numpy(dtype=np.float64)
     dim  = np.asarray(u.dimensions, dtype=np.float64)
 
     if pbc:
         bA = distance_overlap(pos1, pos2, removedr, u.dimensions)
     else:
         bA = distance_overlap(pos1, pos2, removedr)
 
     u.atoms = pd.concat([u.atoms, wateru.atoms[bA]], ignore_index=True)
 
-    if out: u.write(out, guess_atomic_number=False)
+    if out: u.write(out)
     return u
 
 
 def ionize(u, out=None, qtot=None,
-           conc = 0.15, pos='SOD', neg='CLA', waterresname='W', ionchain=''):
+           conc = 0.15, pos='SOD', neg='CLA', waterresname='W', ionchain='',
+           posionchain=None, negionchain=None):
     """Add ions at a given concentration.
     conc = ( N_positive_ion / 6.02e23 ) / ( V * 1e-27 ) = (N * 1e4) / (V * 6.02)
     """
     
     # if system is not parameterized, all q = 0;
     if all(u.atoms.type == 'tbd') and not all(u.atoms.resname == waterresname) and not qtot:
-        print("\nYou need to parameterize a system first before adding ions")
+        #print("\nYou need to parameterize a system first before adding ions")
         print("Adding ions while assuming the input structure has a net charge of 0")
     
     if qtot:
         qtot = qtot
     else:
         qtot = round(u.atoms.charge.sum())
-
-    vol  = u.dimensions[0] * u.dimensions[1] * u.dimensions[2]
+    
+    # instead of using vol, use the number of water * water volume per each bead
+    # vol  = u.dimensions[0] * u.dimensions[1] * u.dimensions[2]
+    vol = len(u.atoms[u.atoms.name == 'W']) * 4.93 ** 3
 
     if pos in ['MG', 'CAL', 'BAR', 'ZN2', 'CD2']:
         factor = 2
     else:
         factor = 1
     
     # number of positive ions and negative ions
@@ -109,15 +112,18 @@
     wateratoms    = u.atoms[bA].sample(frac=1, ignore_index=True) # a new object
 
     # Positive ions
     # Note that contrary to usual python slices, both the start and the stop are included
     wateratoms.loc[0:Npos-1, 'charge']  = factor
     wateratoms.loc[0:Npos-1, 'name']    = pos
     wateratoms.loc[0:Npos-1, 'resname'] = pos
-    wateratoms.loc[0:Npos-1, 'chain']   = ionchain + '1'
+    if posionchain:
+        wateratoms.loc[0:Npos-1, 'chain']   = posionchain
+    else:
+        wateratoms.loc[0:Npos-1, 'chain']   = ionchain + '1'
     
     pos_preexisting = u.atoms[u.atoms['name'] == pos]
     if len(pos_preexisting) == 0:
         resid = 0
     else:
         resid = pos_preexisting.resid.max()
 
@@ -125,15 +131,18 @@
     wateratoms.loc[0:Npos-1, 'resid'] = resids
 
 
     # Negative ions
     wateratoms.loc[Npos:Npos+Nneg-1, 'charge']  = -1
     wateratoms.loc[Npos:Npos+Nneg-1, 'name']    = neg
     wateratoms.loc[Npos:Npos+Nneg-1, 'resname'] = neg
-    wateratoms.loc[Npos:Npos+Nneg-1, 'chain']   = ionchain + '2'
+    if negionchain:
+        wateratoms.loc[Npos:Npos+Nneg-1, 'chain']   = negionchain
+    else:
+        wateratoms.loc[Npos:Npos+Nneg-1, 'chain']   = ionchain + '2'
 
     neg_preexisting = u.atoms[u.atoms['name'] == neg]
     if len(neg_preexisting) == 0:
         resid = 0
     else:
         resid  = neg_preexisting.resid.max()
 
@@ -154,24 +163,24 @@
     #assert 0 == round(u.atoms.charge.sum()), 'net charge is not zero'
     num_final  = len(u.atoms[u.atoms['name'] == pos])
     conc_final = (num_final * 1e4) / (vol * 6.02)
     print(f"{pos}: {Npos}")
     print(f"{neg}: {Nneg}")
     print(f"{pos}.{neg}: {conc_final:.3f} M\n")
     
-    if out: u.write(out, guess_atomic_number=False)
+    if out: u.write(out)
     return u
 
 
 
 def SolvateMartini(structure=None, out=None, t=None,
                    dimensions=None,
                    solventdr=4.93, removedr=6.0, waterslab=0.8, waterchain='W', center=True,
                    conc=0.15, qtot=None, pos='SOD', neg='CLA', waterresname='W', ionchain='ZZ', pbc=True,
-                   membrane=False):
+                   membrane=False, posionchain=None, negionchain=None):
         
     # make a water box
     if dimensions:
         if isinstance(dimensions, int) or isinstance(dimensions, float):
             dimensions = [dimensions] * 3
 
         u = Universe()
@@ -198,15 +207,15 @@
             dim  = maxd + 2 * t
             u.dimensions = np.array([dim] * 3 + [90] * 3)
             u.cell = np.array([[dim, 0, 0], [0, dim, 0], [0, 0, dim]])
 
     solvatedu = solvate(u, solventdr=solventdr, removedr=removedr, waterslab=waterslab,
                         waterchain=waterchain, center=center, pbc=pbc, membrane=membrane)
     if conc == 0.0:
-        if out: solvatedu.write(out, guess_atomic_number=False)
+        if out: solvatedu.write(out)
         return solvatedu
 
 
     ionizedu  = ionize(solvatedu, out=out, qtot=qtot, conc=conc, pos=pos, neg=neg, 
-                       waterresname=waterresname, ionchain=ionchain)
+                       waterresname=waterresname, ionchain=ionchain, posionchain=posionchain, negionchain=negionchain)
     return ionizedu
```

### Comparing `mstool-0.2.0/src/mstool/core/truncateprotein.py` & `mstool-0.3.0/src/mstool/core/truncateprotein.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/core/ungroup.py` & `mstool-0.3.0/src/mstool/backup/ungroup_240430.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 n_atoms  = len(aaatoms)
 
                 self.list2data(name    = aaatoms['name'].values,
                                chain   = [chain]   * n_atoms,
                                resname = [resname] * n_atoms,
                                resid   = [resid]   * n_atoms,
                                pos     = pos)
-
+     
 
     def construct_backbone(self):
         '''
         Construct a backbone according to the following CG2AA paper.
         CG2AA: backmapping protein coarse-grained structures
         Leandro E. Lombardi, Marcelo A. Marti, and Luciana Capece
         https://www.ic.fcen.uba.ar/cg2aa/cg2aa.py
```

### Comparing `mstool-0.2.0/src/mstool/core/universe.py` & `mstool-0.3.0/src/mstool/backup/universe_20240510.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 
 # bfactor
 # if dms file doesn't have bfactor, make a column with a default value of 0.0
 # if dms file has bfactor, read values from there
 # if pdb file is provided, reset bfactor value to 0.0
 
 
+def custom_sort(value):
+    if isinstance(value, int):
+        return(0, value)
+    elif value.isdigit():
+        return (2, value)
+    else:
+        return (1, value)
+
 anum_mass_from_name = {
    'H':  [1,   1.00],
    'C':  [6,  12.00],
    'N':  [7,  14.00],
    'O':  [8,  16.00],
    'F':  [9,  19.00],
    'NA': [11, 23.00],
@@ -474,15 +482,16 @@
         #for bond in self.bonds:
         #    i1 = bond[0]
         #    i2 = bond[1]
         #    bonds_tmp.append([self.atoms.loc[i1].newindex, 
         #                      self.atoms.loc[i2].newindex])
         #self.bonds = bonds_tmp
 
-        self.atoms = self.atoms.sort_values(by=by, ignore_index=ignore_index)
+        #self.atoms = self.atoms.sort_values(by=by, ignore_index=ignore_index)
+        self.atoms = self.atoms.sort_values(by=by, ignore_index=ignore_index, key=lambda x: x.apply(custom_sort))
         self.bonds = []
 
 
     def guess_anum_mass(self, name):
         anum = 0
         mass = 0.0
```

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example1_methane/cg.pdb` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example1_methane/cg.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example1_methane/ff.xml` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example1_methane/ff.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example2_ethane/cg.pdb` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example2_ethane/cg.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example3_butene/cg.pdb` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example3_butene/cg.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example3_butene/ff.xml` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example3_butene/ff.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example4_POPC/cg.pdb` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example4_POPC/cg.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example5_Sphere/cg.pdb` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example5_Sphere/cg.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example6_TRIO/cg.pdb` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/cg.pdb`

 * *Files 22% similar despite different names*

```diff
@@ -1,1158 +1,1729 @@
-CRYST1   37.844   37.844   92.507  90.00  90.00  90.00 P 1           1
-ATOM      1  NC3 POPCU   1       1.757  -7.123  20.464  0.00  0.00            
-ATOM      2  PO4 POPCU   1      -1.184  -3.377  18.304  0.00  0.00            
-ATOM      3  GL1 POPCU   1       0.152   0.187  14.806  0.00  1.00            
-ATOM      4  GL2 POPCU   1       2.741  -0.013  14.876  0.00  1.00            
-ATOM      5  C1A POPCU   1      -2.015   2.492  12.929  0.00  0.00            
-ATOM      6  D2A POPCU   1      -1.935   0.788   8.797  0.00  0.00            
-ATOM      7  C3A POPCU   1      -5.229  -1.631   7.356  0.00  0.00            
-ATOM      8  C4A POPCU   1      -8.215  -4.323  10.149  0.00  0.00            
-ATOM      9  C1B POPCU   1       3.029  -1.644  10.502  0.00  0.00            
-ATOM     10  C2B POPCU   1       3.558  -0.623   6.009  0.00  0.00            
-ATOM     11  C3B POPCU   1       4.371   2.078   3.279  0.00  0.00            
-ATOM     12  C4B POPCU   1       5.770   2.522  -1.328  0.00  0.00            
-ATOM     13  NC3 POPCU   2      -7.187   1.498  19.711  0.00  0.00            
-ATOM     14  PO4 POPCU   2      -9.628  -1.808  18.263  0.00  0.00            
-ATOM     15  GL1 POPCU   2      -8.369   0.114  14.802  0.00  1.00            
-ATOM     16  GL2 POPCU   2      -5.434  -0.227  14.897  0.00  1.00            
-ATOM     17  C1A POPCU   2      -9.371   0.161  10.699  0.00  0.00            
-ATOM     18  D2A POPCU   2     -10.054  -0.287   6.358  0.00  0.00            
-ATOM     19  C3A POPCU   2      -7.218   1.556   2.364  0.00  0.00            
-ATOM     20  C4A POPCU   2      -6.233  -0.556  -1.944  0.00  0.00            
-ATOM     21  C1B POPCU   2      -2.889  -3.591  12.471  0.00  0.00            
-ATOM     22  C2B POPCU   2      -0.525  -4.193   8.293  0.00  0.00            
-ATOM     23  C3B POPCU   2      -2.351  -5.722   4.522  0.00  0.00            
-ATOM     24  C4B POPCU   2      -4.234  -7.933   1.273  0.00  0.00            
-ATOM     25  NC3 POPCU   3      -5.685 -11.538  19.539  0.00  0.00            
-ATOM     26  PO4 POPCU   3      -2.719  -8.194  18.940  0.00  0.00            
-ATOM     27  GL1 POPCU   3      -0.165  -7.631  15.112  0.00  1.00            
-ATOM     28  GL2 POPCU   3       2.553  -7.755  15.103  0.00  1.00            
-ATOM     29  C1A POPCU   3      -0.140 -10.638  11.705  0.00  0.00            
-ATOM     30  D2A POPCU   3       2.022 -10.987   9.219  0.00  0.00            
-ATOM     31  C3A POPCU   3       0.355  -9.716   5.857  0.00  0.00            
-ATOM     32  C4A POPCU   3       0.901  -8.775   1.346  0.00  0.00            
-ATOM     33  C1B POPCU   3       4.695  -6.455  11.571  0.00  0.00            
-ATOM     34  C2B POPCU   3       4.381  -5.375   6.733  0.00  0.00            
-ATOM     35  C3B POPCU   3       2.210  -4.407   2.918  0.00  0.00            
-ATOM     36  C4B POPCU   3       2.266  -1.198  -0.019  0.00  0.00            
-ATOM     37  NC3 POPCU   4       8.625   3.714  18.260  0.00  0.00            
-ATOM     38  PO4 POPCU   4       6.560  -0.208  20.661  0.00  0.00            
-ATOM     39  GL1 POPCU   4       7.929   0.076  14.710  0.00  1.00            
-ATOM     40  GL2 POPCU   4      11.055   0.231  15.267  0.00  1.00            
-ATOM     41  C1A POPCU   4       8.977  -3.114  12.478  0.00  0.00            
-ATOM     42  D2A POPCU   4       9.071  -5.196   8.641  0.00  0.00            
-ATOM     43  C3A POPCU   4       9.315  -4.423   4.659  0.00  0.00            
-ATOM     44  C4A POPCU   4       6.769  -2.403   1.869  0.00  0.00            
-ATOM     45  C1B POPCU   4      12.806  -0.569  11.082  0.00  0.00            
-ATOM     46  C2B POPCU   4      13.512  -2.588   7.242  0.00  0.00            
-ATOM     47  C3B POPCU   4      13.808  -2.215   2.940  0.00  0.00            
-ATOM     48  C4B POPCU   4      15.718  -3.887   0.002  0.00  0.00            
-ATOM     49  NC3 POPCU   5       1.938  11.805  18.529  0.00  0.00            
-ATOM     50  PO4 POPCU   5      -1.694   9.818  18.077  0.00  0.00            
-ATOM     51  GL1 POPCU   5      -0.350   7.960  14.683  0.00  1.00            
-ATOM     52  GL2 POPCU   5       2.930   7.923  14.995  0.00  1.00            
-ATOM     53  C1A POPCU   5      -0.597   6.829  11.075  0.00  0.00            
-ATOM     54  D2A POPCU   5      -2.078   5.149   7.459  0.00  0.00            
-ATOM     55  C3A POPCU   5      -0.221   3.469   5.056  0.00  0.00            
-ATOM     56  C4A POPCU   5      -1.497  -0.072   2.873  0.00  0.00            
-ATOM     57  C1B POPCU   5       3.960   4.540  13.149  0.00  0.00            
-ATOM     58  C2B POPCU   5       3.239   3.715   9.446  0.00  0.00            
-ATOM     59  C3B POPCU   5       2.809   6.797   6.574  0.00  0.00            
-ATOM     60  C4B POPCU   5       1.765   8.536   4.182  0.00  0.00            
-ATOM     61  NC3 POPCU   6      -5.722  -4.567  18.711  0.00  0.00            
-ATOM     62  PO4 POPCU   6      -9.444  -7.082  19.184  0.00  0.00            
-ATOM     63  GL1 POPCU   6      -8.023  -7.567  15.180  0.00  1.00            
-ATOM     64  GL2 POPCU   6      -5.543  -8.270  14.976  0.00  1.00            
-ATOM     65  C1A POPCU   6      -8.903 -10.956  11.704  0.00  0.00            
-ATOM     66  D2A POPCU   6      -9.735 -13.256   9.681  0.00  0.00            
-ATOM     67  C3A POPCU   6     -10.295 -12.864   5.366  0.00  0.00            
-ATOM     68  C4A POPCU   6      -7.830 -11.322   2.645  0.00  0.00            
-ATOM     69  C1B POPCU   6      -4.408  -8.268  10.677  0.00  0.00            
-ATOM     70  C2B POPCU   6      -4.541 -10.372   6.343  0.00  0.00            
-ATOM     71  C3B POPCU   6      -2.424 -12.122   2.208  0.00  0.00            
-ATOM     72  C4B POPCU   6       0.153 -15.979   2.017  0.00  0.00            
-ATOM     73  NC3 POPCU   7      -6.326  10.025  19.244  0.00  0.00            
-ATOM     74  PO4 POPCU   7      -9.468   6.353  19.040  0.00  0.00            
-ATOM     75  GL1 POPCU   7      -8.033   8.036  14.948  0.00  1.00            
-ATOM     76  GL2 POPCU   7      -5.386   7.756  14.696  0.00  1.00            
-ATOM     77  C1A POPCU   7      -6.446   8.864  10.664  0.00  0.00            
-ATOM     78  D2A POPCU   7      -3.369   9.895   7.771  0.00  0.00            
-ATOM     79  C3A POPCU   7      -2.404  14.204   6.607  0.00  0.00            
-ATOM     80  C4A POPCU   7      -1.386  17.287   4.157  0.00  0.00            
-ATOM     81  C1B POPCU   7      -6.475   3.894  11.619  0.00  0.00            
-ATOM     82  C2B POPCU   7      -6.599   3.086   6.900  0.00  0.00            
-ATOM     83  C3B POPCU   7     -10.967   4.597   4.462  0.00  0.00            
-ATOM     84  C4B POPCU   7     -13.979   7.177   1.610  0.00  0.00            
-ATOM     85  NC3 POPCU   8       4.468  -3.421  17.474  0.00  0.00            
-ATOM     86  PO4 POPCU   8       6.408  -8.441  19.074  0.00  0.00            
-ATOM     87  GL1 POPCU   8       8.156  -7.976  15.023  0.00  1.00            
-ATOM     88  GL2 POPCU   8      10.679  -8.311  14.824  0.00  1.00            
-ATOM     89  C1A POPCU   8       8.911 -10.500  10.404  0.00  0.00            
-ATOM     90  D2A POPCU   8       7.491 -10.844   6.294  0.00  0.00            
-ATOM     91  C3A POPCU   8       6.200  -8.894   3.385  0.00  0.00            
-ATOM     92  C4A POPCU   8       6.913  -7.903  -1.621  0.00  0.00            
-ATOM     93  C1B POPCU   8      12.414  -7.134  11.306  0.00  0.00            
-ATOM     94  C2B POPCU   8      12.341  -8.949   6.753  0.00  0.00            
-ATOM     95  C3B POPCU   8      10.749  -9.595   2.294  0.00  0.00            
-ATOM     96  C4B POPCU   8       9.375 -13.081   1.494  0.00  0.00            
-ATOM     97  NC3 POPCU   9       5.985   5.741  22.191  0.00  0.00            
-ATOM     98  PO4 POPCU   9       5.717   8.545  18.607  0.00  0.00            
-ATOM     99  GL1 POPCU   9       7.895   7.400  15.112  0.00  1.00            
-ATOM    100  GL2 POPCU   9      10.791   7.861  14.728  0.00  1.00            
-ATOM    101  C1A POPCU   9       8.662   3.463  11.738  0.00  0.00            
-ATOM    102  D2A POPCU   9       7.684   0.574   8.634  0.00  0.00            
-ATOM    103  C3A POPCU   9       9.753   0.469   4.909  0.00  0.00            
-ATOM    104  C4A POPCU   9       9.583   3.314   1.439  0.00  0.00            
-ATOM    105  C1B POPCU   9      10.653   7.888   9.858  0.00  0.00            
-ATOM    106  C2B POPCU   9      11.164   8.999   5.619  0.00  0.00            
-ATOM    107  C3B POPCU   9      11.533   9.099   0.577  0.00  0.00            
-ATOM    108  C4B POPCU   9      12.656   5.514  -1.743  0.00  0.00            
-ATOM    109  NC3 POPCU  10     -18.181  -4.477  17.342  0.00  0.00            
-ATOM    110  PO4 POPCU  10     -17.658  -8.749  18.948  0.00  0.00            
-ATOM    111  GL1 POPCU  10     -15.737  -8.029  15.351  0.00  1.00            
-ATOM    112  GL2 POPCU  10     -13.030  -8.062  15.059  0.00  1.00            
-ATOM    113  C1A POPCU  10     -15.214 -11.947  12.734  0.00  0.00            
-ATOM    114  D2A POPCU  10     -14.836 -11.716   8.825  0.00  0.00            
-ATOM    115  C3A POPCU  10     -14.668 -13.504   3.973  0.00  0.00            
-ATOM    116  C4A POPCU  10     -13.886 -13.843  -0.380  0.00  0.00            
-ATOM    117  C1B POPCU  10     -12.455  -8.184  10.980  0.00  0.00            
-ATOM    118  C2B POPCU  10     -10.545  -8.509   7.859  0.00  0.00            
-ATOM    119  C3B POPCU  10      -8.194  -7.158   5.707  0.00  0.00            
-ATOM    120  C4B POPCU  10      -6.264  -3.693   2.882  0.00  0.00            
-ATOM    121  NC3 POPCU  11     -12.143   2.638  19.549  0.00  0.00            
-ATOM    122  PO4 POPCU  11     -15.837   0.329  19.358  0.00  0.00            
-ATOM    123  GL1 POPCU  11     -15.525  -0.249  15.133  0.00  1.00            
-ATOM    124  GL2 POPCU  11     -13.725  -0.346  15.025  0.00  1.00            
-ATOM    125  C1A POPCU  11     -17.539  -1.035  10.908  0.00  0.00            
-ATOM    126  D2A POPCU  11     -20.437   1.033   9.181  0.00  0.00            
-ATOM    127  C3A POPCU  11     -21.438   1.455   5.313  0.00  0.00            
-ATOM    128  C4A POPCU  11     -23.601   2.208   2.189  0.00  0.00            
-ATOM    129  C1B POPCU  11     -13.072  -3.381  12.319  0.00  0.00            
-ATOM    130  C2B POPCU  11     -13.786  -3.002   8.085  0.00  0.00            
-ATOM    131  C3B POPCU  11     -12.954  -3.809   3.798  0.00  0.00            
-ATOM    132  C4B POPCU  11     -14.292  -3.382   0.360  0.00  0.00            
-ATOM    133  NC3 POPCU  12     -14.060   8.107  19.789  0.00  0.00            
-ATOM    134  PO4 POPCU  12     -16.642  10.714  18.570  0.00  0.00            
-ATOM    135  GL1 POPCU  12     -15.127   7.831  15.247  0.00  1.00            
-ATOM    136  GL2 POPCU  12     -13.094   8.076  14.986  0.00  1.00            
-ATOM    137  C1A POPCU  12     -13.912   7.648  10.388  0.00  0.00            
-ATOM    138  D2A POPCU  12     -10.263   6.324   8.700  0.00  0.00            
-ATOM    139  C3A POPCU  12      -7.032   7.727   5.385  0.00  0.00            
-ATOM    140  C4A POPCU  12      -2.936   7.960   3.025  0.00  0.00            
-ATOM    141  C1B POPCU  12     -11.408   3.814  13.305  0.00  0.00            
-ATOM    142  C2B POPCU  12     -13.675   1.850   9.611  0.00  0.00            
-ATOM    143  C3B POPCU  12     -15.507   0.519   5.318  0.00  0.00            
-ATOM    144  C4B POPCU  12     -18.701  -0.936   2.005  0.00  0.00            
-ATOM    145  NC3 POPCU  14       1.300 -11.851  18.797  0.00  0.00            
-ATOM    146  PO4 POPCU  14      -1.658 -14.313  19.266  0.00  0.00            
-ATOM    147  GL1 POPCU  14      -0.008 -16.222  15.079  0.00  1.00            
-ATOM    148  GL2 POPCU  14       2.752 -15.973  15.003  0.00  1.00            
-ATOM    149  C1A POPCU  14      -0.503 -15.311  10.483  0.00  0.00            
-ATOM    150  D2A POPCU  14      -0.839 -14.626   6.624  0.00  0.00            
-ATOM    151  C3A POPCU  14       3.631 -13.962   5.013  0.00  0.00            
-ATOM    152  C4A POPCU  14       6.522 -15.593   5.130  0.00  0.00            
-ATOM    153  C1B POPCU  14       4.423 -17.507  12.115  0.00  0.00            
-ATOM    154  C2B POPCU  14       7.320 -15.128  10.296  0.00  0.00            
-ATOM    155  C3B POPCU  14      11.064 -13.886   7.267  0.00  0.00            
-ATOM    156  C4B POPCU  14      14.736 -13.175   5.107  0.00  0.00            
-ATOM    157  NC3 POPCU  15       9.187 -12.621  18.874  0.00  0.00            
-ATOM    158  PO4 POPCU  15       6.082 -12.739  16.259  0.00  0.00            
-ATOM    159  GL1 POPCU  15       8.143 -16.227  15.320  0.00  1.00            
-ATOM    160  GL2 POPCU  15      10.658 -15.844  15.137  0.00  1.00            
-ATOM    161  C1A POPCU  15      11.225 -18.315  11.402  0.00  0.00            
-ATOM    162  D2A POPCU  15      14.733 -16.856   9.403  0.00  0.00            
-ATOM    163  C3A POPCU  15      18.518 -19.553   8.964  0.00  0.00            
-ATOM    164  C4A POPCU  15      20.764 -21.225  11.668  0.00  0.00            
-ATOM    165  C1B POPCU  15      12.314 -12.832  12.682  0.00  0.00            
-ATOM    166  C2B POPCU  15      16.028 -11.600  10.747  0.00  0.00            
-ATOM    167  C3B POPCU  15      17.624  -9.744   6.876  0.00  0.00            
-ATOM    168  C4B POPCU  15      15.415  -8.865   2.291  0.00  0.00            
-ATOM    169  NC3 POPCU  16     -19.288 -13.963  19.453  0.00  0.00            
-ATOM    170  PO4 POPCU  16     -22.768 -10.927  18.302  0.00  0.00            
-ATOM    171  GL1 POPCU  16     -21.767  -7.759  14.820  0.00  1.00            
-ATOM    172  GL2 POPCU  16     -20.124  -7.873  14.502  0.00  1.00            
-ATOM    173  C1A POPCU  16     -21.350  -4.333  10.751  0.00  0.00            
-ATOM    174  D2A POPCU  16     -19.352  -3.175   6.816  0.00  0.00            
-ATOM    175  C3A POPCU  16     -18.223  -5.873   2.741  0.00  0.00            
-ATOM    176  C4A POPCU  16     -18.050  -5.813  -2.373  0.00  0.00            
-ATOM    177  C1B POPCU  16     -17.500  -7.284  10.217  0.00  0.00            
-ATOM    178  C2B POPCU  16     -15.649  -7.288   6.980  0.00  0.00            
-ATOM    179  C3B POPCU  16     -13.346  -8.645   3.369  0.00  0.00            
-ATOM    180  C4B POPCU  16      -9.697  -6.827   1.029  0.00  0.00            
-ATOM    181  NC3 POPCU  17      15.838  -4.974  21.609  0.00  0.00            
-ATOM    182  PO4 POPCU  17      14.401  -3.730  17.274  0.00  0.00            
-ATOM    183  GL1 POPCU  17      15.950  -0.039  14.746  0.00  1.00            
-ATOM    184  GL2 POPCU  17      17.864   0.507  15.022  0.00  1.00            
-ATOM    185  C1A POPCU  17      14.235   3.840  13.061  0.00  0.00            
-ATOM    186  D2A POPCU  17      15.787   6.814   9.979  0.00  0.00            
-ATOM    187  C3A POPCU  17      16.207   6.573   5.474  0.00  0.00            
-ATOM    188  C4A POPCU  17      16.031   7.128   1.450  0.00  0.00            
-ATOM    189  C1B POPCU  17      20.042   3.677  13.058  0.00  0.00            
-ATOM    190  C2B POPCU  17      20.331   4.759   8.379  0.00  0.00            
-ATOM    191  C3B POPCU  17      20.766   7.494   6.552  0.00  0.00            
-ATOM    192  C4B POPCU  17      20.522  10.296   2.370  0.00  0.00            
-ATOM    193  NC3 POPCU  18      16.050   8.681  19.488  0.00  0.00            
-ATOM    194  PO4 POPCU  18      11.554   7.554  19.360  0.00  0.00            
-ATOM    195  GL1 POPCU  18      15.983   8.090  14.945  0.00  1.00            
-ATOM    196  GL2 POPCU  18      18.139   8.188  15.317  0.00  1.00            
-ATOM    197  C1A POPCU  18      14.704  11.533  11.251  0.00  0.00            
-ATOM    198  D2A POPCU  18      16.411  12.035   7.425  0.00  0.00            
-ATOM    199  C3A POPCU  18      14.559  11.506   3.121  0.00  0.00            
-ATOM    200  C4A POPCU  18      12.153  14.225  -0.796  0.00  0.00            
-ATOM    201  C1B POPCU  18      20.179  10.245  10.558  0.00  0.00            
-ATOM    202  C2B POPCU  18      21.570  13.168   7.005  0.00  0.00            
-ATOM    203  C3B POPCU  18      18.765  15.518   4.777  0.00  0.00            
-ATOM    204  C4B POPCU  18      17.009  16.937   0.102  0.00  0.00            
-ATOM    205  NC3 POPCU  20       0.996  14.926  23.309  0.00  0.00            
-ATOM    206  PO4 POPCU  20      -1.785  14.878  19.360  0.00  0.00            
-ATOM    207  GL1 POPCU  20      -0.473  15.890  14.821  0.00  1.00            
-ATOM    208  GL2 POPCU  20       2.569  16.095  14.822  0.00  1.00            
-ATOM    209  C1A POPCU  20       0.907  16.698   9.888  0.00  0.00            
-ATOM    210  D2A POPCU  20       2.543  19.132   7.029  0.00  0.00            
-ATOM    211  C3A POPCU  20       6.353  16.399   4.436  0.00  0.00            
-ATOM    212  C4A POPCU  20       8.992  13.393   3.260  0.00  0.00            
-ATOM    213  C1B POPCU  20       4.835  12.086  12.816  0.00  0.00            
-ATOM    214  C2B POPCU  20       5.366   8.676  10.386  0.00  0.00            
-ATOM    215  C3B POPCU  20       7.667   5.447   7.458  0.00  0.00            
-ATOM    216  C4B POPCU  20      12.380   3.920   7.338  0.00  0.00            
-ATOM    217  NC3 POPCU  21       8.837  12.061  18.645  0.00  0.00            
-ATOM    218  PO4 POPCU  21       5.359  15.261  18.868  0.00  0.00            
-ATOM    219  GL1 POPCU  21       7.925  16.196  14.902  0.00  1.00            
-ATOM    220  GL2 POPCU  21      10.442  15.740  14.935  0.00  1.00            
-ATOM    221  C1A POPCU  21       7.136  16.459  10.303  0.00  0.00            
-ATOM    222  D2A POPCU  21      10.201  17.342   7.411  0.00  0.00            
-ATOM    223  C3A POPCU  21      14.071  16.120   8.966  0.00  0.00            
-ATOM    224  C4A POPCU  21      15.198  16.164  12.803  0.00  0.00            
-ATOM    225  C1B POPCU  21      10.230  12.906  12.440  0.00  0.00            
-ATOM    226  C2B POPCU  21       8.342  12.606   8.053  0.00  0.00            
-ATOM    227  C3B POPCU  21       5.966  10.768   5.369  0.00  0.00            
-ATOM    228  C4B POPCU  21       6.899   7.661   2.249  0.00  0.00            
-ATOM    229  NC3 POPCU  22     -12.761 -16.953  23.611  0.00  0.00            
-ATOM    230  PO4 POPCU  22     -14.992 -17.216  19.940  0.00  0.00            
-ATOM    231  GL1 POPCU  22     -15.897 -16.188  15.359  0.00  1.00            
-ATOM    232  GL2 POPCU  22     -13.303 -16.175  14.599  0.00  1.00            
-ATOM    233  C1A POPCU  22     -17.364 -16.163  11.244  0.00  0.00            
-ATOM    234  D2A POPCU  22     -19.194 -15.056   7.316  0.00  0.00            
-ATOM    235  C3A POPCU  22     -22.427 -17.595   3.795  0.00  0.00            
-ATOM    236  C4A POPCU  22     -24.183 -21.612   3.722  0.00  0.00            
-ATOM    237  C1B POPCU  22     -13.022 -20.331  14.260  0.00  0.00            
-ATOM    238  C2B POPCU  22     -11.556 -21.491  10.119  0.00  0.00            
-ATOM    239  C3B POPCU  22     -11.433 -22.629   6.216  0.00  0.00            
-ATOM    240  C4B POPCU  22      -9.268 -22.189   1.686  0.00  0.00            
-ATOM    241  GL1 TRIOU  13      -7.944 -16.266  15.250  0.00  1.00            
-ATOM    242  C1A TRIOU  13      -8.510 -17.960  11.053  0.00  0.00            
-ATOM    243  C2A TRIOU  13     -12.828 -16.661   8.692  0.00  0.00            
-ATOM    244  D3A TRIOU  13     -14.948 -19.464   6.548  0.00  0.00            
-ATOM    245  C4A TRIOU  13     -15.970 -18.888   3.681  0.00  0.00            
-ATOM    246  C5A TRIOU  13     -18.985 -16.614   0.833  0.00  0.00            
-ATOM    247  GL2 TRIOU  13      -5.409 -15.907  14.977  0.00  1.00            
-ATOM    248  C1B TRIOU  13      -3.592 -18.810  12.180  0.00  0.00            
-ATOM    249  C2B TRIOU  13      -4.244 -19.032   8.385  0.00  0.00            
-ATOM    250  D3B TRIOU  13      -6.918 -20.211   5.757  0.00  0.00            
-ATOM    251  C4B TRIOU  13     -11.281 -17.877   3.785  0.00  0.00            
-ATOM    252  C5B TRIOU  13     -13.082 -18.939  -0.089  0.00  0.00            
-ATOM    253  GL3 TRIOU  13      -3.406 -12.940  14.193  0.00  0.00            
-ATOM    254  C1C TRIOU  13      -5.118 -13.983   9.878  0.00  0.00            
-ATOM    255  C2C TRIOU  13      -6.045 -15.034   5.206  0.00  0.00            
-ATOM    256  D3C TRIOU  13      -5.841 -18.188   1.571  0.00  0.00            
-ATOM    257  C4C TRIOU  13      -4.404 -16.285  -1.970  0.00  0.00            
-ATOM    258  C5C TRIOU  13      -1.282 -14.293  -2.678  0.00  0.00            
-ATOM    259  GL1 TRIOU  19      -8.041  16.427  15.297  0.00  1.00            
-ATOM    260  C1A TRIOU  19     -10.025  12.829  13.904  0.00  0.00            
-ATOM    261  C2A TRIOU  19     -10.751  11.362   9.982  0.00  0.00            
-ATOM    262  D3A TRIOU  19     -12.140  10.050   5.973  0.00  0.00            
-ATOM    263  C4A TRIOU  19     -13.581  12.850   2.831  0.00  0.00            
-ATOM    264  C5A TRIOU  19     -16.244  15.018   0.621  0.00  0.00            
-ATOM    265  GL2 TRIOU  19      -5.318  16.270  15.449  0.00  1.00            
-ATOM    266  C1B TRIOU  19      -7.036  14.726  10.712  0.00  0.00            
-ATOM    267  C2B TRIOU  19      -7.269  12.858   6.591  0.00  0.00            
-ATOM    268  D3B TRIOU  19      -4.851  12.858   2.043  0.00  0.00            
-ATOM    269  C4B TRIOU  19      -6.193  13.423  -1.888  0.00  0.00            
-ATOM    270  C5B TRIOU  19     -11.265  14.856  -2.603  0.00  0.00            
-ATOM    271  GL3 TRIOU  19      -4.467  13.050  14.697  0.00  0.00            
-ATOM    272  C1C TRIOU  19      -1.322  12.823  11.635  0.00  0.00            
-ATOM    273  C2C TRIOU  19       1.183  11.432   8.085  0.00  0.00            
-ATOM    274  D3C TRIOU  19       2.174  14.058   4.701  0.00  0.00            
-ATOM    275  C4C TRIOU  19       0.132  11.255   0.754  0.00  0.00            
-ATOM    276  C5C TRIOU  19      -1.611   8.364  -1.252  0.00  0.00            
-ATOM    277  NC3 POPCL   1       4.138  -0.093 -23.489  0.00  0.00            
-ATOM    278  PO4 POPCL   1       1.991  -1.172 -19.092  0.00  0.00            
-ATOM    279  GL1 POPCL   1       0.183  -0.053 -15.184  0.00  1.00            
-ATOM    280  GL2 POPCL   1      -2.678  -0.489 -15.004  0.00  1.00            
-ATOM    281  C1A POPCL   1       1.438  -0.108 -10.165  0.00  0.00            
-ATOM    282  D2A POPCL   1       0.351  -1.176  -6.381  0.00  0.00            
-ATOM    283  C3A POPCL   1      -0.871   1.441  -3.232  0.00  0.00            
-ATOM    284  C4A POPCL   1      -3.723   3.897  -0.701  0.00  0.00            
-ATOM    285  C1B POPCL   1      -3.974  -0.384 -10.400  0.00  0.00            
-ATOM    286  C2B POPCL   1      -4.573  -2.085  -6.562  0.00  0.00            
-ATOM    287  C3B POPCL   1      -4.538  -5.151  -3.167  0.00  0.00            
-ATOM    288  C4B POPCL   1      -1.593  -4.337  -1.070  0.00  0.00            
-ATOM    289  NC3 POPCL   2      -1.705   2.886 -18.469  0.00  0.00            
-ATOM    290  PO4 POPCL   2      -5.710   0.222 -19.027  0.00  0.00            
-ATOM    291  GL1 POPCL   2      -7.711   0.177 -14.802  0.00  1.00            
-ATOM    292  GL2 POPCL   2     -10.701  -0.262 -14.776  0.00  1.00            
-ATOM    293  C1A POPCL   2      -8.949  -1.658 -10.339  0.00  0.00            
-ATOM    294  D2A POPCL   2      -9.783  -0.493  -6.796  0.00  0.00            
-ATOM    295  C3A POPCL   2     -11.478  -0.173  -2.814  0.00  0.00            
-ATOM    296  C4A POPCL   2     -12.559   0.777   1.806  0.00  0.00            
-ATOM    297  C1B POPCL   2     -12.854  -3.765 -12.989  0.00  0.00            
-ATOM    298  C2B POPCL   2     -11.344  -6.052 -10.698  0.00  0.00            
-ATOM    299  C3B POPCL   2      -9.002  -5.233  -6.960  0.00  0.00            
-ATOM    300  C4B POPCL   2     -10.981  -4.772  -2.959  0.00  0.00            
-ATOM    301  NC3 POPCL   3       5.989  -3.800 -19.513  0.00  0.00            
-ATOM    302  PO4 POPCL   3       2.235  -7.321 -18.835  0.00  0.00            
-ATOM    303  GL1 POPCL   3       0.448  -7.554 -14.911  0.00  1.00            
-ATOM    304  GL2 POPCL   3      -2.587  -8.083 -15.060  0.00  1.00            
-ATOM    305  C1A POPCL   3      -0.967  -4.358 -11.708  0.00  0.00            
-ATOM    306  D2A POPCL   3      -5.231  -5.026 -10.592  0.00  0.00            
-ATOM    307  C3A POPCL   3      -4.652  -8.382  -7.175  0.00  0.00            
-ATOM    308  C4A POPCL   3      -1.641  -9.019  -3.887  0.00  0.00            
-ATOM    309  C1B POPCL   3      -2.616 -10.385 -11.292  0.00  0.00            
-ATOM    310  C2B POPCL   3      -3.745 -13.064  -7.731  0.00  0.00            
-ATOM    311  C3B POPCL   3      -7.628 -14.450  -5.230  0.00  0.00            
-ATOM    312  C4B POPCL   3     -12.294 -14.032  -5.003  0.00  0.00            
-ATOM    313  NC3 POPCL   4       9.546   4.199 -17.725  0.00  0.00            
-ATOM    314  PO4 POPCL   4       7.657   0.820 -19.547  0.00  0.00            
-ATOM    315  GL1 POPCL   4       8.121   0.002 -15.206  0.00  1.00            
-ATOM    316  GL2 POPCL   4       5.508   0.030 -14.944  0.00  1.00            
-ATOM    317  C1A POPCL   4       7.932   0.133 -10.637  0.00  0.00            
-ATOM    318  D2A POPCL   4      10.435  -1.930  -7.127  0.00  0.00            
-ATOM    319  C3A POPCL   4       9.911  -6.499  -5.767  0.00  0.00            
-ATOM    320  C4A POPCL   4       6.240  -7.841  -6.461  0.00  0.00            
-ATOM    321  C1B POPCL   4       3.962  -3.328 -12.914  0.00  0.00            
-ATOM    322  C2B POPCL   4       2.792  -6.872 -10.419  0.00  0.00            
-ATOM    323  C3B POPCL   4       1.144  -6.180  -6.577  0.00  0.00            
-ATOM    324  C4B POPCL   4       2.873  -6.247  -3.374  0.00  0.00            
-ATOM    325  NC3 POPCL   5       0.012  11.728 -17.972  0.00  0.00            
-ATOM    326  PO4 POPCL   5       1.412   7.672 -19.427  0.00  0.00            
-ATOM    327  GL1 POPCL   5       0.156   8.010 -15.281  0.00  1.00            
-ATOM    328  GL2 POPCL   5      -2.722   8.129 -14.802  0.00  1.00            
-ATOM    329  C1A POPCL   5       1.681   7.229 -11.388  0.00  0.00            
-ATOM    330  D2A POPCL   5       1.310   4.507  -7.190  0.00  0.00            
-ATOM    331  C3A POPCL   5       2.620   5.894  -3.190  0.00  0.00            
-ATOM    332  C4A POPCL   5       1.521   4.316   0.301  0.00  0.00            
-ATOM    333  C1B POPCL   5      -2.641   7.886  -9.886  0.00  0.00            
-ATOM    334  C2B POPCL   5      -3.894   7.910  -5.661  0.00  0.00            
-ATOM    335  C3B POPCL   5      -6.680   8.456  -1.545  0.00  0.00            
-ATOM    336  C4B POPCL   5      -9.450  10.255   2.238  0.00  0.00            
-ATOM    337  NC3 POPCL   6      -2.631  -4.230 -18.435  0.00  0.00            
-ATOM    338  PO4 POPCL   6      -6.542  -4.470 -16.339  0.00  0.00            
-ATOM    339  GL1 POPCL   6      -7.801  -7.757 -15.014  0.00  1.00            
-ATOM    340  GL2 POPCL   6     -10.667  -7.835 -15.058  0.00  1.00            
-ATOM    341  C1A POPCL   6      -7.472  -9.238 -11.277  0.00  0.00            
-ATOM    342  D2A POPCL   6      -9.776 -10.450  -7.151  0.00  0.00            
-ATOM    343  C3A POPCL   6      -8.349  -8.922  -3.599  0.00  0.00            
-ATOM    344  C4A POPCL   6      -5.729 -11.430  -1.505  0.00  0.00            
-ATOM    345  C1B POPCL   6     -12.725 -10.863 -11.859  0.00  0.00            
-ATOM    346  C2B POPCL   6     -14.997 -12.051  -8.587  0.00  0.00            
-ATOM    347  C3B POPCL   6     -16.478 -16.256  -9.303  0.00  0.00            
-ATOM    348  C4B POPCL   6     -17.521 -20.084  -8.281  0.00  0.00            
-ATOM    349  NC3 POPCL   7      -2.847   8.880 -21.085  0.00  0.00            
-ATOM    350  PO4 POPCL   7      -6.779   6.682 -19.221  0.00  0.00            
-ATOM    351  GL1 POPCL   7      -7.769   7.819 -15.079  0.00  1.00            
-ATOM    352  GL2 POPCL   7     -10.924   8.215 -14.910  0.00  1.00            
-ATOM    353  C1A POPCL   7      -7.966   9.023 -10.384  0.00  0.00            
-ATOM    354  D2A POPCL   7     -10.245   6.488  -7.064  0.00  0.00            
-ATOM    355  C3A POPCL   7      -8.463   4.395  -5.999  0.00  0.00            
-ATOM    356  C4A POPCL   7      -4.393   3.074  -6.054  0.00  0.00            
-ATOM    357  C1B POPCL   7     -13.187   8.997 -10.180  0.00  0.00            
-ATOM    358  C2B POPCL   7     -14.763   8.416  -6.496  0.00  0.00            
-ATOM    359  C3B POPCL   7     -13.488   5.326  -3.187  0.00  0.00            
-ATOM    360  C4B POPCL   7      -9.539   4.386  -1.302  0.00  0.00            
-ATOM    361  NC3 POPCL   8      13.777  -9.671 -19.933  0.00  0.00            
-ATOM    362  PO4 POPCL   8      10.011  -6.245 -19.192  0.00  0.00            
-ATOM    363  GL1 POPCL   8       8.026  -8.820 -15.196  0.00  1.00            
-ATOM    364  GL2 POPCL   8       5.250  -7.337 -14.692  0.00  1.00            
-ATOM    365  C1A POPCL   8       7.046 -11.030 -12.037  0.00  0.00            
-ATOM    366  D2A POPCL   8       5.562 -12.989  -8.121  0.00  0.00            
-ATOM    367  C3A POPCL   8       6.709 -12.591  -4.406  0.00  0.00            
-ATOM    368  C4A POPCL   8      10.927 -10.652  -2.788  0.00  0.00            
-ATOM    369  C1B POPCL   8       7.488  -5.244 -10.698  0.00  0.00            
-ATOM    370  C2B POPCL   8       5.515  -2.736  -7.266  0.00  0.00            
-ATOM    371  C3B POPCL   8       7.112  -2.173  -3.428  0.00  0.00            
-ATOM    372  C4B POPCL   8      10.708  -4.882  -0.579  0.00  0.00            
-ATOM    373  NC3 POPCL   9      13.318  10.022 -20.076  0.00  0.00            
-ATOM    374  PO4 POPCL   9       9.226   8.415 -19.251  0.00  0.00            
-ATOM    375  GL1 POPCL   9       8.029   7.999 -14.963  0.00  1.00            
-ATOM    376  GL2 POPCL   9       5.078   8.161 -14.833  0.00  1.00            
-ATOM    377  C1A POPCL   9       9.952   8.673 -10.994  0.00  0.00            
-ATOM    378  D2A POPCL   9      11.260   7.592  -6.342  0.00  0.00            
-ATOM    379  C3A POPCL   9      13.610  10.118  -3.808  0.00  0.00            
-ATOM    380  C4A POPCL   9      17.929   8.780  -5.015  0.00  0.00            
-ATOM    381  C1B POPCL   9       5.832   4.309 -11.276  0.00  0.00            
-ATOM    382  C2B POPCL   9       9.751   4.313  -8.964  0.00  0.00            
-ATOM    383  C3B POPCL   9      10.125   2.789  -5.051  0.00  0.00            
-ATOM    384  C4B POPCL   9      11.937  -0.054  -2.882  0.00  0.00            
-ATOM    385  NC3 POPCL  10     -15.890  -5.477 -19.361  0.00  0.00            
-ATOM    386  PO4 POPCL  10     -15.556 -10.303 -18.946  0.00  0.00            
-ATOM    387  GL1 POPCL  10     -15.869  -8.266 -14.860  0.00  1.00            
-ATOM    388  GL2 POPCL  10     -18.048  -8.210 -14.933  0.00  1.00            
-ATOM    389  C1A POPCL  10     -16.769  -6.283 -10.941  0.00  0.00            
-ATOM    390  D2A POPCL  10     -18.473  -7.012  -7.424  0.00  0.00            
-ATOM    391  C3A POPCL  10     -17.802 -10.628  -4.955  0.00  0.00            
-ATOM    392  C4A POPCL  10     -18.213 -14.610  -3.825  0.00  0.00            
-ATOM    393  C1B POPCL  10     -17.960 -11.726 -12.714  0.00  0.00            
-ATOM    394  C2B POPCL  10     -20.735 -13.641 -10.133  0.00  0.00            
-ATOM    395  C3B POPCL  10     -24.375 -13.989 -10.359  0.00  0.00            
-ATOM    396  C4B POPCL  10     -25.842 -12.914 -13.337  0.00  0.00            
-ATOM    397  NC3 POPCL  11     -10.555  -2.648 -19.794  0.00  0.00            
-ATOM    398  PO4 POPCL  11     -13.731  -0.546 -18.822  0.00  0.00            
-ATOM    399  GL1 POPCL  11     -15.725   0.142 -15.158  0.00  1.00            
-ATOM    400  GL2 POPCL  11     -17.647   0.060 -14.770  0.00  1.00            
-ATOM    401  C1A POPCL  11     -15.575  -0.843 -10.437  0.00  0.00            
-ATOM    402  D2A POPCL  11     -14.074  -3.200  -8.193  0.00  0.00            
-ATOM    403  C3A POPCL  11     -13.726  -6.905  -5.832  0.00  0.00            
-ATOM    404  C4A POPCL  11     -13.999  -8.937  -2.157  0.00  0.00            
-ATOM    405  C1B POPCL  11     -19.582   3.324 -11.310  0.00  0.00            
-ATOM    406  C2B POPCL  11     -18.353   7.448  -9.473  0.00  0.00            
-ATOM    407  C3B POPCL  11     -17.100  11.661 -10.919  0.00  0.00            
-ATOM    408  C4B POPCL  11     -16.843  15.223 -12.300  0.00  0.00            
-ATOM    409  NC3 POPCL  12     -10.302   2.925 -18.710  0.00  0.00            
-ATOM    410  PO4 POPCL  12     -13.456   7.286 -19.898  0.00  0.00            
-ATOM    411  GL1 POPCL  12     -15.879   7.941 -15.123  0.00  1.00            
-ATOM    412  GL2 POPCL  12     -18.188   7.493 -15.261  0.00  1.00            
-ATOM    413  C1A POPCL  12     -14.176   4.931 -12.721  0.00  0.00            
-ATOM    414  D2A POPCL  12      -9.844   3.682 -11.161  0.00  0.00            
-ATOM    415  C3A POPCL  12      -5.560   4.501 -12.314  0.00  0.00            
-ATOM    416  C4A POPCL  12      -2.009   4.096 -12.536  0.00  0.00            
-ATOM    417  C1B POPCL  12     -18.885  11.685 -16.041  0.00  0.00            
-ATOM    418  C2B POPCL  12     -21.179  16.109 -15.093  0.00  0.00            
-ATOM    419  C3B POPCL  12     -21.290  15.378 -10.166  0.00  0.00            
-ATOM    420  C4B POPCL  12     -21.863  10.883  -9.012  0.00  0.00            
-ATOM    421  NC3 POPCL  13     -10.105 -11.985 -17.594  0.00  0.00            
-ATOM    422  PO4 POPCL  13      -6.238 -13.181 -18.294  0.00  0.00            
-ATOM    423  GL1 POPCL  13      -7.717 -15.763 -15.009  0.00  1.00            
-ATOM    424  GL2 POPCL  13     -10.719 -15.855 -14.919  0.00  1.00            
-ATOM    425  C1A POPCL  13      -6.789 -15.440 -10.429  0.00  0.00            
-ATOM    426  D2A POPCL  13      -4.528 -17.954  -7.101  0.00  0.00            
-ATOM    427  C3A POPCL  13      -2.116 -19.925  -5.233  0.00  0.00            
-ATOM    428  C4A POPCL  13      -2.717 -21.154  -0.880  0.00  0.00            
-ATOM    429  C1B POPCL  13     -11.382 -15.265 -10.325  0.00  0.00            
-ATOM    430  C2B POPCL  13     -11.263 -17.631  -7.598  0.00  0.00            
-ATOM    431  C3B POPCL  13     -13.978 -18.809  -4.873  0.00  0.00            
-ATOM    432  C4B POPCL  13     -17.964 -20.326  -3.335  0.00  0.00            
-ATOM    433  NC3 POPCL  14      -1.187 -12.010 -18.587  0.00  0.00            
-ATOM    434  PO4 POPCL  14       0.144 -15.989 -19.773  0.00  0.00            
-ATOM    435  GL1 POPCL  14       0.410 -15.915 -15.293  0.00  1.00            
-ATOM    436  GL2 POPCL  14      -2.269 -15.607 -14.874  0.00  1.00            
-ATOM    437  C1A POPCL  14       2.709 -13.232 -12.229  0.00  0.00            
-ATOM    438  D2A POPCL  14       1.093 -11.061  -7.346  0.00  0.00            
-ATOM    439  C3A POPCL  14       2.343 -11.422  -2.540  0.00  0.00            
-ATOM    440  C4A POPCL  14       4.772 -12.719   0.022  0.00  0.00            
-ATOM    441  C1B POPCL  14      -1.158 -15.304 -10.832  0.00  0.00            
-ATOM    442  C2B POPCL  14       0.726 -15.993  -7.201  0.00  0.00            
-ATOM    443  C3B POPCL  14       3.606 -17.250  -2.966  0.00  0.00            
-ATOM    444  C4B POPCL  14       4.808 -18.086   1.138  0.00  0.00            
-ATOM    445  NC3 POPCL  15       4.609 -12.135 -18.017  0.00  0.00            
-ATOM    446  PO4 POPCL  15       8.158 -13.563 -18.503  0.00  0.00            
-ATOM    447  GL1 POPCL  15       8.256 -15.771 -14.760  0.00  1.00            
-ATOM    448  GL2 POPCL  15       5.456 -16.217 -15.069  0.00  1.00            
-ATOM    449  C1A POPCL  15       8.892 -15.806 -10.689  0.00  0.00            
-ATOM    450  D2A POPCL  15       5.593 -17.705  -7.678  0.00  0.00            
-ATOM    451  C3A POPCL  15       2.604 -21.171  -6.744  0.00  0.00            
-ATOM    452  C4A POPCL  15       3.063 -23.955  -8.397  0.00  0.00            
-ATOM    453  C1B POPCL  15       2.879 -19.332 -11.771  0.00  0.00            
-ATOM    454  C2B POPCL  15      -0.765 -20.470 -10.391  0.00  0.00            
-ATOM    455  C3B POPCL  15      -4.102 -19.081 -12.598  0.00  0.00            
-ATOM    456  C4B POPCL  15      -4.719 -18.922 -17.245  0.00  0.00            
-ATOM    457  NC3 POPCL  16      12.074  -1.260 -19.514  0.00  0.00            
-ATOM    458  PO4 POPCL  16      15.344  -4.826 -18.634  0.00  0.00            
-ATOM    459  GL1 POPCL  16      15.315  -8.084 -15.238  0.00  1.00            
-ATOM    460  GL2 POPCL  16      12.949  -8.058 -14.668  0.00  1.00            
-ATOM    461  C1A POPCL  16      16.463  -8.748 -11.288  0.00  0.00            
-ATOM    462  D2A POPCL  16      15.129  -9.313  -7.525  0.00  0.00            
-ATOM    463  C3A POPCL  16      15.183 -12.610  -4.982  0.00  0.00            
-ATOM    464  C4A POPCL  16      14.811 -13.310   0.333  0.00  0.00            
-ATOM    465  C1B POPCL  16      11.467  -8.505 -10.927  0.00  0.00            
-ATOM    466  C2B POPCL  16      10.125 -11.353  -7.655  0.00  0.00            
-ATOM    467  C3B POPCL  16      10.514 -14.858  -5.354  0.00  0.00            
-ATOM    468  C4B POPCL  16       8.669 -16.138  -2.044  0.00  0.00            
-ATOM    469  NC3 POPCL  18      19.922   5.182 -20.074  0.00  0.00            
-ATOM    470  PO4 POPCL  18      16.082   4.808 -17.580  0.00  0.00            
-ATOM    471  GL1 POPCL  18      15.165   8.074 -15.389  0.00  1.00            
-ATOM    472  GL2 POPCL  18      13.014   7.696 -15.366  0.00  1.00            
-ATOM    473  C1A POPCL  18      14.623  11.740 -13.541  0.00  0.00            
-ATOM    474  D2A POPCL  18      11.623  13.371 -11.428  0.00  0.00            
-ATOM    475  C3A POPCL  18      12.079  13.129  -7.071  0.00  0.00            
-ATOM    476  C4A POPCL  18      15.549  15.042  -4.176  0.00  0.00            
-ATOM    477  C1B POPCL  18      14.139   6.461 -10.864  0.00  0.00            
-ATOM    478  C2B POPCL  18      15.808   5.246  -7.322  0.00  0.00            
-ATOM    479  C3B POPCL  18      20.133   2.952  -6.648  0.00  0.00            
-ATOM    480  C4B POPCL  18      24.478   3.000  -7.621  0.00  0.00            
-ATOM    481  NC3 POPCL  19      -8.630  12.250 -23.206  0.00  0.00            
-ATOM    482  PO4 POPCL  19      -7.237  12.764 -19.249  0.00  0.00            
-ATOM    483  GL1 POPCL  19      -7.878  15.946 -15.092  0.00  1.00            
-ATOM    484  GL2 POPCL  19     -10.857  15.995 -15.114  0.00  1.00            
-ATOM    485  C1A POPCL  19      -8.720  17.783 -10.968  0.00  0.00            
-ATOM    486  D2A POPCL  19      -8.234  16.017  -7.055  0.00  0.00            
-ATOM    487  C3A POPCL  19      -7.598  18.570  -3.117  0.00  0.00            
-ATOM    488  C4A POPCL  19      -9.382  22.326  -0.309  0.00  0.00            
-ATOM    489  C1B POPCL  19      -9.764  13.293 -11.085  0.00  0.00            
-ATOM    490  C2B POPCL  19      -9.428  11.237  -6.160  0.00  0.00            
-ATOM    491  C3B POPCL  19     -11.344   9.899  -2.888  0.00  0.00            
-ATOM    492  C4B POPCL  19     -14.947  10.803  -2.170  0.00  0.00            
-ATOM    493  NC3 POPCL  20       6.506  18.507 -19.656  0.00  0.00            
-ATOM    494  PO4 POPCL  20       1.961  17.023 -18.865  0.00  0.00            
-ATOM    495  GL1 POPCL  20       0.143  15.917 -15.035  0.00  1.00            
-ATOM    496  GL2 POPCL  20      -2.007  15.631 -15.049  0.00  1.00            
-ATOM    497  C1A POPCL  20      -0.216  12.293 -11.812  0.00  0.00            
-ATOM    498  D2A POPCL  20       0.972   9.603  -6.778  0.00  0.00            
-ATOM    499  C3A POPCL  20       2.877  11.248  -4.010  0.00  0.00            
-ATOM    500  C4A POPCL  20       5.405  12.086  -0.143  0.00  0.00            
-ATOM    501  C1B POPCL  20      -5.007  12.312 -13.765  0.00  0.00            
-ATOM    502  C2B POPCL  20      -4.282  12.406  -8.341  0.00  0.00            
-ATOM    503  C3B POPCL  20      -1.547  12.856  -4.143  0.00  0.00            
-ATOM    504  C4B POPCL  20       1.792  15.819  -1.001  0.00  0.00            
-ATOM    505  NC3 POPCL  21       5.676  12.454 -18.919  0.00  0.00            
-ATOM    506  PO4 POPCL  21       9.935  14.022 -18.601  0.00  0.00            
-ATOM    507  GL1 POPCL  21       8.061  16.027 -15.172  0.00  1.00            
-ATOM    508  GL2 POPCL  21       5.491  16.019 -14.901  0.00  1.00            
-ATOM    509  C1A POPCL  21       7.351  15.841 -10.186  0.00  0.00            
-ATOM    510  D2A POPCL  21       7.649  14.584  -5.500  0.00  0.00            
-ATOM    511  C3A POPCL  21       8.364  10.947  -3.605  0.00  0.00            
-ATOM    512  C4A POPCL  21       7.873   7.121  -2.773  0.00  0.00            
-ATOM    513  C1B POPCL  21       4.603  12.389 -12.861  0.00  0.00            
-ATOM    514  C2B POPCL  21       5.909  10.093  -8.973  0.00  0.00            
-ATOM    515  C3B POPCL  21       5.666   6.624  -7.036  0.00  0.00            
-ATOM    516  C4B POPCL  21       5.277   2.314  -6.197  0.00  0.00            
-ATOM    517  GL1 TRIOL  17      15.770  -0.296 -15.608  0.00  1.00            
-ATOM    518  C1A TRIOL  17      16.939  -2.878 -12.700  0.00  0.00            
-ATOM    519  C2A TRIOL  17      18.602  -2.259  -7.601  0.00  0.00            
-ATOM    520  D3A TRIOL  17      21.828  -1.870  -4.017  0.00  0.00            
-ATOM    521  C4A TRIOL  17      21.343   1.486  -1.601  0.00  0.00            
-ATOM    522  C5A TRIOL  17      19.710   3.644   2.237  0.00  0.00            
-ATOM    523  GL2 TRIOL  17      13.167   0.205 -15.235  0.00  1.00            
-ATOM    524  C1B TRIOL  17      11.697  -3.639 -12.908  0.00  0.00            
-ATOM    525  C2B TRIOL  17      13.851  -4.746  -9.714  0.00  0.00            
-ATOM    526  D3B TRIOL  17      14.505  -4.206  -5.105  0.00  0.00            
-ATOM    527  C4B TRIOL  17      15.761  -8.241  -2.725  0.00  0.00            
-ATOM    528  C5B TRIOL  17      20.212 -10.693   0.558  0.00  0.00            
-ATOM    529  GL3 TRIOL  17      12.414   3.233 -13.792  0.00  0.00            
-ATOM    530  C1C TRIOL  17      13.643   0.947  -9.898  0.00  0.00            
-ATOM    531  C2C TRIOL  17      14.700   0.383  -6.688  0.00  0.00            
-ATOM    532  D3C TRIOL  17      16.929   0.544  -2.963  0.00  0.00            
-ATOM    533  C4C TRIOL  17      17.522   4.318  -2.554  0.00  0.00            
-ATOM    534  C5C TRIOL  17      20.079   6.728  -1.425  0.00  0.00            
-ATOM    535  GL1 TRIOL  22      21.982  21.943 -14.928  0.00  1.00            
-ATOM    536  C1A TRIOL  22      23.904  18.702 -12.237  0.00  0.00            
-ATOM    537  C2A TRIOL  22      24.640  15.866  -9.446  0.00  0.00            
-ATOM    538  D3A TRIOL  22      24.246  14.615  -6.654  0.00  0.00            
-ATOM    539  C4A TRIOL  22      20.210  13.211  -5.244  0.00  0.00            
-ATOM    540  C5A TRIOL  22      17.648  12.085  -0.959  0.00  0.00            
-ATOM    541  GL2 TRIOL  22      19.482  22.263 -15.223  0.00  1.00            
-ATOM    542  C1B TRIOL  22      17.851  19.878 -12.165  0.00  0.00            
-ATOM    543  C2B TRIOL  22      15.579  19.411  -6.944  0.00  0.00            
-ATOM    544  D3B TRIOL  22      15.509  20.587  -3.430  0.00  0.00            
-ATOM    545  C4B TRIOL  22      12.695  19.993  -0.391  0.00  0.00            
-ATOM    546  C5B TRIOL  22       9.742  19.130   2.559  0.00  0.00            
-ATOM    547  GL3 TRIOL  22      15.985  24.809 -15.839  0.00  0.00            
-ATOM    548  C1C TRIOL  22      14.806  20.938 -16.207  0.00  0.00            
-ATOM    549  C2C TRIOL  22      12.449  19.298 -12.624  0.00  0.00            
-ATOM    550  D3C TRIOL  22      11.606  18.117  -9.144  0.00  0.00            
-ATOM    551  C4C TRIOL  22      11.140  18.273  -4.720  0.00  0.00            
-ATOM    552  C5C TRIOL  22       7.868  16.798  -1.238  0.00  0.00            
-ATOM    553  SOD SOD 1   1       9.503  10.903 -40.829  0.00  0.00            
-ATOM    554  SOD SOD 1   2      -9.563   9.831  35.826  0.00  0.00            
-ATOM    555  SOD SOD 1   3       5.011  -4.036 -45.054  0.00  0.00            
-ATOM    556  SOD SOD 1   4     -13.720  -4.365  18.590  0.00  0.00            
-ATOM    557  SOD SOD 1   5      -1.211  -3.931  27.761  0.00  0.00            
-ATOM    558  SOD SOD 1   6      -6.933  14.585  21.072  0.00  0.00            
-ATOM    559  SOD SOD 1   7     -13.303   3.436 -45.367  0.00  0.00            
-ATOM    560  SOD SOD 1   8      17.706 -11.807  34.536  0.00  0.00            
-ATOM    561  SOD SOD 1   9     -15.405 -12.080 -43.434  0.00  0.00            
-ATOM    562  SOD SOD 1  10       6.650 -13.707  38.284  0.00  0.00            
-ATOM    563  SOD SOD 1  11       0.333  14.681 -41.488  0.00  0.00            
-ATOM    564  SOD SOD 1  12      14.405  12.841 -36.025  0.00  0.00            
-ATOM    565  SOD SOD 1  13       4.385   2.418 -34.247  0.00  0.00            
-ATOM    566  SOD SOD 1  14      -0.957  13.433 -31.833  0.00  0.00            
-ATOM    567  SOD SOD 1  15     -14.438  -3.266 -38.076  0.00  0.00            
-ATOM    568  SOD SOD 1  16      10.048 -17.090  30.645  0.00  0.00            
-ATOM    569  SOD SOD 1  17      18.655   4.976  27.139  0.00  0.00            
-ATOM    570  SOD SOD 1  18       3.781 -13.644 -43.524  0.00  0.00            
-ATOM    571  SOD SOD 1  19      13.508  -4.696 -28.451  0.00  0.00            
-ATOM    572  SOD SOD 1  20       4.911  -2.686  34.461  0.00  0.00            
-ATOM    573  CLA CLA 2   1     -13.599  -8.250 -39.766  0.00  0.00            
-ATOM    574  CLA CLA 2   2      11.918  14.900  32.853  0.00  0.00            
-ATOM    575  CLA CLA 2   3     -17.333   5.077 -42.036  0.00  0.00            
-ATOM    576  CLA CLA 2   4       4.123 -18.372  38.944  0.00  0.00            
-ATOM    577  CLA CLA 2   5      17.683 -11.564  27.900  0.00  0.00            
-ATOM    578  CLA CLA 2   6     -18.798   2.847  32.155  0.00  0.00            
-ATOM    579  CLA CLA 2   7       4.801  15.686 -43.265  0.00  0.00            
-ATOM    580  CLA CLA 2   8       2.428  -4.376  30.435  0.00  0.00            
-ATOM    581  CLA CLA 2   9       4.998  -8.686 -42.901  0.00  0.00            
-ATOM    582  CLA CLA 2  10     -16.194  -8.503  39.337  0.00  0.00            
-ATOM    583  CLA CLA 2  11       9.582  11.486 -35.794  0.00  0.00            
-ATOM    584  CLA CLA 2  12      -2.044  13.172 -36.974  0.00  0.00            
-ATOM    585  CLA CLA 2  13       9.770  -1.348  31.096  0.00  0.00            
-ATOM    586  CLA CLA 2  14      -2.197  12.948 -25.828  0.00  0.00            
-ATOM    587  CLA CLA 2  15      -7.805   7.832 -31.370  0.00  0.00            
-ATOM    588  CLA CLA 2  16       9.523 -13.316  33.598  0.00  0.00            
-ATOM    589  CLA CLA 2  17      -9.158  17.130  24.658  0.00  0.00            
-ATOM    590  CLA CLA 2  18      -5.429  18.822  34.423  0.00  0.00            
-ATOM    591  CLA CLA 2  19     -17.273  -3.341  22.673  0.00  0.00            
-ATOM    592  CLA CLA 2  20       9.862  -8.023 -28.140  0.00  0.00            
-ATOM    593  W   W   W   1       6.384  -8.822 -21.574  0.00  0.00            
-ATOM    594  W   W   W   2      -4.343 -16.066 -26.395  0.00  0.00            
-ATOM    595  W   W   W   3       5.789   0.484  38.954  0.00  0.00            
-ATOM    596  W   W   W   4      17.523  -6.029 -30.688  0.00  0.00            
-ATOM    597  W   W   W   5      17.852 -16.593  42.367  0.00  0.00            
-ATOM    598  W   W   W   6      18.352   0.650  42.994  0.00  0.00            
-ATOM    599  W   W   W   7      -0.261  -6.634 -41.682  0.00  0.00            
-ATOM    600  W   W   W   8      -0.448  18.408 -23.429  0.00  0.00            
-ATOM    601  W   W   W   9      -0.178 -14.953  46.249  0.00  0.00            
-ATOM    602  W   W   W  10     -16.758  17.447  23.683  0.00  0.00            
-ATOM    603  W   W   W  11       8.999 -18.136  23.937  0.00  0.00            
-ATOM    604  W   W   W  12      -8.663 -15.850  20.429  0.00  0.00            
-ATOM    605  W   W   W  13     -11.939  10.070 -33.290  0.00  0.00            
-ATOM    606  W   W   W  14       9.262 -11.131  41.625  0.00  0.00            
-ATOM    607  W   W   W  15     -12.859  12.929 -18.618  0.00  0.00            
-ATOM    608  W   W   W  16      -5.853  -5.162  28.102  0.00  0.00            
-ATOM    609  W   W   W  17       9.912  -1.445  40.740  0.00  0.00            
-ATOM    610  W   W   W  18       1.541 -15.613  30.468  0.00  0.00            
-ATOM    611  W   W   W  19      15.802  -0.811  39.101  0.00  0.00            
-ATOM    612  W   W   W  20       5.786  -5.689 -25.726  0.00  0.00            
-ATOM    613  W   W   W  21     -15.804  15.720  18.252  0.00  0.00            
-ATOM    614  W   W   W  22     -10.188  -4.065  22.965  0.00  0.00            
-ATOM    615  W   W   W  23      -9.409  -1.200  40.654  0.00  0.00            
-ATOM    616  W   W   W  24       3.396   8.958  44.334  0.00  0.00            
-ATOM    617  W   W   W  25      -6.768 -11.020  44.403  0.00  0.00            
-ATOM    618  W   W   W  26      -9.086   6.550 -36.198  0.00  0.00            
-ATOM    619  W   W   W  27      -3.710   6.996 -35.638  0.00  0.00            
-ATOM    620  W   W   W  28       9.120 -18.673  36.340  0.00  0.00            
-ATOM    621  W   W   W  29       0.513 -14.301  38.883  0.00  0.00            
-ATOM    622  W   W   W  30      -2.531 -18.415  30.546  0.00  0.00            
-ATOM    623  W   W   W  31      -2.772  -8.552  27.043  0.00  0.00            
-ATOM    624  W   W   W  32       2.781   6.424 -39.277  0.00  0.00            
-ATOM    625  W   W   W  33       1.009  -2.477  38.565  0.00  0.00            
-ATOM    626  W   W   W  34     -10.878  18.462 -35.477  0.00  0.00            
-ATOM    627  W   W   W  35     -18.232  -3.561  44.993  0.00  0.00            
-ATOM    628  W   W   W  36     -15.768  18.663 -40.710  0.00  0.00            
-ATOM    629  W   W   W  37     -13.337  11.636  30.769  0.00  0.00            
-ATOM    630  W   W   W  38      -8.920   3.855  41.536  0.00  0.00            
-ATOM    631  W   W   W  39      -2.663   2.796  32.214  0.00  0.00            
-ATOM    632  W   W   W  40      16.639 -14.115 -44.911  0.00  0.00            
-ATOM    633  W   W   W  41       9.069  -3.160 -28.420  0.00  0.00            
-ATOM    634  W   W   W  42      -9.005  -8.218 -25.887  0.00  0.00            
-ATOM    635  W   W   W  43      -1.896  -1.077 -22.529  0.00  0.00            
-ATOM    636  W   W   W  44       9.989  -3.339  35.887  0.00  0.00            
-ATOM    637  W   W   W  45      -3.150  12.620  41.989  0.00  0.00            
-ATOM    638  W   W   W  46       9.585 -16.045 -37.757  0.00  0.00            
-ATOM    639  W   W   W  47      12.751   6.940 -25.532  0.00  0.00            
-ATOM    640  W   W   W  48       1.706   3.765 -22.188  0.00  0.00            
-ATOM    641  W   W   W  49      -8.132 -11.830 -41.374  0.00  0.00            
-ATOM    642  W   W   W  50     -16.385  -6.420 -43.546  0.00  0.00            
-ATOM    643  W   W   W  51       7.702  -6.272 -33.056  0.00  0.00            
-ATOM    644  W   W   W  52       9.639  -0.578  26.084  0.00  0.00            
-ATOM    645  W   W   W  53      -4.487 -15.575  24.195  0.00  0.00            
-ATOM    646  W   W   W  54      14.420 -18.864  45.947  0.00  0.00            
-ATOM    647  W   W   W  55       2.222  16.114  31.535  0.00  0.00            
-ATOM    648  W   W   W  56      -2.037 -14.171  33.982  0.00  0.00            
-ATOM    649  W   W   W  57     -16.021   2.166 -27.788  0.00  0.00            
-ATOM    650  W   W   W  58      -1.522  -1.460  45.094  0.00  0.00            
-ATOM    651  W   W   W  59      17.159  13.782  46.045  0.00  0.00            
-ATOM    652  W   W   W  60      -5.725   9.182 -26.148  0.00  0.00            
-ATOM    653  W   W   W  61       8.535 -16.595  41.386  0.00  0.00            
-ATOM    654  W   W   W  62      -2.785  -6.759  45.576  0.00  0.00            
-ATOM    655  W   W   W  63       5.675  18.655 -29.382  0.00  0.00            
-ATOM    656  W   W   W  64     -12.589 -13.376  26.841  0.00  0.00            
-ATOM    657  W   W   W  65       7.908  -8.509  24.422  0.00  0.00            
-ATOM    658  W   W   W  66     -10.810  13.648 -42.602  0.00  0.00            
-ATOM    659  W   W   W  67      -4.783 -18.768  20.115  0.00  0.00            
-ATOM    660  W   W   W  68      16.005   3.605  22.396  0.00  0.00            
-ATOM    661  W   W   W  69      -4.569   2.285  43.312  0.00  0.00            
-ATOM    662  W   W   W  70      -5.184  -1.267  23.626  0.00  0.00            
-ATOM    663  W   W   W  71       7.876  12.222  30.196  0.00  0.00            
-ATOM    664  W   W   W  72     -13.172  13.959  35.411  0.00  0.00            
-ATOM    665  W   W   W  73       3.222  -1.411  43.576  0.00  0.00            
-ATOM    666  W   W   W  74       5.880 -16.468  19.988  0.00  0.00            
-ATOM    667  W   W   W  75      18.555  -2.509 -33.341  0.00  0.00            
-ATOM    668  W   W   W  76       3.001   2.017  35.072  0.00  0.00            
-ATOM    669  W   W   W  77      -1.606  -9.823  36.786  0.00  0.00            
-ATOM    670  W   W   W  78      15.046  11.813  35.973  0.00  0.00            
-ATOM    671  W   W   W  79     -11.668 -13.182  44.537  0.00  0.00            
-ATOM    672  W   W   W  80      -9.221   0.664  45.248  0.00  0.00            
-ATOM    673  W   W   W  81      -2.481  11.361  22.805  0.00  0.00            
-ATOM    674  W   W   W  82      -5.711  -3.895 -34.998  0.00  0.00            
-ATOM    675  W   W   W  83     -14.709   2.974 -37.262  0.00  0.00            
-ATOM    676  W   W   W  84     -12.014  -2.536 -24.703  0.00  0.00            
-ATOM    677  W   W   W  85      13.243   2.281  43.183  0.00  0.00            
-ATOM    678  W   W   W  86      -2.565   2.458 -31.278  0.00  0.00            
-ATOM    679  W   W   W  87       3.584  -9.342 -32.205  0.00  0.00            
-ATOM    680  W   W   W  88     -14.512 -11.834  21.393  0.00  0.00            
-ATOM    681  W   W   W  89       4.770  11.633  40.207  0.00  0.00            
-ATOM    682  W   W   W  90      -3.579  -4.487  37.161  0.00  0.00            
-ATOM    683  W   W   W  91      -8.620  -7.535 -38.939  0.00  0.00            
-ATOM    684  W   W   W  92       1.563 -18.377 -43.002  0.00  0.00            
-ATOM    685  W   W   W  93      -9.536  12.351  27.347  0.00  0.00            
-ATOM    686  W   W   W  94       1.393  17.484 -31.923  0.00  0.00            
-ATOM    687  W   W   W  95      -7.624 -15.499 -45.221  0.00  0.00            
-ATOM    688  W   W   W  96       1.853  -4.551 -22.924  0.00  0.00            
-ATOM    689  W   W   W  97       4.439  10.058 -43.064  0.00  0.00            
-ATOM    690  W   W   W  98       8.625 -13.455  45.794  0.00  0.00            
-ATOM    691  W   W   W  99      -1.291  -1.401 -42.544  0.00  0.00            
-ATOM    692  W   W   W 100      -6.794  17.108  44.964  0.00  0.00            
-ATOM    693  W   W   W 101      10.636 -11.673  28.650  0.00  0.00            
-ATOM    694  W   W   W 102      -5.125  -3.848  42.045  0.00  0.00            
-ATOM    695  W   W   W 103      -3.013  17.031 -28.702  0.00  0.00            
-ATOM    696  W   W   W 104       4.762  13.485  26.888  0.00  0.00            
-ATOM    697  W   W   W 105     -17.124 -14.422  24.671  0.00  0.00            
-ATOM    698  W   W   W 106      14.586   3.395 -29.866  0.00  0.00            
-ATOM    699  W   W   W 107     -16.909   2.819  23.340  0.00  0.00            
-ATOM    700  W   W   W 108      17.771  -0.296 -28.986  0.00  0.00            
-ATOM    701  W   W   W 109      13.144  12.561  21.605  0.00  0.00            
-ATOM    702  W   W   W 110     -17.536  16.804  43.413  0.00  0.00            
-ATOM    703  W   W   W 111       5.230   0.323  30.663  0.00  0.00            
-ATOM    704  W   W   W 112     -13.195 -13.633  38.788  0.00  0.00            
-ATOM    705  W   W   W 113     -10.820  14.804 -31.984  0.00  0.00            
-ATOM    706  W   W   W 114     -11.231   7.094  31.435  0.00  0.00            
-ATOM    707  W   W   W 115      -0.673  14.077  28.258  0.00  0.00            
-ATOM    708  W   W   W 116      10.012 -10.851 -37.253  0.00  0.00            
-ATOM    709  W   W   W 117     -17.350   4.389  44.586  0.00  0.00            
-ATOM    710  W   W   W 118      -8.475   6.300  27.928  0.00  0.00            
-ATOM    711  W   W   W 119       0.368   9.322  26.575  0.00  0.00            
-ATOM    712  W   W   W 120      11.537  -5.104 -35.768  0.00  0.00            
-ATOM    713  W   W   W 121      -3.983 -10.398 -38.571  0.00  0.00            
-ATOM    714  W   W   W 122     -18.832  11.036 -36.695  0.00  0.00            
-ATOM    715  W   W   W 123      11.735   3.903  31.925  0.00  0.00            
-ATOM    716  W   W   W 124      -8.648  -6.607  44.943  0.00  0.00            
-ATOM    717  W   W   W 125     -13.690   3.385  33.776  0.00  0.00            
-ATOM    718  W   W   W 126      17.148 -16.474  37.151  0.00  0.00            
-ATOM    719  W   W   W 127       9.527   4.792 -29.378  0.00  0.00            
-ATOM    720  W   W   W 128      18.281  13.325  15.305  0.00  0.00            
-ATOM    721  W   W   W 129     -16.943   6.929 -35.313  0.00  0.00            
-ATOM    722  W   W   W 130     -13.647   1.749  41.896  0.00  0.00            
-ATOM    723  W   W   W 131      17.111   8.367  45.618  0.00  0.00            
-ATOM    724  W   W   W 132       4.746   0.329  25.869  0.00  0.00            
-ATOM    725  W   W   W 133     -16.619  11.572  43.729  0.00  0.00            
-ATOM    726  W   W   W 134      11.235 -15.195 -23.845  0.00  0.00            
-ATOM    727  W   W   W 135       7.787   5.775 -41.370  0.00  0.00            
-ATOM    728  W   W   W 136      10.399  -1.973 -44.962  0.00  0.00            
-ATOM    729  W   W   W 137      14.513  -5.822 -44.743  0.00  0.00            
-ATOM    730  W   W   W 138      -4.983   6.137  38.591  0.00  0.00            
-ATOM    731  W   W   W 139      -9.953  -2.160 -36.749  0.00  0.00            
-ATOM    732  W   W   W 140      13.351 -16.119  26.503  0.00  0.00            
-ATOM    733  W   W   W 141      12.587  12.658 -28.378  0.00  0.00            
-ATOM    734  W   W   W 142     -17.430  12.898  38.308  0.00  0.00            
-ATOM    735  W   W   W 143       2.132   5.047  30.791  0.00  0.00            
-ATOM    736  W   W   W 144     -18.509  -1.344  35.332  0.00  0.00            
-ATOM    737  W   W   W 145       7.152   1.993  43.515  0.00  0.00            
-ATOM    738  W   W   W 146       2.222  16.687 -36.700  0.00  0.00            
-ATOM    739  W   W   W 147      -7.857  -3.120 -29.811  0.00  0.00            
-ATOM    740  W   W   W 148      -2.575 -13.651  28.676  0.00  0.00            
-ATOM    741  W   W   W 149       1.570 -17.290 -27.367  0.00  0.00            
-ATOM    742  W   W   W 150       0.790  14.740  40.256  0.00  0.00            
-ATOM    743  W   W   W 151      14.639  12.613 -41.179  0.00  0.00            
-ATOM    744  W   W   W 152      18.577  -8.698  23.550  0.00  0.00            
-ATOM    745  W   W   W 153      12.171  11.842 -45.939  0.00  0.00            
-ATOM    746  W   W   W 154     -10.112   0.954 -42.077  0.00  0.00            
-ATOM    747  W   W   W 155       1.939   4.341  18.019  0.00  0.00            
-ATOM    748  W   W   W 156      11.046   7.780  28.176  0.00  0.00            
-ATOM    749  W   W   W 157      -3.481  14.422  32.847  0.00  0.00            
-ATOM    750  W   W   W 158     -12.673  10.674  39.619  0.00  0.00            
-ATOM    751  W   W   W 159       2.525  10.574 -29.307  0.00  0.00            
-ATOM    752  W   W   W 160       7.363  16.154  40.428  0.00  0.00            
-ATOM    753  W   W   W 161      18.228  -8.010 -23.209  0.00  0.00            
-ATOM    754  W   W   W 162      13.196  17.386  23.620  0.00  0.00            
-ATOM    755  W   W   W 163      18.273  -4.432 -40.109  0.00  0.00            
-ATOM    756  W   W   W 164       1.667 -15.486  22.497  0.00  0.00            
-ATOM    757  W   W   W 165       4.570 -17.977  45.661  0.00  0.00            
-ATOM    758  W   W   W 166     -13.334  11.165 -23.307  0.00  0.00            
-ATOM    759  W   W   W 167     -13.668  13.777 -36.941  0.00  0.00            
-ATOM    760  W   W   W 168      16.840 -11.293 -32.231  0.00  0.00            
-ATOM    761  W   W   W 169      14.258  -4.040  33.615  0.00  0.00            
-ATOM    762  W   W   W 170       5.616   8.355  27.242  0.00  0.00            
-ATOM    763  W   W   W 171      -9.763 -11.736  31.313  0.00  0.00            
-ATOM    764  W   W   W 172       7.166   0.217 -42.307  0.00  0.00            
-ATOM    765  W   W   W 173      16.299  10.929  41.650  0.00  0.00            
-ATOM    766  W   W   W 174       8.698   0.432 -33.167  0.00  0.00            
-ATOM    767  W   W   W 175      12.404 -15.761 -42.409  0.00  0.00            
-ATOM    768  W   W   W 176      16.151   7.268 -32.747  0.00  0.00            
-ATOM    769  W   W   W 177      -2.892  -6.754 -23.613  0.00  0.00            
-ATOM    770  W   W   W 178      -8.802 -16.461  27.178  0.00  0.00            
-ATOM    771  W   W   W 179      16.873   4.753 -38.438  0.00  0.00            
-ATOM    772  W   W   W 180      17.326  -6.383  41.792  0.00  0.00            
-ATOM    773  W   W   W 181      -9.805  -1.595  27.605  0.00  0.00            
-ATOM    774  W   W   W 182     -16.936 -12.888  43.870  0.00  0.00            
-ATOM    775  W   W   W 183       0.255   1.167  28.367  0.00  0.00            
-ATOM    776  W   W   W 184       8.587   7.137  37.466  0.00  0.00            
-ATOM    777  W   W   W 185     -18.414  15.549  29.246  0.00  0.00            
-ATOM    778  W   W   W 186       4.882 -10.588 -26.519  0.00  0.00            
-ATOM    779  W   W   W 187      -9.638 -12.850 -22.576  0.00  0.00            
-ATOM    780  W   W   W 188      10.038  17.848 -27.497  0.00  0.00            
-ATOM    781  W   W   W 189      -6.322  15.727 -37.743  0.00  0.00            
-ATOM    782  W   W   W 190       4.745   9.224 -23.430  0.00  0.00            
-ATOM    783  W   W   W 191     -14.393 -10.452 -31.663  0.00  0.00            
-ATOM    784  W   W   W 192     -14.963 -10.535  34.898  0.00  0.00            
-ATOM    785  W   W   W 193      -6.756 -11.693  27.226  0.00  0.00            
-ATOM    786  W   W   W 194      13.411  -1.289 -32.459  0.00  0.00            
-ATOM    787  W   W   W 195     -14.515   9.188  35.209  0.00  0.00            
-ATOM    788  W   W   W 196      -6.315  15.647  29.056  0.00  0.00            
-ATOM    789  W   W   W 197       7.369 -17.789 -42.440  0.00  0.00            
-ATOM    790  W   W   W 198      17.884  -6.994  35.697  0.00  0.00            
-ATOM    791  W   W   W 199       3.560  -4.123 -30.831  0.00  0.00            
-ATOM    792  W   W   W 200      -2.269   3.427 -40.089  0.00  0.00            
-ATOM    793  W   W   W 201       6.712  18.906 -34.693  0.00  0.00            
-ATOM    794  W   W   W 202     -10.144  -8.319  35.148  0.00  0.00            
-ATOM    795  W   W   W 203      15.440 -10.621 -26.635  0.00  0.00            
-ATOM    796  W   W   W 204      -0.148   5.886  35.695  0.00  0.00            
-ATOM    797  W   W   W 205      15.818   4.234  35.902  0.00  0.00            
-ATOM    798  W   W   W 206     -10.706   0.532 -28.006  0.00  0.00            
-ATOM    799  W   W   W 207       9.521   9.049  23.520  0.00  0.00            
-ATOM    800  W   W   W 208      -6.515 -15.418  31.217  0.00  0.00            
-ATOM    801  W   W   W 209      16.301   7.762  31.021  0.00  0.00            
-ATOM    802  W   W   W 210     -18.862   9.621 -20.945  0.00  0.00            
-ATOM    803  W   W   W 211     -17.921  -8.689  31.450  0.00  0.00            
-ATOM    804  W   W   W 212      15.681 -11.884 -37.521  0.00  0.00            
-ATOM    805  W   W   W 213      11.558  14.834  38.221  0.00  0.00            
-ATOM    806  W   W   W 214      -8.948   2.182  36.048  0.00  0.00            
-ATOM    807  W   W   W 215      16.088 -13.184  23.511  0.00  0.00            
-ATOM    808  W   W   W 216      14.453  17.831  29.418  0.00  0.00            
-ATOM    809  W   W   W 217      -1.207 -12.229 -34.693  0.00  0.00            
-ATOM    810  W   W   W 218      11.717   9.153 -31.507  0.00  0.00            
-ATOM    811  W   W   W 219      11.844  15.536  43.442  0.00  0.00            
-ATOM    812  W   W   W 220       0.893   2.106 -26.691  0.00  0.00            
-ATOM    813  W   W   W 221       3.916   4.916  39.788  0.00  0.00            
-ATOM    814  W   W   W 222       7.602   6.543 -36.353  0.00  0.00            
-ATOM    815  W   W   W 223       8.211  16.075 -38.704  0.00  0.00            
-ATOM    816  W   W   W 224      16.859   5.308  41.176  0.00  0.00            
-ATOM    817  W   W   W 225     -10.162 -12.263  16.914  0.00  0.00            
-ATOM    818  W   W   W 226     -13.921 -14.435 -35.989  0.00  0.00            
-ATOM    819  W   W   W 227      -2.913   4.033 -23.673  0.00  0.00            
-ATOM    820  W   W   W 228       4.561  11.398 -38.332  0.00  0.00            
-ATOM    821  W   W   W 229       7.280  13.950 -23.777  0.00  0.00            
-ATOM    822  W   W   W 230      -2.064   9.564  31.727  0.00  0.00            
-ATOM    823  W   W   W 231      -5.168   2.040 -44.065  0.00  0.00            
-ATOM    824  W   W   W 232      10.800 -10.206 -23.971  0.00  0.00            
-ATOM    825  W   W   W 233     -15.923   8.835 -30.151  0.00  0.00            
-ATOM    826  W   W   W 234      -2.870  15.077 -20.510  0.00  0.00            
-ATOM    827  W   W   W 235      17.103   8.427 -26.541  0.00  0.00            
-ATOM    828  W   W   W 236     -14.020  -4.415  27.420  0.00  0.00            
-ATOM    829  W   W   W 237      16.243  15.495  39.886  0.00  0.00            
-ATOM    830  W   W   W 238      11.323  -8.109  20.071  0.00  0.00            
-ATOM    831  W   W   W 239      -8.396  14.583  35.641  0.00  0.00            
-ATOM    832  W   W   W 240      -1.540 -10.456  22.868  0.00  0.00            
-ATOM    833  W   W   W 241      -9.345 -14.906  35.378  0.00  0.00            
-ATOM    834  W   W   W 242     -18.469   4.864  18.661  0.00  0.00            
-ATOM    835  W   W   W 243     -13.909  -1.670 -31.717  0.00  0.00            
-ATOM    836  W   W   W 244      13.319   8.220 -42.933  0.00  0.00            
-ATOM    837  W   W   W 245      -1.635 -11.831  42.977  0.00  0.00            
-ATOM    838  W   W   W 246      11.085  15.607 -32.840  0.00  0.00            
-ATOM    839  W   W   W 247      -6.583  10.165 -38.727  0.00  0.00            
-ATOM    840  W   W   W 248      16.522  14.243  25.567  0.00  0.00            
-ATOM    841  W   W   W 249     -13.086   6.834  43.257  0.00  0.00            
-ATOM    842  W   W   W 250     -14.672  12.530  13.761  0.00  0.00            
-ATOM    843  W   W   W 251       6.780   8.258 -31.917  0.00  0.00            
-ATOM    844  W   W   W 252       9.721  11.172  41.197  0.00  0.00            
-ATOM    845  W   W   W 253     -17.723  12.323  33.084  0.00  0.00            
-ATOM    846  W   W   W 254      13.154  -7.903  25.380  0.00  0.00            
-ATOM    847  W   W   W 255       9.573  -3.724  17.800  0.00  0.00            
-ATOM    848  W   W   W 256     -16.956   7.427  39.617  0.00  0.00            
-ATOM    849  W   W   W 257      -6.410  13.360 -28.749  0.00  0.00            
-ATOM    850  W   W   W 258       8.781 -12.498 -41.837  0.00  0.00            
-ATOM    851  W   W   W 259     -10.546  -3.701  32.308  0.00  0.00            
-ATOM    852  W   W   W 260       3.244 -11.888  35.142  0.00  0.00            
-ATOM    853  W   W   W 261       7.811   3.619  28.002  0.00  0.00            
-ATOM    854  W   W   W 262      11.756 -13.527 -28.580  0.00  0.00            
-ATOM    855  W   W   W 263     -11.928   5.650 -27.782  0.00  0.00            
-ATOM    856  W   W   W 264      -1.279  -2.336 -37.835  0.00  0.00            
-ATOM    857  W   W   W 265      18.107  -9.431 -41.061  0.00  0.00            
-ATOM    858  W   W   W 266      13.694   2.428 -41.432  0.00  0.00            
-ATOM    859  W   W   W 267      -4.709  14.241 -42.342  0.00  0.00            
-ATOM    860  W   W   W 268       5.788 -10.986  29.505  0.00  0.00            
-ATOM    861  W   W   W 269     -13.386   3.337 -32.427  0.00  0.00            
-ATOM    862  W   W   W 270      13.771  -2.879 -40.582  0.00  0.00            
-ATOM    863  W   W   W 271      10.450   3.340 -45.269  0.00  0.00            
-ATOM    864  W   W   W 272      -4.732 -15.708 -35.539  0.00  0.00            
-ATOM    865  W   W   W 273      12.577 -14.204 -34.202  0.00  0.00            
-ATOM    866  W   W   W 274      13.209   8.433  38.926  0.00  0.00            
-ATOM    867  W   W   W 275     -17.401 -15.570 -31.179  0.00  0.00            
-ATOM    868  W   W   W 276       3.733   1.332 -38.966  0.00  0.00            
-ATOM    869  W   W   W 277      -6.481  -8.949 -21.189  0.00  0.00            
-ATOM    870  W   W   W 278     -11.869  -6.380 -29.570  0.00  0.00            
-ATOM    871  W   W   W 279       2.885  10.786  31.430  0.00  0.00            
-ATOM    872  W   W   W 280      17.851  -5.455  27.023  0.00  0.00            
-ATOM    873  W   W   W 281      -9.958   8.620 -42.820  0.00  0.00            
-ATOM    874  W   W   W 282      11.026  15.823 -43.554  0.00  0.00            
-ATOM    875  W   W   W 283     -10.588  15.980  31.567  0.00  0.00            
-ATOM    876  W   W   W 284     -15.607  17.567  33.113  0.00  0.00            
-ATOM    877  W   W   W 285     -14.379 -16.920  42.391  0.00  0.00            
-ATOM    878  W   W   W 286      -6.099  -1.965 -40.502  0.00  0.00            
-ATOM    879  W   W   W 287       4.104   9.293  35.797  0.00  0.00            
-ATOM    880  W   W   W 288      -3.577  -5.713  32.482  0.00  0.00            
-ATOM    881  W   W   W 289      17.225  17.957 -43.035  0.00  0.00            
-ATOM    882  W   W   W 290      18.421   9.711 -42.238  0.00  0.00            
-ATOM    883  W   W   W 291       8.634  -4.217 -40.492  0.00  0.00            
-ATOM    884  W   W   W 292      16.445   1.116 -21.259  0.00  0.00            
-ATOM    885  W   W   W 293      -6.035   6.229  33.598  0.00  0.00            
-ATOM    886  W   W   W 294     -14.666  -0.916  31.611  0.00  0.00            
-ATOM    887  W   W   W 295       2.503   0.860 -44.309  0.00  0.00            
-ATOM    888  W   W   W 296       0.076 -17.676  26.205  0.00  0.00            
-ATOM    889  W   W   W 297      -8.274  13.930  40.855  0.00  0.00            
-ATOM    890  W   W   W 298      13.579  12.035  16.837  0.00  0.00            
-ATOM    891  W   W   W 299       1.691  -5.974 -35.432  0.00  0.00            
-ATOM    892  W   W   W 300     -13.877  15.535  27.096  0.00  0.00            
-ATOM    893  W   W   W 301      10.317  -8.007  31.778  0.00  0.00            
-ATOM    894  W   W   W 302     -16.619 -15.348  35.337  0.00  0.00            
-ATOM    895  W   W   W 303      17.104   3.585 -25.487  0.00  0.00            
-ATOM    896  W   W   W 304      -8.578 -13.891  40.507  0.00  0.00            
-ATOM    897  W   W   W 305       4.372 -11.062  22.473  0.00  0.00            
-ATOM    898  W   W   W 306      13.107  -5.493 -23.158  0.00  0.00            
-ATOM    899  W   W   W 307       5.380   4.755 -45.842  0.00  0.00            
-ATOM    900  W   W   W 308     -15.048  15.246 -45.182  0.00  0.00            
-ATOM    901  W   W   W 309      -4.956   0.094  38.612  0.00  0.00            
-ATOM    902  W   W   W 310      -4.559 -15.764  43.305  0.00  0.00            
-ATOM    903  W   W   W 311     -13.446  -0.439  24.569  0.00  0.00            
-ATOM    904  W   W   W 312      -8.496   1.755 -32.102  0.00  0.00            
-ATOM    905  W   W   W 313      -8.957 -18.769  40.973  0.00  0.00            
-ATOM    906  W   W   W 314       4.496  13.015 -33.206  0.00  0.00            
-ATOM    907  W   W   W 315      15.639  -0.980  25.164  0.00  0.00            
-ATOM    908  W   W   W 316       1.556  -7.685 -27.767  0.00  0.00            
-ATOM    909  W   W   W 317      -3.114   5.926  27.426  0.00  0.00            
-ATOM    910  W   W   W 318       5.067   5.622 -26.945  0.00  0.00            
-ATOM    911  W   W   W 319     -12.218   5.319  38.281  0.00  0.00            
-ATOM    912  W   W   W 320      -8.130   1.929 -23.300  0.00  0.00            
-ATOM    913  W   W   W 321     -11.204  10.981 -28.094  0.00  0.00            
-ATOM    914  W   W   W 322     -15.276  -9.111  26.895  0.00  0.00            
-ATOM    915  W   W   W 323       4.972  -7.960  33.159  0.00  0.00            
-ATOM    916  W   W   W 324       1.197   8.804 -34.953  0.00  0.00            
-ATOM    917  W   W   W 325      15.509   8.950  25.830  0.00  0.00            
-ATOM    918  W   W   W 326       4.718  17.692  24.069  0.00  0.00            
-ATOM    919  W   W   W 327      -6.224  -1.523  32.940  0.00  0.00            
-ATOM    920  W   W   W 328       1.890 -12.031  26.733  0.00  0.00            
-ATOM    921  W   W   W 329       0.309  -1.527  23.189  0.00  0.00            
-ATOM    922  W   W   W 330      -6.563  11.979  45.781  0.00  0.00            
-ATOM    923  W   W   W 331       1.623  -7.094  25.400  0.00  0.00            
-ATOM    924  W   W   W 332     -16.397 -13.192  30.257  0.00  0.00            
-ATOM    925  W   W   W 333       6.719  13.254 -28.860  0.00  0.00            
-ATOM    926  W   W   W 334       0.582   9.180  39.522  0.00  0.00            
-ATOM    927  W   W   W 335      12.504 -14.129  38.568  0.00  0.00            
-ATOM    928  W   W   W 336     -15.839  14.764 -32.237  0.00  0.00            
-ATOM    929  W   W   W 337     -11.913 -16.492 -42.540  0.00  0.00            
-ATOM    930  W   W   W 338      -1.420   9.213 -40.059  0.00  0.00            
-ATOM    931  W   W   W 339      -6.889  -3.538 -23.080  0.00  0.00            
-ATOM    932  W   W   W 340      -8.022   9.203  41.170  0.00  0.00            
-ATOM    933  W   W   W 341       9.932  -6.011  43.408  0.00  0.00            
-ATOM    934  W   W   W 342       3.997 -14.387 -22.469  0.00  0.00            
-ATOM    935  W   W   W 343     -17.292 -10.281 -36.507  0.00  0.00            
-ATOM    936  W   W   W 344       4.220  15.403  36.056  0.00  0.00            
-ATOM    937  W   W   W 345      13.262 -14.048  44.021  0.00  0.00            
-ATOM    938  W   W   W 346      -8.446  17.417 -20.259  0.00  0.00            
-ATOM    939  W   W   W 347      -5.083  -7.736 -29.068  0.00  0.00            
-ATOM    940  W   W   W 348     -10.562  -6.637 -34.219  0.00  0.00            
-ATOM    941  W   W   W 349      13.733  -9.426  42.775  0.00  0.00            
-ATOM    942  W   W   W 350      13.194 -10.957 -44.521  0.00  0.00            
-ATOM    943  W   W   W 351      14.246   3.473  17.858  0.00  0.00            
-ATOM    944  W   W   W 352     -15.138 -10.054 -25.747  0.00  0.00            
-ATOM    945  W   W   W 353     -11.604  12.193  44.317  0.00  0.00            
-ATOM    946  W   W   W 354      17.380  -3.306 -24.900  0.00  0.00            
-ATOM    947  W   W   W 355      -9.715 -11.754  22.986  0.00  0.00            
-ATOM    948  W   W   W 356       5.179 -18.700  28.854  0.00  0.00            
-ATOM    949  W   W   W 357       5.002  -4.312  23.575  0.00  0.00            
-ATOM    950  W   W   W 358      -8.861 -16.508 -38.549  0.00  0.00            
-ATOM    951  W   W   W 359      -1.048   2.920  39.647  0.00  0.00            
-ATOM    952  W   W   W 360      10.081   0.243 -38.208  0.00  0.00            
-ATOM    953  W   W   W 361     -18.112  10.582  28.241  0.00  0.00            
-ATOM    954  W   W   W 362      -2.649   8.582 -30.806  0.00  0.00            
-ATOM    955  W   W   W 363     -18.473 -15.221 -40.153  0.00  0.00            
-ATOM    956  W   W   W 364     -16.066   7.131 -25.193  0.00  0.00            
-ATOM    957  W   W   W 365     -16.869  18.388  38.563  0.00  0.00            
-ATOM    958  W   W   W 366      13.436   3.862  27.255  0.00  0.00            
-ATOM    959  W   W   W 367       3.233 -14.274 -31.823  0.00  0.00            
-ATOM    960  W   W   W 368      -3.089 -17.602 -43.451  0.00  0.00            
-ATOM    961  W   W   W 369      -3.324  17.210 -33.873  0.00  0.00            
-ATOM    962  W   W   W 370     -16.085   6.993  31.523  0.00  0.00            
-ATOM    963  W   W   W 371      11.925  -0.195  20.838  0.00  0.00            
-ATOM    964  W   W   W 372      13.726   3.102 -34.972  0.00  0.00            
-ATOM    965  W   W   W 373      -2.334   2.740  24.092  0.00  0.00            
-ATOM    966  W   W   W 374      -1.199  -1.688  33.091  0.00  0.00            
-ATOM    967  W   W   W 375      -0.013   7.550 -25.434  0.00  0.00            
-ATOM    968  W   W   W 376      17.964   2.342 -33.140  0.00  0.00            
-ATOM    969  W   W   W 377       5.409 -12.635 -35.915  0.00  0.00            
-ATOM    970  W   W   W 378       0.661  -0.940 -32.790  0.00  0.00            
-ATOM    971  W   W   W 379       9.777  17.961  19.375  0.00  0.00            
-ATOM    972  W   W   W 380       6.925  -4.591  28.630  0.00  0.00            
-ATOM    973  W   W   W 381       1.263  -6.485  42.709  0.00  0.00            
-ATOM    974  W   W   W 382      10.059   3.858  23.067  0.00  0.00            
-ATOM    975  W   W   W 383       6.176  -4.997  39.084  0.00  0.00            
-ATOM    976  W   W   W 384     -10.259  -9.234  40.119  0.00  0.00            
-ATOM    977  W   W   W 385      13.064  -7.986 -39.962  0.00  0.00            
-ATOM    978  W   W   W 386       9.726  -7.382 -44.104  0.00  0.00            
-ATOM    979  W   W   W 387     -18.544  -3.779  31.185  0.00  0.00            
-ATOM    980  W   W   W 388      -4.905 -10.498  31.964  0.00  0.00            
-ATOM    981  W   W   W 389      11.281  12.548  26.368  0.00  0.00            
-ATOM    982  W   W   W 390     -11.160  -9.313 -44.410  0.00  0.00            
-ATOM    983  W   W   W 391      15.179  12.461  30.381  0.00  0.00            
-ATOM    984  W   W   W 392      -8.235  -3.547  36.661  0.00  0.00            
-ATOM    985  W   W   W 393     -13.074  15.442  41.158  0.00  0.00            
-ATOM    986  W   W   W 394      -3.831  16.687  38.805  0.00  0.00            
-ATOM    987  W   W   W 395      -0.027 -10.139  31.849  0.00  0.00            
-ATOM    988  W   W   W 396     -16.444  -6.278 -34.006  0.00  0.00            
-ATOM    989  W   W   W 397     -11.046  -3.614 -43.584  0.00  0.00            
-ATOM    990  W   W   W 398      -0.823 -14.633 -40.503  0.00  0.00            
-ATOM    991  W   W   W 399      15.253  -8.164  30.934  0.00  0.00            
-ATOM    992  W   W   W 400       0.444  12.392  35.768  0.00  0.00            
-ATOM    993  W   W   W 401       8.143  14.343  22.964  0.00  0.00            
-ATOM    994  W   W   W 402     -16.895   0.289 -42.908  0.00  0.00            
-ATOM    995  W   W   W 403       0.049 -18.151  42.326  0.00  0.00            
-ATOM    996  W   W   W 404      13.151  17.654 -38.375  0.00  0.00            
-ATOM    997  W   W   W 405      17.533 -17.791  25.831  0.00  0.00            
-ATOM    998  W   W   W 406      16.039   3.591 -45.364  0.00  0.00            
-ATOM    999  W   W   W 407     -14.283  12.633  22.639  0.00  0.00            
-ATOM   1000  W   W   W 408       5.331  -8.579  44.156  0.00  0.00            
-ATOM   1001  W   W   W 409      18.053  13.710  21.048  0.00  0.00            
-ATOM   1002  W   W   W 410     -13.117  -7.696  31.112  0.00  0.00            
-ATOM   1003  W   W   W 411       0.688   3.697  44.044  0.00  0.00            
-ATOM   1004  W   W   W 412       3.927 -13.559  43.186  0.00  0.00            
-ATOM   1005  W   W   W 413      17.905 -18.823  20.612  0.00  0.00            
-ATOM   1006  W   W   W 414      11.523   3.036 -22.222  0.00  0.00            
-ATOM   1007  W   W   W 415      14.503 -13.072  31.240  0.00  0.00            
-ATOM   1008  W   W   W 416     -13.808   3.668  28.362  0.00  0.00            
-ATOM   1009  W   W   W 417      -4.244 -15.710  38.150  0.00  0.00            
-ATOM   1010  W   W   W 418      -5.467  16.818 -24.267  0.00  0.00            
-ATOM   1011  W   W   W 419      12.117  16.936 -22.674  0.00  0.00            
-ATOM   1012  W   W   W 420       1.092  -6.031  34.917  0.00  0.00            
-ATOM   1013  W   W   W 421      -3.892   7.827  44.175  0.00  0.00            
-ATOM   1014  W   W   W 422     -11.404  18.680  36.717  0.00  0.00            
-ATOM   1015  W   W   W 423     -13.114   3.340 -23.167  0.00  0.00            
-ATOM   1016  W   W   W 424      16.442 -16.687 -36.291  0.00  0.00            
-ATOM   1017  W   W   W 425      -5.748  -2.795 -45.548  0.00  0.00            
-ATOM   1018  W   W   W 426       4.415 -16.484 -39.284  0.00  0.00            
-ATOM   1019  W   W   W 427      -4.786  11.165  36.586  0.00  0.00            
-ATOM   1020  W   W   W 428     -12.299 -16.198  31.643  0.00  0.00            
-ATOM   1021  W   W   W 429      13.206  -5.166  39.370  0.00  0.00            
-ATOM   1022  W   W   W 430      11.128 -12.531  23.386  0.00  0.00            
-ATOM   1023  W   W   W 431      -4.631  -0.012 -26.782  0.00  0.00            
-ATOM   1024  W   W   W 432      18.825   8.094  35.235  0.00  0.00            
-ATOM   1025  W   W   W 433       7.953   6.972  42.454  0.00  0.00            
-ATOM   1026  W   W   W 434     -16.334  -4.908 -26.299  0.00  0.00            
-ATOM   1027  W   W   W 435      16.938  -0.140  20.047  0.00  0.00            
-ATOM   1028  W   W   W 436      -3.812 -11.685 -44.379  0.00  0.00            
-ATOM   1029  W   W   W 437     -11.200 -14.545 -32.044  0.00  0.00            
-ATOM   1030  W   W   W 438      14.212  16.299  18.543  0.00  0.00            
-ATOM   1031  W   W   W 439      18.226  -9.444  46.213  0.00  0.00            
-ATOM   1032  W   W   W 440     -16.424  -2.458  40.391  0.00  0.00            
-ATOM   1033  W   W   W 441     -16.278 -17.647 -45.246  0.00  0.00            
-ATOM   1034  W   W   W 442      12.728   0.512  34.966  0.00  0.00            
-ATOM   1035  W   W   W 443      10.078  16.851  27.587  0.00  0.00            
-ATOM   1036  W   W   W 444      -1.937   1.402  19.091  0.00  0.00            
-ATOM   1037  W   W   W 445       0.226 -10.922 -24.135  0.00  0.00            
-ATOM   1038  W   W   W 446      -2.275  18.578 -38.797  0.00  0.00            
-ATOM   1039  W   W   W 447      -5.825 -13.271 -30.441  0.00  0.00            
-ATOM   1040  W   W   W 448       0.054   3.702 -35.867  0.00  0.00            
-ATOM   1041  W   W   W 449       9.495 -18.438  45.770  0.00  0.00            
-ATOM   1042  W   W   W 450       1.934   4.703  25.444  0.00  0.00            
-ATOM   1043  W   W   W 451       3.431  10.038  22.818  0.00  0.00            
-ATOM   1044  W   W   W 452      17.044 -13.954  14.170  0.00  0.00            
-ATOM   1045  W   W   W 453     -15.899  18.849 -35.932  0.00  0.00            
-ATOM   1046  W   W   W 454       3.641  -9.679  39.359  0.00  0.00            
-ATOM   1047  W   W   W 455       7.828   1.608  34.657  0.00  0.00            
-ATOM   1048  W   W   W 456       6.606   5.008 -22.251  0.00  0.00            
-ATOM   1049  W   W   W 457     -17.065  -0.493 -23.189  0.00  0.00            
-ATOM   1050  W   W   W 458      16.492  -1.245 -44.644  0.00  0.00            
-ATOM   1051  W   W   W 459      -0.838  -3.438 -27.854  0.00  0.00            
-ATOM   1052  W   W   W 460      13.283  -0.583 -25.765  0.00  0.00            
-ATOM   1053  W   W   W 461      -8.257  17.562 -42.467  0.00  0.00            
-ATOM   1054  W   W   W 462      -9.410 -10.250 -30.820  0.00  0.00            
-ATOM   1055  W   W   W 463       6.340  -7.661 -37.405  0.00  0.00            
-ATOM   1056  W   W   W 464      -8.148  18.564 -31.498  0.00  0.00            
-ATOM   1057  W   W   W 465      -4.909   8.332 -43.349  0.00  0.00            
-ATOM   1058  W   W   W 466      -2.452  -5.546  23.133  0.00  0.00            
-ATOM   1059  W   W   W 467      -6.364   4.349 -27.720  0.00  0.00            
-ATOM   1060  W   W   W 468     -15.229 -17.830  27.912  0.00  0.00            
-ATOM   1061  W   W   W 469      -7.908   5.824  46.068  0.00  0.00            
-ATOM   1062  W   W   W 470     -16.979   2.977  37.346  0.00  0.00            
-ATOM   1063  W   W   W 471      16.257  16.445 -33.302  0.00  0.00            
-ATOM   1064  W   W   W 472      10.196  -4.242  22.781  0.00  0.00            
-ATOM   1065  W   W   W 473      12.537   7.602 -37.501  0.00  0.00            
-ATOM   1066  W   W   W 474      -0.905 -12.159 -28.744  0.00  0.00            
-ATOM   1067  W   W   W 475     -13.363  -0.453  36.918  0.00  0.00            
-ATOM   1068  W   W   W 476      -9.458 -11.956 -36.037  0.00  0.00            
-ATOM   1069  W   W   W 477      -7.629  11.595  31.905  0.00  0.00            
-ATOM   1070  W   W   W 478      13.110 -18.526  40.496  0.00  0.00            
-ATOM   1071  W   W   W 479     -10.000   7.322 -23.105  0.00  0.00            
-ATOM   1072  W   W   W 480     -18.483   8.027  23.387  0.00  0.00            
-ATOM   1073  W   W   W 481     -14.251  -7.919  44.438  0.00  0.00            
-ATOM   1074  W   W   W 482      -1.477 -16.181 -31.651  0.00  0.00            
-ATOM   1075  W   W   W 483      16.974  -0.350 -37.601  0.00  0.00            
-ATOM   1076  W   W   W 484       6.477   6.429  32.724  0.00  0.00            
-ATOM   1077  W   W   W 485       2.226  15.047 -27.200  0.00  0.00            
-ATOM   1078  W   W   W 486       5.958  -2.954 -36.010  0.00  0.00            
-ATOM   1079  W   W   W 487       1.507   5.345 -30.879  0.00  0.00            
-ATOM   1080  W   W   W 488       3.765  -3.982 -40.105  0.00  0.00            
-ATOM   1081  W   W   W 489       1.261  18.642  19.438  0.00  0.00            
-ATOM   1082  W   W   W 490     -13.897  -1.809  45.355  0.00  0.00            
-ATOM   1083  W   W   W 491     -17.518  -0.129  27.369  0.00  0.00            
-ATOM   1084  W   W   W 492      -9.322   2.387  30.948  0.00  0.00            
-ATOM   1085  W   W   W 493       1.538 -10.136 -39.274  0.00  0.00            
-ATOM   1086  W   W   W 494      14.753 -17.141 -30.561  0.00  0.00            
-ATOM   1087  W   W   W 495      -7.056   4.673 -40.240  0.00  0.00            
-ATOM   1088  W   W   W 496      -5.096   0.958 -36.087  0.00  0.00            
-ATOM   1089  W   W   W 497       5.001 -16.911  34.309  0.00  0.00            
-ATOM   1090  W   W   W 498      15.201   0.016  30.724  0.00  0.00            
-ATOM   1091  W   W   W 499       8.154   1.579 -25.950  0.00  0.00            
-ATOM   1092  W   W   W 500      -5.719  -8.883 -34.297  0.00  0.00            
-ATOM   1093  W   W   W 501      17.681  16.166  34.825  0.00  0.00            
-ATOM   1094  W   W   W 502       8.856   8.483 -45.367  0.00  0.00            
-ATOM   1095  W   W   W 503      17.760  18.641  15.680  0.00  0.00            
-ATOM   1096  W   W   W 504     -12.115   5.347  23.473  0.00  0.00            
-ATOM   1097  W   W   W 505      -8.345   2.452  24.745  0.00  0.00            
-ATOM   1098  W   W   W 506      13.879 -18.093  33.938  0.00  0.00            
-ATOM   1099  W   W   W 507     -11.734  12.187  18.074  0.00  0.00            
-ATOM   1100  W   W   W 508       9.850 -17.248 -31.609  0.00  0.00            
-ATOM   1101  W   W   W 509      12.599   7.408  43.813  0.00  0.00            
-ATOM   1102  W   W   W 510      -0.976  11.063 -44.958  0.00  0.00            
-ATOM   1103  W   W   W 511      14.220  -2.997  43.775  0.00  0.00            
-ATOM   1104  W   W   W 512       3.869   4.057 -17.401  0.00  0.00            
-ATOM   1105  W   W   W 513     -13.888   8.534  26.837  0.00  0.00            
-ATOM   1106  W   W   W 514      12.315  -4.124  28.100  0.00  0.00            
-ATOM   1107  W   W   W 515      13.141  -9.549  35.632  0.00  0.00            
-ATOM   1108  W   W   W 516      11.980  -9.096 -32.460  0.00  0.00            
-ATOM   1109  W   W   W 517     -13.365   8.127 -38.954  0.00  0.00            
-ATOM   1110  W   W   W 518      -4.524   0.786  28.100  0.00  0.00            
-ATOM   1111  W   W   W 519      -1.676  16.115 -46.185  0.00  0.00            
-ATOM   1112  W   W   W 520      18.283 -16.930  31.762  0.00  0.00            
-ATOM   1113  W   W   W 521       4.965   0.152 -29.051  0.00  0.00            
-ATOM   1114  W   W   W 522      -6.018   7.258  23.583  0.00  0.00            
-ATOM   1115  W   W   W 523      -5.205  -7.236 -42.093  0.00  0.00            
-ATOM   1116  W   W   W 524       0.929 -16.625 -36.206  0.00  0.00            
-ATOM   1117  W   W   W 525     -10.373  10.189  22.756  0.00  0.00            
-ATOM   1118  W   W   W 526      -0.604   5.816 -44.176  0.00  0.00            
-ATOM   1119  W   W   W 527      -6.733  -7.840  23.068  0.00  0.00            
-ATOM   1120  W   W   W 528      11.556   3.526  38.825  0.00  0.00            
-ATOM   1121  W   W   W 529       8.190  -8.961  36.924  0.00  0.00            
-ATOM   1122  W   W   W 530       1.365  -9.974 -45.639  0.00  0.00            
-ATOM   1123  W   W   W 531     -11.179  16.678  19.735  0.00  0.00            
-ATOM   1124  W   W   W 532      -3.540  16.268  23.891  0.00  0.00            
-ATOM   1125  W   W   W 533      -6.280 -10.930  36.571  0.00  0.00            
-ATOM   1126  W   W   W 534     -11.736  -7.842 -21.110  0.00  0.00            
-ATOM   1127  W   W   W 535     -10.153  -7.768  27.187  0.00  0.00            
-ATOM   1128  W   W   W 536     -12.388  -5.087  39.063  0.00  0.00            
-ATOM   1129  W   W   W 537      -4.787  10.603  27.786  0.00  0.00            
-ATOM   1130  W   W   W 538      -4.759  -8.718  40.961  0.00  0.00            
-ATOM   1131  W   W   W 539       1.842  13.266 -22.480  0.00  0.00            
-ATOM   1132  W   W   W 540       8.366  11.757  35.938  0.00  0.00            
-ATOM   1133  W   W   W 541       2.832  14.474  44.951  0.00  0.00            
-ATOM   1134  W   W   W 542       0.148   6.713  21.462  0.00  0.00            
-ATOM   1135  W   W   W 543      -1.449  -7.803 -32.141  0.00  0.00            
-ATOM   1136  W   W   W 544     -15.214  -5.542  35.025  0.00  0.00            
-ATOM   1137  W   W   W 545      17.557 -12.068  39.701  0.00  0.00            
-ATOM   1138  W   W   W 546       9.033  -2.486 -23.189  0.00  0.00            
-ATOM   1139  W   W   W 547      11.760   8.937  33.153  0.00  0.00            
-ATOM   1140  W   W   W 548      13.606 -16.121  19.607  0.00  0.00            
-ATOM   1141  W   W   W 549       7.099  16.444  32.219  0.00  0.00            
-ATOM   1142  W   W   W 550      -4.315   5.558  18.943  0.00  0.00            
-ATOM   1143  W   W   W 551       5.133  18.295 -24.296  0.00  0.00            
-ATOM   1144  W   W   W 552     -13.948  -7.223  22.378  0.00  0.00            
-ATOM   1145  W   W   W 553      -0.890  18.691  35.481  0.00  0.00            
-ATOM   1146  W   W   W 554      16.650  -7.237 -35.645  0.00  0.00            
-ATOM   1147  W   W   W 555       6.462 -14.281  25.964  0.00  0.00            
-ATOM   1148  W   W   W 556       8.005 -12.303 -31.416  0.00  0.00            
-ATOM   1149  W   W   W 557     -15.184   8.897 -44.746  0.00  0.00            
-ATOM   1150  W   W   W 558      -6.146  11.831 -33.738  0.00  0.00            
-ATOM   1151  W   W   W 559     -15.876  12.702 -41.081  0.00  0.00            
-ATOM   1152  W   W   W 560      17.465  11.886 -31.416  0.00  0.00            
-ATOM   1153  W   W   W 561       8.764   9.429 -26.462  0.00  0.00            
-ATOM   1154  W   W   W 562      18.529  15.164 -38.518  0.00  0.00            
-ATOM   1155  W   W   W 563       7.196 -15.431 -26.772  0.00  0.00            
-ATOM   1156  W   W   W 564     -11.444  17.822  45.887  0.00  0.00            
-ATOM   1157  W   W   W 565       7.802  13.267  45.637  0.00  0.00            
+CRYST1   36.860   36.860  146.646  90.00  90.00  90.00 P 1           1
+ATOM      1  GL1 TRIO0   1       6.457   2.085  13.400  0.00  0.00            
+ATOM      2  C1A TRIO0   1       5.548   5.217   9.482  0.00  0.00            
+ATOM      3  D2A TRIO0   1       4.528   7.895   6.770  0.00  0.00            
+ATOM      4  C3A TRIO0   1       5.742   6.573   2.379  0.00  0.00            
+ATOM      5  C4A TRIO0   1       7.131   6.746  -2.462  0.00  0.00            
+ATOM      6  GL2 TRIO0   1       5.633  -1.215  14.290  0.00  0.00            
+ATOM      7  C1B TRIO0   1       5.994  -1.895   9.630  0.00  0.00            
+ATOM      8  D2B TRIO0   1       3.808  -3.494   6.065  0.00  0.00            
+ATOM      9  C3B TRIO0   1       5.272  -3.288   1.691  0.00  0.00            
+ATOM     10  C4B TRIO0   1       9.109  -3.976   0.745  0.00  0.00            
+ATOM     11  GL3 TRIO0   1       4.140  -4.181  14.061  0.00  0.00            
+ATOM     12  C1C TRIO0   1       1.339  -4.722  10.345  0.00  0.00            
+ATOM     13  D2C TRIO0   1      -0.128  -6.253   6.342  0.00  0.00            
+ATOM     14  C3C TRIO0   1      -0.111  -5.822   2.426  0.00  0.00            
+ATOM     15  C4C TRIO0   1       0.710  -3.772  -1.698  0.00  0.00            
+ATOM     16  NC3 POPC0   2       4.417   2.971  17.589  0.00  0.00            
+ATOM     17  PO4 POPC0   2       2.087  -2.168  18.273  0.00  0.00            
+ATOM     18  GL1 POPC0   2      -0.304  -1.391  14.908  0.00  0.00            
+ATOM     19  GL2 POPC0   2       0.971   1.670  13.709  0.00  0.00            
+ATOM     20  C1A POPC0   2      -3.193  -0.796  11.465  0.00  0.00            
+ATOM     21  D2A POPC0   2      -1.236  -1.169   7.157  0.00  0.00            
+ATOM     22  C3A POPC0   2      -3.950  -2.971   4.950  0.00  0.00            
+ATOM     23  C4A POPC0   2      -4.403  -3.422   0.349  0.00  0.00            
+ATOM     24  C1B POPC0   2       2.294   1.587  10.293  0.00  0.00            
+ATOM     25  C2B POPC0   2       0.682   3.715   7.249  0.00  0.00            
+ATOM     26  C3B POPC0   2       0.572   6.596   4.368  0.00  0.00            
+ATOM     27  C4B POPC0   2      -1.207   4.945   1.248  0.00  0.00            
+ATOM     28  NC3 POPC0   3      -0.859 -10.796  20.457  0.00  0.00            
+ATOM     29  PO4 POPC0   3      -2.169 -15.294  20.051  0.00  0.00            
+ATOM     30  GL1 POPC0   3      -1.551 -14.551  16.473  0.00  0.00            
+ATOM     31  GL2 POPC0   3       0.927 -12.393  15.746  0.00  0.00            
+ATOM     32  C1A POPC0   3      -5.285 -13.539  12.938  0.00  0.00            
+ATOM     33  D2A POPC0   3      -7.211  -9.965  11.399  0.00  0.00            
+ATOM     34  C3A POPC0   3      -5.781  -7.318   6.965  0.00  0.00            
+ATOM     35  C4A POPC0   3      -4.909  -7.676   2.518  0.00  0.00            
+ATOM     36  C1B POPC0   3       0.344 -13.190  11.545  0.00  0.00            
+ATOM     37  C2B POPC0   3       1.978 -10.336   8.188  0.00  0.00            
+ATOM     38  C3B POPC0   3       3.526  -8.393   4.281  0.00  0.00            
+ATOM     39  C4B POPC0   3       5.332  -8.147   0.752  0.00  0.00            
+ATOM     40  NC3 POPC0   4       9.677  -3.122  22.393  0.00  0.00            
+ATOM     41  PO4 POPC0   4       7.864   0.194  20.000  0.00  0.00            
+ATOM     42  GL1 POPC0   4      10.366   1.387  17.179  0.00  0.00            
+ATOM     43  GL2 POPC0   4      13.619   2.625  15.608  0.00  0.00            
+ATOM     44  C1A POPC0   4      10.821  -0.530  12.866  0.00  0.00            
+ATOM     45  D2A POPC0   4       9.049   1.926   9.049  0.00  0.00            
+ATOM     46  C3A POPC0   4       4.959   1.648   6.085  0.00  0.00            
+ATOM     47  C4A POPC0   4       2.370   0.665   2.978  0.00  0.00            
+ATOM     48  C1B POPC0   4      14.465   2.350  11.464  0.00  0.00            
+ATOM     49  C2B POPC0   4      13.755   0.441   7.589  0.00  0.00            
+ATOM     50  C3B POPC0   4      13.750  -0.562   3.847  0.00  0.00            
+ATOM     51  C4B POPC0   4      12.143  -0.269  -0.410  0.00  0.00            
+ATOM     52  NC3 POPC0   5      -1.371   3.959  24.490  0.00  0.00            
+ATOM     53  PO4 POPC0   5      -4.346   2.099  22.091  0.00  0.00            
+ATOM     54  GL1 POPC0   5      -4.829   6.133  19.249  0.00  0.00            
+ATOM     55  GL2 POPC0   5      -3.616   8.744  17.024  0.00  0.00            
+ATOM     56  C1A POPC0   5      -6.516   5.625  14.225  0.00  0.00            
+ATOM     57  D2A POPC0   5      -3.836   8.655  11.785  0.00  0.00            
+ATOM     58  C3A POPC0   5      -3.229   8.614   7.477  0.00  0.00            
+ATOM     59  C4A POPC0   5      -5.390   7.487   3.250  0.00  0.00            
+ATOM     60  C1B POPC0   5      -1.710   5.403  14.896  0.00  0.00            
+ATOM     61  C2B POPC0   5      -2.717   3.778  10.620  0.00  0.00            
+ATOM     62  C3B POPC0   5      -4.154   3.115   6.100  0.00  0.00            
+ATOM     63  C4B POPC0   5      -7.276   3.211   2.352  0.00  0.00            
+ATOM     64  NC3 POPC0   6      -7.761  -1.291  23.727  0.00  0.00            
+ATOM     65  PO4 POPC0   6     -11.744  -0.545  22.590  0.00  0.00            
+ATOM     66  GL1 POPC0   6      -9.406  -1.810  18.651  0.00  0.00            
+ATOM     67  GL2 POPC0   6      -9.016   1.526  18.315  0.00  0.00            
+ATOM     68  C1A POPC0   6     -10.361  -4.957  17.244  0.00  0.00            
+ATOM     69  D2A POPC0   6     -12.619  -5.901  13.287  0.00  0.00            
+ATOM     70  C3A POPC0   6     -12.214  -8.727  10.010  0.00  0.00            
+ATOM     71  C4A POPC0   6     -10.191  -8.730   5.048  0.00  0.00            
+ATOM     72  C1B POPC0   6      -4.912   0.838  15.662  0.00  0.00            
+ATOM     73  C2B POPC0   6      -5.405  -3.955  14.566  0.00  0.00            
+ATOM     74  C3B POPC0   6      -7.230  -5.028  11.532  0.00  0.00            
+ATOM     75  C4B POPC0   6      -9.191  -4.989   9.325  0.00  0.00            
+ATOM     76  NC3 POPC0   7      -8.732   9.775  21.898  0.00  0.00            
+ATOM     77  PO4 POPC0   7     -12.839   7.687  21.128  0.00  0.00            
+ATOM     78  GL1 POPC0   7     -14.421  10.008  16.841  0.00  0.00            
+ATOM     79  GL2 POPC0   7     -16.712  12.979  16.410  0.00  0.00            
+ATOM     80  C1A POPC0   7     -12.693   8.869  12.920  0.00  0.00            
+ATOM     81  D2A POPC0   7     -13.828   9.224   8.784  0.00  0.00            
+ATOM     82  C3A POPC0   7     -11.774   9.283   5.047  0.00  0.00            
+ATOM     83  C4A POPC0   7      -8.963  10.172   1.609  0.00  0.00            
+ATOM     84  C1B POPC0   7     -19.063  15.232  13.062  0.00  0.00            
+ATOM     85  C2B POPC0   7     -20.108  19.168  10.336  0.00  0.00            
+ATOM     86  C3B POPC0   7     -18.896  20.972   6.797  0.00  0.00            
+ATOM     87  C4B POPC0   7     -17.629  24.110   2.882  0.00  0.00            
+ATOM     88  NC3 POPC0   8       4.573  -4.294  22.001  0.00  0.00            
+ATOM     89  PO4 POPC0   8      -0.401  -5.312  20.945  0.00  0.00            
+ATOM     90  GL1 POPC0   8      -0.303  -7.275  16.963  0.00  0.00            
+ATOM     91  GL2 POPC0   8      -3.901  -8.506  15.656  0.00  0.00            
+ATOM     92  C1A POPC0   8       2.977  -9.099  13.020  0.00  0.00            
+ATOM     93  D2A POPC0   8       6.069 -12.252  10.311  0.00  0.00            
+ATOM     94  C3A POPC0   8       4.895 -14.561   6.132  0.00  0.00            
+ATOM     95  C4A POPC0   8       1.033 -15.526   5.920  0.00  0.00            
+ATOM     96  C1B POPC0   8      -2.175  -8.226  11.481  0.00  0.00            
+ATOM     97  C2B POPC0   8      -3.159 -11.507   8.157  0.00  0.00            
+ATOM     98  C3B POPC0   8      -1.365 -10.915   3.788  0.00  0.00            
+ATOM     99  C4B POPC0   8       2.356 -13.067   1.914  0.00  0.00            
+ATOM    100  NC3 POPC0   9       5.139   9.571  22.353  0.00  0.00            
+ATOM    101  PO4 POPC0   9       2.775   7.655  19.165  0.00  0.00            
+ATOM    102  GL1 POPC0   9       2.402   8.487  15.479  0.00  0.00            
+ATOM    103  GL2 POPC0   9       3.136   5.723  13.502  0.00  0.00            
+ATOM    104  C1A POPC0   9       3.584  10.999  12.305  0.00  0.00            
+ATOM    105  D2A POPC0   9       5.253  12.870   7.565  0.00  0.00            
+ATOM    106  C3A POPC0   9       4.220  12.530   3.371  0.00  0.00            
+ATOM    107  C4A POPC0   9       1.886  13.699  -0.584  0.00  0.00            
+ATOM    108  C1B POPC0   9       0.726   7.476  10.061  0.00  0.00            
+ATOM    109  C2B POPC0   9       0.555  11.453   7.367  0.00  0.00            
+ATOM    110  C3B POPC0   9      -0.907  11.652   3.313  0.00  0.00            
+ATOM    111  C4B POPC0   9      -2.405   9.300  -0.597  0.00  0.00            
+ATOM    112  NC3 POPC0  10     -21.704 -15.736  21.269  0.00  0.00            
+ATOM    113  PO4 POPC0  10     -18.636 -19.094  20.744  0.00  0.00            
+ATOM    114  GL1 POPC0  10     -19.008 -17.559  15.876  0.00  0.00            
+ATOM    115  GL2 POPC0  10     -17.523 -14.952  16.877  0.00  0.00            
+ATOM    116  C1A POPC0  10     -15.219 -17.306  13.195  0.00  0.00            
+ATOM    117  D2A POPC0  10     -13.917 -18.246   9.345  0.00  0.00            
+ATOM    118  C3A POPC0  10     -16.832 -20.726   6.186  0.00  0.00            
+ATOM    119  C4A POPC0  10     -21.764 -20.979   7.549  0.00  0.00            
+ATOM    120  C1B POPC0  10     -18.077 -13.255  12.422  0.00  0.00            
+ATOM    121  C2B POPC0  10     -16.960 -11.360   8.856  0.00  0.00            
+ATOM    122  C3B POPC0  10     -14.169 -12.089   6.278  0.00  0.00            
+ATOM    123  C4B POPC0  10     -12.162 -12.475   2.152  0.00  0.00            
+ATOM    124  GL1 TRIO0  11     -17.594   1.961  16.912  0.00  0.00            
+ATOM    125  C1A TRIO0  11     -17.530   2.042  12.427  0.00  0.00            
+ATOM    126  D2A TRIO0  11     -18.477   1.649   8.066  0.00  0.00            
+ATOM    127  C3A TRIO0  11     -18.412  -1.635   5.857  0.00  0.00            
+ATOM    128  C4A TRIO0  11     -18.699  -3.763   2.585  0.00  0.00            
+ATOM    129  GL2 TRIO0  11     -15.057   4.875  15.803  0.00  0.00            
+ATOM    130  C1B TRIO0  11     -13.102   0.739  15.654  0.00  0.00            
+ATOM    131  D2B TRIO0  11      -9.850  -0.906  13.320  0.00  0.00            
+ATOM    132  C3B TRIO0  11      -8.308   1.085  10.881  0.00  0.00            
+ATOM    133  C4B TRIO0  11      -7.832   5.705   9.019  0.00  0.00            
+ATOM    134  GL3 TRIO0  11     -11.362   5.099  15.876  0.00  0.00            
+ATOM    135  C1C TRIO0  11     -11.727   4.314  12.346  0.00  0.00            
+ATOM    136  D2C TRIO0  11     -12.789   1.303   8.957  0.00  0.00            
+ATOM    137  C3C TRIO0  11     -13.924   0.830   4.489  0.00  0.00            
+ATOM    138  C4C TRIO0  11     -17.572   1.087   1.849  0.00  0.00            
+ATOM    139  NC3 POPC0  12     -18.142   7.392  23.100  0.00  0.00            
+ATOM    140  PO4 POPC0  12     -18.941   6.218  19.402  0.00  0.00            
+ATOM    141  GL1 POPC0  12     -19.001   8.240  15.972  0.00  0.00            
+ATOM    142  GL2 POPC0  12     -20.531   6.317  13.787  0.00  0.00            
+ATOM    143  C1A POPC0  12     -17.526   9.848  12.392  0.00  0.00            
+ATOM    144  D2A POPC0  12     -18.082  12.061   8.496  0.00  0.00            
+ATOM    145  C3A POPC0  12     -16.399  10.676   4.280  0.00  0.00            
+ATOM    146  C4A POPC0  12     -16.857   7.224   1.668  0.00  0.00            
+ATOM    147  C1B POPC0  12     -18.233   6.543   9.240  0.00  0.00            
+ATOM    148  C2B POPC0  12     -15.202   5.137   6.681  0.00  0.00            
+ATOM    149  C3B POPC0  12     -10.684   4.744   5.409  0.00  0.00            
+ATOM    150  C4B POPC0  12      -8.480   0.433   5.948  0.00  0.00            
+ATOM    151  NC3 POPC0  13      -7.948 -14.733  26.481  0.00  0.00            
+ATOM    152  PO4 POPC0  13     -11.287 -13.659  22.721  0.00  0.00            
+ATOM    153  GL1 POPC0  13     -11.534 -15.635  18.229  0.00  0.00            
+ATOM    154  GL2 POPC0  13      -9.689 -17.652  16.262  0.00  0.00            
+ATOM    155  C1A POPC0  13     -11.578 -12.411  14.958  0.00  0.00            
+ATOM    156  D2A POPC0  13     -11.599 -13.815  10.257  0.00  0.00            
+ATOM    157  C3A POPC0  13      -7.865 -13.834   8.280  0.00  0.00            
+ATOM    158  C4A POPC0  13      -6.653 -12.101   4.327  0.00  0.00            
+ATOM    159  C1B POPC0  13      -8.648 -17.498  12.839  0.00  0.00            
+ATOM    160  C2B POPC0  13      -8.640 -18.759   8.276  0.00  0.00            
+ATOM    161  C3B POPC0  13     -11.407 -18.171   4.855  0.00  0.00            
+ATOM    162  C4B POPC0  13     -14.471 -16.747   3.769  0.00  0.00            
+ATOM    163  NC3 POPC0  14      -0.873   8.626  22.343  0.00  0.00            
+ATOM    164  PO4 POPC0  14      -4.388  11.775  21.324  0.00  0.00            
+ATOM    165  GL1 POPC0  14      -3.862  13.923  18.087  0.00  0.00            
+ATOM    166  GL2 POPC0  14      -4.279  17.992  17.147  0.00  0.00            
+ATOM    167  C1A POPC0  14      -2.468  13.120  14.169  0.00  0.00            
+ATOM    168  D2A POPC0  14      -5.470  13.729  10.565  0.00  0.00            
+ATOM    169  C3A POPC0  14      -3.157  14.703   7.753  0.00  0.00            
+ATOM    170  C4A POPC0  14      -0.035  16.976   4.836  0.00  0.00            
+ATOM    171  C1B POPC0  14      -2.867  18.269  12.980  0.00  0.00            
+ATOM    172  C2B POPC0  14      -3.014  20.017   9.072  0.00  0.00            
+ATOM    173  C3B POPC0  14      -4.489  19.781   4.910  0.00  0.00            
+ATOM    174  C4B POPC0  14      -4.072  21.825   1.376  0.00  0.00            
+ATOM    175  NC3 POPC0  15       8.656  -9.629  28.492  0.00  0.00            
+ATOM    176  PO4 POPC0  15       8.351  -9.368  23.709  0.00  0.00            
+ATOM    177  GL1 POPC0  15       8.652 -11.207  19.716  0.00  0.00            
+ATOM    178  GL2 POPC0  15      11.543 -12.988  18.496  0.00  0.00            
+ATOM    179  C1A POPC0  15       6.330 -11.683  16.262  0.00  0.00            
+ATOM    180  D2A POPC0  15       4.825 -15.422  14.446  0.00  0.00            
+ATOM    181  C3A POPC0  15       1.680 -17.629  13.437  0.00  0.00            
+ATOM    182  C4A POPC0  15       1.035 -21.094  10.395  0.00  0.00            
+ATOM    183  C1B POPC0  15      10.799 -10.619  14.814  0.00  0.00            
+ATOM    184  C2B POPC0  15       7.811  -7.694  13.753  0.00  0.00            
+ATOM    185  C3B POPC0  15       6.103  -7.205   8.799  0.00  0.00            
+ATOM    186  C4B POPC0  15       7.364  -6.439   5.609  0.00  0.00            
+ATOM    187  NC3 POPC0  16      11.982   1.554  22.124  0.00  0.00            
+ATOM    188  PO4 POPC0  16      13.614  -1.121  20.043  0.00  0.00            
+ATOM    189  GL1 POPC0  16      15.546  -2.449  16.573  0.00  0.00            
+ATOM    190  GL2 POPC0  16      14.892  -6.615  16.150  0.00  0.00            
+ATOM    191  C1A POPC0  16      15.938  -2.597  11.864  0.00  0.00            
+ATOM    192  D2A POPC0  16      15.042  -5.756   8.067  0.00  0.00            
+ATOM    193  C3A POPC0  16      12.476  -5.618   4.447  0.00  0.00            
+ATOM    194  C4A POPC0  16      10.271  -9.406   2.095  0.00  0.00            
+ATOM    195  C1B POPC0  16      11.907  -5.541  12.684  0.00  0.00            
+ATOM    196  C2B POPC0  16      10.436  -3.719   8.807  0.00  0.00            
+ATOM    197  C3B POPC0  16       8.706  -1.416   5.114  0.00  0.00            
+ATOM    198  C4B POPC0  16       7.641   1.246   1.650  0.00  0.00            
+ATOM    199  NC3 POPC0  17     -14.775   2.998  20.796  0.00  0.00            
+ATOM    200  PO4 POPC0  17     -17.180  -1.788  20.895  0.00  0.00            
+ATOM    201  GL1 POPC0  17     -15.762  -3.343  16.504  0.00  0.00            
+ATOM    202  GL2 POPC0  17     -17.253  -6.256  15.128  0.00  0.00            
+ATOM    203  C1A POPC0  17     -15.645  -2.362  11.828  0.00  0.00            
+ATOM    204  D2A POPC0  17     -13.984  -4.609   8.726  0.00  0.00            
+ATOM    205  C3A POPC0  17     -12.630  -3.873   4.955  0.00  0.00            
+ATOM    206  C4A POPC0  17      -8.524  -4.395   4.100  0.00  0.00            
+ATOM    207  C1B POPC0  17     -17.846  -6.690  11.131  0.00  0.00            
+ATOM    208  C2B POPC0  17     -17.759  -7.419   5.824  0.00  0.00            
+ATOM    209  C3B POPC0  17     -14.858  -7.539   2.746  0.00  0.00            
+ATOM    210  C4B POPC0  17     -10.975  -6.627  -0.095  0.00  0.00            
+ATOM    211  NC3 POPC0  18      12.879   5.888  19.088  0.00  0.00            
+ATOM    212  PO4 POPC0  18       8.389   5.469  20.560  0.00  0.00            
+ATOM    213  GL1 POPC0  18       8.507   5.979  16.326  0.00  0.00            
+ATOM    214  GL2 POPC0  18       7.455   8.361  15.075  0.00  0.00            
+ATOM    215  C1A POPC0  18      10.741   5.470  11.593  0.00  0.00            
+ATOM    216  D2A POPC0  18      12.690   5.465   7.816  0.00  0.00            
+ATOM    217  C3A POPC0  18       9.624   4.593   4.613  0.00  0.00            
+ATOM    218  C4A POPC0  18      10.698   5.340   0.189  0.00  0.00            
+ATOM    219  C1B POPC0  18       8.447  10.352  11.608  0.00  0.00            
+ATOM    220  C2B POPC0  18       8.992   9.397   7.257  0.00  0.00            
+ATOM    221  C3B POPC0  18      12.416   9.890   2.901  0.00  0.00            
+ATOM    222  C4B POPC0  18      15.827  10.218  -1.259  0.00  0.00            
+ATOM    223  NC3 POPC0  19       5.873  18.467  20.207  0.00  0.00            
+ATOM    224  PO4 POPC0  19      10.116  20.025  21.955  0.00  0.00            
+ATOM    225  GL1 POPC0  19      10.315  18.948  16.871  0.00  0.00            
+ATOM    226  GL2 POPC0  19      13.417  16.786  16.442  0.00  0.00            
+ATOM    227  C1A POPC0  19       9.810  20.147  12.247  0.00  0.00            
+ATOM    228  D2A POPC0  19       9.821  20.070   7.349  0.00  0.00            
+ATOM    229  C3A POPC0  19      12.409  21.766   4.410  0.00  0.00            
+ATOM    230  C4A POPC0  19      13.428  19.474   0.774  0.00  0.00            
+ATOM    231  C1B POPC0  19      12.364  16.005  12.688  0.00  0.00            
+ATOM    232  C2B POPC0  19       9.464  15.224  10.062  0.00  0.00            
+ATOM    233  C3B POPC0  19      10.252  15.011   4.965  0.00  0.00            
+ATOM    234  C4B POPC0  19      14.038  14.649   2.773  0.00  0.00            
+ATOM    235  NC3 POPC0  20      -7.107  16.923  25.200  0.00  0.00            
+ATOM    236  PO4 POPC0  20      -8.163  15.190  20.729  0.00  0.00            
+ATOM    237  GL1 POPC0  20      -9.757  13.472  17.346  0.00  0.00            
+ATOM    238  GL2 POPC0  20      -8.532  10.264  16.901  0.00  0.00            
+ATOM    239  C1A POPC0  20     -11.235  14.677  14.086  0.00  0.00            
+ATOM    240  D2A POPC0  20     -14.457  13.476  11.754  0.00  0.00            
+ATOM    241  C3A POPC0  20     -12.523  14.386   7.859  0.00  0.00            
+ATOM    242  C4A POPC0  20     -12.648  14.456   3.335  0.00  0.00            
+ATOM    243  C1B POPC0  20      -7.822  10.992  13.452  0.00  0.00            
+ATOM    244  C2B POPC0  20      -8.882  10.841   8.686  0.00  0.00            
+ATOM    245  C3B POPC0  20      -7.290  13.812   5.591  0.00  0.00            
+ATOM    246  C4B POPC0  20      -7.275  16.377   2.112  0.00  0.00            
+ATOM    247  NC3 POPC0  21       0.188  12.436  19.808  0.00  0.00            
+ATOM    248  PO4 POPC0  21       3.469  14.426  22.012  0.00  0.00            
+ATOM    249  GL1 POPC0  21       5.714  12.527  17.674  0.00  0.00            
+ATOM    250  GL2 POPC0  21       2.486  13.938  15.866  0.00  0.00            
+ATOM    251  C1A POPC0  21       9.672  13.347  15.921  0.00  0.00            
+ATOM    252  D2A POPC0  21      12.457  10.465  14.246  0.00  0.00            
+ATOM    253  C3A POPC0  21      14.102  10.048  10.424  0.00  0.00            
+ATOM    254  C4A POPC0  21      15.478   9.191   6.600  0.00  0.00            
+ATOM    255  C1B POPC0  21       5.504  15.887  13.513  0.00  0.00            
+ATOM    256  C2B POPC0  21       5.356  18.185  10.094  0.00  0.00            
+ATOM    257  C3B POPC0  21       5.121  17.599   5.912  0.00  0.00            
+ATOM    258  C4B POPC0  21       6.731  17.452   2.434  0.00  0.00            
+ATOM    259  NC3 POPC0  22      21.188 -15.469  21.989  0.00  0.00            
+ATOM    260  PO4 POPC0  22      17.771 -11.625  20.306  0.00  0.00            
+ATOM    261  GL1 POPC0  22      15.364 -11.823  15.581  0.00  0.00            
+ATOM    262  GL2 POPC0  22      13.797 -14.959  13.853  0.00  0.00            
+ATOM    263  C1A POPC0  22      14.778  -9.368  11.500  0.00  0.00            
+ATOM    264  D2A POPC0  22      10.610  -8.957   9.455  0.00  0.00            
+ATOM    265  C3A POPC0  22       9.337 -11.680   6.034  0.00  0.00            
+ATOM    266  C4A POPC0  22       7.437 -13.492   2.018  0.00  0.00            
+ATOM    267  C1B POPC0  22      13.764 -13.724   8.818  0.00  0.00            
+ATOM    268  C2B POPC0  22      14.278 -10.869   5.351  0.00  0.00            
+ATOM    269  C3B POPC0  22      15.802  -9.024   2.921  0.00  0.00            
+ATOM    270  C4B POPC0  22      18.283  -8.092  -0.354  0.00  0.00            
+ATOM    271  NC3 POPC1   1       7.670  11.311 -23.173  0.00  0.00            
+ATOM    272  PO4 POPC1   1       5.612   6.809 -21.427  0.00  0.00            
+ATOM    273  GL1 POPC1   1       5.841   3.712 -19.733  0.00  0.00            
+ATOM    274  GL2 POPC1   1       3.679   0.808 -18.255  0.00  0.00            
+ATOM    275  C1A POPC1   1       7.606   4.424 -15.654  0.00  0.00            
+ATOM    276  D2A POPC1   1      11.136   3.839 -12.882  0.00  0.00            
+ATOM    277  C3A POPC1   1      11.466   5.426  -8.212  0.00  0.00            
+ATOM    278  C4A POPC1   1      12.522   6.890  -4.809  0.00  0.00            
+ATOM    279  C1B POPC1   1       3.241   2.286 -14.532  0.00  0.00            
+ATOM    280  C2B POPC1   1       3.189   2.749 -10.139  0.00  0.00            
+ATOM    281  C3B POPC1   1       3.180   4.907  -5.424  0.00  0.00            
+ATOM    282  C4B POPC1   1       3.204   3.287  -0.893  0.00  0.00            
+ATOM    283  NC3 POPC1   2      -3.712  -3.663 -23.729  0.00  0.00            
+ATOM    284  PO4 POPC1   2      -6.268  -5.648 -21.938  0.00  0.00            
+ATOM    285  GL1 POPC1   2      -4.546  -4.809 -18.888  0.00  0.00            
+ATOM    286  GL2 POPC1   2      -6.141  -6.540 -16.542  0.00  0.00            
+ATOM    287  C1A POPC1   2      -3.871  -1.250 -15.425  0.00  0.00            
+ATOM    288  D2A POPC1   2      -3.905  -1.122 -11.215  0.00  0.00            
+ATOM    289  C3A POPC1   2      -4.087  -5.344  -9.315  0.00  0.00            
+ATOM    290  C4A POPC1   2      -5.208  -9.116  -7.875  0.00  0.00            
+ATOM    291  C1B POPC1   2      -1.606  -6.313 -14.046  0.00  0.00            
+ATOM    292  C2B POPC1   2       0.203  -8.564 -11.146  0.00  0.00            
+ATOM    293  C3B POPC1   2       0.693  -9.730  -7.075  0.00  0.00            
+ATOM    294  C4B POPC1   2       3.328  -7.540  -3.576  0.00  0.00            
+ATOM    295  NC3 POPC1   3       7.793  -5.991 -20.811  0.00  0.00            
+ATOM    296  PO4 POPC1   3       4.411  -3.724 -20.946  0.00  0.00            
+ATOM    297  GL1 POPC1   3       7.340  -3.554 -16.579  0.00  0.00            
+ATOM    298  GL2 POPC1   3       9.194  -5.147 -16.383  0.00  0.00            
+ATOM    299  C1A POPC1   3       6.265  -0.523 -12.611  0.00  0.00            
+ATOM    300  D2A POPC1   3       4.682  -1.397  -7.867  0.00  0.00            
+ATOM    301  C3A POPC1   3       0.982   0.583  -6.392  0.00  0.00            
+ATOM    302  C4A POPC1   3      -1.073   0.578  -2.510  0.00  0.00            
+ATOM    303  C1B POPC1   3       9.153  -7.893 -13.022  0.00  0.00            
+ATOM    304  C2B POPC1   3       9.456 -10.806 -10.579  0.00  0.00            
+ATOM    305  C3B POPC1   3       9.951 -15.810 -10.327  0.00  0.00            
+ATOM    306  C4B POPC1   3       8.632 -19.699 -11.766  0.00  0.00            
+ATOM    307  NC3 POPC1   4      16.374  -9.646 -22.074  0.00  0.00            
+ATOM    308  PO4 POPC1   4      12.882  -6.630 -20.332  0.00  0.00            
+ATOM    309  GL1 POPC1   4      13.796  -7.418 -16.282  0.00  0.00            
+ATOM    310  GL2 POPC1   4      14.246  -4.567 -15.126  0.00  0.00            
+ATOM    311  C1A POPC1   4      13.486  -7.249 -11.429  0.00  0.00            
+ATOM    312  D2A POPC1   4      11.480  -6.485  -7.310  0.00  0.00            
+ATOM    313  C3A POPC1   4       8.394  -8.905  -3.987  0.00  0.00            
+ATOM    314  C4A POPC1   4       5.800 -12.005  -2.418  0.00  0.00            
+ATOM    315  C1B POPC1   4      10.515  -3.203 -11.931  0.00  0.00            
+ATOM    316  C2B POPC1   4       9.523  -1.871  -8.925  0.00  0.00            
+ATOM    317  C3B POPC1   4       7.848   2.395  -7.689  0.00  0.00            
+ATOM    318  C4B POPC1   4       9.152   2.347  -4.389  0.00  0.00            
+ATOM    319  NC3 POPC1   5      -3.146   5.547 -22.991  0.00  0.00            
+ATOM    320  PO4 POPC1   5      -3.102   8.774 -20.321  0.00  0.00            
+ATOM    321  GL1 POPC1   5      -2.262   8.012 -16.888  0.00  0.00            
+ATOM    322  GL2 POPC1   5      -0.269  11.083 -16.558  0.00  0.00            
+ATOM    323  C1A POPC1   5      -5.526   6.052 -13.501  0.00  0.00            
+ATOM    324  D2A POPC1   5      -6.808   3.656  -9.762  0.00  0.00            
+ATOM    325  C3A POPC1   5      -4.228   0.978  -6.829  0.00  0.00            
+ATOM    326  C4A POPC1   5      -4.732  -3.345  -4.890  0.00  0.00            
+ATOM    327  C1B POPC1   5      -1.206  10.207 -12.327  0.00  0.00            
+ATOM    328  C2B POPC1   5      -1.242  12.625  -7.901  0.00  0.00            
+ATOM    329  C3B POPC1   5      -1.923  13.147  -3.889  0.00  0.00            
+ATOM    330  C4B POPC1   5      -3.321  14.488  -0.245  0.00  0.00            
+ATOM    331  NC3 POPC1   6      -0.208  -6.193 -21.354  0.00  0.00            
+ATOM    332  PO4 POPC1   6       2.973  -8.220 -21.748  0.00  0.00            
+ATOM    333  GL1 POPC1   6       3.162  -6.741 -17.144  0.00  0.00            
+ATOM    334  GL2 POPC1   6       1.902  -3.518 -16.523  0.00  0.00            
+ATOM    335  C1A POPC1   6       4.588  -5.917 -12.717  0.00  0.00            
+ATOM    336  D2A POPC1   6       6.785  -6.428  -8.622  0.00  0.00            
+ATOM    337  C3A POPC1   6       7.385  -4.033  -4.498  0.00  0.00            
+ATOM    338  C4A POPC1   6       5.501  -0.974  -2.640  0.00  0.00            
+ATOM    339  C1B POPC1   6       1.376  -2.266 -11.794  0.00  0.00            
+ATOM    340  C2B POPC1   6       0.442  -4.384  -7.053  0.00  0.00            
+ATOM    341  C3B POPC1   6      -2.340  -7.563  -3.614  0.00  0.00            
+ATOM    342  C4B POPC1   6      -0.511 -11.496  -1.753  0.00  0.00            
+ATOM    343  NC3 POPC1   7      -8.463   8.868 -18.816  0.00  0.00            
+ATOM    344  PO4 POPC1   7      -6.218  12.407 -21.613  0.00  0.00            
+ATOM    345  GL1 POPC1   7      -5.757  12.664 -16.768  0.00  0.00            
+ATOM    346  GL2 POPC1   7      -7.358  10.798 -14.343  0.00  0.00            
+ATOM    347  C1A POPC1   7      -4.484  14.458 -12.897  0.00  0.00            
+ATOM    348  D2A POPC1   7      -0.832  16.868 -11.441  0.00  0.00            
+ATOM    349  C3A POPC1   7      -0.689  18.912  -8.301  0.00  0.00            
+ATOM    350  C4A POPC1   7       1.637  21.394  -5.059  0.00  0.00            
+ATOM    351  C1B POPC1   7      -5.819   9.635  -9.781  0.00  0.00            
+ATOM    352  C2B POPC1   7      -6.016   7.947  -6.121  0.00  0.00            
+ATOM    353  C3B POPC1   7      -7.475   6.737  -2.335  0.00  0.00            
+ATOM    354  C4B POPC1   7     -10.981   5.895   0.586  0.00  0.00            
+ATOM    355  NC3 POPC1   8      19.252  -5.446 -26.095  0.00  0.00            
+ATOM    356  PO4 POPC1   8      21.536  -7.486 -21.726  0.00  0.00            
+ATOM    357  GL1 POPC1   8      18.664  -7.904 -17.897  0.00  0.00            
+ATOM    358  GL2 POPC1   8      17.436 -10.892 -15.977  0.00  0.00            
+ATOM    359  C1A POPC1   8      18.717  -5.256 -12.639  0.00  0.00            
+ATOM    360  D2A POPC1   8      16.183  -3.231 -10.484  0.00  0.00            
+ATOM    361  C3A POPC1   8      14.770  -3.196  -7.043  0.00  0.00            
+ATOM    362  C4A POPC1   8      11.967  -2.654  -4.419  0.00  0.00            
+ATOM    363  C1B POPC1   8      17.509 -10.897 -11.690  0.00  0.00            
+ATOM    364  C2B POPC1   8      16.912  -7.756  -8.033  0.00  0.00            
+ATOM    365  C3B POPC1   8      15.751  -8.029  -4.432  0.00  0.00            
+ATOM    366  C4B POPC1   8      13.363  -6.060  -0.494  0.00  0.00            
+ATOM    367  NC3 POPC1   9       4.767   3.129 -25.574  0.00  0.00            
+ATOM    368  PO4 POPC1   9       1.370   5.179 -24.399  0.00  0.00            
+ATOM    369  GL1 POPC1   9       0.768   4.690 -19.662  0.00  0.00            
+ATOM    370  GL2 POPC1   9       2.574   6.651 -17.148  0.00  0.00            
+ATOM    371  C1A POPC1   9      -1.522   3.365 -15.814  0.00  0.00            
+ATOM    372  D2A POPC1   9      -1.213   2.928 -11.878  0.00  0.00            
+ATOM    373  C3A POPC1   9      -2.200   5.881  -9.271  0.00  0.00            
+ATOM    374  C4A POPC1   9      -1.459   6.155  -4.736  0.00  0.00            
+ATOM    375  C1B POPC1   9       2.627   7.221 -13.388  0.00  0.00            
+ATOM    376  C2B POPC1   9       2.405   9.601  -9.010  0.00  0.00            
+ATOM    377  C3B POPC1   9       1.933   9.553  -4.691  0.00  0.00            
+ATOM    378  C4B POPC1   9       2.667   8.606  -0.744  0.00  0.00            
+ATOM    379  NC3 POPC1  10      -9.862 -11.357 -21.912  0.00  0.00            
+ATOM    380  PO4 POPC1  10     -12.288 -15.622 -21.480  0.00  0.00            
+ATOM    381  GL1 POPC1  10     -10.050 -14.213 -17.292  0.00  0.00            
+ATOM    382  GL2 POPC1  10      -9.340 -10.594 -16.170  0.00  0.00            
+ATOM    383  C1A POPC1  10     -10.342 -15.419 -12.681  0.00  0.00            
+ATOM    384  D2A POPC1  10      -8.830 -14.900  -8.828  0.00  0.00            
+ATOM    385  C3A POPC1  10      -9.251 -12.602  -5.946  0.00  0.00            
+ATOM    386  C4A POPC1  10      -8.694  -9.903  -2.751  0.00  0.00            
+ATOM    387  C1B POPC1  10     -10.202 -10.791 -12.026  0.00  0.00            
+ATOM    388  C2B POPC1  10     -10.415  -7.411  -8.635  0.00  0.00            
+ATOM    389  C3B POPC1  10     -10.566  -5.782  -5.187  0.00  0.00            
+ATOM    390  C4B POPC1  10      -9.039  -2.353  -2.598  0.00  0.00            
+ATOM    391  GL1 TRIO1  11      -8.741   2.107 -15.493  0.00  0.00            
+ATOM    392  C1A TRIO1  11      -8.579  -0.908 -12.314  0.00  0.00            
+ATOM    393  D2A TRIO1  11      -8.161  -1.851  -8.031  0.00  0.00            
+ATOM    394  C3A TRIO1  11     -12.369  -0.927  -6.606  0.00  0.00            
+ATOM    395  C4A TRIO1  11     -12.965   0.588  -2.582  0.00  0.00            
+ATOM    396  GL2 TRIO1  11     -11.622   1.738 -14.639  0.00  0.00            
+ATOM    397  C1B TRIO1  11     -11.867   2.663 -10.489  0.00  0.00            
+ATOM    398  D2B TRIO1  11     -11.035   5.307  -6.953  0.00  0.00            
+ATOM    399  C3B TRIO1  11      -9.200   2.248  -4.808  0.00  0.00            
+ATOM    400  C4B TRIO1  11      -6.028   1.431  -2.056  0.00  0.00            
+ATOM    401  GL3 TRIO1  11     -13.156  -1.052 -13.841  0.00  0.00            
+ATOM    402  C1C TRIO1  11     -13.496  -3.251 -10.518  0.00  0.00            
+ATOM    403  D2C TRIO1  11     -16.759  -2.895  -7.338  0.00  0.00            
+ATOM    404  C3C TRIO1  11     -16.430  -4.892  -3.805  0.00  0.00            
+ATOM    405  C4C TRIO1  11     -14.689  -3.190  -0.076  0.00  0.00            
+ATOM    406  NC3 POPC1  12     -12.607   0.335 -19.419  0.00  0.00            
+ATOM    407  PO4 POPC1  12     -10.752   4.413 -19.343  0.00  0.00            
+ATOM    408  GL1 POPC1  12     -11.714   6.650 -15.531  0.00  0.00            
+ATOM    409  GL2 POPC1  12     -13.149   9.083 -15.505  0.00  0.00            
+ATOM    410  C1A POPC1  12     -10.643   7.762 -11.154  0.00  0.00            
+ATOM    411  D2A POPC1  12     -11.349  10.000  -7.863  0.00  0.00            
+ATOM    412  C3A POPC1  12     -10.924   9.397  -3.919  0.00  0.00            
+ATOM    413  C4A POPC1  12     -13.407  10.267  -0.539  0.00  0.00            
+ATOM    414  C1B POPC1  12     -13.241  12.619 -12.410  0.00  0.00            
+ATOM    415  C2B POPC1  12     -15.231  14.021  -8.438  0.00  0.00            
+ATOM    416  C3B POPC1  12     -13.418  15.396  -5.053  0.00  0.00            
+ATOM    417  C4B POPC1  12     -10.949  15.226  -1.324  0.00  0.00            
+ATOM    418  NC3 POPC1  13      -4.667 -19.403 -22.302  0.00  0.00            
+ATOM    419  PO4 POPC1  13       0.182 -17.735 -22.416  0.00  0.00            
+ATOM    420  GL1 POPC1  13      -0.448 -14.889 -18.946  0.00  0.00            
+ATOM    421  GL2 POPC1  13       2.414 -13.258 -19.494  0.00  0.00            
+ATOM    422  C1A POPC1  13      -0.897 -11.990 -16.146  0.00  0.00            
+ATOM    423  D2A POPC1  13      -3.893 -10.853 -12.677  0.00  0.00            
+ATOM    424  C3A POPC1  13      -6.912  -7.700 -12.188  0.00  0.00            
+ATOM    425  C4A POPC1  13     -10.491  -5.516 -13.915  0.00  0.00            
+ATOM    426  C1B POPC1  13       3.002 -15.230 -14.979  0.00  0.00            
+ATOM    427  C2B POPC1  13      -0.359 -13.996 -11.003  0.00  0.00            
+ATOM    428  C3B POPC1  13      -3.493 -14.257  -8.194  0.00  0.00            
+ATOM    429  C4B POPC1  13      -4.468 -12.763  -4.099  0.00  0.00            
+ATOM    430  NC3 POPC1  14       5.117 -16.812 -21.319  0.00  0.00            
+ATOM    431  PO4 POPC1  14       9.826 -15.502 -21.797  0.00  0.00            
+ATOM    432  GL1 POPC1  14      11.935 -12.840 -18.035  0.00  0.00            
+ATOM    433  GL2 POPC1  14       9.842  -9.955 -17.728  0.00  0.00            
+ATOM    434  C1A POPC1  14      12.734 -12.720 -13.765  0.00  0.00            
+ATOM    435  D2A POPC1  14      13.776 -11.438  -8.522  0.00  0.00            
+ATOM    436  C3A POPC1  14      17.277 -12.740  -5.324  0.00  0.00            
+ATOM    437  C4A POPC1  14      18.769 -12.758  -1.911  0.00  0.00            
+ATOM    438  C1B POPC1  14       6.065 -10.920 -15.993  0.00  0.00            
+ATOM    439  C2B POPC1  14       3.918 -11.394 -12.481  0.00  0.00            
+ATOM    440  C3B POPC1  14       5.249 -11.868  -7.699  0.00  0.00            
+ATOM    441  C4B POPC1  14       9.746 -13.156  -6.067  0.00  0.00            
+ATOM    442  NC3 POPC1  15     -20.754 -25.442 -22.586  0.00  0.00            
+ATOM    443  PO4 POPC1  15     -20.386 -21.763 -19.456  0.00  0.00            
+ATOM    444  GL1 POPC1  15     -17.863 -18.537 -16.030  0.00  0.00            
+ATOM    445  GL2 POPC1  15     -19.469 -15.654 -14.338  0.00  0.00            
+ATOM    446  C1A POPC1  15     -15.044 -18.149 -13.000  0.00  0.00            
+ATOM    447  D2A POPC1  15     -12.945 -18.182  -8.701  0.00  0.00            
+ATOM    448  C3A POPC1  15      -9.722 -17.888  -5.127  0.00  0.00            
+ATOM    449  C4A POPC1  15      -8.401 -15.431  -1.481  0.00  0.00            
+ATOM    450  C1B POPC1  15     -17.785 -15.533 -10.037  0.00  0.00            
+ATOM    451  C2B POPC1  15     -17.804 -18.474  -6.326  0.00  0.00            
+ATOM    452  C3B POPC1  15     -18.815 -17.285  -1.700  0.00  0.00            
+ATOM    453  C4B POPC1  15     -18.904 -18.585   2.218  0.00  0.00            
+ATOM    454  NC3 POPC1  16      16.228   1.753 -20.138  0.00  0.00            
+ATOM    455  PO4 POPC1  16      19.629   0.085 -17.800  0.00  0.00            
+ATOM    456  GL1 POPC1  16      18.524  -0.548 -14.149  0.00  0.00            
+ATOM    457  GL2 POPC1  16      15.636   0.021 -14.145  0.00  0.00            
+ATOM    458  C1A POPC1  16      19.589   0.982 -10.246  0.00  0.00            
+ATOM    459  D2A POPC1  16      19.989   3.499  -7.231  0.00  0.00            
+ATOM    460  C3A POPC1  16      19.148   1.944  -3.377  0.00  0.00            
+ATOM    461  C4A POPC1  16      16.890  -1.616  -1.491  0.00  0.00            
+ATOM    462  C1B POPC1  16      14.462   1.227  -9.747  0.00  0.00            
+ATOM    463  C2B POPC1  16      14.646   1.589  -4.791  0.00  0.00            
+ATOM    464  C3B POPC1  16      14.856   3.909  -1.178  0.00  0.00            
+ATOM    465  C4B POPC1  16      15.399   3.760   3.546  0.00  0.00            
+ATOM    466  NC3 POPC1  17     -17.250   7.934 -24.831  0.00  0.00            
+ATOM    467  PO4 POPC1  17     -20.315   6.080 -21.694  0.00  0.00            
+ATOM    468  GL1 POPC1  17     -20.063   4.893 -16.720  0.00  0.00            
+ATOM    469  GL2 POPC1  17     -16.878   5.110 -15.671  0.00  0.00            
+ATOM    470  C1A POPC1  17     -19.961   4.623 -12.404  0.00  0.00            
+ATOM    471  D2A POPC1  17     -20.541   6.552  -8.417  0.00  0.00            
+ATOM    472  C3A POPC1  17     -18.947   6.744  -4.449  0.00  0.00            
+ATOM    473  C4A POPC1  17     -14.924   6.150  -3.008  0.00  0.00            
+ATOM    474  C1B POPC1  17     -15.398   6.413 -11.363  0.00  0.00            
+ATOM    475  C2B POPC1  17     -15.805   8.567  -7.759  0.00  0.00            
+ATOM    476  C3B POPC1  17     -16.689  11.090  -4.399  0.00  0.00            
+ATOM    477  C4B POPC1  17     -17.391  15.164  -1.650  0.00  0.00            
+ATOM    478  NC3 POPC1  18      22.971  16.857 -23.465  0.00  0.00            
+ATOM    479  PO4 POPC1  18      21.061  13.370 -20.959  0.00  0.00            
+ATOM    480  GL1 POPC1  18      20.614  13.029 -16.379  0.00  0.00            
+ATOM    481  GL2 POPC1  18      19.326  10.118 -14.244  0.00  0.00            
+ATOM    482  C1A POPC1  18      18.402  14.218 -11.846  0.00  0.00            
+ATOM    483  D2A POPC1  18      17.137  11.506  -8.568  0.00  0.00            
+ATOM    484  C3A POPC1  18      15.574  13.236  -5.261  0.00  0.00            
+ATOM    485  C4A POPC1  18      14.473  15.276  -2.351  0.00  0.00            
+ATOM    486  C1B POPC1  18      14.804   9.207 -12.347  0.00  0.00            
+ATOM    487  C2B POPC1  18      10.953  10.065  -8.441  0.00  0.00            
+ATOM    488  C3B POPC1  18      10.522  10.771  -3.434  0.00  0.00            
+ATOM    489  C4B POPC1  18       7.721  10.854   0.065  0.00  0.00            
+ATOM    490  NC3 POPC1  19      -5.536  -9.858 -20.109  0.00  0.00            
+ATOM    491  PO4 POPC1  19      -6.095 -14.924 -20.915  0.00  0.00            
+ATOM    492  GL1 POPC1  19      -5.252 -15.338 -16.487  0.00  0.00            
+ATOM    493  GL2 POPC1  19      -4.069 -18.198 -16.903  0.00  0.00            
+ATOM    494  C1A POPC1  19      -4.846 -16.926 -11.896  0.00  0.00            
+ATOM    495  D2A POPC1  19      -5.794 -19.603  -8.714  0.00  0.00            
+ATOM    496  C3A POPC1  19      -4.250 -18.928  -4.386  0.00  0.00            
+ATOM    497  C4A POPC1  19      -1.130 -17.689  -1.772  0.00  0.00            
+ATOM    498  C1B POPC1  19      -8.301 -19.450 -16.049  0.00  0.00            
+ATOM    499  C2B POPC1  19      -9.447 -20.730 -13.068  0.00  0.00            
+ATOM    500  C3B POPC1  19      -9.733 -21.850  -8.918  0.00  0.00            
+ATOM    501  C4B POPC1  19      -7.194 -23.168  -4.834  0.00  0.00            
+ATOM    502  NC3 POPC1  20       1.838   9.839 -20.630  0.00  0.00            
+ATOM    503  PO4 POPC1  20       3.727  13.955 -21.329  0.00  0.00            
+ATOM    504  GL1 POPC1  20       5.781  13.679 -17.909  0.00  0.00            
+ATOM    505  GL2 POPC1  20       4.745  11.051 -16.299  0.00  0.00            
+ATOM    506  C1A POPC1  20       4.370  16.385 -13.932  0.00  0.00            
+ATOM    507  D2A POPC1  20       4.710  20.130 -10.180  0.00  0.00            
+ATOM    508  C3A POPC1  20       6.593  19.105  -5.870  0.00  0.00            
+ATOM    509  C4A POPC1  20       8.926  20.827  -1.803  0.00  0.00            
+ATOM    510  C1B POPC1  20       5.903  12.608 -11.301  0.00  0.00            
+ATOM    511  C2B POPC1  20       3.756  14.266  -8.912  0.00  0.00            
+ATOM    512  C3B POPC1  20       2.064  16.722  -4.810  0.00  0.00            
+ATOM    513  C4B POPC1  20       3.670  19.088  -1.085  0.00  0.00            
+ATOM    514  GL1 TRIO1  21      10.136  12.666 -14.299  0.00  0.00            
+ATOM    515  C1A TRIO1  21       9.998   8.213 -14.160  0.00  0.00            
+ATOM    516  D2A TRIO1  21       7.350   6.510 -10.652  0.00  0.00            
+ATOM    517  C3A TRIO1  21       6.792   8.333  -7.277  0.00  0.00            
+ATOM    518  C4A TRIO1  21       5.663  12.271  -4.646  0.00  0.00            
+ATOM    519  GL2 TRIO1  21      13.888  14.848 -14.667  0.00  0.00            
+ATOM    520  C1B TRIO1  21      12.530  14.240 -10.004  0.00  0.00            
+ATOM    521  D2B TRIO1  21       9.045  15.071  -7.505  0.00  0.00            
+ATOM    522  C3B TRIO1  21       9.608  15.592  -3.713  0.00  0.00            
+ATOM    523  C4B TRIO1  21      10.062  14.826  -0.038  0.00  0.00            
+ATOM    524  GL3 TRIO1  21      13.464  18.170 -14.003  0.00  0.00            
+ATOM    525  C1C TRIO1  21      15.230  18.112 -10.250  0.00  0.00            
+ATOM    526  D2C TRIO1  21      13.252  18.181  -6.021  0.00  0.00            
+ATOM    527  C3C TRIO1  21      13.661  21.630  -3.866  0.00  0.00            
+ATOM    528  C4C TRIO1  21      13.776  24.581  -0.366  0.00  0.00            
+ATOM    529  NC3 POPC1  22     -17.479 -17.987 -20.857  0.00  0.00            
+ATOM    530  PO4 POPC1  22     -18.209 -13.440 -20.226  0.00  0.00            
+ATOM    531  GL1 POPC1  22     -15.453 -14.068 -17.622  0.00  0.00            
+ATOM    532  GL2 POPC1  22     -13.916 -10.875 -18.420  0.00  0.00            
+ATOM    533  C1A POPC1  22     -15.134 -13.320 -13.693  0.00  0.00            
+ATOM    534  D2A POPC1  22     -13.706 -13.320  -9.267  0.00  0.00            
+ATOM    535  C3A POPC1  22     -14.380 -14.387  -5.422  0.00  0.00            
+ATOM    536  C4A POPC1  22     -13.677 -17.404  -1.315  0.00  0.00            
+ATOM    537  C1B POPC1  22     -14.284  -8.580 -14.586  0.00  0.00            
+ATOM    538  C2B POPC1  22     -15.228  -8.966 -10.900  0.00  0.00            
+ATOM    539  C3B POPC1  22     -15.085  -8.568  -6.586  0.00  0.00            
+ATOM    540  C4B POPC1  22     -13.291 -10.239  -3.187  0.00  0.00            
+ATOM    541  SOD SOD 4   1       9.409   0.980  49.363  0.00  0.00            
+ATOM    542  SOD SOD 4   2       4.343  14.992 -33.563  0.00  0.00            
+ATOM    543  SOD SOD 4   3     -11.293 -11.994 -49.759  0.00  0.00            
+ATOM    544  SOD SOD 4   4     -14.597 -17.604  70.668  0.00  0.00            
+ATOM    545  SOD SOD 4   5      -3.428  15.159  47.642  0.00  0.00            
+ATOM    546  SOD SOD 4   6      16.768  12.263  53.236  0.00  0.00            
+ATOM    547  SOD SOD 4   7       8.894  -3.571  36.670  0.00  0.00            
+ATOM    548  SOD SOD 4   8      -3.179  -6.753 -36.948  0.00  0.00            
+ATOM    549  SOD SOD 4   9       9.016  10.237 -56.886  0.00  0.00            
+ATOM    550  SOD SOD 4  10      -4.347   7.887 -66.103  0.00  0.00            
+ATOM    551  SOD SOD 4  11      17.990  -6.327  20.498  0.00  0.00            
+ATOM    552  SOD SOD 4  12       3.340  18.174 -50.920  0.00  0.00            
+ATOM    553  CLA CLA 5   1      13.719   7.654 -59.188  0.00  0.00            
+ATOM    554  CLA CLA 5   2     -16.741 -13.500  72.540  0.00  0.00            
+ATOM    555  CLA CLA 5   3      -7.308  17.172  49.994  0.00  0.00            
+ATOM    556  CLA CLA 5   4       2.265   7.328  25.838  0.00  0.00            
+ATOM    557  CLA CLA 5   5       7.572  -6.171  32.002  0.00  0.00            
+ATOM    558  CLA CLA 5   6     -10.934  14.498  71.104  0.00  0.00            
+ATOM    559  CLA CLA 5   7      12.299   4.306  52.419  0.00  0.00            
+ATOM    560  CLA CLA 5   8       2.521  12.879  54.278  0.00  0.00            
+ATOM    561  CLA CLA 5   9      16.268   8.349  27.534  0.00  0.00            
+ATOM    562  CLA CLA 5  10      10.873  10.439 -27.895  0.00  0.00            
+ATOM    563  CLA CLA 5  11      -6.030  -0.032 -37.216  0.00  0.00            
+ATOM    564  CLA CLA 5  12      11.090  15.044  34.240  0.00  0.00            
+ATOM    565  W   W   6   1      -3.314  17.042 -41.337  0.00  0.00            
+ATOM    566  W   W   6   2     -17.601   2.036 -41.764  0.00  0.00            
+ATOM    567  W   W   6   3      16.935  16.590  46.143  0.00  0.00            
+ATOM    568  W   W   6   4     -17.280 -16.664  58.958  0.00  0.00            
+ATOM    569  W   W   6   5      -5.650 -16.889 -44.694  0.00  0.00            
+ATOM    570  W   W   6   6      -0.469   3.740  35.382  0.00  0.00            
+ATOM    571  W   W   6   7      11.759  11.250 -39.618  0.00  0.00            
+ATOM    572  W   W   6   8      -1.614   6.800 -70.541  0.00  0.00            
+ATOM    573  W   W   6   9      -7.094   4.741  67.814  0.00  0.00            
+ATOM    574  W   W   6  10       5.728  -7.759  36.859  0.00  0.00            
+ATOM    575  W   W   6  11     -13.158 -12.634  42.404  0.00  0.00            
+ATOM    576  W   W   6  12       8.296   3.218 -35.334  0.00  0.00            
+ATOM    577  W   W   6  13     -16.461  13.456 -43.148  0.00  0.00            
+ATOM    578  W   W   6  14      -7.467 -11.562 -52.473  0.00  0.00            
+ATOM    579  W   W   6  15      -2.502  12.048 -46.070  0.00  0.00            
+ATOM    580  W   W   6  16     -16.524   5.145  67.459  0.00  0.00            
+ATOM    581  W   W   6  17       9.865   4.210  68.894  0.00  0.00            
+ATOM    582  W   W   6  18     -14.565  -3.282 -58.784  0.00  0.00            
+ATOM    583  W   W   6  19      -9.752 -14.828 -67.910  0.00  0.00            
+ATOM    584  W   W   6  20      17.716 -10.390  46.341  0.00  0.00            
+ATOM    585  W   W   6  21       4.321  -3.204  35.301  0.00  0.00            
+ATOM    586  W   W   6  22      13.598   3.872 -55.436  0.00  0.00            
+ATOM    587  W   W   6  23     -13.538   7.424 -64.260  0.00  0.00            
+ATOM    588  W   W   6  24      -2.151   2.690 -34.640  0.00  0.00            
+ATOM    589  W   W   6  25      -5.420   5.973 -36.991  0.00  0.00            
+ATOM    590  W   W   6  26      10.703  -4.627 -24.776  0.00  0.00            
+ATOM    591  W   W   6  27     -17.213 -13.324  63.060  0.00  0.00            
+ATOM    592  W   W   6  28       5.333 -12.637 -65.694  0.00  0.00            
+ATOM    593  W   W   6  29      -2.493 -14.801  67.536  0.00  0.00            
+ATOM    594  W   W   6  30     -18.370 -13.369  35.194  0.00  0.00            
+ATOM    595  W   W   6  31       3.095   1.949  26.508  0.00  0.00            
+ATOM    596  W   W   6  32       5.750 -17.185 -30.478  0.00  0.00            
+ATOM    597  W   W   6  33       1.275   3.938 -42.640  0.00  0.00            
+ATOM    598  W   W   6  34     -14.648   5.477  42.114  0.00  0.00            
+ATOM    599  W   W   6  35      -8.385   7.169 -44.117  0.00  0.00            
+ATOM    600  W   W   6  36     -11.524   2.158 -64.501  0.00  0.00            
+ATOM    601  W   W   6  37       7.114 -13.500  51.938  0.00  0.00            
+ATOM    602  W   W   6  38      -6.784 -12.574 -25.288  0.00  0.00            
+ATOM    603  W   W   6  39      -6.078  17.433 -29.637  0.00  0.00            
+ATOM    604  W   W   6  40     -10.052   8.055 -38.238  0.00  0.00            
+ATOM    605  W   W   6  41      15.278 -14.294  65.666  0.00  0.00            
+ATOM    606  W   W   6  42     -17.219 -17.768  65.241  0.00  0.00            
+ATOM    607  W   W   6  43     -16.207  -9.290 -70.796  0.00  0.00            
+ATOM    608  W   W   6  44      17.956   4.589 -59.541  0.00  0.00            
+ATOM    609  W   W   6  45     -11.434  -1.435  64.561  0.00  0.00            
+ATOM    610  W   W   6  46      18.031 -14.416 -47.149  0.00  0.00            
+ATOM    611  W   W   6  47      17.737  -1.042  65.946  0.00  0.00            
+ATOM    612  W   W   6  48       6.827  12.441 -47.022  0.00  0.00            
+ATOM    613  W   W   6  49       5.730  -4.924 -46.730  0.00  0.00            
+ATOM    614  W   W   6  50       8.590   3.571  29.112  0.00  0.00            
+ATOM    615  W   W   6  51      -2.274  -4.111 -50.886  0.00  0.00            
+ATOM    616  W   W   6  52      -2.026   7.486 -57.837  0.00  0.00            
+ATOM    617  W   W   6  53      17.900 -12.871 -68.502  0.00  0.00            
+ATOM    618  W   W   6  54     -15.175  -1.499 -63.162  0.00  0.00            
+ATOM    619  W   W   6  55      11.074 -11.708  63.009  0.00  0.00            
+ATOM    620  W   W   6  56      14.569 -10.594  38.374  0.00  0.00            
+ATOM    621  W   W   6  57      -8.574  12.947 -38.851  0.00  0.00            
+ATOM    622  W   W   6  58       0.952  -5.512  44.542  0.00  0.00            
+ATOM    623  W   W   6  59       9.064   5.937  33.602  0.00  0.00            
+ATOM    624  W   W   6  60       3.844  16.009  33.136  0.00  0.00            
+ATOM    625  W   W   6  61       6.367   4.860 -44.069  0.00  0.00            
+ATOM    626  W   W   6  62     -15.357  10.913  25.553  0.00  0.00            
+ATOM    627  W   W   6  63      -6.146   5.722 -31.698  0.00  0.00            
+ATOM    628  W   W   6  64      -8.951  -2.572 -17.954  0.00  0.00            
+ATOM    629  W   W   6  65      -8.813 -13.404  57.897  0.00  0.00            
+ATOM    630  W   W   6  66     -13.844   3.024  50.462  0.00  0.00            
+ATOM    631  W   W   6  67      18.386 -10.131 -34.245  0.00  0.00            
+ATOM    632  W   W   6  68     -13.166 -12.340  59.420  0.00  0.00            
+ATOM    633  W   W   6  69       0.243  12.845  40.365  0.00  0.00            
+ATOM    634  W   W   6  70       8.522  -4.822 -53.586  0.00  0.00            
+ATOM    635  W   W   6  71      -2.563   1.310 -26.169  0.00  0.00            
+ATOM    636  W   W   6  72      10.048  13.182  72.131  0.00  0.00            
+ATOM    637  W   W   6  73      -9.399  16.958 -20.560  0.00  0.00            
+ATOM    638  W   W   6  74      -6.705  14.743  67.440  0.00  0.00            
+ATOM    639  W   W   6  75      -6.977  16.850 -48.980  0.00  0.00            
+ATOM    640  W   W   6  76      -2.528   2.344 -57.324  0.00  0.00            
+ATOM    641  W   W   6  77      11.036 -10.237 -22.893  0.00  0.00            
+ATOM    642  W   W   6  78      17.429   4.689  59.181  0.00  0.00            
+ATOM    643  W   W   6  79     -10.780 -15.294 -34.508  0.00  0.00            
+ATOM    644  W   W   6  80      -7.627  14.754 -63.836  0.00  0.00            
+ATOM    645  W   W   6  81     -10.723  -2.545 -23.027  0.00  0.00            
+ATOM    646  W   W   6  82       0.288   4.385 -47.978  0.00  0.00            
+ATOM    647  W   W   6  83     -10.435  -7.260 -19.290  0.00  0.00            
+ATOM    648  W   W   6  84       6.200  10.394  62.155  0.00  0.00            
+ATOM    649  W   W   6  85     -12.818 -14.551  37.150  0.00  0.00            
+ATOM    650  W   W   6  86       4.409 -10.227  41.800  0.00  0.00            
+ATOM    651  W   W   6  87       1.381 -15.089  62.563  0.00  0.00            
+ATOM    652  W   W   6  88      16.742  14.877 -48.191  0.00  0.00            
+ATOM    653  W   W   6  89       5.393   0.338  52.575  0.00  0.00            
+ATOM    654  W   W   6  90      14.121 -16.395 -41.400  0.00  0.00            
+ATOM    655  W   W   6  91      -9.904  -6.277  63.657  0.00  0.00            
+ATOM    656  W   W   6  92     -13.854   4.517  25.505  0.00  0.00            
+ATOM    657  W   W   6  93      16.166  15.719  26.104  0.00  0.00            
+ATOM    658  W   W   6  94       2.145  13.459  45.351  0.00  0.00            
+ATOM    659  W   W   6  95      -4.022  16.022  38.802  0.00  0.00            
+ATOM    660  W   W   6  96      -0.197  16.487  61.231  0.00  0.00            
+ATOM    661  W   W   6  97       7.391 -12.751 -70.423  0.00  0.00            
+ATOM    662  W   W   6  98      16.157  -4.142 -67.153  0.00  0.00            
+ATOM    663  W   W   6  99     -16.257  14.237  50.357  0.00  0.00            
+ATOM    664  W   W   6 100      17.778   5.125 -45.156  0.00  0.00            
+ATOM    665  W   W   6 101       7.717   6.419  25.534  0.00  0.00            
+ATOM    666  W   W   6 102      -1.302  11.480 -73.021  0.00  0.00            
+ATOM    667  W   W   6 103     -10.245  12.577  64.478  0.00  0.00            
+ATOM    668  W   W   6 104      -0.792  13.411  57.681  0.00  0.00            
+ATOM    669  W   W   6 105       7.524 -12.324 -36.624  0.00  0.00            
+ATOM    670  W   W   6 106      -8.354  15.129  29.483  0.00  0.00            
+ATOM    671  W   W   6 107       8.969  11.602 -51.677  0.00  0.00            
+ATOM    672  W   W   6 108      -4.453 -13.270  55.016  0.00  0.00            
+ATOM    673  W   W   6 109     -14.543   8.778 -29.401  0.00  0.00            
+ATOM    674  W   W   6 110      15.126   1.339  39.168  0.00  0.00            
+ATOM    675  W   W   6 111      -5.178   9.894 -70.558  0.00  0.00            
+ATOM    676  W   W   6 112      -8.265  -2.512  61.212  0.00  0.00            
+ATOM    677  W   W   6 113     -10.753   5.663 -60.531  0.00  0.00            
+ATOM    678  W   W   6 114      -4.153 -17.338 -64.895  0.00  0.00            
+ATOM    679  W   W   6 115      16.926  -9.949  51.246  0.00  0.00            
+ATOM    680  W   W   6 116     -13.727  -2.267  30.148  0.00  0.00            
+ATOM    681  W   W   6 117       0.536  -1.962  49.560  0.00  0.00            
+ATOM    682  W   W   6 118      14.123  -5.427  29.547  0.00  0.00            
+ATOM    683  W   W   6 119      -9.465  13.662 -52.576  0.00  0.00            
+ATOM    684  W   W   6 120       5.896  -4.446  56.402  0.00  0.00            
+ATOM    685  W   W   6 121      11.205   0.116  55.178  0.00  0.00            
+ATOM    686  W   W   6 122      -2.970   5.251  62.305  0.00  0.00            
+ATOM    687  W   W   6 123       6.838  -3.445 -58.127  0.00  0.00            
+ATOM    688  W   W   6 124       5.515 -15.403 -46.781  0.00  0.00            
+ATOM    689  W   W   6 125      12.336  -7.764  20.130  0.00  0.00            
+ATOM    690  W   W   6 126      -0.383  -3.698 -64.532  0.00  0.00            
+ATOM    691  W   W   6 127       1.796   0.457 -22.704  0.00  0.00            
+ATOM    692  W   W   6 128      12.856 -12.333 -27.529  0.00  0.00            
+ATOM    693  W   W   6 129     -11.893 -17.229  50.242  0.00  0.00            
+ATOM    694  W   W   6 130      11.717  16.673 -61.358  0.00  0.00            
+ATOM    695  W   W   6 131      16.781   3.397  63.739  0.00  0.00            
+ATOM    696  W   W   6 132      11.247 -14.757  42.853  0.00  0.00            
+ATOM    697  W   W   6 133      -2.877  -6.474  70.424  0.00  0.00            
+ATOM    698  W   W   6 134     -12.583 -13.569 -71.638  0.00  0.00            
+ATOM    699  W   W   6 135      -0.533  11.233  63.169  0.00  0.00            
+ATOM    700  W   W   6 136      17.764 -11.641 -28.290  0.00  0.00            
+ATOM    701  W   W   6 137      -4.453  10.194  69.381  0.00  0.00            
+ATOM    702  W   W   6 138       2.857 -13.947 -24.630  0.00  0.00            
+ATOM    703  W   W   6 139     -18.289 -17.067 -30.645  0.00  0.00            
+ATOM    704  W   W   6 140     -10.576 -18.305 -57.580  0.00  0.00            
+ATOM    705  W   W   6 141      13.352  12.608 -56.365  0.00  0.00            
+ATOM    706  W   W   6 142       3.023 -12.893 -50.380  0.00  0.00            
+ATOM    707  W   W   6 143      -6.441  17.678  43.751  0.00  0.00            
+ATOM    708  W   W   6 144      -8.036 -14.182 -73.114  0.00  0.00            
+ATOM    709  W   W   6 145      11.937 -13.053 -68.183  0.00  0.00            
+ATOM    710  W   W   6 146      18.117  11.034  46.406  0.00  0.00            
+ATOM    711  W   W   6 147     -16.822  17.385 -40.229  0.00  0.00            
+ATOM    712  W   W   6 148      -2.126  10.206 -25.247  0.00  0.00            
+ATOM    713  W   W   6 149      -0.221   0.901  58.704  0.00  0.00            
+ATOM    714  W   W   6 150     -13.710  15.696  38.118  0.00  0.00            
+ATOM    715  W   W   6 151      15.997 -14.605  40.949  0.00  0.00            
+ATOM    716  W   W   6 152      -2.336   9.339  27.135  0.00  0.00            
+ATOM    717  W   W   6 153      -0.494   7.331 -33.462  0.00  0.00            
+ATOM    718  W   W   6 154       0.232  11.074 -67.524  0.00  0.00            
+ATOM    719  W   W   6 155      -1.242   4.613  70.552  0.00  0.00            
+ATOM    720  W   W   6 156      -7.461  14.698 -44.193  0.00  0.00            
+ATOM    721  W   W   6 157      -5.504 -10.696 -39.651  0.00  0.00            
+ATOM    722  W   W   6 158     -17.116  15.172  71.949  0.00  0.00            
+ATOM    723  W   W   6 159      15.812 -18.236 -35.707  0.00  0.00            
+ATOM    724  W   W   6 160       3.701 -12.464  68.256  0.00  0.00            
+ATOM    725  W   W   6 161      -5.854  -0.205  41.715  0.00  0.00            
+ATOM    726  W   W   6 162      17.617   3.561  42.971  0.00  0.00            
+ATOM    727  W   W   6 163     -10.621 -14.236  69.703  0.00  0.00            
+ATOM    728  W   W   6 164      18.144   2.374 -24.791  0.00  0.00            
+ATOM    729  W   W   6 165      12.086 -17.917  64.904  0.00  0.00            
+ATOM    730  W   W   6 166      -0.226  12.604  67.969  0.00  0.00            
+ATOM    731  W   W   6 167      17.608  -4.074  52.501  0.00  0.00            
+ATOM    732  W   W   6 168     -16.060   4.290 -28.419  0.00  0.00            
+ATOM    733  W   W   6 169      15.435   4.030 -38.853  0.00  0.00            
+ATOM    734  W   W   6 170      13.219 -10.244  67.651  0.00  0.00            
+ATOM    735  W   W   6 171       8.472  -3.597 -29.663  0.00  0.00            
+ATOM    736  W   W   6 172     -18.404  -8.272 -66.097  0.00  0.00            
+ATOM    737  W   W   6 173      -1.262  16.430  43.330  0.00  0.00            
+ATOM    738  W   W   6 174       0.610 -10.304 -39.606  0.00  0.00            
+ATOM    739  W   W   6 175      -4.176  -6.493  45.744  0.00  0.00            
+ATOM    740  W   W   6 176      14.138  12.088  64.616  0.00  0.00            
+ATOM    741  W   W   6 177      -2.242  -6.193  28.491  0.00  0.00            
+ATOM    742  W   W   6 178      14.327   1.685 -42.892  0.00  0.00            
+ATOM    743  W   W   6 179      -1.033  -8.628  24.787  0.00  0.00            
+ATOM    744  W   W   6 180      -1.109 -16.931 -37.709  0.00  0.00            
+ATOM    745  W   W   6 181       6.282   2.015 -31.070  0.00  0.00            
+ATOM    746  W   W   6 182     -13.555  17.417 -17.924  0.00  0.00            
+ATOM    747  W   W   6 183       5.897  -9.704 -45.827  0.00  0.00            
+ATOM    748  W   W   6 184      -6.436 -12.549  17.861  0.00  0.00            
+ATOM    749  W   W   6 185     -17.052  11.636 -65.973  0.00  0.00            
+ATOM    750  W   W   6 186       7.606 -15.274 -16.914  0.00  0.00            
+ATOM    751  W   W   6 187       4.888   9.725  39.764  0.00  0.00            
+ATOM    752  W   W   6 188      13.496  14.033 -34.957  0.00  0.00            
+ATOM    753  W   W   6 189       9.190  14.259  42.206  0.00  0.00            
+ATOM    754  W   W   6 190       5.560   5.984 -39.295  0.00  0.00            
+ATOM    755  W   W   6 191      11.426   8.006  29.093  0.00  0.00            
+ATOM    756  W   W   6 192      -6.119 -13.134 -34.403  0.00  0.00            
+ATOM    757  W   W   6 193      -3.948 -17.999  63.465  0.00  0.00            
+ATOM    758  W   W   6 194      15.491   7.973  55.493  0.00  0.00            
+ATOM    759  W   W   6 195     -13.694  -1.138 -41.711  0.00  0.00            
+ATOM    760  W   W   6 196      -3.149  16.945  22.074  0.00  0.00            
+ATOM    761  W   W   6 197       8.484   5.108  38.678  0.00  0.00            
+ATOM    762  W   W   6 198      -8.802   8.433 -64.634  0.00  0.00            
+ATOM    763  W   W   6 199       3.254   3.749  56.757  0.00  0.00            
+ATOM    764  W   W   6 200      -2.264 -11.286 -49.587  0.00  0.00            
+ATOM    765  W   W   6 201     -14.847  10.878 -61.194  0.00  0.00            
+ATOM    766  W   W   6 202      -4.908   4.897 -47.015  0.00  0.00            
+ATOM    767  W   W   6 203      12.025  12.988  54.241  0.00  0.00            
+ATOM    768  W   W   6 204       4.227   4.017  31.192  0.00  0.00            
+ATOM    769  W   W   6 205      17.734   7.499 -31.582  0.00  0.00            
+ATOM    770  W   W   6 206     -13.676  11.265  46.454  0.00  0.00            
+ATOM    771  W   W   6 207      12.779  18.276 -66.556  0.00  0.00            
+ATOM    772  W   W   6 208      10.504  -7.636 -44.140  0.00  0.00            
+ATOM    773  W   W   6 209       3.772   6.733  35.038  0.00  0.00            
+ATOM    774  W   W   6 210     -12.085 -13.899  54.293  0.00  0.00            
+ATOM    775  W   W   6 211       3.261   4.508  40.015  0.00  0.00            
+ATOM    776  W   W   6 212     -16.260 -16.754  39.440  0.00  0.00            
+ATOM    777  W   W   6 213     -17.974   2.704 -51.213  0.00  0.00            
+ATOM    778  W   W   6 214      11.682  -7.507  73.074  0.00  0.00            
+ATOM    779  W   W   6 215       8.640  -7.048 -37.670  0.00  0.00            
+ATOM    780  W   W   6 216      14.239  -7.330 -25.867  0.00  0.00            
+ATOM    781  W   W   6 217     -14.742 -18.037 -54.609  0.00  0.00            
+ATOM    782  W   W   6 218       8.984 -13.639  31.593  0.00  0.00            
+ATOM    783  W   W   6 219      -8.421  -3.319  37.527  0.00  0.00            
+ATOM    784  W   W   6 220     -13.003  -4.823  21.344  0.00  0.00            
+ATOM    785  W   W   6 221       2.549  -4.238  39.806  0.00  0.00            
+ATOM    786  W   W   6 222      16.814  17.375 -44.195  0.00  0.00            
+ATOM    787  W   W   6 223       1.606  -3.478  26.606  0.00  0.00            
+ATOM    788  W   W   6 224      -9.585 -12.771 -38.388  0.00  0.00            
+ATOM    789  W   W   6 225       3.648  15.497  69.574  0.00  0.00            
+ATOM    790  W   W   6 226      10.933   2.725 -51.487  0.00  0.00            
+ATOM    791  W   W   6 227       5.688 -13.603  24.008  0.00  0.00            
+ATOM    792  W   W   6 228     -16.717  -7.378 -40.083  0.00  0.00            
+ATOM    793  W   W   6 229      14.897   4.643 -64.322  0.00  0.00            
+ATOM    794  W   W   6 230     -14.377  10.257  70.968  0.00  0.00            
+ATOM    795  W   W   6 231       2.387 -17.977 -65.735  0.00  0.00            
+ATOM    796  W   W   6 232       3.219   2.197 -69.623  0.00  0.00            
+ATOM    797  W   W   6 233       7.769   1.131  24.826  0.00  0.00            
+ATOM    798  W   W   6 234     -14.046  16.928  17.534  0.00  0.00            
+ATOM    799  W   W   6 235      -8.600  -9.922  53.923  0.00  0.00            
+ATOM    800  W   W   6 236       0.555   0.039  22.657  0.00  0.00            
+ATOM    801  W   W   6 237      -5.889  -3.417 -46.100  0.00  0.00            
+ATOM    802  W   W   6 238     -14.867 -13.422  49.023  0.00  0.00            
+ATOM    803  W   W   6 239       1.608 -15.237  34.932  0.00  0.00            
+ATOM    804  W   W   6 240      14.266   7.675  40.528  0.00  0.00            
+ATOM    805  W   W   6 241     -10.828 -10.192  49.277  0.00  0.00            
+ATOM    806  W   W   6 242      -5.322 -14.496  45.849  0.00  0.00            
+ATOM    807  W   W   6 243       0.628 -10.442  45.574  0.00  0.00            
+ATOM    808  W   W   6 244       6.283  18.348  50.777  0.00  0.00            
+ATOM    809  W   W   6 245     -17.579  12.260  30.177  0.00  0.00            
+ATOM    810  W   W   6 246     -14.637 -15.477 -66.875  0.00  0.00            
+ATOM    811  W   W   6 247     -10.658  12.708 -23.652  0.00  0.00            
+ATOM    812  W   W   6 248      -9.064  13.845  45.840  0.00  0.00            
+ATOM    813  W   W   6 249      -8.381 -14.961 -30.174  0.00  0.00            
+ATOM    814  W   W   6 250       6.902 -15.294 -52.346  0.00  0.00            
+ATOM    815  W   W   6 251      -5.923   4.973 -18.658  0.00  0.00            
+ATOM    816  W   W   6 252      14.116 -10.299  43.341  0.00  0.00            
+ATOM    817  W   W   6 253     -11.276  -5.208 -30.758  0.00  0.00            
+ATOM    818  W   W   6 254      10.664 -16.791 -71.470  0.00  0.00            
+ATOM    819  W   W   6 255      -0.480   4.499 -61.353  0.00  0.00            
+ATOM    820  W   W   6 256       6.224  -0.654  39.509  0.00  0.00            
+ATOM    821  W   W   6 257       8.018   4.651 -71.750  0.00  0.00            
+ATOM    822  W   W   6 258       1.363   6.025 -66.839  0.00  0.00            
+ATOM    823  W   W   6 259      -8.326  -7.355  70.910  0.00  0.00            
+ATOM    824  W   W   6 260       7.243  -3.327  62.452  0.00  0.00            
+ATOM    825  W   W   6 261      -9.828 -10.247  25.772  0.00  0.00            
+ATOM    826  W   W   6 262     -10.154  -4.325 -55.782  0.00  0.00            
+ATOM    827  W   W   6 263      17.734  10.511 -57.394  0.00  0.00            
+ATOM    828  W   W   6 264       7.667 -18.072  34.880  0.00  0.00            
+ATOM    829  W   W   6 265     -13.367   1.929 -49.246  0.00  0.00            
+ATOM    830  W   W   6 266     -16.901 -16.016  44.587  0.00  0.00            
+ATOM    831  W   W   6 267      -3.968  10.786 -36.011  0.00  0.00            
+ATOM    832  W   W   6 268      17.414  -4.128 -20.653  0.00  0.00            
+ATOM    833  W   W   6 269      -7.669 -15.138  66.100  0.00  0.00            
+ATOM    834  W   W   6 270       0.059  -6.892  49.854  0.00  0.00            
+ATOM    835  W   W   6 271     -10.512  -9.400 -56.164  0.00  0.00            
+ATOM    836  W   W   6 272      12.119  16.141 -44.501  0.00  0.00            
+ATOM    837  W   W   6 273     -14.993   7.560  29.555  0.00  0.00            
+ATOM    838  W   W   6 274     -12.334 -17.415  58.407  0.00  0.00            
+ATOM    839  W   W   6 275      15.090 -12.984 -51.143  0.00  0.00            
+ATOM    840  W   W   6 276       9.466 -14.977  26.790  0.00  0.00            
+ATOM    841  W   W   6 277     -12.406 -18.387  41.910  0.00  0.00            
+ATOM    842  W   W   6 278      -2.081  10.013  46.525  0.00  0.00            
+ATOM    843  W   W   6 279      -9.321   4.536  23.266  0.00  0.00            
+ATOM    844  W   W   6 280     -10.877  -5.015 -66.449  0.00  0.00            
+ATOM    845  W   W   6 281      -0.347  16.037 -54.013  0.00  0.00            
+ATOM    846  W   W   6 282       7.826  -0.414 -49.805  0.00  0.00            
+ATOM    847  W   W   6 283      -5.196  -4.262  50.141  0.00  0.00            
+ATOM    848  W   W   6 284       6.073  -6.939  18.062  0.00  0.00            
+ATOM    849  W   W   6 285     -14.980  -4.164 -17.585  0.00  0.00            
+ATOM    850  W   W   6 286      -1.396  15.392 -25.668  0.00  0.00            
+ATOM    851  W   W   6 287     -11.031  11.067 -42.362  0.00  0.00            
+ATOM    852  W   W   6 288       9.529   0.003 -55.624  0.00  0.00            
+ATOM    853  W   W   6 289      -9.500 -17.198 -63.305  0.00  0.00            
+ATOM    854  W   W   6 290       6.141  -1.696 -25.873  0.00  0.00            
+ATOM    855  W   W   6 291       4.091 -11.451  73.156  0.00  0.00            
+ATOM    856  W   W   6 292     -11.483 -10.935 -30.096  0.00  0.00            
+ATOM    857  W   W   6 293      14.760   9.455 -36.670  0.00  0.00            
+ATOM    858  W   W   6 294      -2.459 -16.324 -32.322  0.00  0.00            
+ATOM    859  W   W   6 295      10.167 -11.770 -41.011  0.00  0.00            
+ATOM    860  W   W   6 296      10.515  -8.488  35.427  0.00  0.00            
+ATOM    861  W   W   6 297     -16.837  17.843  34.815  0.00  0.00            
+ATOM    862  W   W   6 298     -11.042  13.232  50.592  0.00  0.00            
+ATOM    863  W   W   6 299      18.055  15.186 -54.196  0.00  0.00            
+ATOM    864  W   W   6 300      12.356  -2.083 -51.249  0.00  0.00            
+ATOM    865  W   W   6 301       5.747  -0.028 -45.030  0.00  0.00            
+ATOM    866  W   W   6 302      -7.914 -17.651  54.360  0.00  0.00            
+ATOM    867  W   W   6 303       7.878   6.869 -53.500  0.00  0.00            
+ATOM    868  W   W   6 304       9.278  -8.401 -28.545  0.00  0.00            
+ATOM    869  W   W   6 305      -3.166   0.469 -49.038  0.00  0.00            
+ATOM    870  W   W   6 306      -2.622   8.526 -49.770  0.00  0.00            
+ATOM    871  W   W   6 307      -3.196  10.790 -30.777  0.00  0.00            
+ATOM    872  W   W   6 308      13.187  -8.969  58.998  0.00  0.00            
+ATOM    873  W   W   6 309      -4.453  10.957 -60.490  0.00  0.00            
+ATOM    874  W   W   6 310       8.214 -16.903  55.334  0.00  0.00            
+ATOM    875  W   W   6 311      -3.378 -15.213  73.203  0.00  0.00            
+ATOM    876  W   W   6 312      17.291  -7.859  25.464  0.00  0.00            
+ATOM    877  W   W   6 313       7.014 -18.408  29.782  0.00  0.00            
+ATOM    878  W   W   6 314      -3.723  -8.131  32.476  0.00  0.00            
+ATOM    879  W   W   6 315      16.684 -16.922  70.682  0.00  0.00            
+ATOM    880  W   W   6 316     -10.086 -10.711 -43.168  0.00  0.00            
+ATOM    881  W   W   6 317      -7.979 -13.461 -57.073  0.00  0.00            
+ATOM    882  W   W   6 318       7.361 -17.255 -40.500  0.00  0.00            
+ATOM    883  W   W   6 319      -3.575 -12.009  37.695  0.00  0.00            
+ATOM    884  W   W   6 320       1.481  -4.657  59.211  0.00  0.00            
+ATOM    885  W   W   6 321       0.406 -18.205 -61.176  0.00  0.00            
+ATOM    886  W   W   6 322       1.850  -8.275 -48.082  0.00  0.00            
+ATOM    887  W   W   6 323       7.474  -9.005  70.597  0.00  0.00            
+ATOM    888  W   W   6 324     -14.648  -9.816  18.100  0.00  0.00            
+ATOM    889  W   W   6 325       3.401  -3.809 -61.477  0.00  0.00            
+ATOM    890  W   W   6 326      -3.706  -0.002  69.810  0.00  0.00            
+ATOM    891  W   W   6 327      -9.641  -0.126 -31.444  0.00  0.00            
+ATOM    892  W   W   6 328      15.301   6.911 -27.433  0.00  0.00            
+ATOM    893  W   W   6 329       3.127   8.341 -47.364  0.00  0.00            
+ATOM    894  W   W   6 330     -16.054  -5.047 -33.549  0.00  0.00            
+ATOM    895  W   W   6 331      11.537  11.529  46.414  0.00  0.00            
+ATOM    896  W   W   6 332       2.030  -8.744 -66.224  0.00  0.00            
+ATOM    897  W   W   6 333      -3.455 -16.381  25.720  0.00  0.00            
+ATOM    898  W   W   6 334      12.780   8.393 -53.452  0.00  0.00            
+ATOM    899  W   W   6 335      12.376  -0.124  27.782  0.00  0.00            
+ATOM    900  W   W   6 336      10.655  15.126 -69.840  0.00  0.00            
+ATOM    901  W   W   6 337      14.389   9.318 -17.919  0.00  0.00            
+ATOM    902  W   W   6 338      -1.555   1.314 -39.392  0.00  0.00            
+ATOM    903  W   W   6 339       3.874  -8.751  27.315  0.00  0.00            
+ATOM    904  W   W   6 340      -5.384   6.157 -61.200  0.00  0.00            
+ATOM    905  W   W   6 341       8.167   6.591 -66.590  0.00  0.00            
+ATOM    906  W   W   6 342     -11.499  12.103 -29.272  0.00  0.00            
+ATOM    907  W   W   6 343     -17.138  -0.796 -36.864  0.00  0.00            
+ATOM    908  W   W   6 344     -15.330 -13.669 -31.156  0.00  0.00            
+ATOM    909  W   W   6 345       0.804   0.186 -29.946  0.00  0.00            
+ATOM    910  W   W   6 346      13.146   7.615 -44.255  0.00  0.00            
+ATOM    911  W   W   6 347      -2.294  -4.462 -28.807  0.00  0.00            
+ATOM    912  W   W   6 348     -12.011  15.311 -61.828  0.00  0.00            
+ATOM    913  W   W   6 349     -13.207  -7.823 -45.665  0.00  0.00            
+ATOM    914  W   W   6 350     -16.474  -6.473 -48.839  0.00  0.00            
+ATOM    915  W   W   6 351     -17.753  12.785  62.553  0.00  0.00            
+ATOM    916  W   W   6 352     -16.189   0.499  25.219  0.00  0.00            
+ATOM    917  W   W   6 353       8.757  13.855 -36.263  0.00  0.00            
+ATOM    918  W   W   6 354       8.919  14.258 -64.547  0.00  0.00            
+ATOM    919  W   W   6 355     -12.702  17.896 -37.461  0.00  0.00            
+ATOM    920  W   W   6 356      -6.183 -17.695  31.211  0.00  0.00            
+ATOM    921  W   W   6 357      14.991  12.946 -67.143  0.00  0.00            
+ATOM    922  W   W   6 358       3.653  18.102 -56.381  0.00  0.00            
+ATOM    923  W   W   6 359      12.910 -13.375 -58.780  0.00  0.00            
+ATOM    924  W   W   6 360      -7.173  -5.855 -27.815  0.00  0.00            
+ATOM    925  W   W   6 361     -14.262  14.803 -70.321  0.00  0.00            
+ATOM    926  W   W   6 362      -2.707  -3.518 -72.688  0.00  0.00            
+ATOM    927  W   W   6 363       8.689  15.466  47.666  0.00  0.00            
+ATOM    928  W   W   6 364     -12.995  -5.053 -72.414  0.00  0.00            
+ATOM    929  W   W   6 365       2.669 -14.483  20.557  0.00  0.00            
+ATOM    930  W   W   6 366     -10.651   0.604 -55.679  0.00  0.00            
+ATOM    931  W   W   6 367     -16.325 -15.570 -36.183  0.00  0.00            
+ATOM    932  W   W   6 368     -15.249  14.935  67.038  0.00  0.00            
+ATOM    933  W   W   6 369      -0.138   7.377  66.327  0.00  0.00            
+ATOM    934  W   W   6 370      -1.293 -11.512 -35.254  0.00  0.00            
+ATOM    935  W   W   6 371      -2.808   6.010 -28.299  0.00  0.00            
+ATOM    936  W   W   6 372     -13.080  13.850 -56.789  0.00  0.00            
+ATOM    937  W   W   6 373      11.275 -17.541  70.301  0.00  0.00            
+ATOM    938  W   W   6 374       5.249 -17.889  61.234  0.00  0.00            
+ATOM    939  W   W   6 375      -3.354  -0.501  37.260  0.00  0.00            
+ATOM    940  W   W   6 376      11.851 -15.686 -37.304  0.00  0.00            
+ATOM    941  W   W   6 377      -2.250  14.861 -58.167  0.00  0.00            
+ATOM    942  W   W   6 378       2.239   3.170  62.753  0.00  0.00            
+ATOM    943  W   W   6 379     -15.087   6.440 -57.957  0.00  0.00            
+ATOM    944  W   W   6 380      12.217  -2.585  47.164  0.00  0.00            
+ATOM    945  W   W   6 381       8.221 -18.099 -67.179  0.00  0.00            
+ATOM    946  W   W   6 382      10.995  -3.341 -40.832  0.00  0.00            
+ATOM    947  W   W   6 383       3.073  -7.043 -34.878  0.00  0.00            
+ATOM    948  W   W   6 384       7.608  14.643  37.602  0.00  0.00            
+ATOM    949  W   W   6 385      -7.482   9.462  39.125  0.00  0.00            
+ATOM    950  W   W   6 386      -8.851  13.349  55.500  0.00  0.00            
+ATOM    951  W   W   6 387      17.178  -9.981 -54.944  0.00  0.00            
+ATOM    952  W   W   6 388       8.699  17.636 -49.547  0.00  0.00            
+ATOM    953  W   W   6 389      -3.260  -3.439 -40.570  0.00  0.00            
+ATOM    954  W   W   6 390      10.146  -6.600  55.371  0.00  0.00            
+ATOM    955  W   W   6 391       4.920  -8.971 -61.759  0.00  0.00            
+ATOM    956  W   W   6 392      -2.843   4.714  56.879  0.00  0.00            
+ATOM    957  W   W   6 393       2.031  -6.675 -71.621  0.00  0.00            
+ATOM    958  W   W   6 394       4.987  10.234 -66.833  0.00  0.00            
+ATOM    959  W   W   6 395     -16.092  -6.477 -54.019  0.00  0.00            
+ATOM    960  W   W   6 396       5.686   6.363  46.031  0.00  0.00            
+ATOM    961  W   W   6 397       1.102  -2.362 -69.330  0.00  0.00            
+ATOM    962  W   W   6 398      10.799   6.184 -39.467  0.00  0.00            
+ATOM    963  W   W   6 399      -5.752   6.007  72.624  0.00  0.00            
+ATOM    964  W   W   6 400      -8.744  -8.874 -34.803  0.00  0.00            
+ATOM    965  W   W   6 401      -6.338 -17.645  70.348  0.00  0.00            
+ATOM    966  W   W   6 402     -14.952 -15.976  31.809  0.00  0.00            
+ATOM    967  W   W   6 403      -1.372  14.336 -20.311  0.00  0.00            
+ATOM    968  W   W   6 404      -2.860  -0.440 -61.325  0.00  0.00            
+ATOM    969  W   W   6 405       5.279  -7.979  46.161  0.00  0.00            
+ATOM    970  W   W   6 406     -17.260 -11.200  40.241  0.00  0.00            
+ATOM    971  W   W   6 407      -1.366  11.268  51.407  0.00  0.00            
+ATOM    972  W   W   6 408     -14.127 -11.952 -40.627  0.00  0.00            
+ATOM    973  W   W   6 409       1.077 -10.268 -58.028  0.00  0.00            
+ATOM    974  W   W   6 410      -7.697 -14.253  50.284  0.00  0.00            
+ATOM    975  W   W   6 411     -12.477   1.282  40.410  0.00  0.00            
+ATOM    976  W   W   6 412       1.366 -15.141 -29.239  0.00  0.00            
+ATOM    977  W   W   6 413       9.831   1.052  59.894  0.00  0.00            
+ATOM    978  W   W   6 414       9.662 -11.005 -62.960  0.00  0.00            
+ATOM    979  W   W   6 415     -11.621   5.786  38.287  0.00  0.00            
+ATOM    980  W   W   6 416       0.932  -8.715 -52.924  0.00  0.00            
+ATOM    981  W   W   6 417      16.540  -1.421  70.981  0.00  0.00            
+ATOM    982  W   W   6 418       8.993   7.666 -47.947  0.00  0.00            
+ATOM    983  W   W   6 419     -14.839   0.098  68.367  0.00  0.00            
+ATOM    984  W   W   6 420      13.148  -3.072 -29.497  0.00  0.00            
+ATOM    985  W   W   6 421      -4.930  -7.061  37.201  0.00  0.00            
+ATOM    986  W   W   6 422      -8.162   2.504  37.129  0.00  0.00            
+ATOM    987  W   W   6 423       0.558  17.567  18.630  0.00  0.00            
+ATOM    988  W   W   6 424     -15.555  -4.596 -67.294  0.00  0.00            
+ATOM    989  W   W   6 425     -11.201   7.846 -68.722  0.00  0.00            
+ATOM    990  W   W   6 426       6.425  14.373 -59.279  0.00  0.00            
+ATOM    991  W   W   6 427       8.515 -11.436  44.783  0.00  0.00            
+ATOM    992  W   W   6 428      14.113  11.630  59.494  0.00  0.00            
+ATOM    993  W   W   6 429      13.395 -18.146 -56.757  0.00  0.00            
+ATOM    994  W   W   6 430       1.893  -1.618 -48.065  0.00  0.00            
+ATOM    995  W   W   6 431       4.891 -10.731  32.309  0.00  0.00            
+ATOM    996  W   W   6 432     -10.395  -7.814 -61.806  0.00  0.00            
+ATOM    997  W   W   6 433      -9.172  -5.412  47.448  0.00  0.00            
+ATOM    998  W   W   6 434       9.432  11.160  25.336  0.00  0.00            
+ATOM    999  W   W   6 435      -5.622 -15.705 -50.473  0.00  0.00            
+ATOM   1000  W   W   6 436      -3.003  -0.045 -44.234  0.00  0.00            
+ATOM   1001  W   W   6 437      13.695   9.719 -31.728  0.00  0.00            
+ATOM   1002  W   W   6 438      12.314   8.790 -22.657  0.00  0.00            
+ATOM   1003  W   W   6 439     -14.612  11.403 -33.355  0.00  0.00            
+ATOM   1004  W   W   6 440      -3.801 -11.229  42.419  0.00  0.00            
+ATOM   1005  W   W   6 441      17.887   6.491 -54.351  0.00  0.00            
+ATOM   1006  W   W   6 442      15.047   3.047  68.357  0.00  0.00            
+ATOM   1007  W   W   6 443     -17.903  -0.001  49.328  0.00  0.00            
+ATOM   1008  W   W   6 444      17.605   2.639 -33.218  0.00  0.00            
+ATOM   1009  W   W   6 445       5.147   1.880  35.276  0.00  0.00            
+ATOM   1010  W   W   6 446      -7.295   2.215 -22.792  0.00  0.00            
+ATOM   1011  W   W   6 447      -2.594   5.111 -53.115  0.00  0.00            
+ATOM   1012  W   W   6 448      -8.583  11.116  59.819  0.00  0.00            
+ATOM   1013  W   W   6 449       4.552  12.299 -53.751  0.00  0.00            
+ATOM   1014  W   W   6 450       2.597 -15.513  51.050  0.00  0.00            
+ATOM   1015  W   W   6 451     -17.524  -2.014  58.724  0.00  0.00            
+ATOM   1016  W   W   6 452     -15.890  16.109 -64.910  0.00  0.00            
+ATOM   1017  W   W   6 453     -16.765  16.892 -34.562  0.00  0.00            
+ATOM   1018  W   W   6 454      17.796   9.976 -46.713  0.00  0.00            
+ATOM   1019  W   W   6 455       7.270   0.506 -60.801  0.00  0.00            
+ATOM   1020  W   W   6 456      -5.845  11.245  49.970  0.00  0.00            
+ATOM   1021  W   W   6 457      -3.329  -8.409 -25.593  0.00  0.00            
+ATOM   1022  W   W   6 458      17.903  16.139 -69.160  0.00  0.00            
+ATOM   1023  W   W   6 459     -10.096   4.290 -71.762  0.00  0.00            
+ATOM   1024  W   W   6 460     -10.848   3.006  44.990  0.00  0.00            
+ATOM   1025  W   W   6 461     -11.003  13.010  25.865  0.00  0.00            
+ATOM   1026  W   W   6 462       4.330 -14.476  28.619  0.00  0.00            
+ATOM   1027  W   W   6 463       8.304  14.373 -41.263  0.00  0.00            
+ATOM   1028  W   W   6 464      -3.666  -8.176  53.596  0.00  0.00            
+ATOM   1029  W   W   6 465      11.805 -10.234 -35.918  0.00  0.00            
+ATOM   1030  W   W   6 466     -13.755   3.946 -44.360  0.00  0.00            
+ATOM   1031  W   W   6 467      12.211   2.757  43.371  0.00  0.00            
+ATOM   1032  W   W   6 468       7.596  -8.495  60.500  0.00  0.00            
+ATOM   1033  W   W   6 469      17.951 -14.799  54.051  0.00  0.00            
+ATOM   1034  W   W   6 470      -2.097   3.012  40.907  0.00  0.00            
+ATOM   1035  W   W   6 471      15.094   7.535  45.414  0.00  0.00            
+ATOM   1036  W   W   6 472       4.094   1.093 -40.100  0.00  0.00            
+ATOM   1037  W   W   6 473     -11.987 -17.309  26.913  0.00  0.00            
+ATOM   1038  W   W   6 474     -11.500   4.320 -29.178  0.00  0.00            
+ATOM   1039  W   W   6 475       9.889   8.014  55.214  0.00  0.00            
+ATOM   1040  W   W   6 476       6.999   1.442 -65.277  0.00  0.00            
+ATOM   1041  W   W   6 477      18.336  -2.488 -51.745  0.00  0.00            
+ATOM   1042  W   W   6 478       0.609  -0.144  32.147  0.00  0.00            
+ATOM   1043  W   W   6 479     -14.052  -7.546  29.600  0.00  0.00            
+ATOM   1044  W   W   6 480       2.217   8.906  59.549  0.00  0.00            
+ATOM   1045  W   W   6 481     -12.612  17.132 -50.512  0.00  0.00            
+ATOM   1046  W   W   6 482       8.879  14.770  22.129  0.00  0.00            
+ATOM   1047  W   W   6 483      -1.133 -17.262  54.028  0.00  0.00            
+ATOM   1048  W   W   6 484       9.020   9.661 -70.538  0.00  0.00            
+ATOM   1049  W   W   6 485     -11.957 -12.749 -59.957  0.00  0.00            
+ATOM   1050  W   W   6 486     -16.308   0.308 -55.639  0.00  0.00            
+ATOM   1051  W   W   6 487       2.723   7.175 -52.486  0.00  0.00            
+ATOM   1052  W   W   6 488       6.371 -12.471  36.944  0.00  0.00            
+ATOM   1053  W   W   6 489      10.128   1.323  36.537  0.00  0.00            
+ATOM   1054  W   W   6 490      12.207 -17.646 -32.263  0.00  0.00            
+ATOM   1055  W   W   6 491      14.852 -15.334  46.207  0.00  0.00            
+ATOM   1056  W   W   6 492      -3.729 -12.864  32.161  0.00  0.00            
+ATOM   1057  W   W   6 493      -1.302 -15.704 -46.266  0.00  0.00            
+ATOM   1058  W   W   6 494      10.489  -2.335 -45.839  0.00  0.00            
+ATOM   1059  W   W   6 495      15.470 -17.995  36.635  0.00  0.00            
+ATOM   1060  W   W   6 496       3.507  17.990  55.852  0.00  0.00            
+ATOM   1061  W   W   6 497       2.712   0.653 -58.019  0.00  0.00            
+ATOM   1062  W   W   6 498       0.374 -13.616 -64.327  0.00  0.00            
+ATOM   1063  W   W   6 499     -11.233  -5.894 -41.660  0.00  0.00            
+ATOM   1064  W   W   6 500       4.903 -11.324 -28.887  0.00  0.00            
+ATOM   1065  W   W   6 501      -6.131 -16.041 -38.526  0.00  0.00            
+ATOM   1066  W   W   6 502      -7.086  -0.397 -64.072  0.00  0.00            
+ATOM   1067  W   W   6 503     -14.089   8.593 -45.950  0.00  0.00            
+ATOM   1068  W   W   6 504      -3.466   6.456  49.586  0.00  0.00            
+ATOM   1069  W   W   6 505       4.031 -16.444 -70.831  0.00  0.00            
+ATOM   1070  W   W   6 506     -10.335  13.639  40.612  0.00  0.00            
+ATOM   1071  W   W   6 507      10.215  -1.894  42.982  0.00  0.00            
+ATOM   1072  W   W   6 508     -13.406   4.495 -53.390  0.00  0.00            
+ATOM   1073  W   W   6 509      12.902  11.435 -48.208  0.00  0.00            
+ATOM   1074  W   W   6 510      -7.134   7.804 -51.673  0.00  0.00            
+ATOM   1075  W   W   6 511     -13.534  -2.381 -51.688  0.00  0.00            
+ATOM   1076  W   W   6 512       3.254  10.758 -37.414  0.00  0.00            
+ATOM   1077  W   W   6 513      14.790  11.378  23.691  0.00  0.00            
+ATOM   1078  W   W   6 514       2.466   0.765 -63.118  0.00  0.00            
+ATOM   1079  W   W   6 515       5.099   3.900 -49.126  0.00  0.00            
+ATOM   1080  W   W   6 516      -0.309  -4.833  35.598  0.00  0.00            
+ATOM   1081  W   W   6 517       0.319 -10.034  34.820  0.00  0.00            
+ATOM   1082  W   W   6 518      -6.172  -9.514 -60.057  0.00  0.00            
+ATOM   1083  W   W   6 519      -0.803  -8.576  39.676  0.00  0.00            
+ATOM   1084  W   W   6 520      -1.999 -10.033 -44.583  0.00  0.00            
+ATOM   1085  W   W   6 521      13.321 -15.660  55.674  0.00  0.00            
+ATOM   1086  W   W   6 522      -6.783  -2.723  28.401  0.00  0.00            
+ATOM   1087  W   W   6 523      16.999   9.415  35.834  0.00  0.00            
+ATOM   1088  W   W   6 524       5.924   2.251 -53.698  0.00  0.00            
+ATOM   1089  W   W   6 525       1.649  -4.038 -25.529  0.00  0.00            
+ATOM   1090  W   W   6 526     -14.976 -15.393 -49.889  0.00  0.00            
+ATOM   1091  W   W   6 527      -6.381  -6.763  25.433  0.00  0.00            
+ATOM   1092  W   W   6 528      -1.638   1.233 -71.122  0.00  0.00            
+ATOM   1093  W   W   6 529      11.547 -14.935  35.391  0.00  0.00            
+ATOM   1094  W   W   6 530       7.426  -8.559 -32.949  0.00  0.00            
+ATOM   1095  W   W   6 531      -6.070   3.828  53.472  0.00  0.00            
+ATOM   1096  W   W   6 532      -7.843   2.013 -59.195  0.00  0.00            
+ATOM   1097  W   W   6 533      12.649  -1.418 -19.281  0.00  0.00            
+ATOM   1098  W   W   6 534      -5.700 -17.583 -69.978  0.00  0.00            
+ATOM   1099  W   W   6 535       0.211 -10.588  29.559  0.00  0.00            
+ATOM   1100  W   W   6 536     -16.799   9.040  50.542  0.00  0.00            
+ATOM   1101  W   W   6 537     -12.703 -17.595 -29.375  0.00  0.00            
+ATOM   1102  W   W   6 538       5.507  -3.891  67.882  0.00  0.00            
+ATOM   1103  W   W   6 539       3.623  17.844  46.354  0.00  0.00            
+ATOM   1104  W   W   6 540     -17.401  -4.782 -43.982  0.00  0.00            
+ATOM   1105  W   W   6 541       6.628   1.328  65.011  0.00  0.00            
+ATOM   1106  W   W   6 542     -11.152  17.819  67.106  0.00  0.00            
+ATOM   1107  W   W   6 543     -16.773  15.509 -59.674  0.00  0.00            
+ATOM   1108  W   W   6 544      10.672 -15.796 -63.603  0.00  0.00            
+ATOM   1109  W   W   6 545      16.371 -16.451 -60.712  0.00  0.00            
+ATOM   1110  W   W   6 546      -7.381  -5.014 -71.003  0.00  0.00            
+ATOM   1111  W   W   6 547      15.809  -7.440 -50.634  0.00  0.00            
+ATOM   1112  W   W   6 548      -3.229 -16.738  35.996  0.00  0.00            
+ATOM   1113  W   W   6 549     -15.876  -8.479 -29.760  0.00  0.00            
+ATOM   1114  W   W   6 550     -18.376  13.890  37.953  0.00  0.00            
+ATOM   1115  W   W   6 551       8.377  16.829 -23.585  0.00  0.00            
+ATOM   1116  W   W   6 552      13.300  -6.374 -54.712  0.00  0.00            
+ATOM   1117  W   W   6 553     -18.141   6.575 -67.209  0.00  0.00            
+ATOM   1118  W   W   6 554     -14.376  -9.429  23.524  0.00  0.00            
+ATOM   1119  W   W   6 555       4.586  -4.655  51.783  0.00  0.00            
+ATOM   1120  W   W   6 556      10.175   5.555 -62.023  0.00  0.00            
+ATOM   1121  W   W   6 557      14.965  -2.888  24.904  0.00  0.00            
+ATOM   1122  W   W   6 558      -7.213   4.755  41.301  0.00  0.00            
+ATOM   1123  W   W   6 559       9.589 -15.361 -44.427  0.00  0.00            
+ATOM   1124  W   W   6 560      -7.783  -5.758  42.616  0.00  0.00            
+ATOM   1125  W   W   6 561      -1.839   0.064  27.949  0.00  0.00            
+ATOM   1126  W   W   6 562      13.653 -14.955  50.849  0.00  0.00            
+ATOM   1127  W   W   6 563      18.158  -0.502 -59.829  0.00  0.00            
+ATOM   1128  W   W   6 564      -5.381  18.203 -59.898  0.00  0.00            
+ATOM   1129  W   W   6 565      -6.884  -3.442  66.477  0.00  0.00            
+ATOM   1130  W   W   6 566       6.894  11.547 -31.707  0.00  0.00            
+ATOM   1131  W   W   6 567       4.300  14.238  58.962  0.00  0.00            
+ATOM   1132  W   W   6 568      16.784  -6.264 -31.214  0.00  0.00            
+ATOM   1133  W   W   6 569     -15.795   7.266 -50.323  0.00  0.00            
+ATOM   1134  W   W   6 570      17.568   0.575 -70.386  0.00  0.00            
+ATOM   1135  W   W   6 571      13.180  16.746  57.968  0.00  0.00            
+ATOM   1136  W   W   6 572     -15.642   0.062  44.335  0.00  0.00            
+ATOM   1137  W   W   6 573      15.070  -1.230 -33.335  0.00  0.00            
+ATOM   1138  W   W   6 574     -11.206  11.420  30.572  0.00  0.00            
+ATOM   1139  W   W   6 575      15.709   6.218 -50.114  0.00  0.00            
+ATOM   1140  W   W   6 576       2.487  12.418 -25.849  0.00  0.00            
+ATOM   1141  W   W   6 577     -15.764   0.276  62.549  0.00  0.00            
+ATOM   1142  W   W   6 578      -9.873   8.230  53.301  0.00  0.00            
+ATOM   1143  W   W   6 579       4.039  15.912  41.591  0.00  0.00            
+ATOM   1144  W   W   6 580      17.657   8.831 -40.850  0.00  0.00            
+ATOM   1145  W   W   6 581     -11.207  12.989 -17.837  0.00  0.00            
+ATOM   1146  W   W   6 582     -12.044   3.448  65.099  0.00  0.00            
+ATOM   1147  W   W   6 583      12.537   0.104 -37.183  0.00  0.00            
+ATOM   1148  W   W   6 584     -11.561  10.173 -50.272  0.00  0.00            
+ATOM   1149  W   W   6 585       9.275 -13.650  67.390  0.00  0.00            
+ATOM   1150  W   W   6 586      -7.897   8.261 -28.229  0.00  0.00            
+ATOM   1151  W   W   6 587       7.419 -18.064  43.905  0.00  0.00            
+ATOM   1152  W   W   6 588      -9.125   0.683  68.765  0.00  0.00            
+ATOM   1153  W   W   6 589     -15.107  -7.108  50.306  0.00  0.00            
+ATOM   1154  W   W   6 590      -3.136  14.773 -69.463  0.00  0.00            
+ATOM   1155  W   W   6 591     -16.291   6.368  54.833  0.00  0.00            
+ATOM   1156  W   W   6 592     -17.790 -13.342 -58.105  0.00  0.00            
+ATOM   1157  W   W   6 593     -10.631 -13.500  30.193  0.00  0.00            
+ATOM   1158  W   W   6 594      -1.011 -16.528 -51.628  0.00  0.00            
+ATOM   1159  W   W   6 595      -5.458   3.200  45.499  0.00  0.00            
+ATOM   1160  W   W   6 596      -4.287  -1.733 -68.173  0.00  0.00            
+ATOM   1161  W   W   6 597      -8.020 -10.030  34.248  0.00  0.00            
+ATOM   1162  W   W   6 598      13.002  -3.951 -59.639  0.00  0.00            
+ATOM   1163  W   W   6 599     -14.796   5.311 -32.864  0.00  0.00            
+ATOM   1164  W   W   6 600      17.129   5.619  32.267  0.00  0.00            
+ATOM   1165  W   W   6 601     -12.672   0.391  72.971  0.00  0.00            
+ATOM   1166  W   W   6 602      -5.514  -8.320  65.312  0.00  0.00            
+ATOM   1167  W   W   6 603      11.871  17.222  44.531  0.00  0.00            
+ATOM   1168  W   W   6 604     -13.923  -9.934  63.947  0.00  0.00            
+ATOM   1169  W   W   6 605      -8.524 -15.269  41.525  0.00  0.00            
+ATOM   1170  W   W   6 606       8.266  16.219  67.644  0.00  0.00            
+ATOM   1171  W   W   6 607      14.351 -12.887 -32.373  0.00  0.00            
+ATOM   1172  W   W   6 608      12.696   5.151  59.189  0.00  0.00            
+ATOM   1173  W   W   6 609      10.892  14.267 -30.651  0.00  0.00            
+ATOM   1174  W   W   6 610     -16.318   5.398  46.993  0.00  0.00            
+ATOM   1175  W   W   6 611     -10.615 -14.204  46.228  0.00  0.00            
+ATOM   1176  W   W   6 612      -1.800  -2.907 -34.390  0.00  0.00            
+ATOM   1177  W   W   6 613     -13.272  10.824  61.160  0.00  0.00            
+ATOM   1178  W   W   6 614       1.932  16.627  28.276  0.00  0.00            
+ATOM   1179  W   W   6 615       0.281   3.184  52.744  0.00  0.00            
+ATOM   1180  W   W   6 616      -1.465 -17.082 -56.851  0.00  0.00            
+ATOM   1181  W   W   6 617      11.315  13.770 -21.336  0.00  0.00            
+ATOM   1182  W   W   6 618      12.214   9.036 -64.912  0.00  0.00            
+ATOM   1183  W   W   6 619      14.641  13.878  49.352  0.00  0.00            
+ATOM   1184  W   W   6 620      15.763  16.139  67.325  0.00  0.00            
+ATOM   1185  W   W   6 621      -6.669  -3.667 -33.773  0.00  0.00            
+ATOM   1186  W   W   6 622       8.024  -1.562 -37.508  0.00  0.00            
+ATOM   1187  W   W   6 623     -17.296  -3.314  33.691  0.00  0.00            
+ATOM   1188  W   W   6 624      14.225  -1.750  34.435  0.00  0.00            
+ATOM   1189  W   W   6 625       6.719  -7.879 -66.512  0.00  0.00            
+ATOM   1190  W   W   6 626      13.846   2.648 -29.483  0.00  0.00            
+ATOM   1191  W   W   6 627      -1.397  -4.845 -45.831  0.00  0.00            
+ATOM   1192  W   W   6 628       3.556  14.691  63.860  0.00  0.00            
+ATOM   1193  W   W   6 629      -9.796  10.197 -73.022  0.00  0.00            
+ATOM   1194  W   W   6 630      -9.401  -1.688  32.462  0.00  0.00            
+ATOM   1195  W   W   6 631       9.583  10.956  67.616  0.00  0.00            
+ATOM   1196  W   W   6 632     -16.756 -12.712 -63.044  0.00  0.00            
+ATOM   1197  W   W   6 633       5.093  -2.271 -33.569  0.00  0.00            
+ATOM   1198  W   W   6 634      -7.809  -0.835  46.448  0.00  0.00            
+ATOM   1199  W   W   6 635      -9.933   3.903 -34.973  0.00  0.00            
+ATOM   1200  W   W   6 636       1.297  -3.904 -38.170  0.00  0.00            
+ATOM   1201  W   W   6 637     -11.351   7.240  48.175  0.00  0.00            
+ATOM   1202  W   W   6 638      10.025 -11.848 -47.822  0.00  0.00            
+ATOM   1203  W   W   6 639      -3.352  11.020  36.829  0.00  0.00            
+ATOM   1204  W   W   6 640      -8.557  -7.019  30.596  0.00  0.00            
+ATOM   1205  W   W   6 641       2.266  -7.468  69.379  0.00  0.00            
+ATOM   1206  W   W   6 642      13.947   7.636  66.666  0.00  0.00            
+ATOM   1207  W   W   6 643      -1.974 -16.632  48.430  0.00  0.00            
+ATOM   1208  W   W   6 644       3.799 -14.306  57.656  0.00  0.00            
+ATOM   1209  W   W   6 645      -6.197  14.741  34.682  0.00  0.00            
+ATOM   1210  W   W   6 646     -10.631   8.184  42.560  0.00  0.00            
+ATOM   1211  W   W   6 647      14.778  15.596  72.973  0.00  0.00            
+ATOM   1212  W   W   6 648       4.834   5.157 -62.085  0.00  0.00            
+ATOM   1213  W   W   6 649      13.656  17.896 -22.670  0.00  0.00            
+ATOM   1214  W   W   6 650       9.531  -1.115  32.515  0.00  0.00            
+ATOM   1215  W   W   6 651      13.499 -11.477  32.602  0.00  0.00            
+ATOM   1216  W   W   6 652     -15.546  -6.855 -62.424  0.00  0.00            
+ATOM   1217  W   W   6 653     -10.560  -0.988  56.857  0.00  0.00            
+ATOM   1218  W   W   6 654      17.244  -3.915  38.410  0.00  0.00            
+ATOM   1219  W   W   6 655      -5.245  12.525  42.435  0.00  0.00            
+ATOM   1220  W   W   6 656      14.797   0.469  60.344  0.00  0.00            
+ATOM   1221  W   W   6 657     -11.684  -5.139  26.344  0.00  0.00            
+ATOM   1222  W   W   6 658       4.971  -9.786  55.820  0.00  0.00            
+ATOM   1223  W   W   6 659      -6.725  -7.870  60.303  0.00  0.00            
+ATOM   1224  W   W   6 660      15.636  -4.198  61.609  0.00  0.00            
+ATOM   1225  W   W   6 661      16.028  15.656 -30.795  0.00  0.00            
+ATOM   1226  W   W   6 662      12.422 -17.459  30.827  0.00  0.00            
+ATOM   1227  W   W   6 663       6.951  16.375 -72.838  0.00  0.00            
+ATOM   1228  W   W   6 664     -16.352 -11.201 -24.403  0.00  0.00            
+ATOM   1229  W   W   6 665       5.211  -0.170  59.084  0.00  0.00            
+ATOM   1230  W   W   6 666     -13.500   9.188  66.218  0.00  0.00            
+ATOM   1231  W   W   6 667      11.820   4.766 -18.126  0.00  0.00            
+ATOM   1232  W   W   6 668       0.966  17.533  38.556  0.00  0.00            
+ATOM   1233  W   W   6 669      -7.368   6.115  58.803  0.00  0.00            
+ATOM   1234  W   W   6 670     -15.187  12.300 -25.958  0.00  0.00            
+ATOM   1235  W   W   6 671       6.798  -5.350  41.351  0.00  0.00            
+ATOM   1236  W   W   6 672      -6.029   4.209 -69.062  0.00  0.00            
+ATOM   1237  W   W   6 673      -4.336  12.024  31.089  0.00  0.00            
+ATOM   1238  W   W   6 674       6.489  17.170 -45.016  0.00  0.00            
+ATOM   1239  W   W   6 675      -8.065  14.396 -57.533  0.00  0.00            
+ATOM   1240  W   W   6 676       1.091  -6.462  54.637  0.00  0.00            
+ATOM   1241  W   W   6 677       1.993  10.870 -31.581  0.00  0.00            
+ATOM   1242  W   W   6 678     -11.787  -6.245  34.232  0.00  0.00            
+ATOM   1243  W   W   6 679     -15.539   2.381  30.225  0.00  0.00            
+ATOM   1244  W   W   6 680      -3.262  -0.018 -20.180  0.00  0.00            
+ATOM   1245  W   W   6 681      15.783 -13.098 -38.061  0.00  0.00            
+ATOM   1246  W   W   6 682       2.038  -5.477  31.386  0.00  0.00            
+ATOM   1247  W   W   6 683      -2.733  -9.742 -63.841  0.00  0.00            
+ATOM   1248  W   W   6 684      -2.003  14.176 -63.653  0.00  0.00            
+ATOM   1249  W   W   6 685     -12.489   7.148  58.077  0.00  0.00            
+ATOM   1250  W   W   6 686      13.140  -1.972  65.096  0.00  0.00            
+ATOM   1251  W   W   6 687      12.847   2.440  72.911  0.00  0.00            
+ATOM   1252  W   W   6 688      12.700  12.246 -61.224  0.00  0.00            
+ATOM   1253  W   W   6 689     -15.388 -13.392  67.591  0.00  0.00            
+ATOM   1254  W   W   6 690      12.656   6.592 -70.405  0.00  0.00            
+ATOM   1255  W   W   6 691     -10.811   2.555  60.398  0.00  0.00            
+ATOM   1256  W   W   6 692       8.264   4.574 -57.739  0.00  0.00            
+ATOM   1257  W   W   6 693      -4.758   4.189 -42.323  0.00  0.00            
+ATOM   1258  W   W   6 694      -3.951  15.152  53.674  0.00  0.00            
+ATOM   1259  W   W   6 695       3.673  -9.404  21.746  0.00  0.00            
+ATOM   1260  W   W   6 696     -15.427   6.526  62.256  0.00  0.00            
+ATOM   1261  W   W   6 697     -17.889 -17.442  49.679  0.00  0.00            
+ATOM   1262  W   W   6 698     -17.093 -11.056 -50.451  0.00  0.00            
+ATOM   1263  W   W   6 699     -17.417  -3.734  27.027  0.00  0.00            
+ATOM   1264  W   W   6 700       5.454 -16.824  38.931  0.00  0.00            
+ATOM   1265  W   W   6 701       6.447   6.502  65.026  0.00  0.00            
+ATOM   1266  W   W   6 702       6.977   1.865  44.259  0.00  0.00            
+ATOM   1267  W   W   6 703      18.100  15.385  57.847  0.00  0.00            
+ATOM   1268  W   W   6 704      -5.647   1.313  58.827  0.00  0.00            
+ATOM   1269  W   W   6 705      16.737   0.134 -64.779  0.00  0.00            
+ATOM   1270  W   W   6 706       9.278   6.478 -30.884  0.00  0.00            
+ATOM   1271  W   W   6 707      -6.030   2.791  27.090  0.00  0.00            
+ATOM   1272  W   W   6 708      17.644  -5.068 -57.433  0.00  0.00            
+ATOM   1273  W   W   6 709      -6.876   8.898  45.942  0.00  0.00            
+ATOM   1274  W   W   6 710       2.249   0.456  68.086  0.00  0.00            
+ATOM   1275  W   W   6 711     -11.849   2.253 -24.415  0.00  0.00            
+ATOM   1276  W   W   6 712      -0.169  11.218 -54.270  0.00  0.00            
+ATOM   1277  W   W   6 713      -8.594  18.167  62.426  0.00  0.00            
+ATOM   1278  W   W   6 714       1.462   7.682  53.841  0.00  0.00            
+ATOM   1279  W   W   6 715       7.020   9.407  71.652  0.00  0.00            
+ATOM   1280  W   W   6 716      10.682  -0.181 -32.609  0.00  0.00            
+ATOM   1281  W   W   6 717     -12.744 -15.559  63.493  0.00  0.00            
+ATOM   1282  W   W   6 718      12.091  -7.156  63.773  0.00  0.00            
+ATOM   1283  W   W   6 719       0.933  16.515  50.642  0.00  0.00            
+ATOM   1284  W   W   6 720     -17.878  10.586 -70.644  0.00  0.00            
+ATOM   1285  W   W   6 721     -10.574 -16.466 -47.602  0.00  0.00            
+ATOM   1286  W   W   6 722       1.438  -1.981 -42.579  0.00  0.00            
+ATOM   1287  W   W   6 723       5.950  18.148  25.035  0.00  0.00            
+ATOM   1288  W   W   6 724      -8.644  -7.649 -47.741  0.00  0.00            
+ATOM   1289  W   W   6 725     -16.869  -8.189  36.161  0.00  0.00            
+ATOM   1290  W   W   6 726      15.303 -12.525 -73.301  0.00  0.00            
+ATOM   1291  W   W   6 727       0.701 -11.945 -70.015  0.00  0.00            
+ATOM   1292  W   W   6 728      14.819 -17.282 -27.377  0.00  0.00            
+ATOM   1293  W   W   6 729       3.432 -10.502  50.631  0.00  0.00            
+ATOM   1294  W   W   6 730      16.049  -2.642 -39.202  0.00  0.00            
+ATOM   1295  W   W   6 731       3.112   9.637 -42.148  0.00  0.00            
+ATOM   1296  W   W   6 732      -1.294  -2.215 -55.664  0.00  0.00            
+ATOM   1297  W   W   6 733       6.596   0.891  70.986  0.00  0.00            
+ATOM   1298  W   W   6 734     -10.367   8.294  26.204  0.00  0.00            
+ATOM   1299  W   W   6 735       5.972  -7.380 -25.238  0.00  0.00            
+ATOM   1300  W   W   6 736      -3.889 -12.059  62.324  0.00  0.00            
+ATOM   1301  W   W   6 737      -1.867  16.456  70.471  0.00  0.00            
+ATOM   1302  W   W   6 738      18.404  10.766  67.069  0.00  0.00            
+ATOM   1303  W   W   6 739      -9.262 -17.638 -24.870  0.00  0.00            
+ATOM   1304  W   W   6 740       3.183   1.920  48.235  0.00  0.00            
+ATOM   1305  W   W   6 741      -5.476 -11.502  68.955  0.00  0.00            
+ATOM   1306  W   W   6 742      14.181  11.686  69.596  0.00  0.00            
+ATOM   1307  W   W   6 743       4.205  18.314 -25.969  0.00  0.00            
+ATOM   1308  W   W   6 744      -6.941   2.167  63.833  0.00  0.00            
+ATOM   1309  W   W   6 745      14.426 -16.609  26.331  0.00  0.00            
+ATOM   1310  W   W   6 746      16.943 -18.055 -51.006  0.00  0.00            
+ATOM   1311  W   W   6 747      12.265  10.010  33.747  0.00  0.00            
+ATOM   1312  W   W   6 748     -13.288  -9.365  71.766  0.00  0.00            
+ATOM   1313  W   W   6 749       8.233 -16.286 -57.311  0.00  0.00            
+ATOM   1314  W   W   6 750      12.966  15.264 -51.649  0.00  0.00            
+ATOM   1315  W   W   6 751     -14.110   1.092 -68.751  0.00  0.00            
+ATOM   1316  W   W   6 752       6.808  11.291  45.071  0.00  0.00            
+ATOM   1317  W   W   6 753       8.162  -8.231  50.119  0.00  0.00            
+ATOM   1318  W   W   6 754       9.856 -17.259  60.102  0.00  0.00            
+ATOM   1319  W   W   6 755      15.140  -6.902  35.101  0.00  0.00            
+ATOM   1320  W   W   6 756       3.216 -12.480 -33.402  0.00  0.00            
+ATOM   1321  W   W   6 757      15.935  17.706  41.385  0.00  0.00            
+ATOM   1322  W   W   6 758     -17.774   9.876  58.293  0.00  0.00            
+ATOM   1323  W   W   6 759      -3.576 -16.046  40.845  0.00  0.00            
+ATOM   1324  W   W   6 760      -1.747   2.666  66.097  0.00  0.00            
+ATOM   1325  W   W   6 761      13.916 -11.012  27.753  0.00  0.00            
+ATOM   1326  W   W   6 762      -6.592   5.597 -56.146  0.00  0.00            
+ATOM   1327  W   W   6 763       2.036  -6.812 -42.801  0.00  0.00            
+ATOM   1328  W   W   6 764     -17.914   9.829  41.244  0.00  0.00            
+ATOM   1329  W   W   6 765     -11.040  -7.825  57.699  0.00  0.00            
+ATOM   1330  W   W   6 766      10.389  18.104 -27.651  0.00  0.00            
+ATOM   1331  W   W   6 767     -10.816  -4.989  52.355  0.00  0.00            
+ATOM   1332  W   W   6 768     -12.276  16.346 -42.386  0.00  0.00            
+ATOM   1333  W   W   6 769      13.614  16.489  21.589  0.00  0.00            
+ATOM   1334  W   W   6 770       6.527 -15.428  71.235  0.00  0.00            
+ATOM   1335  W   W   6 771      16.026  -5.878  47.246  0.00  0.00            
+ATOM   1336  W   W   6 772       8.035  13.441  30.522  0.00  0.00            
+ATOM   1337  W   W   6 773      10.148   0.726 -16.070  0.00  0.00            
+ATOM   1338  W   W   6 774       9.232 -12.090  57.837  0.00  0.00            
+ATOM   1339  W   W   6 775     -13.442  10.409  38.648  0.00  0.00            
+ATOM   1340  W   W   6 776       5.100  -1.173  30.117  0.00  0.00            
+ATOM   1341  W   W   6 777      18.280 -11.863  58.711  0.00  0.00            
+ATOM   1342  W   W   6 778      -0.978  16.178  32.849  0.00  0.00            
+ATOM   1343  W   W   6 779      -1.640 -12.191  50.130  0.00  0.00            
+ATOM   1344  W   W   6 780     -15.970  -5.483  64.682  0.00  0.00            
+ATOM   1345  W   W   6 781       9.156   5.942 -25.966  0.00  0.00            
+ATOM   1346  W   W   6 782       7.689  -1.238 -69.863  0.00  0.00            
+ATOM   1347  W   W   6 783      14.999  12.788  42.679  0.00  0.00            
+ATOM   1348  W   W   6 784      -0.987   7.763 -44.439  0.00  0.00            
+ATOM   1349  W   W   6 785      -5.774  -9.724  48.947  0.00  0.00            
+ATOM   1350  W   W   6 786      -8.797  13.782 -69.368  0.00  0.00            
+ATOM   1351  W   W   6 787       3.552  -2.935 -52.082  0.00  0.00            
+ATOM   1352  W   W   6 788      13.642  -6.467  52.007  0.00  0.00            
+ATOM   1353  W   W   6 789      12.986  16.136 -39.178  0.00  0.00            
+ATOM   1354  W   W   6 790      15.008 -14.093 -23.374  0.00  0.00            
+ATOM   1355  W   W   6 791      16.301  -1.580  44.361  0.00  0.00            
+ATOM   1356  W   W   6 792       2.083  -1.645  63.040  0.00  0.00            
+ATOM   1357  W   W   6 793       1.949  -0.004  43.618  0.00  0.00            
+ATOM   1358  W   W   6 794      -7.487   7.940 -23.183  0.00  0.00            
+ATOM   1359  W   W   6 795      -2.221  -8.642  58.291  0.00  0.00            
+ATOM   1360  W   W   6 796     -10.711 -18.351 -71.885  0.00  0.00            
+ATOM   1361  W   W   6 797      -3.983  -2.002  18.855  0.00  0.00            
+ATOM   1362  W   W   6 798      -9.039   2.278 -45.456  0.00  0.00            
+ATOM   1363  W   W   6 799       3.212 -14.111 -60.087  0.00  0.00            
+ATOM   1364  W   W   6 800       7.377  15.346  54.463  0.00  0.00            
+ATOM   1365  W   W   6 801      -8.270  -1.355 -41.761  0.00  0.00            
+ATOM   1366  W   W   6 802      14.303 -11.675 -44.105  0.00  0.00            
+ATOM   1367  W   W   6 803      13.542  -6.068  40.945  0.00  0.00            
+ATOM   1368  W   W   6 804      12.290 -10.475  48.638  0.00  0.00            
+ATOM   1369  W   W   6 805      18.090   1.517  34.871  0.00  0.00            
+ATOM   1370  W   W   6 806      12.734   3.618 -23.066  0.00  0.00            
+ATOM   1371  W   W   6 807     -11.049   4.838  29.732  0.00  0.00            
+ATOM   1372  W   W   6 808      17.531  11.624 -28.456  0.00  0.00            
+ATOM   1373  W   W   6 809     -11.959  -7.237 -26.149  0.00  0.00            
+ATOM   1374  W   W   6 810     -15.246 -17.339 -61.613  0.00  0.00            
+ATOM   1375  W   W   6 811      -1.402  16.222 -48.152  0.00  0.00            
+ATOM   1376  W   W   6 812       5.889  18.426 -61.806  0.00  0.00            
+ATOM   1377  W   W   6 813      -6.061 -11.877 -46.514  0.00  0.00            
+ATOM   1378  W   W   6 814      17.926  -1.283 -28.927  0.00  0.00            
+ATOM   1379  W   W   6 815      12.943  -7.377 -63.415  0.00  0.00            
+ATOM   1380  W   W   6 816       7.421 -17.509 -35.010  0.00  0.00            
+ATOM   1381  W   W   6 817       8.900   9.521 -18.634  0.00  0.00            
+ATOM   1382  W   W   6 818       1.829  13.998 -44.859  0.00  0.00            
+ATOM   1383  W   W   6 819     -11.859  16.207 -33.004  0.00  0.00            
+ATOM   1384  W   W   6 820      14.986  -8.387 -69.946  0.00  0.00            
+ATOM   1385  W   W   6 821      -4.050  -3.110  32.429  0.00  0.00            
+ATOM   1386  W   W   6 822      -8.366   2.754 -50.786  0.00  0.00            
+ATOM   1387  W   W   6 823       0.823  16.945 -71.859  0.00  0.00            
+ATOM   1388  W   W   6 824     -15.649  15.599  25.729  0.00  0.00            
+ATOM   1389  W   W   6 825      10.054   9.866  38.859  0.00  0.00            
+ATOM   1390  W   W   6 826      -1.984  -6.222  62.733  0.00  0.00            
+ATOM   1391  W   W   6 827      16.301  -6.942  71.189  0.00  0.00            
+ATOM   1392  W   W   6 828     -15.693  10.299 -54.375  0.00  0.00            
+ATOM   1393  W   W   6 829       7.805 -14.675 -26.072  0.00  0.00            
+ATOM   1394  W   W   6 830      -2.319 -13.150 -59.968  0.00  0.00            
+ATOM   1395  W   W   6 831      -4.415  -8.566 -32.653  0.00  0.00            
+ATOM   1396  W   W   6 832      -7.013 -16.921  21.234  0.00  0.00            
+ATOM   1397  W   W   6 833      11.022  16.528  26.713  0.00  0.00            
+ATOM   1398  W   W   6 834      -7.477  -8.500 -67.048  0.00  0.00            
+ATOM   1399  W   W   6 835      -0.321 -16.057  30.182  0.00  0.00            
+ATOM   1400  W   W   6 836     -16.337  14.852  42.746  0.00  0.00            
+ATOM   1401  W   W   6 837       7.114  13.612 -27.467  0.00  0.00            
+ATOM   1402  W   W   6 838      -8.820  -3.196 -50.889  0.00  0.00            
+ATOM   1403  W   W   6 839      -4.454  13.846  62.009  0.00  0.00            
+ATOM   1404  W   W   6 840      -5.456   7.194  24.261  0.00  0.00            
+ATOM   1405  W   W   6 841      16.420  17.173  53.257  0.00  0.00            
+ATOM   1406  W   W   6 842       7.085  -6.566 -71.190  0.00  0.00            
+ATOM   1407  W   W   6 843     -12.984   9.294 -21.126  0.00  0.00            
+ATOM   1408  W   W   6 844       2.526   3.147 -35.754  0.00  0.00            
+ATOM   1409  W   W   6 845       6.010  10.063 -61.965  0.00  0.00            
+ATOM   1410  W   W   6 846     -14.025  10.732  54.684  0.00  0.00            
+ATOM   1411  W   W   6 847      11.346  17.783  51.321  0.00  0.00            
+ATOM   1412  W   W   6 848     -14.899   6.095 -72.369  0.00  0.00            
+ATOM   1413  W   W   6 849      12.465  -1.794 -63.969  0.00  0.00            
+ATOM   1414  W   W   6 850      17.115   9.087 -63.085  0.00  0.00            
+ATOM   1415  W   W   6 851     -13.038 -10.043 -66.403  0.00  0.00            
+ATOM   1416  W   W   6 852       8.554   0.208 -21.629  0.00  0.00            
+ATOM   1417  W   W   6 853     -11.653  -7.295 -51.599  0.00  0.00            
+ATOM   1418  W   W   6 854      -4.722   9.346 -40.733  0.00  0.00            
+ATOM   1419  W   W   6 855     -17.771  -6.466  43.189  0.00  0.00            
+ATOM   1420  W   W   6 856      11.228  -5.127 -33.468  0.00  0.00            
+ATOM   1421  W   W   6 857      -7.253  -5.215  55.648  0.00  0.00            
+ATOM   1422  W   W   6 858      11.368  -0.457  69.635  0.00  0.00            
+ATOM   1423  W   W   6 859       7.952   3.486  55.754  0.00  0.00            
+ATOM   1424  W   W   6 860       5.289  -9.876 -55.742  0.00  0.00            
+ATOM   1425  W   W   6 861      17.255   4.968  51.003  0.00  0.00            
+ATOM   1426  W   W   6 862      -5.814  17.034 -54.098  0.00  0.00            
+ATOM   1427  W   W   6 863      15.093  12.674 -42.782  0.00  0.00            
+ATOM   1428  W   W   6 864     -10.651   3.683  55.406  0.00  0.00            
+ATOM   1429  W   W   6 865     -15.205  17.823 -46.121  0.00  0.00            
+ATOM   1430  W   W   6 866       0.856  16.696 -30.053  0.00  0.00            
+ATOM   1431  W   W   6 867     -17.534  12.280  21.201  0.00  0.00            
+ATOM   1432  W   W   6 868     -12.086  12.992 -46.385  0.00  0.00            
+ATOM   1433  W   W   6 869       0.570 -11.822  54.677  0.00  0.00            
+ATOM   1434  W   W   6 870      -3.013  -2.864  24.073  0.00  0.00            
+ATOM   1435  W   W   6 871      -5.971  -0.386 -54.023  0.00  0.00            
+ATOM   1436  W   W   6 872      15.785  17.648  62.390  0.00  0.00            
+ATOM   1437  W   W   6 873      17.939  15.543 -24.191  0.00  0.00            
+ATOM   1438  W   W   6 874     -10.749   8.658 -55.087  0.00  0.00            
+ATOM   1439  W   W   6 875       1.756   4.747 -29.621  0.00  0.00            
+ATOM   1440  W   W   6 876       1.668 -13.829 -55.086  0.00  0.00            
+ATOM   1441  W   W   6 877     -15.718  13.309 -50.274  0.00  0.00            
+ATOM   1442  W   W   6 878      -9.993  -8.777  20.961  0.00  0.00            
+ATOM   1443  W   W   6 879     -17.123   8.028 -36.667  0.00  0.00            
+ATOM   1444  W   W   6 880      -1.598 -12.851 -22.916  0.00  0.00            
+ATOM   1445  W   W   6 881      -7.542  -5.298 -38.508  0.00  0.00            
+ATOM   1446  W   W   6 882     -15.887  15.249 -29.903  0.00  0.00            
+ATOM   1447  W   W   6 883      14.962 -12.142 -64.516  0.00  0.00            
+ATOM   1448  W   W   6 884      -7.117 -12.831 -63.795  0.00  0.00            
+ATOM   1449  W   W   6 885       9.724  15.024  62.513  0.00  0.00            
+ATOM   1450  W   W   6 886       5.358 -16.652  66.065  0.00  0.00            
+ATOM   1451  W   W   6 887      10.471  -5.527 -67.736  0.00  0.00            
+ATOM   1452  W   W   6 888     -13.329  16.575  62.401  0.00  0.00            
+ATOM   1453  W   W   6 889       0.034  17.595  66.228  0.00  0.00            
+ATOM   1454  W   W   6 890       0.649 -15.215  43.828  0.00  0.00            
+ATOM   1455  W   W   6 891       1.291  -0.085  38.126  0.00  0.00            
+ATOM   1456  W   W   6 892      -8.913 -12.229  62.480  0.00  0.00            
+ATOM   1457  W   W   6 893      15.337  -4.350 -46.230  0.00  0.00            
+ATOM   1458  W   W   6 894     -12.245  -1.365  48.760  0.00  0.00            
+ATOM   1459  W   W   6 895     -18.090  -9.653 -45.341  0.00  0.00            
+ATOM   1460  W   W   6 896      10.857 -10.776 -53.807  0.00  0.00            
+ATOM   1461  W   W   6 897      -9.774 -16.305 -53.376  0.00  0.00            
+ATOM   1462  W   W   6 898       2.614  11.534  34.894  0.00  0.00            
+ATOM   1463  W   W   6 899      -6.909  12.739 -26.956  0.00  0.00            
+ATOM   1464  W   W   6 900      16.238  15.707 -63.232  0.00  0.00            
+ATOM   1465  W   W   6 901     -13.834  16.021  30.351  0.00  0.00            
+ATOM   1466  W   W   6 902      13.307   2.968  31.543  0.00  0.00            
+ATOM   1467  W   W   6 903       1.700 -15.704  71.650  0.00  0.00            
+ATOM   1468  W   W   6 904     -14.578  12.553 -38.644  0.00  0.00            
+ATOM   1469  W   W   6 905      -8.967   7.455  34.077  0.00  0.00            
+ATOM   1470  W   W   6 906      17.491 -12.585  25.032  0.00  0.00            
+ATOM   1471  W   W   6 907      10.777  -3.738  16.749  0.00  0.00            
+ATOM   1472  W   W   6 908      13.349  13.277  38.153  0.00  0.00            
+ATOM   1473  W   W   6 909     -12.069  12.698 -65.754  0.00  0.00            
+ATOM   1474  W   W   6 910      -0.668 -10.389  72.112  0.00  0.00            
+ATOM   1475  W   W   6 911      -9.478  10.351  68.741  0.00  0.00            
+ATOM   1476  W   W   6 912     -14.342 -12.775 -45.385  0.00  0.00            
+ATOM   1477  W   W   6 913     -15.461  18.156  54.248  0.00  0.00            
+ATOM   1478  W   W   6 914       2.593 -17.314 -34.164  0.00  0.00            
+ATOM   1479  W   W   6 915      -0.678  13.634  25.043  0.00  0.00            
+ATOM   1480  W   W   6 916       9.691 -15.670  47.643  0.00  0.00            
+ATOM   1481  W   W   6 917       2.739  -5.192 -56.351  0.00  0.00            
+ATOM   1482  W   W   6 918      11.870 -16.328 -52.432  0.00  0.00            
+ATOM   1483  W   W   6 919      -7.511  -1.247 -26.477  0.00  0.00            
+ATOM   1484  W   W   6 920     -13.799  -1.018 -27.868  0.00  0.00            
+ATOM   1485  W   W   6 921      17.261 -17.000 -65.712  0.00  0.00            
+ATOM   1486  W   W   6 922      17.927  -8.575  30.954  0.00  0.00            
+ATOM   1487  W   W   6 923      -2.625  -1.677  44.920  0.00  0.00            
+ATOM   1488  W   W   6 924       1.581  12.918 -49.576  0.00  0.00            
+ATOM   1489  W   W   6 925      13.659  -2.911 -72.003  0.00  0.00            
+ATOM   1490  W   W   6 926      -2.739  -4.102  40.936  0.00  0.00            
+ATOM   1491  W   W   6 927       3.582  12.627 -72.536  0.00  0.00            
+ATOM   1492  W   W   6 928      17.997  17.500  30.265  0.00  0.00            
+ATOM   1493  W   W   6 929       5.897  -2.749  46.892  0.00  0.00            
+ATOM   1494  W   W   6 930      16.907   2.489  21.899  0.00  0.00            
+ATOM   1495  W   W   6 931      -8.828  17.809  38.427  0.00  0.00            
+ATOM   1496  W   W   6 932      14.201  -0.897  51.416  0.00  0.00            
+ATOM   1497  W   W   6 933      -1.470   8.315  33.006  0.00  0.00            
+ATOM   1498  W   W   6 934     -10.507   8.339 -33.007  0.00  0.00            
+ATOM   1499  W   W   6 935      10.100  -6.560 -48.837  0.00  0.00            
+ATOM   1500  W   W   6 936       4.265   7.737 -71.069  0.00  0.00            
+ATOM   1501  W   W   6 937      -0.978 -16.648 -68.724  0.00  0.00            
+ATOM   1502  W   W   6 938      10.067  -3.150  51.691  0.00  0.00            
+ATOM   1503  W   W   6 939       2.054   8.007  48.866  0.00  0.00            
+ATOM   1504  W   W   6 940      10.592  18.415  39.399  0.00  0.00            
+ATOM   1505  W   W   6 941     -15.140 -12.297  27.779  0.00  0.00            
+ATOM   1506  W   W   6 942     -17.612 -16.597 -25.545  0.00  0.00            
+ATOM   1507  W   W   6 943      -3.237 -12.178 -29.381  0.00  0.00            
+ATOM   1508  W   W   6 944     -15.731 -17.631 -71.461  0.00  0.00            
+ATOM   1509  W   W   6 945       6.106   5.670  51.620  0.00  0.00            
+ATOM   1510  W   W   6 946      10.494 -12.479  72.308  0.00  0.00            
+ATOM   1511  W   W   6 947      15.924   2.408  55.234  0.00  0.00            
+ATOM   1512  W   W   6 948     -13.395 -11.309  33.862  0.00  0.00            
+ATOM   1513  W   W   6 949      15.502 -16.920 -70.739  0.00  0.00            
+ATOM   1514  W   W   6 950       8.475   9.622 -43.295  0.00  0.00            
+ATOM   1515  W   W   6 951       5.748  -3.924 -41.270  0.00  0.00            
+ATOM   1516  W   W   6 952      10.199  -6.951  45.509  0.00  0.00            
+ATOM   1517  W   W   6 953      -0.636   7.129 -38.531  0.00  0.00            
+ATOM   1518  W   W   6 954     -12.053  18.225  22.206  0.00  0.00            
+ATOM   1519  W   W   6 955      -6.725  17.757 -34.717  0.00  0.00            
+ATOM   1520  W   W   6 956     -17.573   2.613  71.574  0.00  0.00            
+ATOM   1521  W   W   6 957       9.935   7.277  43.390  0.00  0.00            
+ATOM   1522  W   W   6 958     -10.717  17.820  33.571  0.00  0.00            
+ATOM   1523  W   W   6 959      -4.016  -7.860 -54.086  0.00  0.00            
+ATOM   1524  W   W   6 960       3.767   4.060  22.497  0.00  0.00            
+ATOM   1525  W   W   6 961     -12.070   7.236 -25.528  0.00  0.00            
+ATOM   1526  W   W   6 962      12.365 -12.668  23.450  0.00  0.00            
+ATOM   1527  W   W   6 963      14.390 -14.542  61.153  0.00  0.00            
+ATOM   1528  W   W   6 964      -5.209   2.057  32.927  0.00  0.00            
+ATOM   1529  W   W   6 965       9.161  12.258  58.368  0.00  0.00            
+ATOM   1530  W   W   6 966      -2.335 -16.586 -26.428  0.00  0.00            
+ATOM   1531  W   W   6 967     -15.318 -10.276  54.734  0.00  0.00            
+ATOM   1532  W   W   6 968      -6.140  10.790 -55.201  0.00  0.00            
+ATOM   1533  W   W   6 969     -10.137   7.806  62.991  0.00  0.00            
+ATOM   1534  W   W   6 970      -4.486   5.871  37.364  0.00  0.00            
+ATOM   1535  W   W   6 971     -10.057  -2.526 -61.218  0.00  0.00            
+ATOM   1536  W   W   6 972      12.089  -7.021  25.321  0.00  0.00            
+ATOM   1537  W   W   6 973       1.909 -10.408  60.174  0.00  0.00            
+ATOM   1538  W   W   6 974      16.573  -0.681  30.287  0.00  0.00            
+ATOM   1539  W   W   6 975     -15.925  -3.937  46.854  0.00  0.00            
+ATOM   1540  W   W   6 976      -4.803 -12.833 -68.488  0.00  0.00            
+ATOM   1541  W   W   6 977      16.613  10.932 -52.022  0.00  0.00            
+ATOM   1542  W   W   6 978       1.850   8.661  43.370  0.00  0.00            
+ATOM   1543  W   W   6 979       5.985 -12.731  62.323  0.00  0.00            
+ATOM   1544  W   W   6 980      13.367  14.445 -25.808  0.00  0.00            
+ATOM   1545  W   W   6 981     -13.863  14.419  57.712  0.00  0.00            
+ATOM   1546  W   W   6 982     -13.211  -3.616  59.857  0.00  0.00            
+ATOM   1547  W   W   6 983     -11.652  -5.256  67.875  0.00  0.00            
+ATOM   1548  W   W   6 984      10.071   0.576 -26.787  0.00  0.00            
+ATOM   1549  W   W   6 985      -0.322 -10.172  66.093  0.00  0.00            
+ATOM   1550  W   W   6 986       6.930 -11.559 -21.016  0.00  0.00            
+ATOM   1551  W   W   6 987      -4.776  17.267  58.766  0.00  0.00            
+ATOM   1552  W   W   6 988     -14.718   0.689 -32.111  0.00  0.00            
+ATOM   1553  W   W   6 989      12.383   5.875  24.802  0.00  0.00            
+ATOM   1554  W   W   6 990      -9.967  12.096  35.613  0.00  0.00            
+ATOM   1555  W   W   6 991      -2.968   9.229  59.220  0.00  0.00            
+ATOM   1556  W   W   6 992     -13.398   1.335  34.789  0.00  0.00            
+ATOM   1557  W   W   6 993      -0.038   7.729  38.291  0.00  0.00            
+ATOM   1558  W   W   6 994      15.120  -1.312 -55.560  0.00  0.00            
+ATOM   1559  W   W   6 995      14.448   8.908  50.386  0.00  0.00            
+ATOM   1560  W   W   6 996       5.925   9.294  29.866  0.00  0.00            
+ATOM   1561  W   W   6 997     -11.982  -5.466 -36.611  0.00  0.00            
+ATOM   1562  W   W   6 998       4.457   6.926 -33.345  0.00  0.00            
+ATOM   1563  W   W   6 999     -11.063 -15.409 -42.696  0.00  0.00            
+ATOM   1564  W   W   61000      -2.269   2.493 -65.622  0.00  0.00            
+ATOM   1565  W   W   61001      -5.671  13.934  72.655  0.00  0.00            
+ATOM   1566  W   W   61002      -1.141  -3.462  66.929  0.00  0.00            
+ATOM   1567  W   W   61003       3.048 -15.103 -39.385  0.00  0.00            
+ATOM   1568  W   W   61004      -0.635   4.884  29.645  0.00  0.00            
+ATOM   1569  W   W   61005     -11.608  -2.530 -46.060  0.00  0.00            
+ATOM   1570  W   W   61006       9.980  10.558  20.272  0.00  0.00            
+ATOM   1571  W   W   61007     -13.996 -11.993 -54.233  0.00  0.00            
+ATOM   1572  W   W   61008      17.786  12.233 -33.597  0.00  0.00            
+ATOM   1573  W   W   61009      17.431  13.856 -38.119  0.00  0.00            
+ATOM   1574  W   W   61010      -9.579  10.852 -60.334  0.00  0.00            
+ATOM   1575  W   W   61011       9.150   1.473 -41.342  0.00  0.00            
+ATOM   1576  W   W   61012     -15.574  -9.129 -57.930  0.00  0.00            
+ATOM   1577  W   W   61013     -10.204  -9.351 -70.910  0.00  0.00            
+ATOM   1578  W   W   61014      15.071  -6.946 -36.564  0.00  0.00            
+ATOM   1579  W   W   61015       9.537  -9.636  40.436  0.00  0.00            
+ATOM   1580  W   W   61016      16.678  -9.297  63.003  0.00  0.00            
+ATOM   1581  W   W   61017       9.100  15.593 -55.179  0.00  0.00            
+ATOM   1582  W   W   61018      -0.933  -5.869 -60.352  0.00  0.00            
+ATOM   1583  W   W   61019      -9.090 -10.028  44.033  0.00  0.00            
+ATOM   1584  W   W   61020      15.957   3.358  27.158  0.00  0.00            
+ATOM   1585  W   W   61021      -8.045 -11.088  39.532  0.00  0.00            
+ATOM   1586  W   W   61022     -11.468  17.315 -67.005  0.00  0.00            
+ATOM   1587  W   W   61023      16.108  14.411  34.119  0.00  0.00            
+ATOM   1588  W   W   61024       4.304  14.869 -68.261  0.00  0.00            
+ATOM   1589  W   W   61025      -4.042  13.291 -51.032  0.00  0.00            
+ATOM   1590  W   W   61026      11.085  -3.851  59.496  0.00  0.00            
+ATOM   1591  W   W   61027       4.290 -13.780  46.485  0.00  0.00            
+ATOM   1592  W   W   61028       0.231   4.617  45.596  0.00  0.00            
+ATOM   1593  W   W   61029       3.288  10.277 -57.761  0.00  0.00            
+ATOM   1594  W   W   61030       1.828   8.942  71.008  0.00  0.00            
+ATOM   1595  W   W   61031     -11.221  -0.570 -36.540  0.00  0.00            
+ATOM   1596  W   W   61032       9.231  10.398  50.908  0.00  0.00            
+ATOM   1597  W   W   61033      14.698   1.986  47.722  0.00  0.00            
+ATOM   1598  W   W   61034     -14.899  12.721  34.123  0.00  0.00            
+ATOM   1599  W   W   61035       1.283  -9.005 -26.210  0.00  0.00            
+ATOM   1600  W   W   61036       7.547  -8.546  65.788  0.00  0.00            
+ATOM   1601  W   W   61037       7.043   5.015  60.085  0.00  0.00            
+ATOM   1602  W   W   61038      16.582   8.157  62.536  0.00  0.00            
+ATOM   1603  W   W   61039       0.296  15.313 -35.717  0.00  0.00            
+ATOM   1604  W   W   61040      11.643   3.383  64.505  0.00  0.00            
+ATOM   1605  W   W   61041     -12.237  -8.063  39.129  0.00  0.00            
+ATOM   1606  W   W   61042      10.873   3.035 -46.151  0.00  0.00            
+ATOM   1607  W   W   61043       1.179 -18.413  23.487  0.00  0.00            
+ATOM   1608  W   W   61044      13.012  12.840  29.218  0.00  0.00            
+ATOM   1609  W   W   61045     -16.637  -0.425 -46.330  0.00  0.00            
+ATOM   1610  W   W   61046      13.654   5.568  35.981  0.00  0.00            
+ATOM   1611  W   W   61047      15.014 -16.648 -18.396  0.00  0.00            
+ATOM   1612  W   W   61048       4.875  13.321  49.871  0.00  0.00            
+ATOM   1613  W   W   61049      16.561  -9.240 -60.240  0.00  0.00            
+ATOM   1614  W   W   61050       1.523 -12.740  39.018  0.00  0.00            
+ATOM   1615  W   W   61051      -6.032 -11.848  22.704  0.00  0.00            
+ATOM   1616  W   W   61052       0.183  -8.926 -31.259  0.00  0.00            
+ATOM   1617  W   W   61053      -3.773   1.208  49.544  0.00  0.00            
+ATOM   1618  W   W   61054     -18.297 -14.479 -42.199  0.00  0.00            
+ATOM   1619  W   W   61055      -5.882   6.525  30.250  0.00  0.00            
+ATOM   1620  W   W   61056      -5.337  -9.951 -72.728  0.00  0.00            
+ATOM   1621  W   W   61057      -2.776  -0.774  62.953  0.00  0.00            
+ATOM   1622  W   W   61058     -15.803   4.373 -20.866  0.00  0.00            
+ATOM   1623  W   W   61059      -6.852   3.697 -27.317  0.00  0.00            
+ATOM   1624  W   W   61060      -2.113 -14.150 -41.571  0.00  0.00            
+ATOM   1625  W   W   61061      15.155  12.473  19.030  0.00  0.00            
+ATOM   1626  W   W   61062     -15.140  -5.059  55.016  0.00  0.00            
+ATOM   1627  W   W   61063      10.009  17.550 -18.316  0.00  0.00            
+ATOM   1628  W   W   61064      14.821  -3.372  56.312  0.00  0.00            
+ATOM   1629  W   W   61065      -8.636   2.912  49.281  0.00  0.00            
+ATOM   1630  W   W   61066       4.546   5.095  69.216  0.00  0.00            
+ATOM   1631  W   W   61067     -18.263  -4.363 -71.700  0.00  0.00            
+ATOM   1632  W   W   61068     -12.683 -14.034 -26.102  0.00  0.00            
+ATOM   1633  W   W   61069     -10.481   0.082  27.634  0.00  0.00            
+ATOM   1634  W   W   61070     -18.408   5.215  38.258  0.00  0.00            
+ATOM   1635  W   W   61071      15.012   1.516 -48.366  0.00  0.00            
+ATOM   1636  W   W   61072       1.679  -1.652  54.796  0.00  0.00            
+ATOM   1637  W   W   61073       2.604  13.971 -62.227  0.00  0.00            
+ATOM   1638  W   W   61074      -7.686  13.146 -33.104  0.00  0.00            
+ATOM   1639  W   W   61075     -14.860   7.449  35.069  0.00  0.00            
+ATOM   1640  W   W   61076       3.547  15.241 -39.711  0.00  0.00            
+ATOM   1641  W   W   61077       0.959  11.816  29.814  0.00  0.00            
+ATOM   1642  W   W   61078      -0.618  12.034 -40.629  0.00  0.00            
+ATOM   1643  W   W   61079       1.747  17.356 -17.816  0.00  0.00            
+ATOM   1644  W   W   61080      13.626 -16.959 -47.487  0.00  0.00            
+ATOM   1645  W   W   61081     -13.770  -8.946  45.289  0.00  0.00            
+ATOM   1646  W   W   61082     -16.049  -7.698  60.007  0.00  0.00            
+ATOM   1647  W   W   61083      -8.084  -0.841  52.610  0.00  0.00            
+ATOM   1648  W   W   61084      17.595  -7.746  56.112  0.00  0.00            
+ATOM   1649  W   W   61085      -3.226 -12.889 -54.818  0.00  0.00            
+ATOM   1650  W   W   61086      11.478  -5.637  68.649  0.00  0.00            
+ATOM   1651  W   W   61087      10.664  -8.734 -58.666  0.00  0.00            
+ATOM   1652  W   W   61088      -6.351  11.881  26.165  0.00  0.00            
+ATOM   1653  W   W   61089     -13.117  13.627  21.368  0.00  0.00            
+ATOM   1654  W   W   61090      10.994   8.287  62.399  0.00  0.00            
+ATOM   1655  W   W   61091      -4.901  -6.884  20.606  0.00  0.00            
+ATOM   1656  W   W   61092      16.204  -5.573  66.625  0.00  0.00            
+ATOM   1657  W   W   61093      -3.315  16.463  28.117  0.00  0.00            
+ATOM   1658  W   W   61094     -16.476  -0.653  53.853  0.00  0.00            
+ATOM   1659  W   W   61095      -6.945   0.559 -72.939  0.00  0.00            
+ATOM   1660  W   W   61096     -11.047   5.770 -48.302  0.00  0.00            
+ATOM   1661  W   W   61097     -15.056   2.254  57.526  0.00  0.00            
+ATOM   1662  W   W   61098       5.596  -8.419 -50.626  0.00  0.00            
+ATOM   1663  W   W   61099       5.005   8.697 -27.916  0.00  0.00            
+ATOM   1664  W   W   61100      17.359 -13.920  30.045  0.00  0.00            
+ATOM   1665  W   W   61101       7.311  -4.736  26.869  0.00  0.00            
+ATOM   1666  W   W   61102       2.098 -12.504 -43.833  0.00  0.00            
+ATOM   1667  W   W   61103      -7.601  10.993 -47.671  0.00  0.00            
+ATOM   1668  W   W   61104     -16.324  -4.665  69.816  0.00  0.00            
+ATOM   1669  W   W   61105      11.324 -10.957  53.345  0.00  0.00            
+ATOM   1670  W   W   61106       7.434  10.637  34.602  0.00  0.00            
+ATOM   1671  W   W   61107      17.732   8.458  71.491  0.00  0.00            
+ATOM   1672  W   W   61108       8.954 -13.557 -31.962  0.00  0.00            
+ATOM   1673  W   W   61109     -16.418   3.012 -63.818  0.00  0.00            
+ATOM   1674  W   W   61110      12.823   5.120 -34.944  0.00  0.00            
+ATOM   1675  W   W   61111       4.921  -3.202 -66.171  0.00  0.00            
+ATOM   1676  W   W   61112     -10.292 -10.160  66.966  0.00  0.00            
+ATOM   1677  W   W   61113      -4.553 -10.870  27.738  0.00  0.00            
+ATOM   1678  W   W   61114      12.165   7.830  71.438  0.00  0.00            
+ATOM   1679  W   W   61115      -6.482  -7.078 -43.110  0.00  0.00            
+ATOM   1680  W   W   61116     -12.955   1.665 -59.965  0.00  0.00            
+ATOM   1681  W   W   61117       2.125  -1.454  72.276  0.00  0.00            
+ATOM   1682  W   W   61118       8.330  -3.526  72.185  0.00  0.00            
+ATOM   1683  W   W   61119       3.229   5.275 -57.135  0.00  0.00            
+ATOM   1684  W   W   61120      10.443   6.108  48.160  0.00  0.00            
+ATOM   1685  W   W   61121       3.939  -6.287 -29.669  0.00  0.00            
+ATOM   1686  W   W   61122      -3.040  -1.482  53.765  0.00  0.00            
+ATOM   1687  W   W   61123     -14.792   3.826 -37.867  0.00  0.00            
+ATOM   1688  W   W   61124      -1.298 -14.508  58.718  0.00  0.00            
+ATOM   1689  W   W   61125      -9.705   3.781 -40.850  0.00  0.00            
+ATOM   1690  W   W   61126     -12.449  -3.711  43.395  0.00  0.00            
+ATOM   1691  W   W   61127       0.644   9.348 -62.326  0.00  0.00            
+ATOM   1692  W   W   61128     -12.172   5.325  70.208  0.00  0.00            
+ATOM   1693  W   W   61129      -9.257  -0.221 -68.571  0.00  0.00            
+ATOM   1694  W   W   61130     -13.697  -3.844  38.185  0.00  0.00            
+ATOM   1695  W   W   61131      -2.874  -6.795 -69.000  0.00  0.00            
+ATOM   1696  W   W   61132       8.841   8.521 -35.563  0.00  0.00            
+ATOM   1697  W   W   61133      -7.848 -14.540  36.058  0.00  0.00            
+ATOM   1698  W   W   61134      14.250  10.953 -72.021  0.00  0.00            
+ATOM   1699  W   W   61135      17.214  -4.504 -62.258  0.00  0.00            
+ATOM   1700  W   W   61136      -5.700  -3.903 -58.583  0.00  0.00            
+ATOM   1701  W   W   61137     -17.357   8.842 -18.738  0.00  0.00            
+ATOM   1702  W   W   61138       0.647 -13.324  24.960  0.00  0.00            
+ATOM   1703  W   W   61139      -5.104  -5.130 -63.867  0.00  0.00            
+ATOM   1704  W   W   61140     -18.175  -9.593  67.861  0.00  0.00            
+ATOM   1705  W   W   61141       5.458   9.323  55.891  0.00  0.00            
+ATOM   1706  W   W   61142       0.785   1.266 -53.107  0.00  0.00            
+ATOM   1707  W   W   61143      -4.088   0.044 -31.070  0.00  0.00            
+ATOM   1708  W   W   61144       3.178  -6.430  63.790  0.00  0.00            
+ATOM   1709  W   W   61145      -4.635   8.902  54.063  0.00  0.00            
+ATOM   1710  W   W   61146       1.528 -18.202 -42.704  0.00  0.00            
+ATOM   1711  W   W   61147     -16.047  -1.350 -22.686  0.00  0.00            
+ATOM   1712  W   W   61148      11.654   1.798 -68.360  0.00  0.00            
+ATOM   1713  W   W   61149      -3.839  -3.473  58.893  0.00  0.00            
+ATOM   1714  W   W   61150     -17.409 -16.866  26.452  0.00  0.00            
+ATOM   1715  W   W   61151     -14.336   7.708 -40.915  0.00  0.00            
+ATOM   1716  W   W   61152      -3.516   8.095  41.980  0.00  0.00            
+ATOM   1717  W   W   61153      -0.664   3.786  19.214  0.00  0.00            
+ATOM   1718  W   W   61154      14.279  -1.056 -24.152  0.00  0.00            
+ATOM   1719  W   W   61155       8.478  -5.529 -62.621  0.00  0.00            
+ATOM   1720  W   W   61156      13.096   1.536 -60.442  0.00  0.00            
+ATOM   1721  W   W   61157       4.543  11.029  67.226  0.00  0.00            
+ATOM   1722  W   W   61158       5.526  -9.704 -40.532  0.00  0.00            
+ATOM   1723  W   W   61159     -14.026  17.065  46.304  0.00  0.00            
+ATOM   1724  W   W   61160      17.193   5.376 -71.707  0.00  0.00            
+ATOM   1725  W   W   61161       4.703  13.025  27.025  0.00  0.00            
+ATOM   1726  W   W   61162     -16.884   0.202  39.001  0.00  0.00            
+ATOM   1727  W   W   61163      -5.619   9.438  64.622  0.00  0.00            
+ATOM   1728  W   W   61164      15.357  -7.682 -41.401  0.00  0.00
```

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example6_TRIO/ff.xml` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/ff.xml`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example6_TRIO/mapping.dat` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example6_TRIO/mapping.5.dat`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/cg.pdb` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/cg.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/cg_nonprotein.pdb` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/cg_nonprotein.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/protein_AA.pdb` & `mstool-0.3.0/src/mstool/examples/Backmapping/Example7_MembraneProtein/protein_AA.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/Backmapping/run_all.py` & `mstool-0.3.0/src/mstool/examples/Backmapping/run_all.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/examples/BilayerBuilder/run_all.py` & `mstool-0.3.0/src/mstool/examples/BilayerBuilder/run_all.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,97 @@
 import mstool
 
-### Example 1
-mstool.BilayerBuilder(workdir='Example1_POPC', 
+### Example 2A
+mstool.BilayerBuilder(workdir='Example2A_POPC', 
                       upper={'POPC': 40}, lower={'POPC': 40})
 
-### Example 2
+### Example 2B
 lipids = {'DPPC': 5, 'DOPC': 5, 'DMPC': 5, 'DSPC': 5, 'POPC': 5,
           'DOPS': 5, 'POPS': 5, 'POPG': 5, 'DOPG': 5, 'CHL1': 5,
           'POPA': 5, 'DOPA': 5, 'POPE': 5, 'DOPE': 5}
-mstool.BilayerBuilder(workdir='Example2_Lipids',
+mstool.BilayerBuilder(workdir='Example2B_Lipids',
                       upper=lipids, lower=lipids)
 
-### Example 3
-mstool.BilayerBuilder(workdir='Example3_Triolein',
+### Example 2C
+mstool.BilayerBuilder(workdir='Example2C_Triolein',
                       upper={'POPC':100, 'TRIO':6},
                       lower={'POPC':100, 'TRIO':6},
                       mapping_add=mstool.TRIOMAPPING,
                       martini_add=mstool.TRIOMARTINI,
                       ff_add=mstool.TRIOFF)
 
-### Example 4
-mstool.BilayerBuilder(workdir='Example4_MembraneProtein',
+### Example 2D
+mstool.BilayerBuilder(workdir='Example2D_ompF',
                       protein=mstool.MPAA2,
                       upper={'POPC':100, 'POPS': 10, 'POPE': 10, 'CHL1': 10},
                       lower={'POPC':100, 'POPS': 10, 'POPE': 10, 'CHL1': 10})
 
 
-### Example 5
-mstool.BilayerBuilder(workdir='Example5_GPCR',
+### Example 2E
+mstool.BilayerBuilder(workdir='Example2E_3SN6',
                       protein=mstool.GPCR,
                       upper={'DOPC':100, 'DOPS': 10, 'DOPE': 10, 'CHL1': 10},
                       lower={'DOPC':100, 'DOPS': 10, 'DOPE': 10, 'CHL1': 10})
 
+### Example 2F
+# note that the input protein already contains cis/trans bonds
+# therefore, if you see the below two in the final structure, note theses are NOT flipped in mstool
+# peptide bond cis/trans: (chain A and name C O and resid 81 and resname LYS) or 
+# (chain A and name CD N and resid 82 and resname PRO)
+# peptide bond cis/trans: (chain A and name C O and resid 333 and resname ARG) or 
+# (chain A and name H N and resid 334 and resname ARG)
+mstool.BilayerBuilder(workdir='Example2F_4XNV',
+                      protein=mstool.GPCR2,
+                      upper={'DOPC':100, 'DOPS': 10, 'DOPE': 10, 'CHL1': 10},
+                      lower={'DOPC':100, 'DOPS': 10, 'DOPE': 10, 'CHL1': 10})
+
+
+### Example 3A
+mstool.BilayerBuilder(workdir='Example3A_crowded', 
+                      protein={mstool.MPAA2: 4, mstool.GPCR: 5}, 
+                      upper={'POPC':1200}, lower={'POPC': 1200}, 
+                      cg_nsteps=2000000)
+
+
+### Example 3B
+mstool.BilayerBuilder(workdir='Example3B_LD',
+                      upper={'POPC':135, 'CHL1':5},
+                      lower={'POPC':135, 'CHL1':5},
+                      between={'TRIO': 200, 'CHYO': 200},
+                      sep=80.0, ff_add=mstool.TRIOFF,
+                      martini_add=mstool.TRIOMARTINI,
+                      mapping_add=mstool.TRIOMAPPING)
 
-### Example 6
-upper = {'DPPC': 80, 'DOPC': 80, 'DMPC': 80, 'DSPC': 80, 'POPC': 80,
-         'DOPS': 80, 'POPS': 80, 'POPG': 80, 'DOPG': 80, 'CHL1': 80,
-         'POPA': 80, 'DOPA': 80, 'POPE': 80, 'DOPE': 80}
 
-lower = {'DPPC': 30, 'DOPC': 30, 'DMPC': 30, 'DSPC': 30, 'POPC': 30,
-         'DOPS': 30, 'POPS': 30, 'POPG': 30, 'DOPG': 30, 'CHL1': 30,
-         'POPA': 30, 'DOPA': 30, 'POPE': 30, 'DOPE': 30}
+### Example 3C
+mstool.BilayerBuilder(workdir='Example3C_Seipin',
+                      protein=mstool.SEIPIN,
+                      upper={'POPC':437, 'TRIO': 27},
+                      lower={'POPC':360, 'TRIO': 21},
+                      martini_add=mstool.TRIOMARTINI,
+                      mapping_add=mstool.TRIOMAPPING,
+                      ff_add=mstool.TRIOFF,
+                      cg_nsteps=500000,
+                      dx=7.2, removedr=3.0)
 
-mstool.SphereBuilder(workdir='Example7_Sphere',
-                     radius=60, upper=upper, lower=lower)
 
+### Example 3C (is it possible to get rid of all lipids inside protein?)
+mstool.BilayerBuilder(workdir='Example3C_Seipin2',
+                      protein=mstool.SEIPIN,
+                      upper={'POPC':437, 'TRIO': 27},
+                      lower={'POPC':360, 'TRIO': 21},
+                      martini_add=mstool.TRIOMARTINI,
+                      mapping_add=mstool.TRIOMAPPING,
+                      ff_add=mstool.TRIOFF,
+                      cg_nsteps=500000,
+                      dx=7.2, removedr=3.0,
+                      rcut_use_enclosed_protein=True)
 
-### Example 7
-mstool.SphereBuilder(workdir='Example8_SphereProtein',
+### Example 4D
+mstool.SphereBuilder(workdir='Example4D_SphereProtein',
                      radius=100, 
                      protein={mstool.Universe(mstool.MPAA2): 5, 
                               mstool.Universe(mstool.GPCR):  5},
                      upper={'POPC': 1600, 'DOPS': 990, 'CHL1': 10},
                      lower={'POPC': 1000, 'DOPS': 400, 'CHL1': 10})
 
+
```

### Comparing `mstool-0.2.0/src/mstool/lib/align.py` & `mstool-0.3.0/src/mstool/lib/align.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/lib/distance.memory.py` & `mstool-0.3.0/src/mstool/lib/distance.memory.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/lib/distance.py` & `mstool-0.3.0/src/mstool/lib/distance.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/lib/distancelib.c` & `mstool-0.3.0/src/mstool/lib/distancelib.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "mstool.lib.distancelib",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -729,16 +759,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1082,15 +1117,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1169,15 +1204,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1283,32 +1318,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1538,177 +1556,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1755,42 +1773,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2135,30 +2153,30 @@
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -3066,261 +3084,261 @@
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
 #define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
 /* #### Code section: module_code ### */
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3329,29 +3347,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3362,15 +3380,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3379,29 +3397,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3412,15 +3430,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3429,29 +3447,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3462,15 +3480,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3479,29 +3497,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3512,15 +3530,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3529,29 +3547,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3562,217 +3580,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3788,15 +3806,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3804,68 +3822,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -3873,15 +3891,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3896,15 +3914,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3920,15 +3938,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3936,68 +3954,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4005,15 +4023,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4028,15 +4046,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4052,15 +4070,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4068,68 +4086,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4137,15 +4155,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4160,170 +4178,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5725,26 +5743,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
@@ -5864,41 +5882,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -8070,18 +8088,18 @@
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -8127,23 +8145,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -9394,15 +9412,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `mstool-0.2.0/src/mstool/lib/distancelib.pyx` & `mstool-0.3.0/src/mstool/lib/distancelib.pyx`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/lib/qcprot.c` & `mstool-0.3.0/src/mstool/lib/qcprot.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "mstool.lib.qcprot",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -729,16 +759,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1082,15 +1117,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1169,15 +1204,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1285,32 +1320,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1642,177 +1660,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1845,42 +1863,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2842,30 +2860,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -3411,27 +3429,27 @@
 static PyObject *__pyx_builtin_ImportError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = ": ";
 static const char __pyx_k_A[] = "A";
 static const char __pyx_k_N[] = "N";
 static const char __pyx_k_O[] = "O";
 static const char __pyx_k_T[] = "T{";
-  static const char __pyx_k_c[] = "c";
-  static const char __pyx_k_s[] = "s";
-  static const char __pyx_k_E0[] = "E0";
-  static const char __pyx_k__2[] = ".";
-  static const char __pyx_k__3[] = "*";
-  static const char __pyx_k__6[] = "'";
-  static const char __pyx_k__7[] = ")";
-  static const char __pyx_k__9[] = "^";
-  static const char __pyx_k_gc[] = "gc";
-  static const char __pyx_k_id[] = "id";
-  static const char __pyx_k_np[] = "np";
-  static const char __pyx_k__10[] = "";
-  static const char __pyx_k__11[] = ":";
+static const char __pyx_k_c[] = "c";
+static const char __pyx_k_s[] = "s";
+static const char __pyx_k_E0[] = "E0";
+static const char __pyx_k__2[] = ".";
+static const char __pyx_k__3[] = "*";
+static const char __pyx_k__6[] = "'";
+static const char __pyx_k__7[] = ")";
+static const char __pyx_k__9[] = "^";
+static const char __pyx_k_gc[] = "gc";
+static const char __pyx_k_id[] = "id";
+static const char __pyx_k_np[] = "np";
+static const char __pyx_k__10[] = "";
+static const char __pyx_k__11[] = ":";
 static const char __pyx_k__12[] = "}";
 static const char __pyx_k__13[] = "(";
 static const char __pyx_k__14[] = ",";
 static const char __pyx_k__17[] = "()";
 static const char __pyx_k__18[] = "|";
 static const char __pyx_k__42[] = "?";
 static const char __pyx_k_abc[] = "abc";
@@ -18728,261 +18746,261 @@
   __Pyx_XDECREF(__pyx_v_parts);
   __Pyx_XDECREF(__pyx_v_extents);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18991,29 +19009,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19024,15 +19042,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19041,29 +19059,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19074,15 +19092,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19091,29 +19109,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19124,15 +19142,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19141,29 +19159,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19174,15 +19192,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19191,29 +19209,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19224,217 +19242,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19450,15 +19468,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19466,68 +19484,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19535,15 +19553,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19558,15 +19576,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19582,15 +19600,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19598,68 +19616,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19667,15 +19685,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19690,15 +19708,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19714,15 +19732,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19730,68 +19748,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19799,15 +19817,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19822,170 +19840,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -28906,26 +28924,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-b_l_tdxv/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../private/var/folders/bz/vx13pf8x04l1m6z0l2stq2s80000gn/T/pip-build-env-3dsp9pu2/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -29327,41 +29345,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -34113,18 +34131,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -34170,23 +34188,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -35178,15 +35196,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `mstool-0.2.0/src/mstool/lib/qcprot.pyx` & `mstool-0.3.0/src/mstool/lib/qcprot.pyx`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/mapping/martini.amber14.dat` & `mstool-0.3.0/src/mstool/mapping/martini.amber14.dat`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/mapping/martini.lipid.c36.dat` & `mstool-0.3.0/src/mstool/mapping/martini.lipid.c36.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1081,14 +1081,90 @@
 H9   C9   C8   C10  C11
 H8   C8   C9   C7   C14
 H14  C14  C8   C13  C15
 C18  C13  C12  C14  C17
 H17  C17  C13  C20  C16
 H20  C20  C21  C17  C22
 
+
+RESI CHYO
+; cholesterol oleate
+[ ES ]
+O31 C31 O32
+C32 H2X H2Y
+
+[ C3 ]
+C33 H3X H3Y C34 H4X H4Y C35 H5X H5Y C36 H6X H6Y
+
+[ C4 ]
+C37 H7X H7Y C38 H8X H8Y C39 H9X C310 H10X C311 H11X H11Y
+
+[ C5 ]
+C312 H12X H12Y C313 H13X H13Y C314 H14X H14Y
+
+[ C6 ]
+C315 H15X H15Y C316 H16X H16Y C317 H17X H17Y C318 H18X H18Y H18Z
+
+[ R0 ]
+C3 H3
+C2 H2A H2B
+C4 H4A H4B
+
+[ R1 ]
+C1 H1A H1B
+C6 H6
+C19 H19A H19B H19C
+C10
+
+[ R2 ]
+C5
+C7  H7A  H7B
+C8  H8
+
+[ R3 ]
+C9   H9
+C11  H11A  H11B
+C12  H12A  H12B
+
+[ R4 ]
+C14 H14
+C15 H15A H15B
+C16 H16A H16B
+
+[ R5 ]
+C13
+C17 H17
+C18 H18A H18B H18C
+
+[ C1 ]
+C20 H20
+C21 H21A H21B H21C
+C22 H22A H22B
+C23 H23A H23B
+
+[ C2 ]
+C24 H24A H24B
+C25 H25
+C26 H26A H26B H26C
+C27 H27A H27B H27C
+
+[ chiral ]
+H3   C3   O31  C2   C4
+C19  C10  C1   C5   C9
+H9   C9   C8   C10  C11
+H8   C8   C9   C7   C14
+H14  C14  C8   C13  C15
+C18  C13  C12  C14  C17
+H17  C17  C13  C20  C16
+H20  C20  C21  C17  C22
+
+[ cis ]
+C38 C39 C310 C311
+
+
 RESI CHOL
 ; cholesterol
 
 [ ROH ]
 C3 H3 O3 H3'
 C2 H2A H2B
 C4 H4A H4B
```

### Comparing `mstool-0.2.0/src/mstool/mapping/martini.protein.c36m.dat` & `mstool-0.3.0/src/mstool/mapping/martini.protein.c36m.dat`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/mapping/structures/CHL1.pdb` & `mstool-0.3.0/src/mstool/mapping/structures/CHL1.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/mapping/structures/CHL1_AA.pdb` & `mstool-0.3.0/src/mstool/mapping/structures/CHL1_AA.pdb`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/membrane/bilayer.py` & `mstool-0.3.0/src/mstool/backup/bilayer_240429.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/membrane/bilayerbuilder.py` & `mstool-0.3.0/src/mstool/backup/bilayerbuilder_240429.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/membrane/lipid.py` & `mstool-0.3.0/src/mstool/membrane/lipid.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/membrane/sphere.py` & `mstool-0.3.0/src/mstool/membrane/sphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,25 +84,25 @@
 
 
         ### Construct Fibonacchi sphere.
         hht = hydrophobic_thickness * 0.5
 
         # upper
         upperU = self.make_sphere(r+hht, upperN,
-                    monolayer_keys['upper'], monolayer_list['upper'], chain='UPPER',
+                    monolayer_keys['upper'], monolayer_list['upper'], chain='0',
                     inverse=1, alpha=alpha, beta=beta, gamma=gamma)
                         
         # lower
         lowerU = self.make_sphere(r-hht, lowerN,
-                    monolayer_keys['lower'], monolayer_list['lower'], chain='LOWER',
+                    monolayer_keys['lower'], monolayer_list['lower'], chain='1',
                     inverse=-1, alpha=alpha, beta=beta, gamma=gamma)
 
         # trans
         transU = self.make_sphere(r, transN,
-                    monolayer_keys['trans'], monolayer_list['trans'], chain='TRANS',
+                    monolayer_keys['trans'], monolayer_list['trans'], chain='2',
                     inverse=1, alpha=alpha, beta=beta, gamma=gamma)
 
         # pbc
         pbc = (r + hht + water) * 2
 
         # protein
         if protein:
@@ -130,15 +130,15 @@
         self.universe = u
 
 
     def make_sphere(self, finalr, finalN, monolayer_key, monolayer_list, chain, inverse, alpha, beta, gamma):
         if finalN == 0:
             return Universe()
         
-        print(chain + ' leaflet')
+        print('leaflet ' + chain)
         points = fibo(r=finalr, N=finalN, alpha=alpha, beta=beta, gamma=gamma, plot=None)
         data = {'name': [], 'resname': [], 'resid': [], 'chain': [], 'x': [], 'y': [], 'z': []}
 
         for i in range(len(points)):
             
             key = monolayer_key[monolayer_list[i]]
             if isinstance(key, str):
```

### Comparing `mstool-0.2.0/src/mstool/membrane/spherebuilder.py` & `mstool-0.3.0/src/mstool/membrane/spherebuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,49 +108,60 @@
         '''
 
         
         ### workdir
         if (not use_existing_folder) or (use_existing_folder and not os.path.exists(workdir)):
             os.mkdir(workdir)
 
+        ### save args
+        args = locals()
+        with open(workdir + '/args.txt', 'w') as W:
+            for key, value in args.items():
+                if key == 'self': continue
+                W.write(f'{key:30} = {value}\n')
+        
+        ### protein
         if protein:
             if isinstance(protein, str):
                 proteinU = Universe(protein)
 
             elif isinstance(protein, dict):
                 SphereProtein(radius=radius, protein=protein, out=workdir + '/protein.dms')
                 proteinU = Universe(workdir + '/protein.dms')
 
             Hatoms   = proteinU.atoms.name.str.startswith('H')
             proteinU.atoms.bfactor = 0.0
             proteinU.atoms.loc[~Hatoms, 'bfactor'] = 1.0
+            if len(proteinU.bonds) == 0: proteinU.addBondFromDistance()
             proteinU.write(workdir + '/protein.dms', wrap=False)
             proteinU.write(workdir + '/protein.pdb', wrap=False)
        
         ### Read Martini
         #martiniff = ReadMartini(ff=martini, ff_add=martini_add, define={'FLEXIBLE': 'True'})
         martiniff = ReadMartini(ff=martini, ff_add=martini_add, constraint_to_bond=True, Kc2b=10000.0)
 
         ### Mapping & Translate
         #if protein: Map(workdir + '/protein.dms', workdir + '/protein_CG.dms', add_notavailableAAAtoms=True)
-        if protein: Map(workdir + '/protein.dms', workdir + '/protein_CG.dms', add_notavailableAAAtoms=False)
+        if protein: Map(workdir + '/protein.dms', workdir + '/protein_CG.dms', add_notavailableAAAtoms=False,
+                        mapping=mapping, mapping_add=mapping_add)
 
         ### Construct a bilayer
         instance = Sphere( protein=workdir + '/protein_CG.dms' if protein else None, 
                            upper=upper, lower=lower, 
                            water=water, rcut=rcut,
                            out=workdir + '/step1.bilayer.dms', 
                            martini=martiniff, 
                            lipidpath=lipidpath,
                            hydrophobic_thickness=hydrophobic_thickness,
                            alpha=alpha, beta=beta, gamma=gamma, r=radius)
 
         ### Solvate
         if solvate:
-            usol = SolvateMartini(workdir + '/step1.bilayer.dms', removedr=removedr, conc=ionconc)
+            usol = SolvateMartini(workdir + '/step1.bilayer.dms', removedr=removedr, conc=ionconc, 
+                                  posionchain='4', negionchain='5', waterchain='6')
         else:
             usol = instance.universe
             # make it NVT
             barfreq=0
             # remove_solvent is redundant
             remove_solvent=False
 
@@ -202,56 +213,57 @@
         #                                   R0=shift,
         #                                   fc=fc,
         #                                   chain='LOWER'))
         #dms.runEMNPT(workdir + '/step2.tmp.dms', dt=dt, nsteps=0, frictionCoeff=frictionCoeff, T=T)
         
         ### NPT
         martiniU = Universe(workdir + '/step1.martini.dms')
-        martiniU.atoms.loc[((martiniU.atoms.name == 'GL1')), 'bfactor'] = 1.0
+        martiniU.atoms.loc[((martiniU.atoms.name == 'GL1')), 'bfactor'] = 2.0
 
         dms = DMSFile(workdir + '/step1.martini.dms')
         dms.createSystem(REM=True,  tapering=tapering, martini=True, nonbondedCutoff=nonbondedCutoff, nonbondedMethod='CutoffPeriodic', improper_prefactor=improper_prefactor, removeCMMotion=True)
-        dms.system.addForce(addSpherePosre(martiniU, bfactor_posre=0.5, radius=radius + hydrophobic_thickness/2, rfb=0.1, R0=shift, fc=fc, chain='UPPER'))
-        dms.system.addForce(addSpherePosre(martiniU, bfactor_posre=0.5, radius=radius - hydrophobic_thickness/2, rfb=0.1, R0=shift, fc=fc, chain='LOWER'))
-        dms.runEMNPT(dt=dt_rem, nsteps=cg_nsteps_rem, frictionCoeff=frictionCoeff, barfreq=barfreq, T=T, semiisotropic=False, out=workdir + '/step2.rem.dms')
+        dms.system.addForce(addSpherePosre(martiniU, bfactor_posre=1.5, radius=radius + hydrophobic_thickness/2, rfb=0.1, R0=shift, fc=fc, chain='0'))
+        dms.system.addForce(addSpherePosre(martiniU, bfactor_posre=1.5, radius=radius - hydrophobic_thickness/2, rfb=0.1, R0=shift, fc=fc, chain='1'))
+        dms.runEMNPT(dt=dt_rem, nsteps=int(cg_nsteps_rem), frictionCoeff=frictionCoeff, barfreq=barfreq, T=T, semiisotropic=False, out=workdir + '/step2.rem.dms')
 
         dms.createSystem(REM=False, tapering=tapering, martini=True, nonbondedCutoff=nonbondedCutoff, nonbondedMethod='CutoffPeriodic', improper_prefactor=improper_prefactor, removeCMMotion=True)
-        dms.system.addForce(addSpherePosre(martiniU, bfactor_posre=0.5, radius=radius + hydrophobic_thickness/2, rfb=0.1, R0=shift, fc=fc, chain='UPPER'))
-        dms.system.addForce(addSpherePosre(martiniU, bfactor_posre=0.5, radius=radius - hydrophobic_thickness/2, rfb=0.1, R0=shift, fc=fc,chain='LOWER'))
-        dms.runEMNPT(dt=dt, nsteps=cg_nsteps, frictionCoeff=frictionCoeff, barfreq=barfreq, T=T, semiisotropic=False, out=workdir + '/step2.dms')
+        dms.system.addForce(addSpherePosre(martiniU, bfactor_posre=1.5, radius=radius + hydrophobic_thickness/2, rfb=0.1, R0=shift, fc=fc, chain='0'))
+        dms.system.addForce(addSpherePosre(martiniU, bfactor_posre=1.5, radius=radius - hydrophobic_thickness/2, rfb=0.1, R0=shift, fc=fc,chain='1'))
+        dms.runEMNPT(dt=dt, nsteps=int(cg_nsteps), frictionCoeff=frictionCoeff, barfreq=barfreq, T=T, semiisotropic=False, out=workdir + '/step2.dms')
 
 
         #dms.runEMNPT(dt=0.002, nsteps=cg_nsteps_2fs, frictionCoeff=frictionCoeff, barfreq=barfreq, T=T, semiisotropic=False)
         #dms.runEMNPT(dt=0.005, nsteps=cg_nsteps_5fs, frictionCoeff=frictionCoeff, barfreq=0,       T=T, EM=False)
         #dms.runEMNPT(dt=dt,    nsteps=cg_nsteps,     frictionCoeff=frictionCoeff, barfreq=0,       T=T, EM=False, out=workdir + '/step2.dms')
         
         ### Translate Back
         u = Universe(workdir + '/step2.dms')
         u.atoms[['x','y','z']] -= shift
 
         if remove_solvent:
             dimensions = u.dimensions
             cell = u.cell
             bA1  = u.atoms.resname == 'W'
-            bA2  = u.atoms.chain   == 'ZZ1'
-            bA3  = u.atoms.chain   == 'ZZ2'
+            bA2  = u.atoms.chain   == '4'
+            bA3  = u.atoms.chain   == '5'
             bA   = bA1 | bA2 | bA3
             u    = Universe(data=u.atoms[~bA])
             u.dimensions = dimensions
             u.cell = cell
-
+        
+        u.sort()
         u.write(workdir + '/step3.dms', wrap=True)
         u.write(workdir + '/step3.pdb', wrap=True)
 
         if protein:
             noprotein = Universe(data=u.atoms[~u.atoms.resname.isin(three2one.keys())])
             noprotein.dimensions = u.dimensions
             noprotein.cell = u.cell
             noprotein.write(workdir + '/step3.noprotein.dms')
-            Backmap(workdir + '/step3.noprotein.dms', workdir=workdir, use_existing_workdir=True, nsteps=aa_nsteps,
+            Backmap(workdir + '/step3.noprotein.dms', workdir=workdir, use_existing_workdir=True, nsteps=int(aa_nsteps),
                     AA=workdir + '/protein.dms', fileindex=4, mapping=mapping, mapping_add=mapping_add, ff=ff, ff_add=ff_add,
-                    use_AA_structure=use_AA_structure, rockCtype=rockCtype, rockHtype=rockHtype, T=T)
+                    use_AA_structure=use_AA_structure, rockCtype=rockCtype, rockHtype=rockHtype, T=T, water_chain='6789')
         else:
-            Backmap(workdir + '/step3.dms', workdir=workdir, use_existing_workdir=True, nsteps=aa_nsteps,
+            Backmap(workdir + '/step3.dms', workdir=workdir, use_existing_workdir=True, nsteps=int(aa_nsteps),
                     AA=None, fileindex=4, mapping=mapping, mapping_add=mapping_add, ff=ff, ff_add=ff_add,
-                    use_AA_structure=use_AA_structure, rockCtype=rockCtype, rockHtype=rockHtype, T=T)
+                    use_AA_structure=use_AA_structure, rockCtype=rockCtype, rockHtype=rockHtype, T=T, water_chain='6789')
```

### Comparing `mstool-0.2.0/src/mstool/membrane/sphereprotein.py` & `mstool-0.3.0/src/mstool/membrane/sphereprotein.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 positions     = key.atoms[['x','y','z']].to_numpy()
                 save_resname  = key.atoms['resname'].tolist()
                 save_name     = key.atoms['name'].tolist()
                 save_resid    = key.atoms['resid'].tolist()
                 save_chain    = np.char.add(key.atoms['chain'].tolist(), [str(i)] * len(positions))
 
             else:
-                assert 0 == 1, 'resname does not exist or input structure cannot be found'
+                assert 0 == 1, 'input structure cannot be found'
 
             finalpositions = self.place(positions, r=finalr, r_vector=points[i])
             data['chain'].extend(save_chain)
             data['resname'].extend(save_resname)
             data['resid'].extend(save_resid)
             data['name'].extend(save_name)
             data['x'].extend(finalpositions[:,0])
```

### Comparing `mstool-0.2.0/src/mstool/utils/add_termini_atoms.py` & `mstool-0.3.0/src/mstool/utils/add_termini_atoms.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/utils/amberselection.py` & `mstool-0.3.0/src/mstool/backup/amberselection_20240510.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/utils/cap_termini_residues.py` & `mstool-0.3.0/src/mstool/utils/cap_termini_residues.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/utils/change_his.py` & `mstool-0.3.0/src/mstool/utils/change_his.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/utils/dump.py` & `mstool-0.3.0/src/mstool/utils/dump.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/utils/gmx_energy.py` & `mstool-0.3.0/src/mstool/utils/gmx_energy.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/utils/openmmutils.py` & `mstool-0.3.0/src/mstool/utils/openmmutils.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/utils/performance.py` & `mstool-0.3.0/src/mstool/utils/performance.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/utils/rock.py` & `mstool-0.3.0/src/mstool/utils/rock.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         
         if ENM:
             u.atoms.bfactor = 0.0
         else:
             u.atoms.bfactor = 1.0
         u.atoms.charge  = 0.0
         self.dms = out + '.dms'
-        u.write(self.dms, guess_atomic_number=True)
+        u.write(self.dms)
 
 
         ### Save it to XML
         self.xml = out + '.xml'
         W = open(self.xml, 'w')
         W.write('<ForceField>\n')
         W.write('  <Residues>\n')
```

### Comparing `mstool-0.2.0/src/mstool/utils/rockchain.py` & `mstool-0.3.0/src/mstool/utils/rockchain.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,10 +40,10 @@
                 W.write(f'      <Atom charge="0.00" name="{nn}" type="{tt}"/>\n')
             W.write(f'    </Residue>\n')
 
         W.write('  </Residues>\n')
         W.write('</ForceField>\n')
         W.close()
 
-        u.write(self.dms, guess_atomic_number=True)
+        u.write(self.dms)
         self.bonds = []
```

### Comparing `mstool-0.2.0/src/mstool/utils/rockresidue.py` & `mstool-0.3.0/src/mstool/utils/rockresidue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-import numpy as np
-import pandas as pd
 from   ..core.universe import Universe
 
-
 def generate_list(group):
     index = group.groupby('resn').cumcount()
     return [f"{'H' if group['name'].iloc[i][0] == 'H' else 'C'}{index.iloc[i]}" for i in range(len(group))]
 
 def get_resname(group, uniques):
     resname = 'ROCK' + ''.join(group['name'])
     return [resname] * len(group['name'])
 
 
-
 class RockResidue:
     def __init__(self, structure, out='ROCK', resname='ROCK',
                  rockHtype='HAL3', rockCtype='CTL3'):
         
         self.dms = out + '.dms'
         u = Universe(structure)
         u.atoms.mass    = 100.0
         u.atoms.bfactor = 1.0
         u.atoms.charge  = 0.0
 
         # change name to C0 H1 H2 C3 H4 H5 for each residue
         u.atoms['name'] = u.atoms.groupby('resn').apply(generate_list).explode().reset_index(level=0, drop=True)
-
+        anum, mass, vdw = u.update_anum_mass_vdw_from_name()
+        u.atoms['anum'] = anum
         
         # obtain unique residues
         uniques = {}
         for name in u.atoms.groupby('resn').name:
             namelist = name[1].tolist()
             resname  = 'ROCK' + ''.join(namelist)
 
@@ -38,15 +35,15 @@
 
             if resname not in uniques.keys():
                 uniques[resname] = namelist
 
 
         # change resname
         u.atoms['resname'] = u.atoms.groupby('resn').apply(get_resname, uniques=uniques).explode().reset_index(level=0, drop=True)
-        u.write(self.dms, guess_atomic_number=True)
+        u.write(self.dms)
         self.bonds = []
         
 
         ### Save it to XML
         self.xml = out + '.xml'
         W = open(self.xml, 'w')
         W.write('<ForceField>\n')
```

### Comparing `mstool-0.2.0/src/mstool/utils/sqlcmd.py` & `mstool-0.3.0/src/mstool/utils/sqlcmd.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool/utils/util.py` & `mstool-0.3.0/src/mstool/utils/util.py`

 * *Files identical despite different names*

### Comparing `mstool-0.2.0/src/mstool.egg-info/PKG-INFO` & `mstool-0.3.0/src/mstool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mstool
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multiscale Simulation Tool for Backmapping
 Author-email: Siyoung Kim <siyoung.k@icloud.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,11 +680,12 @@
 Project-URL: Repository, https://github.com/ksy141/mstool.git
 Project-URL: documentation, https://mstool.readthedocs.io/en/latest/#
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: matplotlib
+Requires-Dist: scipy
 
 # mstool
 
 [mstool](https://mstool.readthedocs.io/en/latest/#) is a multiscale simulation tool that converts a coarse-grained structure into an all-atom structure. It requires minimal user input (mapping and isomeric information of molecules) and is more powerful than the previous backmapping tools. For more details, please check out the [paper](https://pubs.acs.org/doi/10.1021/acs.jpcb.3c05593) and [documentation](https://mstool.readthedocs.io/en/latest/#).
```

### Comparing `mstool-0.2.0/src/mstool.egg-info/SOURCES.txt` & `mstool-0.3.0/src/mstool.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,27 +21,34 @@
 src/mstool/FF/amber14/tip3p.xml
 src/mstool/FF/amber14/tip3pfb.xml
 src/mstool/FF/amber14/tip4pew.xml
 src/mstool/FF/amber14/tip4pfb.xml
 src/mstool/FF/amber99/amber99sbildn.xml
 src/mstool/FF/amber99/tip3p.xml
 src/mstool/FF/charmm36/charmm36.xml
+src/mstool/FF/charmm36/chyo.xml
 src/mstool/FF/charmm36/clol.xml
 src/mstool/FF/charmm36/pip.xml
 src/mstool/FF/charmm36/water.xml
 src/mstool/FF/martini2.2/martini_lipids_add.itp
 src/mstool/FF/martini2.2/martini_v2.0_ions.itp
 src/mstool/FF/martini2.2/martini_v2.0_lipids_all_201506.itp
 src/mstool/FF/martini2.2/martini_v2.2.itp
 src/mstool/FF/martini2.2/martini_v2.2.modified.LJ.itp
 src/mstool/FF/martini2.2/martini_v2.2.modified.itp
 src/mstool/FF/martini2.2/ti.itp
 src/mstool/FF/martini2.2/toy.itp
 src/mstool/FF/martini2.2/tp.itp
+src/mstool/FF/martini3.0.0/martini.itp
+src/mstool/FF/martini3.0.0/phospholipids.itp
+src/mstool/FF/martini3.0.0/protein.itp
+src/mstool/backup/amberselection_20240510.py
 src/mstool/backup/backmap.py
+src/mstool/backup/bilayer_240429.py
+src/mstool/backup/bilayerbuilder_240429.py
 src/mstool/backup/fill.bck.py
 src/mstool/backup/fill_loops.py
 src/mstool/backup/fill_side.py
 src/mstool/backup/gmx2dms2.py
 src/mstool/backup/loopmodeler_230719.py
 src/mstool/backup/martinizedms.231213.py
 src/mstool/backup/martinizedms.240309.py
@@ -49,27 +56,31 @@
 src/mstool/backup/pandas2dict.py
 src/mstool/backup/rem.bck.py
 src/mstool/backup/rem_230719.py
 src/mstool/backup/rem_230801.py
 src/mstool/backup/rock_240306.py
 src/mstool/backup/sphere_240304.py
 src/mstool/backup/ungroup.py
+src/mstool/backup/ungroup_240430.py
+src/mstool/backup/universe_20240510.py
+src/mstool/backup/universe_20240511.py
 src/mstool/backup/cg2aa/cg2aa.py
 src/mstool/core/__init__.py
 src/mstool/core/backmap.py
 src/mstool/core/checkstructure.py
 src/mstool/core/checktetrahedron.py
 src/mstool/core/dms2openmm.py
 src/mstool/core/dmsfile.py
 src/mstool/core/fill.py
 src/mstool/core/gmx2dms.py
 src/mstool/core/loopmodeler.py
 src/mstool/core/map.py
 src/mstool/core/martinizedms.py
 src/mstool/core/mutate.py
+src/mstool/core/orient.py
 src/mstool/core/readmappings.py
 src/mstool/core/readmartini.py
 src/mstool/core/readxml.py
 src/mstool/core/rem.py
 src/mstool/core/seq.py
 src/mstool/core/solvate_martini.py
 src/mstool/core/truncateprotein.py
@@ -88,54 +99,61 @@
 src/mstool/examples/Backmapping/Example3_butene/mapping.dat
 src/mstool/examples/Backmapping/Example3_butene/run.py
 src/mstool/examples/Backmapping/Example4_POPC/cg.pdb
 src/mstool/examples/Backmapping/Example4_POPC/run.py
 src/mstool/examples/Backmapping/Example5_Sphere/cg.pdb
 src/mstool/examples/Backmapping/Example6_TRIO/cg.pdb
 src/mstool/examples/Backmapping/Example6_TRIO/ff.xml
+src/mstool/examples/Backmapping/Example6_TRIO/mapping.5.dat
 src/mstool/examples/Backmapping/Example6_TRIO/mapping.dat
 src/mstool/examples/Backmapping/Example6_TRIO/run.py
 src/mstool/examples/Backmapping/Example6_TRIO/setup.py
 src/mstool/examples/Backmapping/Example7_MembraneProtein/cg.pdb
 src/mstool/examples/Backmapping/Example7_MembraneProtein/cg_nonprotein.pdb
 src/mstool/examples/Backmapping/Example7_MembraneProtein/protein_AA.pdb
 src/mstool/examples/Backmapping/Example7_MembraneProtein/run.py
 src/mstool/examples/BilayerBuilder/run_all.py
+src/mstool/examples/BilayerBuilder/run_martini3.py
 src/mstool/examples/BilayerBuilder/showhalf.py
-src/mstool/examples/BilayerBuilder/Example5_GPCR/run.py
-src/mstool/examples/BilayerBuilder/Example6_Seipin/run.py
-src/mstool/examples/BilayerBuilder/Example6_Seipin/showhalf.py
-src/mstool/examples/BilayerBuilder/Example8_SARS/run.py
-src/mstool/examples/BilayerBuilder/Example8_SARS_small/run.py
+src/mstool/examples/BilayerBuilder/gpcr/run.py
+src/mstool/examples/BilayerBuilder/sars/run.py
+src/mstool/examples/BilayerBuilder/sars_small/run.py
 src/mstool/lib/align.py
 src/mstool/lib/distance.memory.py
 src/mstool/lib/distance.py
 src/mstool/lib/distancelib.c
 src/mstool/lib/distancelib.pyx
 src/mstool/lib/qcprot.c
 src/mstool/lib/qcprot.pyx
 src/mstool/lib/setup.py
 src/mstool/mapping/martini.amber14.dat
 src/mstool/mapping/martini.lipid.c36.dat
 src/mstool/mapping/martini.protein.c36m.dat
+src/mstool/mapping/martini3.protein.c36m.dat
 src/mstool/mapping/structures/CHL1.pdb
 src/mstool/mapping/structures/CHL1_AA.pdb
+src/mstool/mapping/structures/CHYO.bck.pdb
+src/mstool/mapping/structures/CHYO.pdb
+src/mstool/mapping/structures/CHYO_AA.bck.pdb
+src/mstool/mapping/structures/CHYO_AA.pdb
 src/mstool/membrane/bilayer.py
 src/mstool/membrane/bilayerbuilder.py
 src/mstool/membrane/lipid.py
 src/mstool/membrane/sphere.py
 src/mstool/membrane/spherebuilder.py
 src/mstool/membrane/sphereprotein.py
 src/mstool/utils/__init__.py
 src/mstool/utils/add_termini_atoms.py
 src/mstool/utils/amberselection.py
+src/mstool/utils/atomic_data.py
 src/mstool/utils/cap_termini_residues.py
 src/mstool/utils/change_his.py
 src/mstool/utils/dump.py
 src/mstool/utils/gmx_energy.py
+src/mstool/utils/mdautils.py
 src/mstool/utils/openmmutils.py
 src/mstool/utils/performance.py
 src/mstool/utils/protein_sel.py
 src/mstool/utils/rock.py
 src/mstool/utils/rockchain.py
 src/mstool/utils/rockresidue.py
 src/mstool/utils/saveargs.py
```

