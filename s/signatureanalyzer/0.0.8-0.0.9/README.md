# Comparing `tmp/signatureanalyzer-0.0.8.tar.gz` & `tmp/signatureanalyzer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signatureanalyzer-0.0.8.tar", last modified: Sun May 12 20:39:10 2024, max compression
+gzip compressed data, was "signatureanalyzer-0.0.9.tar", last modified: Mon May 13 03:02:36 2024, max compression
```

## Comparing `signatureanalyzer-0.0.8.tar` & `signatureanalyzer-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.774026 signatureanalyzer-0.0.8/
--rw-r--r--   0 shankaraanand   (501) staff       (20)     1072 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/LICENSE
--rw-r--r--   0 shankaraanand   (501) staff       (20)     5234 2024-05-12 20:39:10.773914 signatureanalyzer-0.0.8/PKG-INFO
--rw-r--r--   0 shankaraanand   (501) staff       (20)     4493 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/README.md
--rw-r--r--   0 shankaraanand   (501) staff       (20)       38 2024-05-12 20:39:10.774069 signatureanalyzer-0.0.8/setup.cfg
--rw-r--r--   0 shankaraanand   (501) staff       (20)     2033 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/setup.py
-drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.767446 signatureanalyzer-0.0.8/signatureanalyzer/
--rw-r--r--   0 shankaraanand   (501) staff       (20)      389 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/__init__.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)     6880 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/__main__.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)     5048 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/bnmf.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)     1187 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/consensus.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)    12204 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/context.py
-drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.769042 signatureanalyzer-0.0.8/signatureanalyzer/pathways/
--rw-r--r--   0 shankaraanand   (501) staff       (20)       66 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/pathways/__init__.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)     5674 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/pathways/_gsea.py
-drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.770942 signatureanalyzer-0.0.8/signatureanalyzer/plotting/
--rw-r--r--   0 shankaraanand   (501) staff       (20)      557 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/__init__.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)     1464 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_cosine.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)    38234 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_muts.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)     7514 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_nmf.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)     7523 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_rna.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)     2312 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_utils.py
-drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.765013 signatureanalyzer-0.0.8/signatureanalyzer/ref/
-drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.771084 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v2/
--rw-r--r--   0 shankaraanand   (501) staff       (20)    36385 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv
-drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.773116 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/
--rw-r--r--   0 shankaraanand   (501) staff       (20)     9695 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv
--rw-r--r--   0 shankaraanand   (501) staff       (20)    23307 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv
--rw-r--r--   0 shankaraanand   (501) staff       (20)    74211 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv
--rw-r--r--   0 shankaraanand   (501) staff       (20)    90771 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv
--rw-r--r--   0 shankaraanand   (501) staff       (20)   180467 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv
--rw-r--r--   0 shankaraanand   (501) staff       (20)    17305 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/signatureanalyzer.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)    14446 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/spectra.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)    12055 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/supervised_bnmf.py
--rw-r--r--   0 shankaraanand   (501) staff       (20)    37040 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/utils.py
-drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.768712 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/
--rw-r--r--   0 shankaraanand   (501) staff       (20)     5234 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/PKG-INFO
--rw-r--r--   0 shankaraanand   (501) staff       (20)     1156 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 shankaraanand   (501) staff       (20)        1 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 shankaraanand   (501) staff       (20)       70 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/entry_points.txt
--rw-r--r--   0 shankaraanand   (501) staff       (20)      200 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/requires.txt
--rw-r--r--   0 shankaraanand   (501) staff       (20)       18 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/top_level.txt
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-13 03:02:36.541585 signatureanalyzer-0.0.9/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     1072 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/LICENSE
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     5234 2024-05-13 03:02:36.541469 signatureanalyzer-0.0.9/PKG-INFO
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     4493 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/README.md
+-rw-r--r--   0 shankaraanand   (501) staff       (20)       38 2024-05-13 03:02:36.541634 signatureanalyzer-0.0.9/setup.cfg
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     2033 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/setup.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-13 03:02:36.537822 signatureanalyzer-0.0.9/signatureanalyzer/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)      389 2024-05-13 03:02:25.000000 signatureanalyzer-0.0.9/signatureanalyzer/__init__.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     6880 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/__main__.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     5048 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/bnmf.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     1187 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/consensus.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    12204 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/context.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-13 03:02:36.538893 signatureanalyzer-0.0.9/signatureanalyzer/pathways/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)       66 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/pathways/__init__.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     5674 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/pathways/_gsea.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-13 03:02:36.539650 signatureanalyzer-0.0.9/signatureanalyzer/plotting/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)      557 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/plotting/__init__.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     1464 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/plotting/_cosine.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    38234 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/plotting/_muts.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     7514 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/plotting/_nmf.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     7523 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/plotting/_rna.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     2312 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/plotting/_utils.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-13 03:02:36.535927 signatureanalyzer-0.0.9/signatureanalyzer/ref/
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-13 03:02:36.539772 signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v2/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    36385 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-13 03:02:36.540557 signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     9695 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    23307 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    74211 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    90771 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)   180467 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    17305 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/signatureanalyzer.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-13 03:02:36.541302 signatureanalyzer-0.0.9/signatureanalyzer/signatureanalyzer_gpu/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    11404 2024-05-13 02:57:06.000000 signatureanalyzer-0.0.9/signatureanalyzer/signatureanalyzer_gpu/ARD_NMF.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     6125 2024-05-13 02:57:06.000000 signatureanalyzer-0.0.9/signatureanalyzer/signatureanalyzer_gpu/NMF_functions.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     8945 2024-05-13 02:57:06.000000 signatureanalyzer-0.0.9/signatureanalyzer/signatureanalyzer_gpu/SignatureAnalyzer-GPU.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)        0 2024-05-13 02:57:06.000000 signatureanalyzer-0.0.9/signatureanalyzer/signatureanalyzer_gpu/__init__.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    14446 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/spectra.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    12055 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/supervised_bnmf.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    37040 2024-05-13 02:57:05.000000 signatureanalyzer-0.0.9/signatureanalyzer/utils.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-13 03:02:36.538616 signatureanalyzer-0.0.9/signatureanalyzer.egg-info/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     5234 2024-05-13 03:02:36.000000 signatureanalyzer-0.0.9/signatureanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     1381 2024-05-13 03:02:36.000000 signatureanalyzer-0.0.9/signatureanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 shankaraanand   (501) staff       (20)        1 2024-05-13 03:02:36.000000 signatureanalyzer-0.0.9/signatureanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 shankaraanand   (501) staff       (20)       70 2024-05-13 03:02:36.000000 signatureanalyzer-0.0.9/signatureanalyzer.egg-info/entry_points.txt
+-rw-r--r--   0 shankaraanand   (501) staff       (20)      200 2024-05-13 03:02:36.000000 signatureanalyzer-0.0.9/signatureanalyzer.egg-info/requires.txt
+-rw-r--r--   0 shankaraanand   (501) staff       (20)       18 2024-05-13 03:02:36.000000 signatureanalyzer-0.0.9/signatureanalyzer.egg-info/top_level.txt
```

### Comparing `signatureanalyzer-0.0.8/LICENSE` & `signatureanalyzer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/PKG-INFO` & `signatureanalyzer-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signatureanalyzer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bayesian NMF methods for mutational signature analysis & transcriptomic profiling on GPUs (Getz Lab).
 Home-page: https://github.com/broadinstitute/getzlab-SignatureAnalyzer
 Author: Shankara Anand & Justin Cha - Broad Institute - Cancer Genome Computational Analysis
 Author-email: sanand@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `signatureanalyzer-0.0.8/README.md` & `signatureanalyzer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/setup.py` & `signatureanalyzer-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/__main__.py` & `signatureanalyzer-0.0.9/signatureanalyzer/__main__.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/bnmf.py` & `signatureanalyzer-0.0.9/signatureanalyzer/bnmf.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/consensus.py` & `signatureanalyzer-0.0.9/signatureanalyzer/consensus.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/context.py` & `signatureanalyzer-0.0.9/signatureanalyzer/context.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/pathways/_gsea.py` & `signatureanalyzer-0.0.9/signatureanalyzer/pathways/_gsea.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/plotting/__init__.py` & `signatureanalyzer-0.0.9/signatureanalyzer/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/plotting/_cosine.py` & `signatureanalyzer-0.0.9/signatureanalyzer/plotting/_cosine.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/plotting/_muts.py` & `signatureanalyzer-0.0.9/signatureanalyzer/plotting/_muts.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/plotting/_nmf.py` & `signatureanalyzer-0.0.9/signatureanalyzer/plotting/_nmf.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/plotting/_rna.py` & `signatureanalyzer-0.0.9/signatureanalyzer/plotting/_rna.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/plotting/_utils.py` & `signatureanalyzer-0.0.9/signatureanalyzer/plotting/_utils.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv` & `signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv` & `signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv` & `signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv` & `signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv` & `signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv` & `signatureanalyzer-0.0.9/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/signatureanalyzer.py` & `signatureanalyzer-0.0.9/signatureanalyzer/signatureanalyzer.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/spectra.py` & `signatureanalyzer-0.0.9/signatureanalyzer/spectra.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/supervised_bnmf.py` & `signatureanalyzer-0.0.9/signatureanalyzer/supervised_bnmf.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer/utils.py` & `signatureanalyzer-0.0.9/signatureanalyzer/utils.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer.egg-info/PKG-INFO` & `signatureanalyzer-0.0.9/signatureanalyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signatureanalyzer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bayesian NMF methods for mutational signature analysis & transcriptomic profiling on GPUs (Getz Lab).
 Home-page: https://github.com/broadinstitute/getzlab-SignatureAnalyzer
 Author: Shankara Anand & Justin Cha - Broad Institute - Cancer Genome Computational Analysis
 Author-email: sanand@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `signatureanalyzer-0.0.8/signatureanalyzer.egg-info/SOURCES.txt` & `signatureanalyzer-0.0.9/signatureanalyzer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -25,8 +25,12 @@
 signatureanalyzer/plotting/_rna.py
 signatureanalyzer/plotting/_utils.py
 signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv
 signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv
 signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv
 signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv
 signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv
-signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv
+signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv
+signatureanalyzer/signatureanalyzer_gpu/ARD_NMF.py
+signatureanalyzer/signatureanalyzer_gpu/NMF_functions.py
+signatureanalyzer/signatureanalyzer_gpu/SignatureAnalyzer-GPU.py
+signatureanalyzer/signatureanalyzer_gpu/__init__.py
```

