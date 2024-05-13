# Comparing `tmp/signatureanalyzer-0.0.7.tar.gz` & `tmp/signatureanalyzer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/signatureanalyzer-0.0.7.tar", last modified: Mon Mar  2 16:03:26 2020, max compression
+gzip compressed data, was "signatureanalyzer-0.0.8.tar", last modified: Sun May 12 20:39:10 2024, max compression
```

## Comparing `signatureanalyzer-0.0.7.tar` & `signatureanalyzer-0.0.8.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     6035 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/PKG-INFO
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     4293 2020-02-20 17:28:32.000000 signatureanalyzer-0.0.7/README.md
--rw-rw-r--   0 sanand    (1001) sanand    (1002)       38 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/setup.cfg
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     2046 2020-02-16 19:51:50.000000 signatureanalyzer-0.0.7/setup.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/signatureanalyzer/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)      342 2020-03-02 16:02:38.000000 signatureanalyzer-0.0.7/signatureanalyzer/__init__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     6434 2019-12-11 21:49:54.000000 signatureanalyzer-0.0.7/signatureanalyzer/__main__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     5047 2020-02-17 21:17:00.000000 signatureanalyzer-0.0.7/signatureanalyzer/bnmf.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     1187 2019-09-30 21:39:15.000000 signatureanalyzer-0.0.7/signatureanalyzer/consensus.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/signatureanalyzer/pathways/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)       66 2019-11-14 21:05:05.000000 signatureanalyzer-0.0.7/signatureanalyzer/pathways/__init__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     5674 2019-11-14 21:51:58.000000 signatureanalyzer-0.0.7/signatureanalyzer/pathways/_gsea.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/signatureanalyzer/plotting/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)      418 2020-02-20 17:28:32.000000 signatureanalyzer-0.0.7/signatureanalyzer/plotting/__init__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     1464 2019-12-09 19:39:28.000000 signatureanalyzer-0.0.7/signatureanalyzer/plotting/_cosine.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    13906 2020-02-20 17:28:32.000000 signatureanalyzer-0.0.7/signatureanalyzer/plotting/_muts.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     6531 2019-09-30 21:39:15.000000 signatureanalyzer-0.0.7/signatureanalyzer/plotting/_nmf.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     7523 2020-01-21 17:53:04.000000 signatureanalyzer-0.0.7/signatureanalyzer/plotting/_rna.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     2312 2020-01-06 00:27:47.000000 signatureanalyzer-0.0.7/signatureanalyzer/plotting/_utils.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/signatureanalyzer/ref/
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v2/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    36385 2019-10-08 20:04:37.000000 signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     9695 2019-12-09 19:51:43.000000 signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    23307 2020-02-20 17:28:32.000000 signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    74211 2019-10-08 21:22:49.000000 signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    90771 2019-10-08 20:05:14.000000 signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv
--rw-rw-r--   0 sanand    (1001) sanand    (1002)   180467 2019-10-08 21:23:44.000000 signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    17175 2020-03-02 15:59:52.000000 signatureanalyzer-0.0.7/signatureanalyzer/signatureanalyzer.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/signatureanalyzer/signatureanalyzer_gpu/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    11404 2019-12-09 21:39:20.000000 signatureanalyzer-0.0.7/signatureanalyzer/signatureanalyzer_gpu/ARD_NMF.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     6125 2019-12-09 21:39:18.000000 signatureanalyzer-0.0.7/signatureanalyzer/signatureanalyzer_gpu/NMF_functions.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     8945 2019-12-09 21:26:33.000000 signatureanalyzer-0.0.7/signatureanalyzer/signatureanalyzer_gpu/SignatureAnalyzer-GPU.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)        0 2019-12-09 21:36:41.000000 signatureanalyzer-0.0.7/signatureanalyzer/signatureanalyzer_gpu/__init__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    11255 2020-02-16 23:34:56.000000 signatureanalyzer-0.0.7/signatureanalyzer/spectra.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    18754 2020-03-02 15:59:52.000000 signatureanalyzer-0.0.7/signatureanalyzer/utils.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2020-03-02 16:03:25.000000 signatureanalyzer-0.0.7/signatureanalyzer.egg-info/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     6035 2020-03-02 16:03:23.000000 signatureanalyzer-0.0.7/signatureanalyzer.egg-info/PKG-INFO
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     1307 2020-03-02 16:03:23.000000 signatureanalyzer-0.0.7/signatureanalyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 sanand    (1001) sanand    (1002)        1 2020-03-02 16:03:23.000000 signatureanalyzer-0.0.7/signatureanalyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 sanand    (1001) sanand    (1002)       71 2020-03-02 16:03:23.000000 signatureanalyzer-0.0.7/signatureanalyzer.egg-info/entry_points.txt
--rw-rw-r--   0 sanand    (1001) sanand    (1002)      203 2020-03-02 16:03:23.000000 signatureanalyzer-0.0.7/signatureanalyzer.egg-info/requires.txt
--rw-rw-r--   0 sanand    (1001) sanand    (1002)       18 2020-03-02 16:03:23.000000 signatureanalyzer-0.0.7/signatureanalyzer.egg-info/top_level.txt
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.774026 signatureanalyzer-0.0.8/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     1072 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/LICENSE
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     5234 2024-05-12 20:39:10.773914 signatureanalyzer-0.0.8/PKG-INFO
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     4493 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/README.md
+-rw-r--r--   0 shankaraanand   (501) staff       (20)       38 2024-05-12 20:39:10.774069 signatureanalyzer-0.0.8/setup.cfg
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     2033 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/setup.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.767446 signatureanalyzer-0.0.8/signatureanalyzer/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)      389 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/__init__.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     6880 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/__main__.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     5048 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/bnmf.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     1187 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/consensus.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    12204 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/context.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.769042 signatureanalyzer-0.0.8/signatureanalyzer/pathways/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)       66 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/pathways/__init__.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     5674 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/pathways/_gsea.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.770942 signatureanalyzer-0.0.8/signatureanalyzer/plotting/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)      557 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/__init__.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     1464 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_cosine.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    38234 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_muts.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     7514 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_nmf.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     7523 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_rna.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     2312 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/plotting/_utils.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.765013 signatureanalyzer-0.0.8/signatureanalyzer/ref/
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.771084 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v2/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    36385 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.773116 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     9695 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    23307 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    74211 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    90771 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)   180467 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    17305 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/signatureanalyzer.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    14446 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/spectra.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    12055 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/supervised_bnmf.py
+-rw-r--r--   0 shankaraanand   (501) staff       (20)    37040 2024-05-12 20:31:25.000000 signatureanalyzer-0.0.8/signatureanalyzer/utils.py
+drwxr-xr-x   0 shankaraanand   (501) staff       (20)        0 2024-05-12 20:39:10.768712 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     5234 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 shankaraanand   (501) staff       (20)     1156 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 shankaraanand   (501) staff       (20)        1 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 shankaraanand   (501) staff       (20)       70 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/entry_points.txt
+-rw-r--r--   0 shankaraanand   (501) staff       (20)      200 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/requires.txt
+-rw-r--r--   0 shankaraanand   (501) staff       (20)       18 2024-05-12 20:39:10.000000 signatureanalyzer-0.0.8/signatureanalyzer.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `signatureanalyzer-0.0.7/PKG-INFO` & `signatureanalyzer-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,142 @@
 Metadata-Version: 2.1
 Name: signatureanalyzer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bayesian NMF methods for mutational signature analysis & transcriptomic profiling on GPUs (Getz Lab).
 Home-page: https://github.com/broadinstitute/getzlab-SignatureAnalyzer
 Author: Shankara Anand & Justin Cha - Broad Institute - Cancer Genome Computational Analysis
 Author-email: sanand@broadinstitute.org
 License: MIT
-Description: # SignatureAnalyzer
-        
-        Automatic Relevance Determination (ARD) - NMF of mutational signature &amp; expression data. Designed for scalability using Pytorch to run using GPUs if available.
-        * See `docs` for a more in-depth description of how to use method.
-        
-        _Requires Python 3.6.0 or higher._
-        
-        ## Installation
-        
-        ##### PIP
-        
-        `pip3 install signatureanalyzer`
-        
-        or
-        
-        ##### Git Clone
-        
-        * `git clone --recursive https://github.com/broadinstitute/getzlab-SignatureAnalyzer.git`
-        * `cd getzlab-SignatureAnalyzer`
-        * `pip3 install -e .`
-        
-        Note `--recurisve` flag is required to clone submodules.
-        
-        ##### Docker
-        
-        Link: `http://gcr.io/broad-cga-sanand-gtex/signatureanalyzer`
-        
-        * `docker pull gcr.io/broad-cga-sanand-gtex/signatureanalyzer:latest`
-        * `docker run -it --rm gcr.io/broad-cga-sanand-gtex/signatureanalyzer`
-        
-        ---
-        
-        ## Source Publications
-        
-        **PCAWG Mutational Signatures**
-        * Alexandrov, L. B., Kim, J., Haradhvala, N. J., Huang, M. N., Ng, A. W. T., Wu, Y., ... & Islam, S. A. (2020). The repertoire of mutational signatures in human cancer. Nature, 578(7793), 94-101.
-         * see: https://www.nature.com/articles/s41586-020-1943-3
-         * see `./PCAWG/`
-        
-        **SignatureAnalyzer-GPU source publication**
-        * Taylor-Weiner, A., Aguet, F., Haradhvala, N.J. et al. Scaling computational genomics to millions of individuals with GPUs. Genome Biol 20, 228 (2019) doi:10.1186/s13059-019-1836-7
-        (https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7)
-          * see: https://github.com/broadinstitute/SignatureAnalyzer-GPU
-        
-        **SignatureAnalyzer-CPU source publications**
-        * Kim, J. et al. Somatic ERCC2 mutations are associated with a distinct genomic signature in urothelial tumors. Nat. Genet. 48, 600–606 (2016). (https://www.nature.com/articles/ng.3557)
-        
-        * Kasar, S. et al. Whole-genome sequencing reveals activation-induced cytidine deaminase signatures during indolent chronic lymphocytic leukaemia evolution. Nat. Commun. 6, 8866 (2015). (https://www.nature.com/articles/ncomms9866)
-        
-        **Mathematical details**
-        * Tan, V. Y. F., Edric, C.  & Evotte, F. Automatic Relevance Determination in Nonnegative Matrix Factorization with the β-Divergence. (2012). (https://arxiv.org/pdf/1111.6085.pdf)
-        
-        
-        ---
-        ## Command Line Interface
-        
-        ```
-        usage: signatureanalyzer [-h] [-t {maf,spectra,matrix}] [-n NRUNS] [-o OUTDIR]
-                                 [--cosmic {cosmic2,cosmic3,cosmic3_exome,cosmic3_DBS,cosmic3_ID,cosmic3_TSB}]
-                                 [--hg_build HG_BUILD] [--cuda_int CUDA_INT]
-                                 [--verbose] [--K0 K0] [--max_iter MAX_ITER]
-                                 [--del_ DEL_] [--tolerance TOLERANCE] [--phi PHI]
-                                 [--a A] [--b B] [--objective {poisson,gaussian}]
-                                 [--prior_on_W {L1,L2}] [--prior_on_H {L1,L2}]
-                                 [--report_freq REPORT_FREQ]
-                                 [--active_thresh ACTIVE_THRESH] [--cut_norm CUT_NORM]
-                                 [--cut_diff CUT_DIFF]
-                                 input
-        ```
-        
-        #### Example:
-        
-        ```
-        signatureanalyzer input.maf -n 10 --cosmic cosmic2 --objective poisson
-        ```
-        
-        
-        ## Python API
-        
-        ```python
-        import signatureanalyzer as sa
-        
-        # ---------------------
-        # RUN SIGNATURE ANALYZER
-        # ---------------------
-        
-        # Run array of decompositions with mutational signature processing
-        sa.run_maf(input.maf, outdir='./ardnmf_output/', cosmic='cosmic2', hg_build='./ref/hg19.2bit', nruns=10)
-        
-        # Run ARD-NMF algorithm standalone
-        sa.ardnmf(...)
-        
-        # ---------------------
-        # LOADING RESULTS
-        # ---------------------
-        import pandas as pd
-        
-        H = pd.read_hdf('nmf_output.h5', 'H')
-        W = pd.read_hdf('nmf_output.h5', 'W')
-        Hraw = pd.read_hdf('nmf_output.h5', 'Hraw')
-        Wraw = pd.read_hdf('nmf_output.h5', 'Wraw')
-        feature_signatures = pd.read_hdf('nmf_output.h5', 'signatures')
-        markers = pd.read_hdf('nmf_output.h5', 'markers')
-        cosine = pd.read_hdf('nmf_output.h5', 'cosine')
-        log = pd.read_hdf('nmf_output.h5', 'log')
-        
-        # Output for each run may be found at...
-        Hrun1 = pd.read_hdf('nmf_output.h5', 'run1/H')
-        Wrun1 = pd.read_hdf('nmf_output.h5', 'run1/W')
-        # etc...
-        
-        # Aggregate output information for each run
-        aggr = pd.read_hdf('nmf_output.h5', 'aggr')
-        
-        # ---------------------
-        # PLOTTING
-        # ---------------------
-        sa.pl.marker_heatmap(...)
-        sa.pl.signature_barplot(...)
-        sa.pl.stacked_bar(...)
-        sa.pl.k_dist(...)
-        sa.pl.consensus_matrix(...)
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SignatureAnalyzer
+
+Automatic Relevance Determination (ARD) - NMF of mutational signature &amp; expression data. Designed for scalability using Pytorch to run using GPUs if available.
+
+_Requires Python 3.6.0 or higher._
+
+Please visit our [wiki](https://github.com/broadinstitute/getzlab-SignatureAnalyzer/wiki) for full documentation.
+## Installation
+
+##### PIP
+
+`pip3 install signatureanalyzer`
+
+or
+
+##### Git Clone
+
+* `git clone --recursive https://github.com/broadinstitute/getzlab-SignatureAnalyzer.git`
+* `cd getzlab-SignatureAnalyzer`
+* `pip3 install -e .`
+
+Note `--recurisve` flag is required to clone submodules.
+
+##### Docker
+
+Link: `http://gcr.io/broad-cga-sanand-gtex/signatureanalyzer`
+
+* `docker pull gcr.io/broad-cga-sanand-gtex/signatureanalyzer:latest`
+* `docker run -it --rm gcr.io/broad-cga-sanand-gtex/signatureanalyzer`
+
+---
+
+## Source Publications
+
+**PCAWG Mutational Signatures**
+* Alexandrov, L. B., Kim, J., Haradhvala, N. J., Huang, M. N., Ng, A. W. T., Wu, Y., ... & Islam, S. A. (2020). The repertoire of mutational signatures in human cancer. Nature, 578(7793), 94-101.
+ * see: https://www.nature.com/articles/s41586-020-1943-3
+ * see `./PCAWG/`
+
+**SignatureAnalyzer-GPU source publication**
+* Taylor-Weiner, A., Aguet, F., Haradhvala, N.J. et al. Scaling computational genomics to millions of individuals with GPUs. Genome Biol 20, 228 (2019) doi:10.1186/s13059-019-1836-7
+(https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7)
+  * see: https://github.com/broadinstitute/SignatureAnalyzer-GPU
+
+**SignatureAnalyzer-CPU source publications**
+* Kim, J. et al. Somatic ERCC2 mutations are associated with a distinct genomic signature in urothelial tumors. Nat. Genet. 48, 600–606 (2016). (https://www.nature.com/articles/ng.3557)
+
+* Kasar, S. et al. Whole-genome sequencing reveals activation-induced cytidine deaminase signatures during indolent chronic lymphocytic leukaemia evolution. Nat. Commun. 6, 8866 (2015). (https://www.nature.com/articles/ncomms9866)
+
+**Mathematical details**
+* Tan, V. Y. F., Edric, C.  & Evotte, F. Automatic Relevance Determination in Nonnegative Matrix Factorization with the β-Divergence. (2012). (https://arxiv.org/pdf/1111.6085.pdf)
+
+
+---
+## Command Line Interface
+
+```
+usage: signatureanalyzer [-h] [-t {maf,spectra,matrix}] [-n NRUNS] [-o OUTDIR]
+                         [--reference {cosmic2,cosmic3,cosmic3_exome,cosmic3_DBS,cosmic3_ID,cosmic3_TSB, 
+			               pcawg_COMPOSITE, pcawg_COMPOSITE96, pcawg_SBS_ID, pcawg_SBS96_ID, pcawg_SBS,
+			 	       polymerase_msi, polymerase_msi96}]
+                         [--hg_build HG_BUILD] [--cuda_int CUDA_INT]
+                         [--verbose] [--K0 K0] [--max_iter MAX_ITER]
+                         [--del_ DEL_] [--tolerance TOLERANCE] [--phi PHI]
+                         [--a A] [--b B] [--objective {poisson,gaussian}]
+                         [--prior_on_W {L1,L2}] [--prior_on_H {L1,L2}]
+                         [--report_freq REPORT_FREQ]
+                         [--active_thresh ACTIVE_THRESH] [--cut_norm CUT_NORM]
+                         [--cut_diff CUT_DIFF]
+                         input
+```
+
+#### Example:
+
+```
+signatureanalyzer input.maf -n 10 --reference cosmic2 --objective poisson
+```
+
+
+## Python API
+
+```python
+import signatureanalyzer as sa
+
+# ---------------------
+# RUN SIGNATURE ANALYZER
+# ---------------------
+
+# Run array of decompositions with mutational signature processing
+sa.run_maf(PATH_TO_MAF, outdir='./ardnmf_output/', reference='cosmic2', hg_build='./ref/hg19.2bit', nruns=10)
+
+# Run ARD-NMF algorithm standalone
+sa.ardnmf(...)
+
+# ---------------------
+# LOADING RESULTS
+# ---------------------
+import pandas as pd
+
+H = pd.read_hdf('nmf_output.h5', 'H')
+W = pd.read_hdf('nmf_output.h5', 'W')
+Hraw = pd.read_hdf('nmf_output.h5', 'Hraw')
+Wraw = pd.read_hdf('nmf_output.h5', 'Wraw')
+feature_signatures = pd.read_hdf('nmf_output.h5', 'signatures')
+markers = pd.read_hdf('nmf_output.h5', 'markers')
+cosine = pd.read_hdf('nmf_output.h5', 'cosine')
+log = pd.read_hdf('nmf_output.h5', 'log')
+
+# Output for each run may be found at...
+Hrun1 = pd.read_hdf('nmf_output.h5', 'run1/H')
+Wrun1 = pd.read_hdf('nmf_output.h5', 'run1/W')
+# etc...
+
+# Aggregate output information for each run
+aggr = pd.read_hdf('nmf_output.h5', 'aggr')
+
+# ---------------------
+# PLOTTING
+# ---------------------
+sa.pl.marker_heatmap(...)
+sa.pl.signature_barplot(...)
+sa.pl.stacked_bar(...)
+sa.pl.k_dist(...)
+sa.pl.consensus_matrix(...)
+
+```
```

### Comparing `signatureanalyzer-0.0.7/README.md` & `signatureanalyzer-0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SignatureAnalyzer
 
 Automatic Relevance Determination (ARD) - NMF of mutational signature &amp; expression data. Designed for scalability using Pytorch to run using GPUs if available.
-* See `docs` for a more in-depth description of how to use method.
 
 _Requires Python 3.6.0 or higher._
 
+Please visit our [wiki](https://github.com/broadinstitute/getzlab-SignatureAnalyzer/wiki) for full documentation.
 ## Installation
 
 ##### PIP
 
 `pip3 install signatureanalyzer`
 
 or
@@ -52,44 +52,46 @@
 
 
 ---
 ## Command Line Interface
 
 ```
 usage: signatureanalyzer [-h] [-t {maf,spectra,matrix}] [-n NRUNS] [-o OUTDIR]
-                         [--cosmic {cosmic2,cosmic3,cosmic3_exome,cosmic3_DBS,cosmic3_ID,cosmic3_TSB}]
+                         [--reference {cosmic2,cosmic3,cosmic3_exome,cosmic3_DBS,cosmic3_ID,cosmic3_TSB, 
+			               pcawg_COMPOSITE, pcawg_COMPOSITE96, pcawg_SBS_ID, pcawg_SBS96_ID, pcawg_SBS,
+			 	       polymerase_msi, polymerase_msi96}]
                          [--hg_build HG_BUILD] [--cuda_int CUDA_INT]
                          [--verbose] [--K0 K0] [--max_iter MAX_ITER]
                          [--del_ DEL_] [--tolerance TOLERANCE] [--phi PHI]
                          [--a A] [--b B] [--objective {poisson,gaussian}]
                          [--prior_on_W {L1,L2}] [--prior_on_H {L1,L2}]
                          [--report_freq REPORT_FREQ]
                          [--active_thresh ACTIVE_THRESH] [--cut_norm CUT_NORM]
                          [--cut_diff CUT_DIFF]
                          input
 ```
 
 #### Example:
 
 ```
-signatureanalyzer input.maf -n 10 --cosmic cosmic2 --objective poisson
+signatureanalyzer input.maf -n 10 --reference cosmic2 --objective poisson
 ```
 
 
 ## Python API
 
 ```python
 import signatureanalyzer as sa
 
 # ---------------------
 # RUN SIGNATURE ANALYZER
 # ---------------------
 
 # Run array of decompositions with mutational signature processing
-sa.run_maf(input.maf, outdir='./ardnmf_output/', cosmic='cosmic2', hg_build='./ref/hg19.2bit', nruns=10)
+sa.run_maf(PATH_TO_MAF, outdir='./ardnmf_output/', reference='cosmic2', hg_build='./ref/hg19.2bit', nruns=10)
 
 # Run ARD-NMF algorithm standalone
 sa.ardnmf(...)
 
 # ---------------------
 # LOADING RESULTS
 # ---------------------
```

### Comparing `signatureanalyzer-0.0.7/setup.py` & `signatureanalyzer-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,29 +22,28 @@
     packages = [
         'signatureanalyzer',
         'signatureanalyzer.plotting',
         'signatureanalyzer.pathways',
         'signatureanalyzer.signatureanalyzer_gpu'
     ],
     install_requires = [
-        "twobitreader>=3.1.7",
-        "torch>=1.2.0",
-        "seaborn>=0.9.0",
+        "gprofiler",
+        "h5py>=2.9.0",
+        "matplotlib",
+        "numpy<1.24.0",
         "pandas>=0.25.0",
         "pyarrow>=0.14.1",
-        "scikit-learn>=0.21.3",
         "scikit-image>=0.15.0",
-        "tqdm>=4.33.0",
-        "h5py>=2.9.0",
+        "scikit-learn>=0.21.3",
+        "scipy",
+        "seaborn>=0.9.0",
         "tables>=3.6.1",
-        "missingpy",
-        "gprofiler",
-        "numpy",
-        "matplotlib",
-        "scipy"
+        "torch>=1.2.0",
+        "tqdm>=4.33.0",
+        "twobitreader>=3.1.7",
     ],
     package_data = {
     "":[
         "ref/cosmic_v2/sa*",
         "ref/cosmic_v3/sa*"
     ]
     },
```

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/__main__.py` & `signatureanalyzer-0.0.8/signatureanalyzer/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,25 +34,32 @@
     )
     parser.add_argument(
         '-o','--outdir',
         help="Directory to save outputs (default: '.')",
         default="."
     )
     parser.add_argument(
-        '--cosmic',
+        '--reference',
         help="Cosmic signatures to map to and provide results for. Support for Cosmic 2 & 3 (default: 'cosmic2')\n"
              "  * Reference: https://cancer.sanger.ac.uk/cosmic/signatures",
         default='cosmic2',
         choices=[
             'cosmic2',
             'cosmic3',
             'cosmic3_exome',
             'cosmic3_DBS',
             'cosmic3_ID',
             'cosmic3_TSB',
+            'pcawg_SBS',
+            'pcawg_COMPOSITE',
+            'pcawg_COMPOSITE96',
+            'pcawg_SBS_ID',
+            'pcawg_SBS96_ID',
+            'polymerase_msi',
+            'polymerase_msi96'
             ]
     )
     parser.add_argument(
         '--hg_build',
         help="Path to 2bit, human genome build for mapping mutational contexts. Required if mutational context is not provided (default: None)",
         default=None
     )
@@ -146,14 +153,19 @@
     )
     parser.add_argument(
         '--active_thresh',
         help="Active threshold for consdiering a threshold relevant (default: 0.01)",
         default=0.01,
         type=float
     )
+    parser.add_argument(
+        '--random_seed',
+        help="Random seed for decomposition",
+        default=None,
+    )
 
     # -----------------------------------------
     # NMF Post-processing Arguments
     # -----------------------------------------
     parser.add_argument(
         '--cut_norm',
         help="Min normalized value for mean signature. Used in marker selection during post-processing (matrix). (default: 0.5)",
@@ -167,14 +179,18 @@
         type=float
     )
 
     args = parser.parse_args()
     if args.cuda_int == 'None':
         args.cuda_int = None
 
+    if args.random_seed is not None:
+        import numpy as np
+        np.random.seed(int(args.random_seed))
+
     print("---------------------------------------------------------")
     print("---------- S I G N A T U R E  A N A L Y Z E R  ----------")
     print("---------------------------------------------------------")
 
     if args.type == 'maf':
         run_maf(
             args.input,
```

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/bnmf.py` & `signatureanalyzer-0.0.8/signatureanalyzer/bnmf.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     prior_on_H: str = 'L1',
     report_freq: int = 100,
     active_thresh: float = 1e-2,
     cut_norm: float = 0.5,
     cut_diff: float = 1.0,
     cuda_int: Union[int, None] = 0,
     verbose: bool = True,
-    tag: str = ""
+    tag: str = "",
     ) -> dict:
     """
     Wrapper for ARD-NMF. Wraps GPU implementaiton from:
     https://github.com/broadinstitute/SignatureAnalyzer-GPU
     ------------------------------------------------------------------------
     Args:
         * X: input matrix (features x samples)
```

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/consensus.py` & `signatureanalyzer-0.0.8/signatureanalyzer/consensus.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/pathways/_gsea.py` & `signatureanalyzer-0.0.8/signatureanalyzer/pathways/_gsea.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/plotting/_cosine.py` & `signatureanalyzer-0.0.8/signatureanalyzer/plotting/_cosine.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/plotting/_nmf.py` & `signatureanalyzer-0.0.8/signatureanalyzer/plotting/_nmf.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,24 +35,28 @@
 
     ax.set_title("Aggregate of ARD-NMF (n={})".format(len(X)), fontsize=20)
     ax.set_ylabel("Number of Iterations", fontsize=18)
     ax.set_xticklabels(ax.get_xticklabels(), fontsize=18)
 
     return fig
 
-
 def consensus_matrix(
     cmatrix: pd.DataFrame,
     metric: str = 'euclidean',
     method: str = 'ward',
     n_clusters: int = 10,
     color_thresh_scale: float = 0.3,
     figsize: tuple = (8,8),
     p: int = 30,
-    metas: Union[list, None] = None
+    metas: Union[list, None] = None,
+    vmax: Union[float, None] = None,
+    vmin: Union[float, None] = None,
+    cbar_label: str = 'ARD-NMF \nMembership',
+    cmap: Union[str, None] = None,
+    plot_cluster_lines: bool = False
     ):
     """
     Plot consensus matrix.
     -----------------------
     Args:
         * cmatrix: consensus matrix. This may be generated by calling:
             df, assign_p = consensus_cluster_ardnmf(filepath)
@@ -76,39 +80,66 @@
 
     # Compute initial linkage to grab ordering
     d_linkage = shc.linkage(cmatrix, metric=metric, method=method)
     dres = shc.dendrogram(d_linkage, p=p, no_plot=True)
     dgram_idx = list(map(int, dres['ivl']))
 
     # Create heatmap
+    if vmax is None:
+        cbar_top_lim = np.max(cmatrix.values)
+    else:
+        cbar_top_lim = vmax
+
+    if vmin is None:
+        cbar_bottom_lim = 0
+    else:
+        cbar_bottom_lim = vmin
+
+    # Create heatmap
     sns.heatmap(
         cmatrix.iloc[dgram_idx,dgram_idx].values,
         ax=ax,
         square=True,
         cbar_ax=cbar_ax,
-        cbar_kws = {'ticks':[0, np.max(cmatrix.values)]},
-        rasterized=True
+        cbar_kws = {'ticks':[cbar_bottom_lim, cbar_top_lim]},
+        rasterized=True,
+        vmax=vmax,
+        vmin=vmin,
+        cmap=cmap
     )
 
-    cbar_ax.set_ylabel('ARD-NMF \nMembership', fontsize=10,rotation=90)
+    cbar_ax.set_ylabel(cbar_label, fontsize=10,rotation=90)
     ax.set_xticks([])
     ax.set_yticks([])
 
-    # -------------
-    # Dendrogram
-    # -------------
-    cmap = cm.rainbow(np.linspace(0, 1, 10))
-    hierarchy.set_link_color_palette([mpl.colors.rgb2hex(rgb[:3]) for rgb in cmap])
-
     x0 = ax.get_position().x0
     x1 = ax.get_position().x1
     y0 = ax.get_position().y0
     y1 = ax.get_position().y1
 
     buf = y1*0.015
+
+    # -------------
+    # Clustering
+    # -------------
+    cluster = AgglomerativeClustering(
+        n_clusters=n_clusters,
+        metric=metric,
+        linkage=method
+    )
+
+    clusters = cluster.fit_predict(cmatrix.iloc[dgram_idx,dgram_idx])
+    cluster_color_list, _ = series_to_colors(pd.Series(clusters))
+
+    # -------------
+    # Dendrogram
+    # -------------
+    cmap = cm.rainbow(np.linspace(0, 1, 10))
+    hierarchy.set_link_color_palette([mpl.colors.rgb2hex(rgb[:3]) for rgb in cmap])
+
     dax = fig.add_axes([x0, y1+buf, x1-x0, 0.15])
 
     dres = shc.dendrogram(
         d_linkage,
         p=p,
         ax=dax,
         above_threshold_color="grey",
@@ -118,24 +149,29 @@
     dax.set_xticks([])
     dax.set_yticks([])
     [dax.spines[x].set_visible(False) for x in ['top','right','bottom','left']]
 
     # -------------
     # Metadata Axes
     # -------------
-
-    # Agglomerative Clustering
-    cluster = AgglomerativeClustering(
-        n_clusters=n_clusters,
-        affinity=metric,
-        linkage=method
-    )
-
-    clusters = cluster.fit_predict(cmatrix.iloc[dgram_idx,dgram_idx])
-    cluster_color_list, _ = series_to_colors(pd.Series(clusters))
+    if plot_cluster_lines:
+        hz_lines = np.sort(np.unique(pd.Series(clusters), return_index=True)[1])
+        v,c = np.unique(clusters, return_counts=True)
+
+        _c = hz_lines
+        _c = np.roll(hz_lines, 1)
+        _c[0] = 0
+        _c[1] = 0
+
+        _ci = hz_lines[1:]
+        _ci = np.append(_ci, clusters.shape[0])
+
+        for idx, hz in enumerate(hz_lines):
+            ax.hlines(hz, _c[idx], _ci[idx], rasterized=True)
+            ax.vlines(hz, _c[idx], _ci[idx], rasterized=True)
 
     # Add axes
     # Plots agglomerative clustering results
     if metas is None:
         lax = fig.add_axes([x0-3*buf, y0, 2*buf, y1-y0])
         mat, cmap = color_list_to_matrix_and_cmap(cluster_color_list)
         sns.heatmap(mat.T, cmap=cmap, ax=lax, xticklabels=False, yticklabels=False, cbar=False, rasterized=True)
@@ -154,15 +190,15 @@
                 ha='left',
                 fontsize=14
             )
 
         for _, spine in lax.spines.items():
             spine.set_visible(True)
 
-        lax.set_xlabel("Consensus", rotation=45)
+        lax.set_xlabel("Consensus", rotation=90)
 
     else:
         for idx,meta in enumerate(metas):
             new_ax = [x0-(idx+3)*buf-(idx*2)*buf, y0, 2*buf, y1-y0]
             lax = fig.add_axes(new_ax)
 
             if isinstance(meta, str) and meta=='aggr':
@@ -180,24 +216,23 @@
                         mat.shape[1]+0.01*mat.shape[1],
                         y_locs[idx],
                         "n={}".format(num_vals[idx]),
                         ha='left',
                         fontsize=14
                     )
 
-                lax.set_xlabel("Consensus", rotation=45)
-
+                lax.set_xlabel("Consensus", rotation=90)
 
             else:
                 meta = meta.loc[cmatrix.index[dgram_idx]]
 
                 cluster_color_list, _ = series_to_colors(meta)
                 mat,cmap = color_list_to_matrix_and_cmap(cluster_color_list)
                 sns.heatmap(mat.T, cmap=cmap, ax=lax, yticklabels=False, xticklabels=False, cbar=False)
-                lax.set_xlabel(meta.name, rotation=45)
+                lax.set_xlabel(meta.name, rotation=90)
 
             for _, spine in lax.spines.items():
                 spine.set_visible(True)
 
     rs = pd.DataFrame(clusters, index=cmatrix.index[dgram_idx]).rename(columns={0:'clusters'})
 
     for _, spine in ax.spines.items():
```

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/plotting/_rna.py` & `signatureanalyzer-0.0.8/signatureanalyzer/plotting/_rna.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/plotting/_utils.py` & `signatureanalyzer-0.0.8/signatureanalyzer/plotting/_utils.py`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv` & `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv` & `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv` & `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv` & `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv` & `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv` & `signatureanalyzer-0.0.8/signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv`

 * *Files identical despite different names*

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/signatureanalyzer.py` & `signatureanalyzer-0.0.8/signatureanalyzer/signatureanalyzer.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,43 +4,45 @@
 import pkg_resources
 import pandas as pd
 from typing import Union
 import numpy as np
 import matplotlib.pyplot as plt
 
 from .utils import postprocess_msigs, get_nlogs_from_output, file_loader
-from .utils import load_cosmic_signatures
+from .utils import load_reference_signatures
 from .utils import split_negatives
 from .utils import assign_signature_weights_to_maf
+from .utils import plot_mutational_signatures
+from .utils import sbs1536_annotation_converter
+
+from .context import context1536_word, context96
 
 from .consensus import consensus_cluster
 
 from .plotting import k_dist, consensus_matrix
-from .plotting import signature_barplot, stacked_bar, signature_barplot_DBS, signature_barplot_ID
 from .plotting import marker_heatmap
-from .plotting import cosine_similarity_plot
 
 from .spectra import get_spectra_from_maf
 from .bnmf import ardnmf
 
 def run_maf(
     maf: Union[str, pd.DataFrame],
     outdir: str = '.',
-    cosmic: str = 'cosmic2',
+    reference: str = 'cosmic2',
     hg_build: Union[str, None] = None,
     nruns: int = 10,
     verbose: bool = False,
     plot_results: bool = True,
     **nmf_kwargs
     ):
     """
     Args:
         * maf: input .maf file format
         * outdir: output directory to save files
-        * cosmic: cosmic signature set to use
+        * reference: reference signature set to use
         * hg_build: human genome build for generating reference context
         * nruns: number of iterations for ARD-NMF
         * verbose: bool
 
     NMF_kwargs:
         * K0: starting number of latent components
         * objective: objective function for optimizaiton
@@ -58,131 +60,119 @@
         * cut_norm: min normalized value for mean signature
             (used in post-processing)
         * cut_diff: difference between mean signature and rest of signatures
             for marker selction
             (used in post-processing)
         * cuda_int: GPU to use. Defaults to 0. If "None" or if no GPU available,
             will perform decomposition using CPU.
-    """
+3    """
     try:
-        [nmf_kwargs.pop(key) for key in ['input', 'type']]
+        [nmf_kwargs.pop(key) for key in ['input', 'type', 'random_seed']]
     except:
         pass
 
-    if outdir is not ".":
+    if outdir != ".":
         print("   * Creating output dir at {}".format(outdir))
         os.makedirs(outdir, exist_ok=True)
 
     # Human Genome Build
     if hg_build is not None:
         print("   * Using {} build".format(hg_build.split("/")[-1].split('.2bit')[0]))
 
-    # Cosmic Signatures
-    cosmic_df, cosmic_index = load_cosmic_signatures(cosmic)
+    # Reference Signatures
+    reference_df, reference_index = load_reference_signatures(reference)
 
     # Generate Spectra from Maf
     print("   * Loading spectra from {}".format(maf))
     maf, spectra = get_spectra_from_maf(
-        pd.read_csv(maf, sep='\t'),
+        pd.read_csv(maf, sep='\t') if type(maf) == str else maf,
         hgfile=hg_build,
-        cosmic=cosmic
+        reference=reference
     )
 
     print("   * Saving ARD-NMF outputs to {}".format(os.path.join(outdir,'nmf_output.h5')))
-    store = pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'w')
+    with pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'w') as store:
 
-    print("   * Running ARD-NMF...")
-    for n_iter in range(nruns):
-        store['X'] = spectra
-
-        res = ardnmf(
-            spectra,
-            tag="\t{}/{}: ".format(n_iter,nruns-1),
-            verbose=verbose,
-            **nmf_kwargs
-        )
-
-        postprocess_msigs(res, cosmic_df, cosmic_index, cosmic)
-        lam = pd.DataFrame(data=res["lam"], columns=["lam"])
-        lam.index.name = "K0"
-
-        store["run{}/H".format(n_iter)] = res["H"]
-        store["run{}/W".format(n_iter)] = res["W"]
-        store["run{}/lam".format(n_iter)] = lam
-        store["run{}/Hraw".format(n_iter)] = res["Hraw"]
-        store["run{}/Wraw".format(n_iter)] = res["Wraw"]
-        store["run{}/markers".format(n_iter)] = res["markers"]
-        store["run{}/signatures".format(n_iter)] = res["signatures"]
-        store["run{}/log".format(n_iter)] = res["log"]
-        store["run{}/cosine".format(n_iter)] = res["cosine"]
-
-    store.close()
+        print("   * Running ARD-NMF...")
+        for n_iter in range(nruns):
+            store['X'] = spectra
+
+            res = ardnmf(
+                spectra,
+                tag="\t{}/{}: ".format(n_iter,nruns-1),
+                verbose=verbose,
+                **nmf_kwargs
+            )
+
+            postprocess_msigs(res, reference_df, reference_index, reference)
+            lam = pd.DataFrame(data=res["lam"], columns=["lam"])
+            lam.index.name = "K0"
+
+            store["run{}/H".format(n_iter)] = res["H"]
+            store["run{}/W".format(n_iter)] = res["W"]
+            store["run{}/lam".format(n_iter)] = lam
+            store["run{}/Hraw".format(n_iter)] = res["Hraw"]
+            store["run{}/Wraw".format(n_iter)] = res["Wraw"]
+            store["run{}/markers".format(n_iter)] = res["markers"]
+            store["run{}/signatures".format(n_iter)] = res["signatures"]
+            store["run{}/log".format(n_iter)] = res["log"]
+            store["run{}/cosine".format(n_iter)] = res["cosine"]
+            if "pcawg" in reference:
+                store["run{}/cosine_cosmic".format(n_iter)] = res["cosine_cosmic"]
+                store["run{}/Wraw96".format(n_iter)] = res["Wraw96"]
+                store["run{}/W96".format(n_iter)] = res["W96"]
 
     # Select Best Result
     aggr = get_nlogs_from_output(os.path.join(outdir,'nmf_output.h5'))
     max_k = aggr.groupby("K").size().idxmax()
     max_k_iter = aggr[aggr['K']==max_k].shape[0]
     best_run = int(aggr[aggr['K']==max_k].obj.idxmin())
     print("   * Run {} had lowest objective with mode (n={:g}) K = {:g}.".format(best_run, max_k_iter, aggr.loc[best_run]['K']))
 
-    store = pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'a')
-    store["H"] = store["run{}/H".format(best_run)]
-    store["W"] = store["run{}/W".format(best_run)]
-    store["lam"] = store["run{}/lam".format(best_run)]
-    store["Hraw"] = store["run{}/Hraw".format(best_run)]
-    store["Wraw"] = store["run{}/Wraw".format(best_run)]
-    store["markers"] = store["run{}/markers".format(best_run)]
-    store["signatures"] = store["run{}/signatures".format(best_run)]
-    store["log"] = store["run{}/log".format(best_run)]
-    store["cosine"] = store["run{}/cosine".format(best_run)]
-    store["aggr"] = aggr
-    store.close()
+    with pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'a') as store:
+        store["H"] = store["run{}/H".format(best_run)]
+        store["W"] = store["run{}/W".format(best_run)]
+        store["lam"] = store["run{}/lam".format(best_run)]
+        store["Hraw"] = store["run{}/Hraw".format(best_run)]
+        store["Wraw"] = store["run{}/Wraw".format(best_run)]
+        store["markers"] = store["run{}/markers".format(best_run)]
+        store["signatures"] = store["run{}/signatures".format(best_run)]
+        store["log"] = store["run{}/log".format(best_run)]
+        store["cosine"] = store["run{}/cosine".format(best_run)]
+        store["aggr"] = aggr
+        if "pcawg" in reference:
+            store["cosine_cosmic"] = store["run{}/cosine_cosmic".format(best_run)]
+            store["Wraw96"] = store["run{}/Wraw96".format(best_run)]
+            store["W96"] = store["run{}/W96".format(best_run)]
 
     H = pd.read_hdf(os.path.join(outdir, 'nmf_output.h5'), "H")
     W = pd.read_hdf(os.path.join(outdir, 'nmf_output.h5'), "W")
 
     weighted_maf = assign_signature_weights_to_maf(maf, W, H)
     weighted_maf.to_csv(os.path.join(outdir, 'signature_weighted_maf.tsv'), sep='\t', index=False)
 
     # Plots
     if plot_results:
-        print("   * Saving report plots to {}".format(outdir))
-
-        cosine = pd.read_hdf(os.path.join(outdir,'nmf_output.h5'), "cosine")
-
-        if cosmic == 'cosmic3_DBS':
-            _ = signature_barplot_DBS(W, contributions=np.sum(H))
-        elif cosmic == 'cosmic3_ID':
-            _ = signature_barplot_ID(W, contributions=np.sum(H))
-        else:
-            _ = signature_barplot(W, contributions=np.sum(H))
-
-        plt.savefig(os.path.join(outdir, "signature_contributions.pdf"), dpi=100, bbox_inches='tight')
-        _ = stacked_bar(H)
-        plt.savefig(os.path.join(outdir, "signature_stacked_barplot.pdf"), dpi=100, bbox_inches='tight')
-        _ = k_dist(np.array(aggr.K, dtype=int))
-        plt.savefig(os.path.join(outdir, "k_dist.pdf"), dpi=100, bbox_inches='tight')
-        _ = cosine_similarity_plot(cosine)
-        plt.savefig(os.path.join(outdir, "cosine_similarity_plot.pdf"), dpi=100, bbox_inches='tight')
+        plot_mutational_signatures(outdir, reference, aggr.K)
 
 def run_spectra(
     spectra: Union[str, pd.DataFrame],
     outdir: str = '.',
-    cosmic: str = 'cosmic2',
+    reference: str = 'cosmic2',
     nruns: int = 10,
     verbose: bool = False,
     plot_results: bool = True,
     **nmf_kwargs
     ):
     """
     Args:
         * spectra: filepath or pd.DataFrame of input spectra file (context x samples)
             NOTE: index should be context in the following format (1234): 3[1>2]4
         * outdir: output directory to save files
-        * cosmic: cosmic signature set to use
+        * reference: reference signature set to use
         * nruns: number of iterations for ARD-NMF
         * verbose: bool
 
     NMF_kwargs:
         * K0: starting number of latent components
         * objective: objective function for optimizaiton
         * max_iter: maximum number of iterations for algorithm
@@ -201,100 +191,96 @@
         * cut_diff: difference between mean signature and rest of signatures
             for marker selction
             (used in post-processing)
         * cuda_int: GPU to use. Defaults to 0. If "None" or if no GPU available,
             will perform decomposition using CPU.
     """
     try:
-        [nmf_kwargs.pop(key) for key in ['input', 'type', 'hg_build']]
+        [nmf_kwargs.pop(key) for key in ['input', 'type', 'hg_build', 'random_seed']]
     except:
         pass
 
     # Load spectra
     if isinstance(spectra, str):
         spectra = file_loader(spectra)
 
-    if outdir is not ".":
+    if outdir != ".":
         print("   * Creating output dir at {}".format(outdir))
         os.makedirs(outdir, exist_ok=True)
 
-    # Cosmic Signatures
-    cosmic_df, cosmic_index = load_cosmic_signatures(cosmic)
+    # Reference Signatures
+    reference_df, reference_index = load_reference_signatures(reference)
 
     print("   * Saving ARD-NMF outputs to {}".format(os.path.join(outdir,'nmf_output.h5')))
-    store = pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'w')
-
-    print("   * Running ARD-NMF...")
-    for n_iter in range(nruns):
-        store['X'] = spectra
-
-        res = ardnmf(
-            spectra,
-            tag="\t{}/{}: ".format(n_iter,nruns-1),
-            verbose=verbose,
-            **nmf_kwargs
-        )
-
-        postprocess_msigs(res, cosmic_df, cosmic_index, cosmic)
-        lam = pd.DataFrame(data=res["lam"], columns=["lam"])
-        lam.index.name = "K0"
-
-        store["run{}/H".format(n_iter)] = res["H"]
-        store["run{}/W".format(n_iter)] = res["W"]
-        store["run{}/lam".format(n_iter)] = lam
-        store["run{}/Hraw".format(n_iter)] = res["Hraw"]
-        store["run{}/Wraw".format(n_iter)] = res["Wraw"]
-        store["run{}/markers".format(n_iter)] = res["markers"]
-        store["run{}/signatures".format(n_iter)] = res["signatures"]
-        store["run{}/log".format(n_iter)] = res["log"]
-        store["run{}/cosine".format(n_iter)] = res["cosine"]
+    with pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'w') as store:
 
-    store.close()
+        # Transform SBS form for composite signatures ahead of analysis
+        if reference in ["pcawg_SBS","pcawg_COMPOSITE","pcawg_SBS_ID"]:
+            if spectra.index.isin(context1536_word).any():
+                spectra.index = spectra.index.map(lambda x: sbs1536_annotation_converter(x) if x in context1536_word else x)
+        elif reference in ["pcawg_COMPOSITE96","pcawg_SBS96_ID"]:
+            if not spectra.index.isin(context96).any():
+                spectra.index = spectra.index.map(lambda x: x[2]+x[4]+x[0]+x[6] if ('>' in x and len(x)==7) else x)
+
+        print("   * Running ARD-NMF...")
+        for n_iter in range(nruns):
+            store['X'] = spectra
+
+            res = ardnmf(
+                spectra,
+                tag="\t{}/{}: ".format(n_iter,nruns-1),
+                verbose=verbose,
+                **nmf_kwargs
+            )
+
+            # Process W, H, and Cosine similarity matrices
+            postprocess_msigs(res, reference_df, reference_index, reference)
+            lam = pd.DataFrame(data=res["lam"], columns=["lam"])
+            lam.index.name = "K0"
+
+            store["run{}/H".format(n_iter)] = res["H"]
+            store["run{}/W".format(n_iter)] = res["W"]
+            store["run{}/lam".format(n_iter)] = lam
+            store["run{}/Hraw".format(n_iter)] = res["Hraw"]
+            store["run{}/Wraw".format(n_iter)] = res["Wraw"]
+            store["run{}/markers".format(n_iter)] = res["markers"]
+            store["run{}/signatures".format(n_iter)] = res["signatures"]
+            store["run{}/log".format(n_iter)] = res["log"]
+            store["run{}/cosine".format(n_iter)] = res["cosine"]
+            if 'pcawg' in reference:
+                store["run{}/cosine_cosmic".format(n_iter)] = res["cosine_cosmic"]
+                store["run{}/Wraw96".format(n_iter)] = res["Wraw96"]
+                store["run{}/W96".format(n_iter)] = res["W96"]
 
     # Select Best Result
     aggr = get_nlogs_from_output(os.path.join(outdir,'nmf_output.h5'))
     max_k = aggr.groupby("K").size().idxmax()
     max_k_iter = aggr[aggr['K']==max_k].shape[0]
     best_run = int(aggr[aggr['K']==max_k].obj.idxmin())
     print("   * Run {} had lowest objective with mode (n={:g}) K = {:g}.".format(best_run, max_k_iter, aggr.loc[best_run]['K']))
 
-    store = pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'a')
-    store["H"] = store["run{}/H".format(best_run)]
-    store["W"] = store["run{}/W".format(best_run)]
-    store["lam"] = store["run{}/lam".format(best_run)]
-    store["Hraw"] = store["run{}/Hraw".format(best_run)]
-    store["Wraw"] = store["run{}/Wraw".format(best_run)]
-    store["markers"] = store["run{}/markers".format(best_run)]
-    store["signatures"] = store["run{}/signatures".format(best_run)]
-    store["log"] = store["run{}/log".format(best_run)]
-    store["cosine"] = store["run{}/cosine".format(best_run)]
-    store["aggr"] = aggr
-    store.close()
+    with pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'a') as store:
+        store["H"] = store["run{}/H".format(best_run)]
+        store["W"] = store["run{}/W".format(best_run)]
+        store["lam"] = store["run{}/lam".format(best_run)]
+        store["Hraw"] = store["run{}/Hraw".format(best_run)]
+        store["Wraw"] = store["run{}/Wraw".format(best_run)]
+        store["markers"] = store["run{}/markers".format(best_run)]
+        store["signatures"] = store["run{}/signatures".format(best_run)]
+        store["log"] = store["run{}/log".format(best_run)]
+        store["cosine"] = store["run{}/cosine".format(best_run)]
+        store["aggr"] = aggr
+        if 'pcawg' in reference:
+            store["cosine_cosmic"] = store["run{}/cosine_cosmic".format(best_run)]
+            store["Wraw96"] = store["run{}/Wraw96".format(best_run)]
+            store["W96"] = store["run{}/W96".format(best_run)]
 
     # Plots
     if plot_results:
-        print("   * Saving report plots to {}".format(outdir))
-        H = pd.read_hdf(os.path.join(outdir,'nmf_output.h5'), "H")
-        W = pd.read_hdf(os.path.join(outdir,'nmf_output.h5'), "W")
-        cosine = pd.read_hdf(os.path.join(outdir,'nmf_output.h5'), "cosine")
-
-        if cosmic == 'cosmic3_DBS':
-            _ = signature_barplot_DBS(W, contributions=np.sum(H))
-        elif cosmic == 'cosmic3_ID':
-            _ = signature_barplot_ID(W, contributions=np.sum(H))
-        else:
-            _ = signature_barplot(W, contributions=np.sum(H))
-
-        plt.savefig(os.path.join(outdir, "signature_contributions.pdf"), dpi=100, bbox_inches='tight')
-        _ = stacked_bar(H)
-        plt.savefig(os.path.join(outdir, "signature_stacked_barplot.pdf"), dpi=100, bbox_inches='tight')
-        _ = k_dist(np.array(aggr.K, dtype=int))
-        plt.savefig(os.path.join(outdir, "k_dist.pdf"), dpi=100, bbox_inches='tight')
-        _ = cosine_similarity_plot(cosine)
-        plt.savefig(os.path.join(outdir, "cosine_similarity_plot.pdf"), dpi=100, bbox_inches='tight')
+        plot_mutational_signatures(outdir, reference, aggr.K)
 
 def run_matrix(
     matrix: Union[str, pd.DataFrame],
     outdir: str = '.',
     nruns: int = 20,
     verbose: bool = False,
     plot_results: bool = True,
@@ -313,15 +299,14 @@
             ]
             *************************************************
 
             NOTE: reccomended to select a set of highly variable genes following
                 this (~ 2000 - 7500 genes)
 
         * outdir: output directory to save files
-        * cosmic: cosmic signature set to use
         * nruns: number of iterations for ARD-NMF
         * verbose: bool
 
     NMF_kwargs:
         * K0: starting number of latent components
         * objective: objective function for optimizaiton
         * max_iter: maximum number of iterations for algorithm
@@ -340,77 +325,74 @@
         * cut_diff: difference between mean signature and rest of signatures
             for marker selction
             (used in post-processing)
         * cuda_int: GPU to use. Defaults to 0. If "None" or if no GPU available,
             will perform decomposition using CPU.
     """
     try:
-        [nmf_kwargs.pop(key) for key in ['input', 'type', 'hg_build', 'cosmic']]
+        [nmf_kwargs.pop(key) for key in ['input', 'type', 'hg_build', 'reference', 'random_seed']]
     except:
         pass
 
     # Load matrix
     if isinstance(matrix, str):
         matrix = file_loader(matrix)
 
     # Check for negativity
     if min(matrix.min()) < 0:
         print("   * Negative values detecting, splitting vars m={} --> m={}".format(matrix.shape[0], matrix.shape[0]*2))
         matrix = split_negatives(matrix, axis=0)
 
-    if outdir is not ".":
+    if outdir != ".":
         print("   * Creating output dir at {}".format(outdir))
         os.makedirs(outdir, exist_ok=True)
 
     print("   * Saving ARD-NMF outputs to {}".format(os.path.join(outdir,'nmf_output.h5')))
-    store = pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'w')
-
-    print("   * Running ARD-NMF...")
-    for n_iter in range(nruns):
-        store['X'] = matrix
-
-        res = ardnmf(
-            matrix,
-            tag="\t{}/{}: ".format(n_iter,nruns-1),
-            verbose=verbose,
-            **nmf_kwargs
-        )
-
-        lam = pd.DataFrame(data=res["lam"], columns=["lam"])
-        lam.index.name = "K0"
-
-        store["run{}/H".format(n_iter)] = res["H"]
-        store["run{}/W".format(n_iter)] = res["W"]
-        store["run{}/lam".format(n_iter)] = lam
-        store["run{}/Hraw".format(n_iter)] = res["Hraw"]
-        store["run{}/Wraw".format(n_iter)] = res["Wraw"]
-        store["run{}/markers".format(n_iter)] = res["markers"]
-        store["run{}/signatures".format(n_iter)] = res["signatures"]
-        store["run{}/log".format(n_iter)] = res["log"]
+    with pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'w') as store:
 
-    store.close()
+        print("   * Running ARD-NMF...")
+        for n_iter in range(nruns):
+            store['X'] = matrix
+
+            res = ardnmf(
+                matrix,
+                tag="\t{}/{}: ".format(n_iter,nruns-1),
+                verbose=verbose,
+                **nmf_kwargs
+            )
+
+            lam = pd.DataFrame(data=res["lam"], columns=["lam"])
+            lam.index.name = "K0"
+
+            store["run{}/H".format(n_iter)] = res["H"]
+            store["run{}/W".format(n_iter)] = res["W"]
+            store["run{}/lam".format(n_iter)] = lam
+            store["run{}/Hraw".format(n_iter)] = res["Hraw"]
+            store["run{}/Wraw".format(n_iter)] = res["Wraw"]
+            store["run{}/markers".format(n_iter)] = res["markers"]
+            store["run{}/signatures".format(n_iter)] = res["signatures"]
+            store["run{}/log".format(n_iter)] = res["log"]
 
     # Select Best Result
     aggr = get_nlogs_from_output(os.path.join(outdir,'nmf_output.h5'))
     max_k = aggr.groupby("K").size().idxmax()
     max_k_iter = aggr[aggr['K']==max_k].shape[0]
     best_run = int(aggr[aggr['K']==max_k].obj.idxmin())
     print("   * Run {} had lowest objective with mode (n={:g}) K = {:g}.".format(best_run, max_k_iter, aggr.loc[best_run]['K']))
 
-    store = pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'a')
-    store["H"] = store["run{}/H".format(best_run)]
-    store["W"] = store["run{}/W".format(best_run)]
-    store["lam"] = store["run{}/lam".format(best_run)]
-    store["Hraw"] = store["run{}/Hraw".format(best_run)]
-    store["Wraw"] = store["run{}/Wraw".format(best_run)]
-    store["markers"] = store["run{}/markers".format(best_run)]
-    store["signatures"] = store["run{}/signatures".format(best_run)]
-    store["log"] = store["run{}/log".format(best_run)]
-    store["aggr"] = aggr
-    store.close()
+    with pd.HDFStore(os.path.join(outdir,'nmf_output.h5'),'a') as store:
+        store["H"] = store["run{}/H".format(best_run)]
+        store["W"] = store["run{}/W".format(best_run)]
+        store["lam"] = store["run{}/lam".format(best_run)]
+        store["Hraw"] = store["run{}/Hraw".format(best_run)]
+        store["Wraw"] = store["run{}/Wraw".format(best_run)]
+        store["markers"] = store["run{}/markers".format(best_run)]
+        store["signatures"] = store["run{}/signatures".format(best_run)]
+        store["log"] = store["run{}/log".format(best_run)]
+        store["aggr"] = aggr
 
 
     # Consensus Clustering
     print("   * Computing consensus matrix")
     cmatrix, _ = consensus_cluster(os.path.join(outdir, 'nmf_output.h5'))
     f,d = consensus_matrix(cmatrix, n_clusters=max_k_iter)
```

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer/spectra.py` & `signatureanalyzer-0.0.8/signatureanalyzer/spectra.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,54 @@
 import itertools
 import pandas as pd
 from twobitreader import TwoBitFile
 from typing import Union
 from sys import stdout
+import numpy as np
 from .utils import compl, get_true_snps_from_maf, get_dnps_from_maf
-
-acontext = itertools.product('A', 'CGT', 'ACGT', 'ACGT')
-ccontext = itertools.product('C', 'AGT', 'ACGT', 'ACGT')
-
-context96 = dict(zip(map(''.join, itertools.chain(acontext, ccontext)), range(1, 97)))
-context78 = dict(zip(['AC>CA', 'AC>CG', 'AC>CT', 'AC>GA', 'AC>GG', 'AC>GT', 'AC>TA', 'AC>TG', 'AC>TT', 'AT>CA',
-                      'AT>CC', 'AT>CG', 'AT>GA', 'AT>GC', 'AT>TA', 'CC>AA', 'CC>AG', 'CC>AT', 'CC>GA', 'CC>GG',
-                      'CC>GT', 'CC>TA', 'CC>TG', 'CC>TT', 'CG>AT', 'CG>GC', 'CG>GT', 'CG>TA', 'CG>TC', 'CG>TT',
-                      'CT>AA', 'CT>AC', 'CT>AG', 'CT>GA', 'CT>GC', 'CT>GG', 'CT>TA', 'CT>TC', 'CT>TG', 'GC>AA',
-                      'GC>AG', 'GC>AT', 'GC>CA', 'GC>CG', 'GC>TA', 'TA>AT', 'TA>CG', 'TA>CT', 'TA>GC', 'TA>GG',
-                      'TA>GT', 'TC>AA', 'TC>AG', 'TC>AT', 'TC>CA', 'TC>CG', 'TC>CT', 'TC>GA', 'TC>GG', 'TC>GT',
-                      'TG>AA', 'TG>AC', 'TG>AT', 'TG>CA', 'TG>CC', 'TG>CT', 'TG>GA', 'TG>GC', 'TG>GT', 'TT>AA',
-                      'TT>AC', 'TT>AG', 'TT>CA', 'TT>CC', 'TT>CG', 'TT>GA', 'TT>GC', 'TT>GG'], range(1, 79)))
-
-context83 = dict(zip(['Cdel1', 'Cdel2', 'Cdel3', 'Cdel4', 'Cdel5', 'Cdel6+',
-                       'Tdel1', 'Tdel2', 'Tdel3', 'Tdel4', 'Tdel5', 'Tdel6+',
-                       'Cins0', 'Cins1', 'Cins2', 'Cins3', 'Cins4', 'Cins5+',
-                       'Tins0', 'Tins1', 'Tins2', 'Tins3', 'Tins4', 'Tins5+',
-                       '2del1', '2del2', '2del3', '2del4', '2del5', '2del6+',
-                       '3del1', '3del2', '3del3', '3del4', '3del5', '3del6+',
-                       '4del1', '4del2', '4del3', '4del4', '4del5', '4del6+',
-                       '5+del1', '5+del2', '5+del3', '5+del4', '5+del5', '5+del6+',
-                       '2ins0', '2ins1', '2ins2', '2ins3', '2ins4', '2ins5+',
-                       '3ins0', '3ins1', '3ins2', '3ins3', '3ins4', '3ins5+',
-                       '4ins0', '4ins1', '4ins2', '4ins3', '4ins4', '4ins5+',
-                       '5+ins0', '5+ins1', '5+ins2', '5+ins3', '5+ins4', '5+ins5+',
-                       '2delm1', '3delm1', '3delm2', '4delm1', '4delm2', '4delm3',
-                       '5+delm1', '5+delm2', '5+delm3', '5+delm4', '5+delm5+'], range(1, 84)))
+from .context import context96, context1536, context78, context83, context_composite, context_polymerase, context_polymerase_id
 
 def get_spectra_from_maf(
     maf: pd.DataFrame,
     hgfile: Union[str,None] = None,
-    cosmic: str = 'cosmic2',
-    real_snps: bool = False
+    reference: str = 'cosmic2',
+    real_snps: bool = False,
     ):
     """
     Attaches context categories to maf and gets counts of contexts for each sample
     ---------------------------
     Args:
         * maf: Pandas DataFrame of maf
         * hgfile: path to 2bit genome build file for computing reference context
-        * cosmic: cosmic signatures to decompose to
+        * ref: reference signatures to decompose to
 
     Returns:
         * Pandas DataFrame of maf with context category attached
         * Pandas DataFrame of counts with samples as columns and context as rows
     """
     maf = maf.copy()
 
     if 'Start_Position' in list(maf):
         maf = maf.rename(columns={'Start_Position':'Start_position'})
 
     maf['sample'] = maf['Tumor_Sample_Barcode']
 
-    if cosmic in ['cosmic2', 'cosmic3', 'cosmic3_exome']:
+    if reference in ['cosmic2', 'cosmic3', 'cosmic3_exome', 'pcawg_SBS']:
+        # Context type
+        if reference in ['cosmic2', 'cosmic3', 'cosmic3_exome']: context_num, context_form, context_use = 'context96.num', 'context96.word', context96
+        else: context_num, context_form, context_use = 'context1536.num', 'context1536.arrow', context1536
+        
         # Subset to SNPs
         if 'Variant_Type' in maf.columns:
             maf = maf.loc[maf['Variant_Type'] == 'SNP']
         else:
             maf = maf.loc[maf['Reference_Allele'].apply(lambda k: len(k) == 1 and k != '-') & \
             maf['Tumor_Seq_Allele2'].apply(lambda k: len(k) == 1 and k != '-')]
         if not real_snps:
+            # Filter out adjacent SNPs
             maf = get_true_snps_from_maf(maf)
 
         ref = maf['Reference_Allele'].str.upper()
         alt = maf['Tumor_Seq_Allele2'].str.upper()
 
         if 'ref_context' in list(maf):
             context = maf['ref_context'].str.upper()
@@ -77,121 +56,143 @@
             assert hgfile is not None, 'Please provide genome build file.'
 
             try:
                 hg = TwoBitFile(hgfile)
             except:
                 raise Exception("{} not a valid 2bit file.".format(hgfile))
 
+            chr_contig = all('chr{}'.format(i) in hg for i in list(range(1, 23)) + ['X', 'Y'])
+
             # Map contexts
             _contexts = list()
             maf_size = maf.shape[0]
             for idx,(pos,chromosome) in enumerate(zip(maf["Start_position"].astype(int), maf["Chromosome"].astype(str))):
                 stdout.write("\r      * Mapping contexts: {} / {}".format(idx, maf_size))
 
                 # Double check version
                 if chromosome == '23':
                     chromosome = 'X'
                 elif chromosome == '24':
                     chromosome = 'Y'
                 elif chromosome == 'MT':
                     chromosome = 'M'
-                if not chromosome.startswith('chr'):
+                if chr_contig and not chromosome.startswith('chr'):
                     chromosome = 'chr' + chromosome
+                if not chr_contig and chromosome.startswith('chr'):
+                    chromosome = chromosome[3:]
 
-                _contexts.append(hg[chromosome][pos-2:pos+1].lower())
+                # 96 context, get reference [pos-1, pos, pos+1]
+                if reference != 'pcawg_SBS':
+                    _contexts.append(hg[chromosome][pos-2:pos+1].lower())
+                # 1536 context, get refernece [pos-2, pos-1, pos, pos+1, pos+2]
+                else:
+                    _contexts.append(hg[chromosome][pos-3:pos+2].lower())
 
             maf['ref_context'] = _contexts
             stdout.write("\n")
             context = maf['ref_context'].str.upper()
 
         n_context = context.str.len()
         mid = n_context // 2
 
-        contig = pd.Series([r + a + c[m - 1] + c[m + 1] if r in 'AC' \
-                            else compl(r + a + c[m + 1] + c[m - 1]) \
-                            for r, a, c, m in zip(ref, alt, context, mid)], index=maf.index)
-
+        if reference != 'pcawg_SBS':
+            contig = pd.Series([r + a + c[m - 1] + c[m + 1] if r in 'AC' \
+                                else compl(r + a + c[m + 1] + c[m - 1]) \
+                                for r, a, c, m in zip(ref, alt, context, mid)], index=maf.index)
+        else:
+            contig = pd.Series([c[m-2:m] + "[" + r + ">" + a + "]" + c[m+1:m+3] if r in 'TC' \
+                                else compl(c[::-1][m-2:m] + "[" + r + ">" + a + "]" + c[::-1][m+1:m+3]) \
+                                for r, a, c, m in zip(ref, alt, context, mid)], index=maf.index)
+        # Common bug: MAF has mutations with malformed sequence contexts. Rather than throwing an error, just print warning
+        exclude_l = [c for c in contig if c not in context_use]
+        print(f"WARNING: Dropping {len(exclude_l)} / {maf.shape[0]} contexts that are not included in the reference. Ensure proper formating of MAF")
+        contig = contig[contig.isin(context_use)]
+        maf = maf.loc[contig.index]
         try:
-            maf['context96.num'] = contig.apply(context96.__getitem__)
+            maf[context_num] = contig.apply(context_use.__getitem__)
         except KeyError as e:
             raise KeyError('Unusual context: ' + str(e))
 
-        maf['context96.word'] = contig
-        spectra = maf.groupby(['context96.word', 'sample']).size().unstack().fillna(0).astype(int)
-        for c in context96:
+        
+        maf[context_form] = contig
+        spectra = maf.groupby([context_form, 'sample']).size().unstack().fillna(0).astype(int)
+        for c in context_use:
             if c not in spectra.index:
                 spectra.loc[c] = 0
-        spectra = spectra.loc[context96]
-
-    elif cosmic == 'cosmic3_DBS':
+        spectra = spectra.loc[context_use.keys()]   
+            
+    elif reference == 'cosmic3_DBS':
         # Subset to DNPs
         if 'Variant_Type' not in maf.columns:
             ref_alt = maf['Reference_Allele'] + '>' + maf['Tumor_Seq_Allele2']
 
             def get_variant_type(ra):
                 r, a = ra.split('>')
                 if len(r) == 1 and r != '-' and len(a) == 1 and a != '-':
                     return 'SNP'
                 if len(r) == 2 and len(a) == 2:
                     return 'DNP'
             maf['Variant_Type'] = ref_alt.apply(get_variant_type)
-        if 'DNP' in maf['Variant_Type']:
+        if maf['Variant_Type'].str.contains('DNP').any():
             maf = maf.loc[maf['Variant_Type'] == 'DNP']
         else:
             maf = get_dnps_from_maf(maf)
-
         ref = maf['Reference_Allele'].str.upper()
         alt = maf['Tumor_Seq_Allele2'].str.upper()
 
         contig = pd.Series([r + '>' + a if r + '>' + a in context78
                             else compl(r, reverse=True) + '>' + compl(a, reverse=True)
                             for r, a in zip(ref, alt)], index=maf.index)
 
         try:
-            maf['context78.num'] = contig.apply(context78.__getitem__)
+           maf['context78.num'] = contig.apply(context78.__getitem__)
         except KeyError as e:
             raise KeyError('Unusual context: ' + str(e))
 
         maf['context78.word'] = contig
         spectra = maf.groupby(['context78.word', 'sample']).size().unstack().fillna(0).astype(int)
         for c in context78:
             if c not in spectra.index:
                 spectra.loc[c] = 0
-        spectra = spectra.loc[context78]
+        spectra = spectra.loc[context78.keys()]     
 
-    elif cosmic == 'cosmic3_ID':
+    elif reference == 'cosmic3_ID':
 
         maf = maf.loc[(maf['Reference_Allele'] == '-') ^ (maf['Tumor_Seq_Allele2'] == '-')]
 
         ref = maf['Reference_Allele'].str.upper()
         alt = maf['Tumor_Seq_Allele2'].str.upper()
 
         assert hgfile is not None, 'Please provide genome build file.'
 
         try:
             hg = TwoBitFile(hgfile)
         except:
             raise Exception("{} not a valid 2bit file.".format(hgfile))
 
+        chr_contig = all('chr{}'.format(i) in hg for i in list(range(1, 23)) + ['X', 'Y'])
+
         # Map contexts
         contig = list()
         maf_size = maf.shape[0]
         for idx,(pos,chromosome,r,a) in enumerate(zip(maf["Start_position"].astype(int),
             maf["Chromosome"].astype(str), ref, alt)):
             stdout.write("\r      * Mapping contexts: {} / {}".format(idx, maf_size))
 
             # Double check version
             if chromosome == '23':
                 chromosome = 'X'
             elif chromosome == '24':
                 chromosome = 'Y'
             elif chromosome == 'MT':
                 chromosome = 'M'
-            if not chromosome.startswith('chr'):
+            if chr_contig and not chromosome.startswith('chr'):
                 chromosome = 'chr' + chromosome
+            if not chr_contig and chromosome.startswith('chr'):
+                chromosome = chromosome[3:]
 
             if a == '-':
                 del_len = len(r)
                 _context = hg[chromosome][pos - 1 + del_len:pos - 1 + del_len * 6].upper()
                 _context_list = [_context[n: n + del_len] for n in range(0, 5 * del_len, del_len)]
                 n_repeats = 1
                 for c in _context_list:
@@ -256,14 +257,79 @@
         except KeyError as e:
             raise KeyError('Unusual context: ' + str(e))
 
         spectra = maf.groupby(['context83.word', 'sample']).size().unstack().fillna(0).astype(int)
         for c in context83:
             if c not in spectra.index:
                 spectra.loc[c] = 0
-        spectra = spectra.loc[context83]
+        spectra = spectra.loc[context83.keys()]
 
         stdout.write("\n")
+    
+    elif reference in ["pcawg_COMPOSITE","pcawg_COMPOSITE96"]:
+        """
+        Concatenate 1536 or 96 SBS, DBS, and ID spectra
+        """
+        maf_dbs,dbs_df = get_spectra_from_maf(maf,hgfile, 'cosmic3_DBS')
+        maf_id,id_df = get_spectra_from_maf(maf,hgfile,'cosmic3_ID')
+        if reference == "pcawg_COMPOSITE":
+            maf_sbs,sbs_df = get_spectra_from_maf(maf,hgfile,'pcawg_SBS',real_snps)
+            maf = pd.concat([maf_sbs,maf_dbs,maf_id])
+            maf['context.pcawg'] = maf['context1536.arrow'].fillna('') + maf['context78.word'].fillna('') +  maf['context83.word'].fillna('')            
+        else:
+            maf_sbs,sbs_df = get_spectra_from_maf(maf,hgfile,'cosmic3_exome',real_snps)
+            maf = pd.concat([maf_sbs,maf_dbs,maf_id])
+            maf['context.pcawg'] = maf['context96.word'].fillna('') + maf['context78.word'].fillna('') +  maf['context83.word'].fillna('')            
+            
+        # concatenate spectra
+        spectra = pd.concat([sbs_df,dbs_df,id_df]).fillna(0)
+        spectra.index.name = "context.pcawg"
+    elif reference in ["pcawg_SBS_ID","pcawg_SBS96_ID"]:
+        """
+        Concatenate 1536 or 96 SBS + ID spectra
+        """
+        maf_id,id_df = get_spectra_from_maf(maf,hgfile,'cosmic3_ID')
+        if reference == "pcawg_SBS96_ID":
+            maf_sbs, sbs_df = get_spectra_from_maf(maf,hgfile,'cosmic3_exome',real_snps)
+            maf = pd.concat([maf_sbs, maf_id])
+            maf['context.pcawg'] = maf['context96.word'].fillna('') + maf['context83.word'].fillna('')
+        else:
+            maf_sbs, sbs_df = get_spectra_from_maf(maf,hgfile,'pcawg_SBS',real_snps)
+            maf = pd.concat([maf_sbs, maf_id])
+            maf['context.pcawg'] = maf['context1536.arrow'].fillna('') + maf['context83.word'].fillna('')
+        spectra = pd.concat([sbs_df, id_df]).fillna(0)
+        spectra.index.name = "context.pcawg"
+
+    elif reference in ['polymerase_msi','polymerase_msi96']:
+        """
+        Concatenate 1536 or 96 SBS + POLE/POLD-MSI ID spectra
+        """
+
+        maf_id = maf[maf['Variant_Type'].isin(['DEL','INS'])].copy()
+        def get_indel_len(x):
+            if len(x) >= 4:
+                return("4")
+            else:
+                return(str(len(x)))
+
+        maf_id['context.polymerase'] = maf_id.apply(lambda x: '' if x['Variant_Type'] not in ['DEL','INS'] else
+                                                    ('DEL' + get_indel_len(x['Reference_Allele']) if x['Variant_Type']=='DEL' else
+                                                     'INS' + get_indel_len(x['Tumor_Seq_Allele2'])),1)
+        id_df = maf_id.groupby(['context.polymerase','sample']).size().unstack().fillna(0).astype(int)
+
+        if reference == "polymerase_msi":
+            sbs_context = 'pcawg_SBS'
+            context_form = 'context1536.arrow'
+        else:
+            sbs_context = 'cosmic3_exome'
+            context_form = 'context96.word'
+
+        maf_sbs, sbs_df = get_spectra_from_maf(maf, hgfile, sbs_context, real_snps)
+        maf = pd.concat([maf_sbs, maf_id])
+        maf['context.polymerase'] = maf[context_form].fillna('') + maf['context.polymerase'].fillna('')
+        maf = maf.drop(columns=context_form)
+        
+        spectra = pd.concat([sbs_df, id_df]).fillna(0)
+        spectra.index.name = "context.polymerase"
     else:
         raise NotImplementedError()
-
     return maf, spectra
```

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer.egg-info/PKG-INFO` & `signatureanalyzer-0.0.8/signatureanalyzer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,142 @@
 Metadata-Version: 2.1
 Name: signatureanalyzer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bayesian NMF methods for mutational signature analysis & transcriptomic profiling on GPUs (Getz Lab).
 Home-page: https://github.com/broadinstitute/getzlab-SignatureAnalyzer
 Author: Shankara Anand & Justin Cha - Broad Institute - Cancer Genome Computational Analysis
 Author-email: sanand@broadinstitute.org
 License: MIT
-Description: # SignatureAnalyzer
-        
-        Automatic Relevance Determination (ARD) - NMF of mutational signature &amp; expression data. Designed for scalability using Pytorch to run using GPUs if available.
-        * See `docs` for a more in-depth description of how to use method.
-        
-        _Requires Python 3.6.0 or higher._
-        
-        ## Installation
-        
-        ##### PIP
-        
-        `pip3 install signatureanalyzer`
-        
-        or
-        
-        ##### Git Clone
-        
-        * `git clone --recursive https://github.com/broadinstitute/getzlab-SignatureAnalyzer.git`
-        * `cd getzlab-SignatureAnalyzer`
-        * `pip3 install -e .`
-        
-        Note `--recurisve` flag is required to clone submodules.
-        
-        ##### Docker
-        
-        Link: `http://gcr.io/broad-cga-sanand-gtex/signatureanalyzer`
-        
-        * `docker pull gcr.io/broad-cga-sanand-gtex/signatureanalyzer:latest`
-        * `docker run -it --rm gcr.io/broad-cga-sanand-gtex/signatureanalyzer`
-        
-        ---
-        
-        ## Source Publications
-        
-        **PCAWG Mutational Signatures**
-        * Alexandrov, L. B., Kim, J., Haradhvala, N. J., Huang, M. N., Ng, A. W. T., Wu, Y., ... & Islam, S. A. (2020). The repertoire of mutational signatures in human cancer. Nature, 578(7793), 94-101.
-         * see: https://www.nature.com/articles/s41586-020-1943-3
-         * see `./PCAWG/`
-        
-        **SignatureAnalyzer-GPU source publication**
-        * Taylor-Weiner, A., Aguet, F., Haradhvala, N.J. et al. Scaling computational genomics to millions of individuals with GPUs. Genome Biol 20, 228 (2019) doi:10.1186/s13059-019-1836-7
-        (https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7)
-          * see: https://github.com/broadinstitute/SignatureAnalyzer-GPU
-        
-        **SignatureAnalyzer-CPU source publications**
-        * Kim, J. et al. Somatic ERCC2 mutations are associated with a distinct genomic signature in urothelial tumors. Nat. Genet. 48, 600–606 (2016). (https://www.nature.com/articles/ng.3557)
-        
-        * Kasar, S. et al. Whole-genome sequencing reveals activation-induced cytidine deaminase signatures during indolent chronic lymphocytic leukaemia evolution. Nat. Commun. 6, 8866 (2015). (https://www.nature.com/articles/ncomms9866)
-        
-        **Mathematical details**
-        * Tan, V. Y. F., Edric, C.  & Evotte, F. Automatic Relevance Determination in Nonnegative Matrix Factorization with the β-Divergence. (2012). (https://arxiv.org/pdf/1111.6085.pdf)
-        
-        
-        ---
-        ## Command Line Interface
-        
-        ```
-        usage: signatureanalyzer [-h] [-t {maf,spectra,matrix}] [-n NRUNS] [-o OUTDIR]
-                                 [--cosmic {cosmic2,cosmic3,cosmic3_exome,cosmic3_DBS,cosmic3_ID,cosmic3_TSB}]
-                                 [--hg_build HG_BUILD] [--cuda_int CUDA_INT]
-                                 [--verbose] [--K0 K0] [--max_iter MAX_ITER]
-                                 [--del_ DEL_] [--tolerance TOLERANCE] [--phi PHI]
-                                 [--a A] [--b B] [--objective {poisson,gaussian}]
-                                 [--prior_on_W {L1,L2}] [--prior_on_H {L1,L2}]
-                                 [--report_freq REPORT_FREQ]
-                                 [--active_thresh ACTIVE_THRESH] [--cut_norm CUT_NORM]
-                                 [--cut_diff CUT_DIFF]
-                                 input
-        ```
-        
-        #### Example:
-        
-        ```
-        signatureanalyzer input.maf -n 10 --cosmic cosmic2 --objective poisson
-        ```
-        
-        
-        ## Python API
-        
-        ```python
-        import signatureanalyzer as sa
-        
-        # ---------------------
-        # RUN SIGNATURE ANALYZER
-        # ---------------------
-        
-        # Run array of decompositions with mutational signature processing
-        sa.run_maf(input.maf, outdir='./ardnmf_output/', cosmic='cosmic2', hg_build='./ref/hg19.2bit', nruns=10)
-        
-        # Run ARD-NMF algorithm standalone
-        sa.ardnmf(...)
-        
-        # ---------------------
-        # LOADING RESULTS
-        # ---------------------
-        import pandas as pd
-        
-        H = pd.read_hdf('nmf_output.h5', 'H')
-        W = pd.read_hdf('nmf_output.h5', 'W')
-        Hraw = pd.read_hdf('nmf_output.h5', 'Hraw')
-        Wraw = pd.read_hdf('nmf_output.h5', 'Wraw')
-        feature_signatures = pd.read_hdf('nmf_output.h5', 'signatures')
-        markers = pd.read_hdf('nmf_output.h5', 'markers')
-        cosine = pd.read_hdf('nmf_output.h5', 'cosine')
-        log = pd.read_hdf('nmf_output.h5', 'log')
-        
-        # Output for each run may be found at...
-        Hrun1 = pd.read_hdf('nmf_output.h5', 'run1/H')
-        Wrun1 = pd.read_hdf('nmf_output.h5', 'run1/W')
-        # etc...
-        
-        # Aggregate output information for each run
-        aggr = pd.read_hdf('nmf_output.h5', 'aggr')
-        
-        # ---------------------
-        # PLOTTING
-        # ---------------------
-        sa.pl.marker_heatmap(...)
-        sa.pl.signature_barplot(...)
-        sa.pl.stacked_bar(...)
-        sa.pl.k_dist(...)
-        sa.pl.consensus_matrix(...)
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SignatureAnalyzer
+
+Automatic Relevance Determination (ARD) - NMF of mutational signature &amp; expression data. Designed for scalability using Pytorch to run using GPUs if available.
+
+_Requires Python 3.6.0 or higher._
+
+Please visit our [wiki](https://github.com/broadinstitute/getzlab-SignatureAnalyzer/wiki) for full documentation.
+## Installation
+
+##### PIP
+
+`pip3 install signatureanalyzer`
+
+or
+
+##### Git Clone
+
+* `git clone --recursive https://github.com/broadinstitute/getzlab-SignatureAnalyzer.git`
+* `cd getzlab-SignatureAnalyzer`
+* `pip3 install -e .`
+
+Note `--recurisve` flag is required to clone submodules.
+
+##### Docker
+
+Link: `http://gcr.io/broad-cga-sanand-gtex/signatureanalyzer`
+
+* `docker pull gcr.io/broad-cga-sanand-gtex/signatureanalyzer:latest`
+* `docker run -it --rm gcr.io/broad-cga-sanand-gtex/signatureanalyzer`
+
+---
+
+## Source Publications
+
+**PCAWG Mutational Signatures**
+* Alexandrov, L. B., Kim, J., Haradhvala, N. J., Huang, M. N., Ng, A. W. T., Wu, Y., ... & Islam, S. A. (2020). The repertoire of mutational signatures in human cancer. Nature, 578(7793), 94-101.
+ * see: https://www.nature.com/articles/s41586-020-1943-3
+ * see `./PCAWG/`
+
+**SignatureAnalyzer-GPU source publication**
+* Taylor-Weiner, A., Aguet, F., Haradhvala, N.J. et al. Scaling computational genomics to millions of individuals with GPUs. Genome Biol 20, 228 (2019) doi:10.1186/s13059-019-1836-7
+(https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7)
+  * see: https://github.com/broadinstitute/SignatureAnalyzer-GPU
+
+**SignatureAnalyzer-CPU source publications**
+* Kim, J. et al. Somatic ERCC2 mutations are associated with a distinct genomic signature in urothelial tumors. Nat. Genet. 48, 600–606 (2016). (https://www.nature.com/articles/ng.3557)
+
+* Kasar, S. et al. Whole-genome sequencing reveals activation-induced cytidine deaminase signatures during indolent chronic lymphocytic leukaemia evolution. Nat. Commun. 6, 8866 (2015). (https://www.nature.com/articles/ncomms9866)
+
+**Mathematical details**
+* Tan, V. Y. F., Edric, C.  & Evotte, F. Automatic Relevance Determination in Nonnegative Matrix Factorization with the β-Divergence. (2012). (https://arxiv.org/pdf/1111.6085.pdf)
+
+
+---
+## Command Line Interface
+
+```
+usage: signatureanalyzer [-h] [-t {maf,spectra,matrix}] [-n NRUNS] [-o OUTDIR]
+                         [--reference {cosmic2,cosmic3,cosmic3_exome,cosmic3_DBS,cosmic3_ID,cosmic3_TSB, 
+			               pcawg_COMPOSITE, pcawg_COMPOSITE96, pcawg_SBS_ID, pcawg_SBS96_ID, pcawg_SBS,
+			 	       polymerase_msi, polymerase_msi96}]
+                         [--hg_build HG_BUILD] [--cuda_int CUDA_INT]
+                         [--verbose] [--K0 K0] [--max_iter MAX_ITER]
+                         [--del_ DEL_] [--tolerance TOLERANCE] [--phi PHI]
+                         [--a A] [--b B] [--objective {poisson,gaussian}]
+                         [--prior_on_W {L1,L2}] [--prior_on_H {L1,L2}]
+                         [--report_freq REPORT_FREQ]
+                         [--active_thresh ACTIVE_THRESH] [--cut_norm CUT_NORM]
+                         [--cut_diff CUT_DIFF]
+                         input
+```
+
+#### Example:
+
+```
+signatureanalyzer input.maf -n 10 --reference cosmic2 --objective poisson
+```
+
+
+## Python API
+
+```python
+import signatureanalyzer as sa
+
+# ---------------------
+# RUN SIGNATURE ANALYZER
+# ---------------------
+
+# Run array of decompositions with mutational signature processing
+sa.run_maf(PATH_TO_MAF, outdir='./ardnmf_output/', reference='cosmic2', hg_build='./ref/hg19.2bit', nruns=10)
+
+# Run ARD-NMF algorithm standalone
+sa.ardnmf(...)
+
+# ---------------------
+# LOADING RESULTS
+# ---------------------
+import pandas as pd
+
+H = pd.read_hdf('nmf_output.h5', 'H')
+W = pd.read_hdf('nmf_output.h5', 'W')
+Hraw = pd.read_hdf('nmf_output.h5', 'Hraw')
+Wraw = pd.read_hdf('nmf_output.h5', 'Wraw')
+feature_signatures = pd.read_hdf('nmf_output.h5', 'signatures')
+markers = pd.read_hdf('nmf_output.h5', 'markers')
+cosine = pd.read_hdf('nmf_output.h5', 'cosine')
+log = pd.read_hdf('nmf_output.h5', 'log')
+
+# Output for each run may be found at...
+Hrun1 = pd.read_hdf('nmf_output.h5', 'run1/H')
+Wrun1 = pd.read_hdf('nmf_output.h5', 'run1/W')
+# etc...
+
+# Aggregate output information for each run
+aggr = pd.read_hdf('nmf_output.h5', 'aggr')
+
+# ---------------------
+# PLOTTING
+# ---------------------
+sa.pl.marker_heatmap(...)
+sa.pl.signature_barplot(...)
+sa.pl.stacked_bar(...)
+sa.pl.k_dist(...)
+sa.pl.consensus_matrix(...)
+
+```
```

### Comparing `signatureanalyzer-0.0.7/signatureanalyzer.egg-info/SOURCES.txt` & `signatureanalyzer-0.0.8/signatureanalyzer.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+LICENSE
 README.md
 setup.py
 signatureanalyzer/__init__.py
 signatureanalyzer/__main__.py
 signatureanalyzer/bnmf.py
 signatureanalyzer/consensus.py
+signatureanalyzer/context.py
 signatureanalyzer/signatureanalyzer.py
 signatureanalyzer/spectra.py
+signatureanalyzer/supervised_bnmf.py
 signatureanalyzer/utils.py
 signatureanalyzer.egg-info/PKG-INFO
 signatureanalyzer.egg-info/SOURCES.txt
 signatureanalyzer.egg-info/dependency_links.txt
 signatureanalyzer.egg-info/entry_points.txt
 signatureanalyzer.egg-info/requires.txt
 signatureanalyzer.egg-info/top_level.txt
@@ -22,12 +25,8 @@
 signatureanalyzer/plotting/_rna.py
 signatureanalyzer/plotting/_utils.py
 signatureanalyzer/ref/cosmic_v2/sa_cosmic2.tsv
 signatureanalyzer/ref/cosmic_v3/sa_cosmic3_dbs.tsv
 signatureanalyzer/ref/cosmic_v3/sa_cosmic3_id.tsv
 signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs.tsv
 signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_exome.tsv
-signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv
-signatureanalyzer/signatureanalyzer_gpu/ARD_NMF.py
-signatureanalyzer/signatureanalyzer_gpu/NMF_functions.py
-signatureanalyzer/signatureanalyzer_gpu/SignatureAnalyzer-GPU.py
-signatureanalyzer/signatureanalyzer_gpu/__init__.py
+signatureanalyzer/ref/cosmic_v3/sa_cosmic3_sbs_t.tsv
```

