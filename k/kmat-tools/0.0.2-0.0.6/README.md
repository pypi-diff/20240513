# Comparing `tmp/kmat_tools-0.0.2.tar.gz` & `tmp/kmat_tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmat_tools-0.0.2.tar", last modified: Fri May 10 15:04:07 2024, max compression
+gzip compressed data, was "kmat_tools-0.0.6.tar", last modified: Mon May 13 11:57:56 2024, max compression
```

## Comparing `kmat_tools-0.0.2.tar` & `kmat_tools-0.0.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-10 15:04:07.402102 kmat_tools-0.0.2/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1075 2024-05-10 13:32:59.000000 kmat_tools-0.0.2/LICENSE
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       36 2024-04-25 14:25:41.000000 kmat_tools-0.0.2/MANIFEST.in
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1478 2024-05-10 15:04:07.393078 kmat_tools-0.0.2/PKG-INFO
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      984 2024-05-10 13:44:58.000000 kmat_tools-0.0.2/README.md
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-10 15:04:07.395812 kmat_tools-0.0.2/kmat_tools.egg-info/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1478 2024-05-10 15:04:07.000000 kmat_tools-0.0.2/kmat_tools.egg-info/PKG-INFO
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1771 2024-05-10 15:04:07.000000 kmat_tools-0.0.2/kmat_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)        1 2024-05-10 15:04:07.000000 kmat_tools-0.0.2/kmat_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      338 2024-05-10 15:04:07.000000 kmat_tools-0.0.2/kmat_tools.egg-info/entry_points.txt
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       44 2024-05-10 15:04:07.000000 kmat_tools-0.0.2/kmat_tools.egg-info/top_level.txt
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-10 15:04:07.322965 kmat_tools-0.0.2/kmtools_cython/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)   301593 2024-05-10 15:04:05.000000 kmat_tools-0.0.2/kmtools_cython/km_basic_filter.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      131 2024-05-02 16:15:26.000000 kmat_tools-0.0.2/kmtools_cython/km_basic_filter.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1117 2024-05-07 12:15:08.000000 kmat_tools-0.0.2/kmtools_cython/km_basic_filter.pyx
--rw-r--r--   0 cduitama (36963) seqbio   (97979)   290013 2024-05-10 15:04:05.000000 kmat_tools-0.0.2/kmtools_cython/km_fasta.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      149 2024-05-07 10:18:19.000000 kmat_tools-0.0.2/kmtools_cython/km_fasta.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1036 2024-05-07 11:08:30.000000 kmat_tools-0.0.2/kmtools_cython/km_fasta.pyx
--rw-r--r--   0 cduitama (36963) seqbio   (97979)   221907 2024-05-06 16:37:02.000000 kmat_tools-0.0.2/kmtools_cython/km_reset.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      104 2024-05-06 16:36:55.000000 kmat_tools-0.0.2/kmtools_cython/km_reset.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       68 2024-05-06 16:33:39.000000 kmat_tools-0.0.2/kmtools_cython/km_reset.pyx
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       92 2024-05-02 13:30:32.000000 kmat_tools-0.0.2/kmtools_cython/km_select.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2631 2024-04-25 14:16:14.000000 kmat_tools-0.0.2/kmtools_cython/km_select.pyx
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-10 15:04:07.335131 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2024-05-07 14:14:50.000000 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/__init__.py
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-10 15:04:07.350930 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/__pycache__/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      210 2024-05-07 14:21:11.000000 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2521 2024-05-09 13:49:00.000000 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1690 2024-05-09 13:49:00.000000 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2177 2024-05-09 14:29:01.000000 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1617 2024-05-09 13:44:33.000000 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/km_basic_filter_wrapper.py
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      917 2024-05-09 13:44:24.000000 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/km_fasta_wrapper.py
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1303 2024-05-09 13:48:28.000000 kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/km_unitig_wrapper.py
--rw-r--r--   0 cduitama (36963) seqbio   (97979)   290130 2024-05-10 15:04:05.000000 kmat_tools-0.0.2/kmtools_cython/km_unitig.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      119 2024-05-03 12:56:30.000000 kmat_tools-0.0.2/kmtools_cython/km_unitig.pxd
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     1048 2024-05-09 14:35:01.000000 kmat_tools-0.0.2/kmtools_cython/km_unitig.pyx
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-10 15:04:07.245545 kmat_tools-0.0.2/kmtools_cython/lib/
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-10 15:04:07.372935 kmat_tools-0.0.2/kmtools_cython/lib/include/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     7236 2024-05-02 14:08:34.000000 kmat_tools-0.0.2/kmtools_cython/lib/include/common.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)    21542 2024-04-15 17:11:50.000000 kmat_tools-0.0.2/kmtools_cython/lib/include/khash.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     7269 2024-04-25 15:01:55.000000 kmat_tools-0.0.2/kmtools_cython/lib/include/km_basic_filter.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     7255 2024-05-02 15:16:58.000000 kmat_tools-0.0.2/kmtools_cython/lib/include/km_fasta.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       85 2024-05-06 16:23:50.000000 kmat_tools-0.0.2/kmtools_cython/lib/include/km_reset.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     7257 2024-05-03 12:56:22.000000 kmat_tools-0.0.2/kmtools_cython/lib/include/km_unitig.h
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     8633 2024-04-15 17:11:50.000000 kmat_tools-0.0.2/kmtools_cython/lib/include/kseq.h
-drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-10 15:04:07.391669 kmat_tools-0.0.2/kmtools_cython/lib/src/
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     4563 2024-05-07 11:48:34.000000 kmat_tools-0.0.2/kmtools_cython/lib/src/km_basic_filter.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     3576 2024-04-08 14:46:29.000000 kmat_tools-0.0.2/kmtools_cython/lib/src/km_diff.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2285 2024-05-09 14:31:18.000000 kmat_tools-0.0.2/kmtools_cython/lib/src/km_fasta.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     4242 2024-04-08 14:46:29.000000 kmat_tools-0.0.2/kmtools_cython/lib/src/km_merge.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      141 2024-05-07 11:23:29.000000 kmat_tools-0.0.2/kmtools_cython/lib/src/km_reset.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2957 2024-04-08 14:46:29.000000 kmat_tools-0.0.2/kmtools_cython/lib/src/km_reverse.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     3591 2024-04-25 13:02:14.000000 kmat_tools-0.0.2/kmtools_cython/lib/src/km_select.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2334 2024-04-24 12:11:44.000000 kmat_tools-0.0.2/kmtools_cython/lib/src/km_tools.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     6253 2024-05-07 11:49:02.000000 kmat_tools-0.0.2/kmtools_cython/lib/src/km_unitig.c
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      117 2024-04-25 13:57:27.000000 kmat_tools-0.0.2/kmtools_cython/pyproject.toml
--rw-r--r--   0 cduitama (36963) seqbio   (97979)      134 2024-04-25 14:19:54.000000 kmat_tools-0.0.2/pyproject.toml
--rw-r--r--   0 cduitama (36963) seqbio   (97979)       38 2024-05-10 15:04:07.399056 kmat_tools-0.0.2/setup.cfg
--rw-r--r--   0 cduitama (36963) seqbio   (97979)     2728 2024-05-10 15:03:50.000000 kmat_tools-0.0.2/setup.py
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.225576 kmat_tools-0.0.6/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1075 2024-05-10 13:32:59.000000 kmat_tools-0.0.6/LICENSE
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       36 2024-04-25 14:25:41.000000 kmat_tools-0.0.6/MANIFEST.in
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1478 2024-05-13 11:57:56.225108 kmat_tools-0.0.6/PKG-INFO
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      984 2024-05-10 13:44:58.000000 kmat_tools-0.0.6/README.md
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.228228 kmat_tools-0.0.6/kmat_tools.egg-info/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1478 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1771 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        1 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      338 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/entry_points.txt
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       44 2024-05-13 11:57:56.000000 kmat_tools-0.0.6/kmat_tools.egg-info/top_level.txt
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.161024 kmat_tools-0.0.6/kmtools_cython/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)   301593 2024-05-13 11:57:55.000000 kmat_tools-0.0.6/kmtools_cython/km_basic_filter.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      131 2024-05-02 16:15:26.000000 kmat_tools-0.0.6/kmtools_cython/km_basic_filter.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1117 2024-05-07 12:15:08.000000 kmat_tools-0.0.6/kmtools_cython/km_basic_filter.pyx
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)   290013 2024-05-13 11:57:55.000000 kmat_tools-0.0.6/kmtools_cython/km_fasta.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      149 2024-05-07 10:18:19.000000 kmat_tools-0.0.6/kmtools_cython/km_fasta.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1036 2024-05-07 11:08:30.000000 kmat_tools-0.0.6/kmtools_cython/km_fasta.pyx
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)   221907 2024-05-06 16:37:02.000000 kmat_tools-0.0.6/kmtools_cython/km_reset.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      104 2024-05-06 16:36:55.000000 kmat_tools-0.0.6/kmtools_cython/km_reset.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       68 2024-05-06 16:33:39.000000 kmat_tools-0.0.6/kmtools_cython/km_reset.pyx
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       92 2024-05-02 13:30:32.000000 kmat_tools-0.0.6/kmtools_cython/km_select.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2631 2024-04-25 14:16:14.000000 kmat_tools-0.0.6/kmtools_cython/km_select.pyx
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.178300 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)        0 2024-05-07 14:14:50.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__init__.py
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.182877 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      210 2024-05-07 14:21:11.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2521 2024-05-09 13:49:00.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1690 2024-05-09 13:49:00.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2177 2024-05-09 14:29:01.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1617 2024-05-09 13:44:33.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_basic_filter_wrapper.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      917 2024-05-09 13:44:24.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_fasta_wrapper.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1303 2024-05-09 13:48:28.000000 kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_unitig_wrapper.py
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)   290130 2024-05-13 11:57:55.000000 kmat_tools-0.0.6/kmtools_cython/km_unitig.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      119 2024-05-03 12:56:30.000000 kmat_tools-0.0.6/kmtools_cython/km_unitig.pxd
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     1048 2024-05-09 14:35:01.000000 kmat_tools-0.0.6/kmtools_cython/km_unitig.pyx
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.080724 kmat_tools-0.0.6/kmtools_cython/lib/
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.199470 kmat_tools-0.0.6/kmtools_cython/lib/include/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     7236 2024-05-02 14:08:34.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/common.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)    21542 2024-04-15 17:11:50.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/khash.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     7269 2024-04-25 15:01:55.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/km_basic_filter.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     7255 2024-05-02 15:16:58.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/km_fasta.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       85 2024-05-06 16:23:50.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/km_reset.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     7257 2024-05-03 12:56:22.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/km_unitig.h
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     8633 2024-04-15 17:11:50.000000 kmat_tools-0.0.6/kmtools_cython/lib/include/kseq.h
+drwxr-xr-x   0 cduitama (36963) seqbio   (97979)        0 2024-05-13 11:57:56.223915 kmat_tools-0.0.6/kmtools_cython/lib/src/
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     4563 2024-05-07 11:48:34.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_basic_filter.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     3576 2024-04-08 14:46:29.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_diff.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2285 2024-05-09 14:31:18.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_fasta.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     4242 2024-04-08 14:46:29.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_merge.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      141 2024-05-07 11:23:29.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_reset.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2957 2024-04-08 14:46:29.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_reverse.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     3591 2024-04-25 13:02:14.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_select.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2334 2024-04-24 12:11:44.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_tools.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     6253 2024-05-07 11:49:02.000000 kmat_tools-0.0.6/kmtools_cython/lib/src/km_unitig.c
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      117 2024-04-25 13:57:27.000000 kmat_tools-0.0.6/kmtools_cython/pyproject.toml
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)      117 2024-05-13 11:00:32.000000 kmat_tools-0.0.6/pyproject.toml
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)       38 2024-05-13 11:57:56.227263 kmat_tools-0.0.6/setup.cfg
+-rw-r--r--   0 cduitama (36963) seqbio   (97979)     2682 2024-05-13 11:57:05.000000 kmat_tools-0.0.6/setup.py
```

### Comparing `kmat_tools-0.0.2/LICENSE` & `kmat_tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/PKG-INFO` & `kmat_tools-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmat_tools
-Version: 0.0.2
+Version: 0.0.6
 Home-page: https://github.com/CamilaDuitama/kmat_tools
 Author: Riccardo Vicedomini, Francesco Andreace, Camila Duitama
 Author-email: cduitama@pasteur.fr
 Project-URL: Bug Tracker, https://github.com/CamilaDuitama/kmat_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kmat_tools-0.0.2/README.md` & `kmat_tools-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmat_tools.egg-info/PKG-INFO` & `kmat_tools-0.0.6/kmat_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmat_tools
-Version: 0.0.2
+Version: 0.0.6
 Home-page: https://github.com/CamilaDuitama/kmat_tools
 Author: Riccardo Vicedomini, Francesco Andreace, Camila Duitama
 Author-email: cduitama@pasteur.fr
 Project-URL: Bug Tracker, https://github.com/CamilaDuitama/kmat_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kmat_tools-0.0.2/kmat_tools.egg-info/SOURCES.txt` & `kmat_tools-0.0.6/kmat_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_basic_filter.c` & `kmat_tools-0.0.6/kmtools_cython/km_basic_filter.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_basic_filter.pyx` & `kmat_tools-0.0.6/kmtools_cython/km_basic_filter.pyx`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_fasta.c` & `kmat_tools-0.0.6/kmtools_cython/km_fasta.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_fasta.pyx` & `kmat_tools-0.0.6/kmtools_cython/km_fasta.pyx`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_reset.c` & `kmat_tools-0.0.6/kmtools_cython/km_reset.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_select.pyx` & `kmat_tools-0.0.6/kmtools_cython/km_select.pyx`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc` & `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_basic_filter_wrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc` & `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_fasta_wrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc` & `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/__pycache__/km_unitig_wrapper.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/km_basic_filter_wrapper.py` & `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_basic_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/km_fasta_wrapper.py` & `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_fasta_wrapper.py`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_tools_wrappers/km_unitig_wrapper.py` & `kmat_tools-0.0.6/kmtools_cython/km_tools_wrappers/km_unitig_wrapper.py`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_unitig.c` & `kmat_tools-0.0.6/kmtools_cython/km_unitig.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/km_unitig.pyx` & `kmat_tools-0.0.6/kmtools_cython/km_unitig.pyx`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/include/common.h` & `kmat_tools-0.0.6/kmtools_cython/lib/include/common.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/include/khash.h` & `kmat_tools-0.0.6/kmtools_cython/lib/include/khash.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/include/km_basic_filter.h` & `kmat_tools-0.0.6/kmtools_cython/lib/include/km_basic_filter.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/include/km_fasta.h` & `kmat_tools-0.0.6/kmtools_cython/lib/include/km_fasta.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/include/km_unitig.h` & `kmat_tools-0.0.6/kmtools_cython/lib/include/km_unitig.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/include/kseq.h` & `kmat_tools-0.0.6/kmtools_cython/lib/include/kseq.h`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/src/km_basic_filter.c` & `kmat_tools-0.0.6/kmtools_cython/lib/src/km_basic_filter.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/src/km_diff.c` & `kmat_tools-0.0.6/kmtools_cython/lib/src/km_diff.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/src/km_fasta.c` & `kmat_tools-0.0.6/kmtools_cython/lib/src/km_fasta.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/src/km_merge.c` & `kmat_tools-0.0.6/kmtools_cython/lib/src/km_merge.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/src/km_reverse.c` & `kmat_tools-0.0.6/kmtools_cython/lib/src/km_reverse.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/src/km_select.c` & `kmat_tools-0.0.6/kmtools_cython/lib/src/km_select.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/src/km_tools.c` & `kmat_tools-0.0.6/kmtools_cython/lib/src/km_tools.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/kmtools_cython/lib/src/km_unitig.c` & `kmat_tools-0.0.6/kmtools_cython/lib/src/km_unitig.c`

 * *Files identical despite different names*

### Comparing `kmat_tools-0.0.2/setup.py` & `kmat_tools-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages,Extension
+from setuptools import setup,Extension
 from Cython.Build import cythonize
 
 EXTENSION_PATH = "kmtools_cython"
 
 ext1 = Extension("km_basic_filter",
                  sources=[f"{EXTENSION_PATH}/km_basic_filter.pyx", f"{EXTENSION_PATH}/lib/src/km_basic_filter.c"],
                  include_dirs=[f"{EXTENSION_PATH}/lib/include"],
@@ -28,15 +28,15 @@
                  libraries=['z', 'm'])
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="kmat_tools",
-    version="0.0.2",
+    version="0.0.6",
     author="Riccardo Vicedomini, Francesco Andreace, Camila Duitama",
     author_email="cduitama@pasteur.fr",
     include_package_data=True,
     package_data={"": ["MANIFEST", "LICENSE"]},
     ext_modules = cythonize([ext1,ext2,ext3,ext4]),
     entry_points={
         "console_scripts": [
@@ -53,9 +53,8 @@
         "Bug Tracker": "https://github.com/CamilaDuitama/kmat_tools/issues",
     },
         classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    setup_requires=["cython"],
 )
```

