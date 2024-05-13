# Comparing `tmp/WangLab-0.1.1.tar.gz` & `tmp/WangLab-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WangLab-0.1.1.tar", last modified: Fri Apr 12 12:59:33 2024, max compression
+gzip compressed data, was "WangLab-1.0.0b0.tar", last modified: Mon May 13 12:41:57 2024, max compression
```

## Comparing `WangLab-0.1.1.tar` & `WangLab-1.0.0b0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.940405 WangLab-0.1.1/
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1066 2023-12-18 21:56:50.000000 WangLab-0.1.1/LICENSE
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     8091 2024-04-12 12:59:33.938410 WangLab-0.1.1/PKG-INFO
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     6948 2024-04-11 20:40:10.000000 WangLab-0.1.1/README.md
-drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.894386 WangLab-0.1.1/WangLab/
-drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.909405 WangLab-0.1.1/WangLab/ChIP_seq/
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1880 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/ChIP_seq/bowtie_ChIP_Seq.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1501 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/ChIP_seq/cutadapt_ChIP_Seq.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1418 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/ChIP_seq/macs.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)       18 2024-04-12 12:54:03.000000 WangLab-0.1.1/WangLab/Constants.py
-drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.911398 WangLab-0.1.1/WangLab/RNA_seq/
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     3284 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/RNA_seq/rna_seq.py
-drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.925403 WangLab-0.1.1/WangLab/Sequence_operate/
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2538 2024-04-12 11:49:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/calc_content.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     3978 2024-04-12 12:32:13.000000 WangLab-0.1.1/WangLab/Sequence_operate/calc_usage_deviation.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     3540 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/extract_seqs.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     5745 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/file_merge.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1023 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/ossutil.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     9147 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/primer_blast.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2803 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/primer_generator.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     4980 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/qPCR.py
-drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.932403 WangLab-0.1.1/WangLab/TIS/
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1342 2024-04-11 20:40:14.000000 WangLab-0.1.1/WangLab/TIS/bowtie.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)      909 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/TIS/combine_reads.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     6293 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/TIS/count_reads.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2623 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/TIS/cutadapt.py
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)       76 2024-04-11 20:40:14.000000 WangLab-0.1.1/WangLab/__init__.py
-drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.904396 WangLab-0.1.1/WangLab.egg-info/
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     8091 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/PKG-INFO
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)      802 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/SOURCES.txt
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)        1 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/dependency_links.txt
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)       68 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/requires.txt
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)        8 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/top_level.txt
-drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.936396 WangLab-0.1.1/bin/
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)    21801 2024-04-12 12:29:52.000000 WangLab-0.1.1/bin/wanglab
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)       24 2024-04-11 20:40:10.000000 WangLab-0.1.1/bin/wanglab.bat
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)       38 2024-04-12 12:59:33.940405 WangLab-0.1.1/setup.cfg
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2479 2024-04-12 12:59:25.000000 WangLab-0.1.1/setup.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-05-13 12:41:57.645444 WangLab-1.0.0b0/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1066 2023-12-18 21:56:50.000000 WangLab-1.0.0b0/LICENSE
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     8093 2024-05-13 12:41:57.643444 WangLab-1.0.0b0/PKG-INFO
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     6948 2024-04-11 20:40:10.000000 WangLab-1.0.0b0/README.md
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-05-13 12:41:57.591431 WangLab-1.0.0b0/WangLab/
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-05-13 12:41:57.609435 WangLab-1.0.0b0/WangLab/ChIP_seq/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1880 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/ChIP_seq/bowtie_ChIP_Seq.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1501 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/ChIP_seq/cutadapt_ChIP_Seq.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1418 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/ChIP_seq/macs.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     4733 2023-12-16 12:41:56.000000 WangLab-1.0.0b0/WangLab/ChIP_seq/read_classifier.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       19 2024-05-13 12:40:43.000000 WangLab-1.0.0b0/WangLab/Constants.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-05-13 12:41:57.610436 WangLab-1.0.0b0/WangLab/RNA_seq/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     3284 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/RNA_seq/rna_seq.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-05-13 12:41:57.627439 WangLab-1.0.0b0/WangLab/Sequence_operate/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2538 2024-04-12 11:49:12.000000 WangLab-1.0.0b0/WangLab/Sequence_operate/calc_content.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     3978 2024-04-12 12:32:13.000000 WangLab-1.0.0b0/WangLab/Sequence_operate/calc_usage_deviation.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     3540 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/Sequence_operate/extract_seqs.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     5745 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/Sequence_operate/file_merge.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1023 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/Sequence_operate/ossutil.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     9147 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/Sequence_operate/primer_blast.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2803 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/Sequence_operate/primer_generator.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     4980 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/Sequence_operate/qPCR.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-05-13 12:41:57.636443 WangLab-1.0.0b0/WangLab/TIS/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1342 2024-04-11 20:40:14.000000 WangLab-1.0.0b0/WangLab/TIS/bowtie.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)      909 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/TIS/combine_reads.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     6293 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/TIS/count_reads.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2623 2024-04-11 20:40:12.000000 WangLab-1.0.0b0/WangLab/TIS/cutadapt.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       76 2024-04-11 20:40:14.000000 WangLab-1.0.0b0/WangLab/__init__.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-05-13 12:41:57.601433 WangLab-1.0.0b0/WangLab.egg-info/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     8093 2024-05-13 12:41:57.000000 WangLab-1.0.0b0/WangLab.egg-info/PKG-INFO
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)      838 2024-05-13 12:41:57.000000 WangLab-1.0.0b0/WangLab.egg-info/SOURCES.txt
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)        1 2024-05-13 12:41:57.000000 WangLab-1.0.0b0/WangLab.egg-info/dependency_links.txt
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       68 2024-05-13 12:41:57.000000 WangLab-1.0.0b0/WangLab.egg-info/requires.txt
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)        8 2024-05-13 12:41:57.000000 WangLab-1.0.0b0/WangLab.egg-info/top_level.txt
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-05-13 12:41:57.641443 WangLab-1.0.0b0/bin/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)    23273 2024-05-13 12:23:33.000000 WangLab-1.0.0b0/bin/wanglab
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       24 2024-04-11 20:40:10.000000 WangLab-1.0.0b0/bin/wanglab.bat
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       38 2024-05-13 12:41:57.645444 WangLab-1.0.0b0/setup.cfg
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2479 2024-04-12 12:59:25.000000 WangLab-1.0.0b0/setup.py
```

### Comparing `WangLab-0.1.1/LICENSE` & `WangLab-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/PKG-INFO` & `WangLab-1.0.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WangLab
-Version: 0.1.1
+Version: 1.0.0b0
 Summary: Simple bioinformatic tools
 Home-page: http://github.com/byf1999/WangLab/
 Author: Yifan Bu
 Author-email: y30210580@163.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `WangLab-0.1.1/README.md` & `WangLab-1.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/ChIP_seq/bowtie_ChIP_Seq.py` & `WangLab-1.0.0b0/WangLab/ChIP_seq/bowtie_ChIP_Seq.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/ChIP_seq/cutadapt_ChIP_Seq.py` & `WangLab-1.0.0b0/WangLab/ChIP_seq/cutadapt_ChIP_Seq.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/ChIP_seq/macs.py` & `WangLab-1.0.0b0/WangLab/ChIP_seq/macs.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/RNA_seq/rna_seq.py` & `WangLab-1.0.0b0/WangLab/RNA_seq/rna_seq.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/Sequence_operate/calc_content.py` & `WangLab-1.0.0b0/WangLab/Sequence_operate/calc_content.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/Sequence_operate/calc_usage_deviation.py` & `WangLab-1.0.0b0/WangLab/Sequence_operate/calc_usage_deviation.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/Sequence_operate/extract_seqs.py` & `WangLab-1.0.0b0/WangLab/Sequence_operate/extract_seqs.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/Sequence_operate/file_merge.py` & `WangLab-1.0.0b0/WangLab/Sequence_operate/file_merge.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/Sequence_operate/ossutil.py` & `WangLab-1.0.0b0/WangLab/Sequence_operate/ossutil.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/Sequence_operate/primer_blast.py` & `WangLab-1.0.0b0/WangLab/Sequence_operate/primer_blast.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/Sequence_operate/primer_generator.py` & `WangLab-1.0.0b0/WangLab/Sequence_operate/primer_generator.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/Sequence_operate/qPCR.py` & `WangLab-1.0.0b0/WangLab/Sequence_operate/qPCR.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/TIS/bowtie.py` & `WangLab-1.0.0b0/WangLab/TIS/bowtie.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/TIS/combine_reads.py` & `WangLab-1.0.0b0/WangLab/TIS/combine_reads.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/TIS/count_reads.py` & `WangLab-1.0.0b0/WangLab/TIS/count_reads.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab/TIS/cutadapt.py` & `WangLab-1.0.0b0/WangLab/TIS/cutadapt.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.1.1/WangLab.egg-info/PKG-INFO` & `WangLab-1.0.0b0/WangLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WangLab
-Version: 0.1.1
+Version: 1.0.0b0
 Summary: Simple bioinformatic tools
 Home-page: http://github.com/byf1999/WangLab/
 Author: Yifan Bu
 Author-email: y30210580@163.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `WangLab-0.1.1/WangLab.egg-info/SOURCES.txt` & `WangLab-1.0.0b0/WangLab.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 WangLab.egg-info/SOURCES.txt
 WangLab.egg-info/dependency_links.txt
 WangLab.egg-info/requires.txt
 WangLab.egg-info/top_level.txt
 WangLab/ChIP_seq/bowtie_ChIP_Seq.py
 WangLab/ChIP_seq/cutadapt_ChIP_Seq.py
 WangLab/ChIP_seq/macs.py
+WangLab/ChIP_seq/read_classifier.py
 WangLab/RNA_seq/rna_seq.py
 WangLab/Sequence_operate/calc_content.py
 WangLab/Sequence_operate/calc_usage_deviation.py
 WangLab/Sequence_operate/extract_seqs.py
 WangLab/Sequence_operate/file_merge.py
 WangLab/Sequence_operate/ossutil.py
 WangLab/Sequence_operate/primer_blast.py
```

### Comparing `WangLab-0.1.1/bin/wanglab` & `WangLab-1.0.0b0/bin/wanglab`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/home/byf1999/anaconda3/bin/python
 """
 Description: WangLab main executable.
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the MIT License (see the file LICENSE included with
 the distribution).
 """
@@ -73,14 +73,19 @@
     elif subcommand == 'qPCR':
         from WangLab.Sequence_operate.qPCR import calc
         calc(args)
 
     elif subcommand == 'calc_usage_deviation':
         from WangLab.Sequence_operate.calc_usage_deviation import main
         main(args)
+
+    elif subcommand == 'read_classifier':
+        from WangLab.ChIP_seq.read_classifier import main
+        main(args)
+
     else:
         print(f'Command {subcommand} not recognized!')
         return
 
 
 def prepare_argparser():
     description = f"WangLab main executable. Version: {VERSION}"
@@ -128,14 +133,17 @@
     add_primer_blast(subparsers)
 
     # command for 'qPCR'
     add_qPCR(subparsers)
 
     # command for 'calc_usage_deviation'
     add_calc_usage_devitation(subparsers)
+
+    # command for 'read_classifier'
+    add_read_classifier(subparsers)
     return argparser
 
 
 def add_qPCR(subparsers):
     """Add function 'qPCR' argument parsers"""
     name = 'qPCR'
 
@@ -415,14 +423,35 @@
     argparser_calc_usage_deviation.add_argument("-n", '--n-max', dest='n', type=str, required=False, nargs="?",
                                                 help='Maximum number of successive  nucleotides', default='3')
     argparser_calc_usage_deviation.add_argument("-l", '--length', dest='length', type=str, required=False, nargs="?",
                                                 help='Length of peaks selected from summits', default='200')
     return
 
 
+def add_read_classifier(subparsers):
+    """Add function 'read_classifier' argument parsers"""
+    name = 'read_classifier'
+
+    # from WangLab.Sequence_operate.calc_usage_deviation import prepare_argparser
+    help_content = 'Classify related genes of ChIP-Seq callpeak results'
+    argparser_read_classifier = subparsers.add_parser(name, help=help_content,
+                                                      formatter_class=ap.RawDescriptionHelpFormatter, epilog=f"""Examples:
+    $ {os.path.basename(sys.argv[0])} {name} -i peak.xlsx -a annot.gff -o output.xlsx
+""")
+
+    argparser_read_classifier.add_argument('-a', '--annot', dest='annot', nargs='?', type=str, required=True,
+                      help='Annotation file, should consist at least 4 columns, each represent gene name, start, end, and strain')
+    argparser_read_classifier.add_argument('-i', '--input', dest='input', nargs='?', type=str, required=True,
+                      help='Peak informations, should be in same format with what MACS3 generates')
+    argparser_read_classifier.add_argument('-o', '--output', dest='output', nargs='?', type=str, required=False, default=None,
+                      help='Output file, will output to the working directory if not assigned.')
+
+    return
+
+
 def run_cutadapt(args):
     if args.data_type.upper() == 'TN-SEQ':
         if not args.plasmid:
             print(f'Please enter transposon plasmid name.')
             return
         from WangLab.TIS.cutadapt import main
         main([args.subcommand, args.dir], args.plasmid.upper())
```

### Comparing `WangLab-0.1.1/setup.py` & `WangLab-1.0.0b0/setup.py`

 * *Files identical despite different names*

